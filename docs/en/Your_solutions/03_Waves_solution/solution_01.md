# Physics Report: Simple Pendulum Calculations

This document explores the relationship between gravitational acceleration, pendulum length, and the resulting period of oscillation.

---

## 1. Gravitational Dependence (Earth vs. Moon)

**The Challenge:** A simple pendulum has a period of **4 seconds** on Earth. We need to determine its period on the Moon, where gravitational acceleration is approximately $1/6$ of Earth's gravity.

### The Physics Formula
The period of a simple pendulum is defined by the following equation:

$$T = 2\pi \sqrt{\frac{L}{g}}$$

Where:
* **$T$**: Period (seconds)
* **$L$**: Length of the pendulum (meters)
* **$g$**: Acceleration due to gravity ($m/s^2$)

### Calculation Steps

1.  **Gravity Ratio:** Since $g_{moon} = \frac{1}{6}g_{earth}$, the relationship between the two periods can be written as:
    $$\frac{T_{moon}}{T_{earth}} = \sqrt{\frac{g_{earth}}{g_{moon}}}$$

2.  **Substitution:**
    $$\frac{T_{moon}}{4} = \sqrt{\frac{g_{earth}}{\frac{1}{6}g_{earth}}} = \sqrt{6}$$

3.  **Final Result:**
    $$T_{moon} = 4 \times \sqrt{6} \approx 9.80 \text{ seconds}$$

> **Conclusion:** Due to the lower gravity on the Moon, the pendulum swings much slower, increasing the period from 4 seconds to approximately **9.80 seconds**.

---

## 2. Calculating Required Length for a Specific Period

**The Challenge:** What is the required length ($L$) of a simple pendulum to have a period of exactly **1 second** on Earth?

### Rearranging the Formula
To find the length, we rearrange the period formula:

$$L = g \left( \frac{T}{2\pi} \right)^2$$

### Calculation (Earth Gravity)
* **Target Period ($T$):** $1.0$ s
* **Gravity ($g$):** $9.81 \text{ m/s}^2$

$$L = 9.81 \times \left( \frac{1}{2\pi} \right)^2$$
$$L = \frac{9.81}{4\pi^2}$$
$$L \approx 0.2484 \text{ meters}$$

### Results Summary

| Parameter | Value |
| :--- | :--- |
| **Required Period** | 1.0 second |
| **Calculated Length (m)** | ~0.248 m |
| **Calculated Length (cm)** | **24.84 cm** |

---
*Generated for Physics Documentation purposes.*