# Physics Report: Energy Dissipation in a Bouncing Ball

This analysis tracks the height of a tennis ball over multiple bounces, accounting for energy loss due to inelastic impacts with the ground.

## 1. Problem Parameters
* **Initial Height ($h_0$):** $2.0 \text{ m}$
* **Energy Loss per Bounce:** $30\%$
* **Energy Retention Factor ($r$):** $0.70$ (70%)

## 2. Mathematical Approach
Potential energy is given by $PE = mgh$. Since energy and height are directly proportional ($E \propto h$), we can calculate the height after $n$ bounces using the formula:
$$h_n = h_0 \times (r)^n$$

## 3. Step-by-Step Heights
| Bounce Number | Calculation | Height (m) |
| :--- | :--- | :--- |
| 0 (Initial Drop) | $2.0$ | 2.00 m |
| 1st Bounce | $2.0 \times 0.70$ | 1.40 m |
| **2nd Bounce** | $1.4 \times 0.70$ | **0.98 m** |

## 4. Conclusion
After the second bounce, the tennis ball loses a total of $51\%$ of its original energy ($0.7 \times 0.7 = 0.49$ retained), resulting in a return height of **0.98 meters**.

---
*Documented for Kinematics & Energy Study*
