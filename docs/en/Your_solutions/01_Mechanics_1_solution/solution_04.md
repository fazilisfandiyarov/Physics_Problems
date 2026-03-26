## 4. Vector Calculus Analysis

The position vector of an object as a function of time $t$ is given by:
$$\vec{r}(t) = (3t^2)\hat{i} + (5t - 8t^2)\hat{j}$$

### 1. Velocity Vector ($\vec{v}$)
Velocity is defined as the first derivative of the position vector with respect to time:
$$\vec{v}(t) = \frac{d\vec{r}}{dt}$$

We differentiate each component independently:
* **x-component:** $\frac{d}{dt}(3t^2) = 6t$
* **y-component:** $\frac{d}{dt}(5t - 8t^2) = 5 - 16t$

Thus, the velocity vector is:
$$\vec{v}(t) = (6t)\hat{i} + (5 - 16t)\hat{j}$$

---

### 2. Acceleration Vector ($\vec{a}$)
Acceleration is defined as the first derivative of the velocity vector (or the second derivative of the position vector) with respect to time:
$$\vec{a}(t) = \frac{d\vec{v}}{dt} = \frac{d^2\vec{r}}{dt^2}$$

Differentiating the velocity components:
* **x-component:** $\frac{d}{dt}(6t) = 6$
* **y-component:** $\frac{d}{dt}(5 - 16t) = -16$

Thus, the acceleration vector is constant:
$$\vec{a}(t) = 6\hat{i} - 16\hat{j}$$

---

### Summary of Results
| Kinematic Quantity | Expression |
| :--- | :--- |
| **Position** $\vec{r}(t)$ | $(3t^2)\hat{i} + (5t - 8t^2)\hat{j}$ |
| **Velocity** $\vec{v}(t)$ | $(6t)\hat{i} + (5 - 16t)\hat{j}$ |
| **Acceleration** $\vec{a}(t)$ | $6\hat{i} - 16\hat{j}$ |

> **Note:** Since the acceleration vector is constant (independent of $t$), this object is undergoing uniformly accelerated motion in two dimensions.