## 9. Damped Oscillator

We study the equation:

m d²x/dt² + b dx/dt + kx = 0

---

### 1. General Solution

Define:

γ = b / (2m)  
ω₀ = √(k/m)

#### Underdamped (b² < 4mk):
x(t) = e^(-γt) [A cos(ω_d t) + B sin(ω_d t)]  
where ω_d = √(ω₀² - γ²)

#### Critically damped (b² = 4mk):
x(t) = (A + Bt)e^(-γt)

#### Overdamped (b² > 4mk):
x(t) = A e^(r₁t) + B e^(r₂t)

---

### 2. Classification

- Underdamped → oscillatory decay  
- Critically damped → fastest return without oscillation  
- Overdamped → slow non-oscillatory decay  

---

### 3–6. Interactive Simulation (RK4 + Graphs)

Save the file below as `damped_oscillator.html` and upload to GitHub.

```html
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Damped Oscillator</title>
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<style>
body { font-family: Arial; text-align: center; }
canvas { max-width: 600px; margin: 20px; }
</style>
</head>
<body>

<h2>Damped Harmonic Oscillator</h2>

<label>Damping b: <span id="bVal">0.5</span></label><br>
<input type="range" id="bSlider" min="0" max="10" step="0.1" value="0.5">

<p id="regime"></p>

<canvas id="xtChart"></canvas>
<canvas id="phaseChart"></canvas>

<script>
const m = 1;
const k = 4;

const xtCtx = document.getElementById('xtChart').getContext('2d');
const phaseCtx = document.getElementById('phaseChart').getContext('2d');

let xtChart = new Chart(xtCtx, {
    type: 'line',
    data: { labels: [], datasets: [{ label: 'x(t)', data: [], borderWidth: 2 }] },
    options: { animation: false }
});

let phaseChart = new Chart(phaseCtx, {
    type: 'line',
    data: { datasets: [{ label: 'Phase (x,v)', data: [], parsing:false, borderWidth: 2 }] },
    options: { animation: false }
});

function classify(b) {
    const crit = 2 * Math.sqrt(m * k);
    if (b < crit) return "Underdamped";
    if (b === crit) return "Critically Damped";
    return "Overdamped";
}

// RK4 solver
function simulate(b) {
    const dt = 0.02;
    const tMax = 20;

    let x = 1;
    let v = 0;

    let tArr = [];
    let xArr = [];
    let phaseArr = [];

    function accel(x, v) {
        return -(b/m)*v - (k/m)*x;
    }

    for (let t = 0; t < tMax; t += dt) {
        tArr.push(t);
        xArr.push(x);
        phaseArr.push({x: x, y: v});

        let k1x = v;
        let k1v = accel(x, v);

        let k2x = v + 0.5*dt*k1v;
        let k2v = accel(x + 0.5*dt*k1x, v + 0.5*dt*k1v);

        let k3x = v + 0.5*dt*k2v;
        let k3v = accel(x + 0.5*dt*k2x, v + 0.5*dt*k2v);

        let k4x = v + dt*k3v;
        let k4v = accel(x + dt*k3x, v + dt*k3v);

        x += dt/6 * (k1x + 2*k2x + 2*k3x + k4x);
        v += dt/6 * (k1v + 2*k2v + 2*k3v + k4v);
    }

    return {tArr, xArr, phaseArr};
}

function update() {
    const b = parseFloat(document.getElementById("bSlider").value);
    document.getElementById("bVal").innerText = b;

    const result = simulate(b);

    xtChart.data.labels = result.tArr;
    xtChart.data.datasets[0].data = result.xArr;
    xtChart.update();

    phaseChart.data.datasets[0].data = result.phaseArr;
    phaseChart.update();

    document.getElementById("regime").innerText = classify(b);
}

document.getElementById("bSlider").addEventListener("input", update);

update();
</script>

</body>
</html>