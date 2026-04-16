# Conservation of Energy: Pendulum Swing

This analysis calculates the maximum velocity of a pendulum bob using energy conservation principles.

## Problem Statement
A pendulum of length $L = 1.0 \text{ m}$ is released from an angle of $\theta = 15^\circ$. We need to find the velocity ($v$) at the equilibrium position (bottom).

---

## 1. Height Calculation
First, we find the vertical drop ($h$) from the release point to the bottom:
$$h = L(1 - \cos\theta)$$
$$h = 1.0(1 - \cos(15^\circ)) \approx 0.0341 \text{ m}$$

## 2. Energy Conversion
Applying the conservation of energy ($PE_{top} = KE_{bottom}$):
$$mgh = \frac{1}{2}mv^2$$

Solving for $v$:
$$v = \sqrt{2gh}$$

## 3. Numerical Result
$$v = \sqrt{2 \times 9.81 \times 0.0341}$$
**Velocity:** $v \approx 0.82 \text{ m/s}$

---
> **Note:** This calculation assumes zero air resistance and a frictionless pivot.