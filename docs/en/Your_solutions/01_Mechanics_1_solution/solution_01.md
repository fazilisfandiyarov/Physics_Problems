# Projectile Motion Analysis

This project provides a detailed derivation of the motion of a projectile fired from the ground with an initial velocity $v_0$ at an angle $\theta$ above the horizontal, assuming no air resistance.

---

## 1. Differential Equations of Motion

We decompose the initial velocity into horizontal and vertical components:
* **Horizontal:** $v_{0x} = v_0 \cos\theta$
* **Vertical:** $v_{0y} = v_0 \sin\theta$

Since the only force acting on the projectile is gravity ($g$) acting downwards:

### Horizontal Direction ($x$):
There is no horizontal acceleration.
$$\frac{d^2x}{dt^2} = 0$$
By integrating once, we get the velocity: $v_x(t) = v_0 \cos\theta$.  
Integrating again gives the position:
$$x(t) = (v_0 \cos\theta)t$$

### Vertical Direction ($y$):
The acceleration is constant due to gravity.
$$\frac{d^2y}{dt^2} = -g$$
By integrating once, we get the vertical velocity: $v_y(t) = v_0 \sin\theta - gt$.  
Integrating again gives the vertical position:
$$y(t) = (v_0 \sin\theta)t - \frac{1}{2}gt^2$$

---

## 2. Time of Flight ($T$)

The projectile hits the ground when the vertical displacement $y(T)$ returns to zero.
$$(v_0 \sin\theta)T - \frac{1}{2}gT^2 = 0$$

Solving for $T$ (where $T \neq 0$):
$$T \left( v_0 \sin\theta - \frac{1}{2}gT \right) = 0$$
$$T = \frac{2v_0 \sin\theta}{g}$$

---

## 3. Maximum Height ($H$)

The maximum height is reached when the vertical velocity is zero ($v_y = 0$).
$$v_0 \sin\theta - gt_{peak} = 0 \implies t_{peak} = \frac{v_0 \sin\theta}{g}$$

Substituting $t_{peak}$ into the $y(t)$ equation:
$$H = (v_0 \sin\theta) \left( \frac{v_0 \sin\theta}{g} \right) - \frac{1}{2}g \left( \frac{v_0 \sin\theta}{g} \right)^2$$
$$H = \frac{v_0^2 \sin^2\theta}{2g}$$

---

## 4. Range ($R$)

The range is the total horizontal distance traveled during the time of flight $T$.
$$R = x(T) = (v_0 \cos\theta) \times T$$
$$R = (v_0 \cos\theta) \left( \frac{2v_0 \sin\theta}{g} \right)$$

Using the trigonometric identity $2 \sin\theta \cos\theta = \sin(2\theta)$:
$$R = \frac{v_0^2 \sin(2\theta)}{g}$$