## 6. Variable Velocity Analysis

We are given the velocity of an object as a function of time:
$$v(t) = t^2 + 2t - 5$$

**Initial Condition:** At $t = 0$, the position $x(0) = 4$.

---

### 1. Finding the Position at $t = 3$

Position $x(t)$ is the integral of velocity with respect to time:
$$x(t) = \int v(t) \, dt = \int (t^2 + 2t - 5) \, dt$$

Performing the integration:
$$x(t) = \frac{1}{3}t^3 + t^2 - 5t + C$$

Using the initial condition $x(0) = 4$ to find the constant $C$:
$$4 = \frac{1}{3}(0)^3 + (0)^2 - 5(0) + C \implies C = 4$$

The general position equation is:
$$x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4$$

Now, calculate the position at **$t = 3$**:
$$x(3) = \frac{1}{3}(3)^3 + (3)^2 - 5(3) + 4$$
$$x(3) = 9 + 9 - 15 + 4 = 7$$

**Result:** The object's position at $t=3$ is **$7 \text{ units}$**.

---

### 2. Finding the Acceleration at $t = 3$

Acceleration $a(t)$ is the derivative of velocity with respect to time:
$$a(t) = \frac{dv}{dt} = \frac{d}{dt}(t^2 + 2t - 5)$$

Performing the differentiation:
$$a(t) = 2t + 2$$

Now, calculate the acceleration at **$t = 3$**:
$$a(3) = 2(3) + 2 = 8$$

**Result:** The object's acceleration at $t=3$ is **$8 \text{ units/s}^2$**.

---

### Summary of State at $t = 3$
| Quantity | Value |
| :--- | :--- |
| **Velocity** $v(3)$ | $10 \text{ units/s}$ |
| **Position** $x(3)$ | $7 \text{ units}$ |
| **Acceleration** $a(3)$ | $8 \text{ units/s}^2$ |