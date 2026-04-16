# Vertical Throw with Linear Air Resistance

This project provides an analytical and numerical look at motion influenced by both gravity and air drag.

## 1. Mathematical Model
The motion is governed by:
$$m\dot{v} = -mg - kv$$

### Velocity Equation
$$v(t) = (v_0 + v_t)e^{-\frac{k}{m}t} - v_t$$
where $v_t = \frac{mg}{k}$ is the terminal velocity magnitude.

## 2. Key Findings
* **Height Reduction:** Drag significantly reduces the peak height reached by the object.
* **Asymmetry:** The time taken to reach the peak is shorter than the time taken to fall back to the initial height.

## 3. Simulation Result
The Python simulation compares the trajectory of a 1kg mass in a vacuum versus a medium with a drag coefficient of 0.5. The "With Drag" curve peaks earlier and lower.