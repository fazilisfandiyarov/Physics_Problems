# Dynamics in a 3D Force Field

This analysis derives kinematic and dynamic properties for a particle with mass $m = 0.5 \text{ kg}$ based on given parametric equations of motion.

## 1. Equations of Motion
The position vector is defined as:
$$\mathbf{r}(t) = (5t^2 - t)\mathbf{i} + (2t^3)\mathbf{j} + (-3t + 2)\mathbf{k}$$

---

## 2. Derived Physical Quantities

| Quantity | Vector Formula | Units |
| :--- | :--- | :--- |
| **Velocity ($\mathbf{v}$)** | $(10t - 1)\mathbf{i} + 6t^2\mathbf{j} - 3\mathbf{k}$ | m/s |
| **Momentum ($\mathbf{p}$)** | $(5t - 0.5)\mathbf{i} + 3t^2\mathbf{j} - 1.5\mathbf{k}$ | kg·m/s |
| **Acceleration ($\mathbf{a}$)** | $10\mathbf{i} + 12t\mathbf{j} + 0\mathbf{k}$ | m/s² |
| **Force ($\mathbf{F}$)** | $5\mathbf{i} + 6t\mathbf{j} + 0\mathbf{k}$ | N |

---

## 3. Power Analysis
Power is calculated using the dot product $P = \mathbf{F} \cdot \mathbf{v}$:

$$P(t) = F_x v_x + F_y v_y + F_z v_z$$
$$P(t) = 5(10t - 1) + 6t(6t^2) + 0$$
**Time-dependent Power:**
$$P(t) = 36t^3 + 50t - 5 \text{ W}$$

---
*Physics Problem Set: Classical Mechanics*