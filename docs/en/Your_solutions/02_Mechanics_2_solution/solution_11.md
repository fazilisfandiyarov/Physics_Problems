# Dynamics Analysis: Time-Dependent Force

This report derives the kinematic equations for a $3 \text{ kg}$ mass subjected to a non-constant force field.

## 1. Input Parameters
* **Mass ($m$):** $3 \text{ kg}$
* **Force Field ($\mathbf{F}$):** $(15t, 3t - 12, -6t^2) \text{ N}$
* **Initial Velocity ($\mathbf{v}_0$):** $(2, 0, 1) \text{ m/s}$
* **Initial Position ($\mathbf{r}_0$):** $(5, 2, -3) \text{ m}$

---

## 2. Velocity Equation
Integrating acceleration $\mathbf{a} = \mathbf{F}/m$ and applying initial conditions:

$$\mathbf{v}(t) = \begin{pmatrix} 2.5t^2 + 2 \\ 0.5t^2 - 4t \\ -\frac{2}{3}t^3 + 1 \end{pmatrix} \text{ m/s}$$

---

## 3. Position Equation
Integrating velocity $\mathbf{v}(t)$ and applying initial conditions:

$$\mathbf{r}(t) = \begin{pmatrix} \frac{5}{6}t^3 + 2t + 5 \\ \frac{1}{6}t^3 - 2t^2 + 2 \\ -\frac{1}{6}t^4 + t - 3 \end{pmatrix} \text{ m}$$

---

## 4. Summary Table
| Component | Acceleration ($m/s^2$) | Velocity ($m/s$) | Position ($m$) |
| :--- | :--- | :--- | :--- |
| **X** | $5t$ | $2.5t^2 + 2$ | $\frac{5}{6}t^3 + 2t + 5$ |
| **Y** | $t - 4$ | $0.5t^2 - 4t$ | $\frac{1}{6}t^3 - 2t^2 + 2$ |
| **Z** | $-2t^2$ | $-\frac{2}{3}t^3 + 1$ | $-\frac{1}{6}t^4 + t - 3$ |

---
*Generated for Kinematics and Dynamics Study*