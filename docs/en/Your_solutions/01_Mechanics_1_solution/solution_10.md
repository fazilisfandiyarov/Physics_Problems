## 10. Kinematics: 3D Parametric Motion

The position of point $M$ is defined by the following vector function:
$$\vec{r}(t) = (a \cos(\omega t), b \sin(\omega t), bt)$$

where $a, b,$ and $\omega$ are positive constants.

---

### a) Equation of the Trajectory
To find the trajectory, we look at the relationship between the coordinates:
1. $x = a \cos(\omega t) \implies \frac{x}{a} = \cos(\omega t)$
2. $y = b \sin(\omega t) \implies \frac{y}{b} = \sin(\omega t)$
3. $z = bt \implies t = \frac{z}{b}$

From (1) and (2), using the identity $\cos^2\theta + \sin^2\theta = 1$:
$$\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = 1$$

**Interpretation:** * In the $xy$-plane, the projection of the motion is an **ellipse**.
* Since $z$ increases linearly with time ($z = bt$), the 3D trajectory is an **elliptical helix** stretched along the $z$-axis.

---

### b) Path Length ($s$) from $t=0$ to $t=t_0$
The path length is calculated using the integral of the speed:
$$s = \int_{0}^{t_0} |\vec{v}(t)| \, dt$$

First, find the velocity vector $\vec{v}(t)$:
$$\vec{v}(t) = \frac{d\vec{r}}{dt} = (-a\omega \sin(\omega t), b\omega \cos(\omega t), b)$$

Now, find the magnitude $|\vec{v}(t)|$:
$$|\vec{v}(t)| = \sqrt{(-a\omega \sin(\omega t))^2 + (b\omega \cos(\omega t))^2 + b^2}$$
$$|\vec{v}(t)| = \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2}$$

**Special Case:** If $a = b$, the expression simplifies significantly:
$$|\vec{v}(t)| = \sqrt{b^2\omega^2(\sin^2\omega t + \cos^2\omega t) + b^2} = \sqrt{b^2\omega^2 + b^2} = b\sqrt{\omega^2 + 1}$$
In this case, the path length is:
$$s = \int_{0}^{t_0} b\sqrt{\omega^2 + 1} \, dt = bt