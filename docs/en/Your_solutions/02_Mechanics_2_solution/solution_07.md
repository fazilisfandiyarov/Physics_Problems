# Physics Analysis: Dynamics with Friction (Two-Block System)

This document calculates the acceleration of a bottom block in a stacked system with friction on multiple surfaces.

## 1. System Components
* **Block 1 (Top):** $m_1 = 5 \text{ kg}$ (Tied to the wall, stationary)
* **Block 2 (Bottom):** $m_2 = 10 \text{ kg}$
* **Applied Force:** $F = 45 \text{ N}$
* **Friction Coefficient:** $\mu_k = 0.2$

---

## 2. Frictional Force Calculations
Friction opposes the motion of the 10 kg block at two interfaces:

1. **Upper Interface (with $m_1$):**
   $$f_1 = \mu_k \cdot m_1 \cdot g = 0.2 \cdot 5 \cdot 9.81 = 9.81 \text{ N}$$

2. **Lower Interface (with Floor):**
   $$f_2 = \mu_k \cdot (m_1 + m_2) \cdot g = 0.2 \cdot 15 \cdot 9.81 = 29.43 \text{ N}$$

---

## 3. Acceleration of the 10 kg Block
Using Newton's Second Law ($F_{net} = m_2 a$):

**Net Force:**
$$F_{net} = F_{applied} - f_1 - f_2$$
$$F_{net} = 45 - 9.81 - 29.43 = 5.76 \text{ N}$$

**Acceleration:**
$$a = \frac{5.76 \text{ N}}{10 \text{ kg}} = 0.576 \text{ m/s}^2$$

## Summary
The 10 kg block moves with an acceleration of **$0.576 \text{ m/s}^2$**. The 5 kg block remains stationary due to the wall tether, but its weight contributes to the floor friction, and its surface creates drag on the moving block.

---
*Generated for Dynamics Lab Exercises*