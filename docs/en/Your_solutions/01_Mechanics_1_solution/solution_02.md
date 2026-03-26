## 2. Range Optimization

To find the launch angle $\theta$ that maximizes the horizontal range $R$, we analyze the range equation:

$$R(\theta) = \frac{v_0^2 \sin(2\theta)}{g}$$

### Analytical Proof

To find the maximum value of $R(\theta)$, we take the derivative of the range with respect to $\theta$ and set it to zero:

$$\frac{dR}{d\theta} = \frac{v_0^2}{g} \cdot \frac{d}{d\theta}(\sin(2\theta)) = 0$$

Using the chain rule:
$$\frac{v_0^2}{g} \cdot 2\cos(2\theta) = 0$$

Since $v_0$ and $g$ are non-zero constants, we must have:
$$\cos(2\theta) = 0$$

We know that $\cos(\alpha) = 0$ when $\alpha = 90^\circ$ (or $\frac{\pi}{2}$ radians). Therefore:
$$2\theta = 90^\circ$$
$$\theta = 45^\circ$$

### Verification (Second Derivative Test)
To ensure this is a maximum, we check the second derivative:
$$\frac{d^2R}{d\theta^2} = -\frac{4v_0^2 \sin(2\theta)}{g}$$

At $\theta = 45^\circ$, $\sin(90^\circ) = 1$, so:
$$\frac{d^2R}{d\theta^2} = -\frac{4v_0^2}{g} < 0$$

Since the second derivative is negative, $\theta = 45^\circ$ is indeed a **local maximum**.

> **Conclusion:** For any given initial velocity $v_0$, the maximum horizontal range is achieved when the projectile is launched at an angle of **45 degrees**.