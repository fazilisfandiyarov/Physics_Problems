## 3. Path Intersection and Collision Analysis

We are given two moving objects, Alice and Bob, with their positions defined by parametric equations:

* **Alice:** $A(t) = (2+t, 8-3t)$
* **Bob:** $B(t) = (2t-1, 2t+2)$

### 1. Determining Collision
A **collision** occurs if there exists a time $t$ such that $A(t) = B(t)$. This requires both the $x$ and $y$ coordinates to be equal at the same instant.

Equating the $x$-coordinates:
$$2 + t = 2t - 1$$
$$t = 3$$

Now, we check if the $y$-coordinates are equal at $t = 3$:
* For Alice: $y_A(3) = 8 - 3(3) = -1$
* For Bob: $y_B(3) = 2(3) + 2 = 8$

Since $-1 \neq 8$, Alice and Bob **do not collide**. They pass through the same x-coordinate at $t=3$, but at different heights.

---

### 2. Determining Path Intersection
A **path intersection** occurs if their trajectories cross at any time, not necessarily simultaneously. We use different time variables $t_1$ and $t_2$:
$A(t_1) = (2+t_1, 8-3t_1)$  
$B(t_2) = (2t_2-1, 2t_2+2)$

Setting $x_A = x_B$ and $y_A = y_B$:
1. $2 + t_1 = 2t_2 - 1 \implies t_1 = 2t_2 - 3$
2. $8 - 3t_1 = 2t_2 + 2$

Substitute (1) into (2):
$$8 - 3(2t_2 - 3) = 2t_2 + 2$$
$$8 - 6t_2 + 9 = 2t_2 + 2$$
$$17 - 6t_2 = 2t_2 + 2$$
$$8t_2 = 15 \implies t_2 = 1.875$$

Now find $t_1$:
$$t_1 = 2(1.875) - 3 = 0.75$$

**Conclusion:** The paths **intersect** at the point where Alice is at $t=0.75$ and Bob is at $t=1.875$.
**Intersection Point:** $P = (2 + 0.75, 8 - 3(0.75)) = (2.75, 5.75)$.

---

### 3. Minimum Distance
Since they do not collide, we find the minimum distance $D(t)$ between them at any time $t$:
$$D^2(t) = (x_B - x_A)^2 + (y_B - y_A)^2$$
$$D^2(t) = ((2t-1) - (2+t))^2 + ((2t+2) - (8-3t))^2$$
$$D^2(t) = (t-3)^2 + (5t-6)^2$$
$$D^2(t) = (t^2 - 6t + 9) + (25t^2 - 60t + 36)$$
$$f(t) = 26t^2 - 66t + 45$$

To find the minimum, take the derivative $f'(t)$ and set to zero:
$$f'(t) = 52t - 66 = 0$$
$$t = \frac{66}{52} \approx 1.27$$

The minimum distance occurs at **$t \approx 1.27$**. 
$$D_{min} = \sqrt{f(1.27)} = \sqrt{26(1.27)^2 - 66(1.27) + 45} \approx 1.76 \text{ units}$$