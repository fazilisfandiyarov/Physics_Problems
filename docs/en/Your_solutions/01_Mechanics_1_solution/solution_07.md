## 7. Elimination of Time and Acceleration Interpretation

Given the parametric equations of the path:
$$x(t) = 2t^2$$
$$y(t) = 3t^3$$

### 1. Eliminating the Parameter $t$
To find the Cartesian equation of the path, we solve for $t$ in the $x(t)$ equation:
$$t^2 = \frac{x}{2} \implies t = \sqrt{\frac{x}{2}}$$

Substitute this into the $y(t)$ equation:
$$y = 3 \left( \sqrt{\frac{x}{2}} \right)^3$$
$$y = 3 \left( \frac{x}{2} \right)^{3/2}$$
$$y = \frac{3}{2\sqrt{2}} x^{3/2}$$

This describes a **semi-cubical parabola**.

---

### 2. Velocity and Acceleration Vectors

**Velocity Vector $\vec{v}(t)$:**
$$\vec{v}(t) = \left( \frac{dx}{dt}, \frac{dy}{dt} \right) = (4t, 9t^2)$$

**Speed (Magnitude of Velocity) $|\vec{v}(t)|$:**
$$|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = \sqrt{16t^2 + 81t^4} = t\sqrt{16 + 81t^2}$$

**Acceleration Vector $\vec{a}(t)$:**
$$\vec{a}(t) = \frac{d\vec{v}}{dt} = (4, 18t)$$

**Magnitude of Acceleration $|\vec{a}(t)|$:**
$$|\vec{a}(t)| = \sqrt{4^2 + (18t)^2} = \sqrt{16 + 324t^2} = 2\sqrt{4 + 81t^2}$$

---

### 3. Interpretation of Acceleration

**Is the acceleration constant?**
No. While the horizontal component of acceleration ($a_x = 4$) is constant, the vertical component ($a_y = 18t$) depends linearly on time. Therefore, the total acceleration vector $\vec{a}(t)$ changes both its magnitude and direction as $t$ increases.

### Summary Table
| Quantity | Expression |
| :--- | :--- |
| **Path Equation** | $y = \frac{3}{2\sqrt{2}} x^{3/2}$ |
| **Velocity** $\vec{v}(t)$ | $4t\hat{i} + 9t^2\hat{j}$ |
| **Acceleration** $\vec{a}(t)$ | $4\hat{i} + 18t\hat{j}$ |
| **Constant Acceleration?** | **No** (Time-dependent) |