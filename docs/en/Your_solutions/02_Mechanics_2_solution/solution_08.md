# Analysis of Variable Force and Potential Energy

This report derives the motion and energy characteristics of a system governed by a linear restoring force.

## 1. Equation of Motion
Based on $F = ma$, the differential equation for a mass $m$ under force $F(x) = -kx$ is:
$$m\ddot{x} + kx = 0$$
The solution represents **Simple Harmonic Motion**:
$$x(t) = A\cos(\omega t + \phi), \text{ where } \omega = \sqrt{k/m}$$

## 2. Work-Energy Theorem
The work done by the force during displacement from $0$ to $x_0$ is:
$$W = \int_{0}^{x_0} -kx \, dx = -\frac{1}{2}kx_0^2$$

## 3. Potential Energy ($U$)
Potential energy is defined as the negative work done by a conservative force:
$$U(x) = -W = \frac{1}{2}kx^2$$

## 4. Verification
Applying the gradient relationship:
$$F = -\frac{dU}{dx} = -\frac{d}{dx}\left(\frac{1}{2}kx^2\right) = -kx$$
*The relationship is consistent with the initial force definition.*

## 5. Visual Summary
* **Force Graph:** Linear ($y = -mx$ style), showing the force always points toward equilibrium.
* **Energy Graph:** Parabolic ($y = x^2$ style), showing energy increases with the square of displacement.