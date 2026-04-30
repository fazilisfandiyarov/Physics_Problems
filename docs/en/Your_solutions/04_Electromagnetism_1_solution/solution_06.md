6. Field at a point from a system of charges
Two point charges are given:

+
q
 
at point
 
(
−
a
,
0
)
+
2
q
 
at point
 
(
a
,
0
)
Determine the field vector 
E
→
(
0
,
y
)
, 
E
→
(
x
,
0
)
 and generally 
E
→
(
x
,
y
)
.
Determine the condition for which the components 
E
x
=
0
, 
E
y
=
0
 and the zero field 
E
→
=
0
.
Calculate the field for: 
a
=
0.2a## 6. Field at a Point from a System of Charges

Two point charges:
- +q at (-a, 0)
- +2q at (a, 0)

---

## 1. General Electric Field

Using Coulomb’s law:

E⃗ = k q r⃗ / r³

Let the observation point be (x, y).

### Field from charge q at (-a,0):

r⃗₁ = (x + a, y)  
r₁ = √((x + a)² + y²)

E⃗₁ = kq (x + a, y) / [(x + a)² + y²]^(3/2)

---

### Field from charge 2q at (a,0):

r⃗₂ = (x - a, y)  
r₂ = √((x - a)² + y²)

E⃗₂ = k(2q)(x - a, y) / [(x - a)² + y²]^(3/2)

---

### Total field:

E⃗(x,y) = E⃗₁ + E⃗₂

---

## 2. Field at (0, y)

Substitute x = 0:

Eₓ = kq [ a/(a² + y²)^(3/2)  - 2a/(a² + y²)^(3/2) ]  
Eₓ = -kq a / (a² + y²)^(3/2)

Eᵧ = kq [ y/(a² + y²)^(3/2) + 2y/(a² + y²)^(3/2) ]  
Eᵧ = 3kq y / (a² + y²)^(3/2)

---

## 3. Field at (x, 0)

Eᵧ = 0 (symmetry)

Eₓ = kq (x + a)/|x + a|³ + 2kq (x - a)/|x - a|³

---

## 4. Conditions

### Eₓ = 0
Solve:
kq (x + a)/r₁³ + 2kq (x - a)/r₂³ = 0

→ occurs at some point between charges (not symmetric because charges differ)

---

### Eᵧ = 0
Occurs when:
y = 0

---

### Total field E⃗ = 0
Requires both:
Eₓ = 0 and Eᵧ = 0

→ Only possible on x-axis at a specific point between charges

---

## 5. Numerical Calculation

Given:
a = 0.2 m  
y = 0.3 m  
q = 2 μC = 2 × 10⁻⁶ C  
k = 9 × 10⁹

Compute:

a² + y² = 0.04 + 0.09 = 0.13  
(0.13)^(3/2) ≈ 0.0469

---

### Eₓ:

Eₓ = -kqa / (a² + y²)^(3/2)

Eₓ = -(9×10⁹)(2×10⁻⁶)(0.2) / 0.0469  
Eₓ ≈ -7.67 × 10⁴ N/C

---

### Eᵧ:

Eᵧ = 3kq y / (a² + y²)^(3/2)

Eᵧ = 3(9×10⁹)(2×10⁻⁶)(0.3) / 0.0469  
Eᵧ ≈ 3.45 × 10⁵ N/C

---

### Final vector:

E⃗ ≈ (-7.67×10⁴ , 3.45×10⁵) N/C

---

## 6. Limit: y ≫ a

When y is much larger than a:

a² + y² ≈ y²

So:

Eₓ → 0  
Eᵧ → 3kq / y²

---

### Interpretation:

At large distances, the system behaves like a **single charge 3q located near the origin**.

---

## Final Summary

- General field = vector sum of both charges  
- Asymmetry comes from charge ratio (q vs 2q)  
- Far away → behaves like total charge 3q  
,
m
, 
y
=
0.3
,
m
, 
q
=
2
,
μ
C
.
Investigate the limit 
y
≫
a
.