# NIOS Senior Secondary Mathematics (311)

## Module IX: Vectors and Three Dimensional Geometry
### Chapter 34: Vectors

### Introduction & Key Objectives
In physical sciences and geometry, we encounter two distinct types of quantities. **Scalars** are completely defined by their magnitude alone (such as mass, temperature, or distance). **Vectors**, however, require both a magnitude and a specific directional orientation to be fully defined (such as force, velocity, or displacement). This chapter establishes the algebraic foundations of vectors, moving from geometric directed line segments to components in 3D coordinate space, and introduces vector multiplication methods heavily emphasized in the public examination.

After studying this chapter, you will be able to:
* Distinguish between scalar and vector quantities.
* Represent a vector geometrically as a **Directed Line Segment** and algebraically in component form ($\hat{i}, \hat{j}, \hat{k}$).
* Compute the **Magnitude** and **Direction Cosines** of a vector.
* Define and identify different types of vectors (Zero, Unit, Co-initial, Collinear, and Equal vectors).
* Perform vector **Addition**, **Subtraction**, and **Scalar Multiplication**.
* Understand and evaluate the **Scalar (Dot) Product** and the **Vector (Cross) Product** of two vectors and apply their properties.

---

### Core Concepts & Formulas

#### 1. Algebraic Component Representation
A vector in 3D space is represented using its components along the three mutually perpendicular coordinate axes. Let $\hat{i}$, $\hat{j}$, and $\hat{k}$ be the standard unit vectors along the positive x, y, and z axes respectively.

A vector $\vec{a}$ running from the origin to a spatial point $P(x, y, z)$ is written as:
> $$\vec{a} = x\hat{i} + y\hat{j} + z\hat{k}$$

* **Magnitude (Length):** The absolute size of the vector, denoted by $|\vec{a}|$:
> $$|\vec{a}| = \sqrt{x^2 + y^2 + z^2}$$
* **Unit Vector ($\hat{a}$):** A vector pointing in the exact same direction but having a magnitude of exactly 1:
> $$\hat{a} = \frac{\vec{a}}{|\vec{a}|} = \frac{x\hat{i} + y\hat{j} + z\hat{k}}{\sqrt{x^2 + y^2 + z^2}}$$

#### 2. Direction Cosines and Ratio Components
If a vector $\vec{a}$ makes angles $\alpha$, $\beta$, and $\gamma$ with the positive x, y, and z axes respectively, then $\cos\alpha$, $\cos\beta$, and $\cos\gamma$ are called its **Direction Cosines (DC)**, usually denoted by $l$, $m$, and $n$.

> **Fundamental Metric Identity:**
> $$l^2 + m^2 + n^2 = \cos^2\alpha + \cos^2\beta + \cos^2\gamma = 1$$
* For a vector $\vec{a} = x\hat{i} + y\hat{j} + z\hat{k}$, the direction cosines are:
$$l = \frac{x}{|\vec{a}|}, \quad m = \frac{y}{|\vec{a}|}, \quad n = \frac{z}{|\vec{a}|}$$

---

#### 3. Vector Multiplication

##### A. Scalar (Dot) Product: $\vec{a} \cdot \vec{b}$
The dot product multiplies two vectors to yield a purely **Scalar** result.
> $$\vec{a} \cdot \vec{b} = |\vec{a}||\vec{b}|\cos\theta$$
> *(where $\theta$ is the angle separating the two vectors)*



* **Component Evaluation:** If $\vec{a} = a_1\hat{i} + a_2\hat{j} + a_3\hat{k}$ and $\vec{b} = b_1\hat{i} + b_2\hat{j} + b_3\hat{k}$:
> $$\vec{a} \cdot \vec{b} = a_1b_1 + a_2b_2 + a_3b_3$$
* **Perpendicular Vectors Check:** Two non-zero vectors are perpendicular ($\theta = 90^\circ$) if and only if their dot product is zero:
> $$\vec{a} \cdot \vec{b} = 0 \iff \vec{a} \perp \vec{b}$$
* **Angle between Vectors:** $$\cos\theta = \frac{a_1b_1 + a_2b_2 + a_3b_3}{|\vec{a}||\vec{b}|}$$

##### B. Vector (Cross) Product: $\vec{a} \times \vec{b}$
The cross product multiplies two vectors to yield a completely new **Vector** that is perpendicular to both original vectors.
> $$\vec{a} \times \vec{b} = (|\vec{a}||\vec{b}|\sin\theta)\hat{n}$$
> *(where $\hat{n}$ is a unit vector perpendicular to the plane containing $\vec{a}$ and $\vec{b}$, determined by the right-hand rule)*



* **Determinant Evaluation Form:** Evaluated using matrix determinants:
> $$\vec{a} \times \vec{b} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ a_1 & a_2 & a_3 \\ b_1 & b_2 & b_3 \end{vmatrix}$$
* **Parallel Vectors Check:** Two non-zero vectors are parallel ($\theta = 0^\circ$ or $180^\circ$) if and only if their cross product yields a zero vector:
> $$\vec{a} \times \vec{b} = \vec{0} \iff \vec{a} \parallel \vec{b}$$
* **Geometric Area Property:** The magnitude $|\vec{a} \times \vec{b}|$ represents the exact area of a parallelogram whose adjacent sides are formed by vectors $\vec{a}$ and $\vec{b}$.

---

### Step-by-Step Examples

**Example 1:** Find the unit vector in the direction of the vector $\vec{a} = 2\hat{i} + 3\hat{j} + 6\hat{k}$.  
**Solution:**
1. Calculate the absolute magnitude (length) of vector $\vec{a}$:
$$|\vec{a}| = \sqrt{2^2 + 3^2 + 6^2} = \sqrt{4 + 9 + 36} = \sqrt{49} = 7$$
2. Apply the unit vector formula $\hat{a} = \frac{\vec{a}}{|\vec{a}|}$:
$$\hat{a} = \frac{2\hat{i} + 3\hat{j} + 6\hat{k}}{7} = \frac{2}{7}\hat{i} + \frac{3}{7}\hat{j} + \frac{6}{7}\hat{k}$$

**Example 2:** Determine the angle $\theta$ between the two vectors $\vec{a} = \hat{i} + \hat{j} - \hat{k}$ and $\vec{b} = \hat{i} - \hat{j} + \hat{k}$.  
**Solution:**
1. Compute the scalar dot product ($\vec{a} \cdot \vec{b}$):
$$\vec{a} \cdot \vec{b} = (1)(1) + (1)(-1) + (-1)(1) = 1 - 1 - 1 = -1$$
2. Compute individual vector magnitudes:
   * $|\vec{a}| = \sqrt{1^2 + 1^2 + (-1)^2} = \sqrt{3}$
   * $|\vec{b}| = \sqrt{1^2 + (-1)^2 + 1^2} = \sqrt{3}$
3. Substitute these values into the angle equation:
$$\cos\theta = \frac{\vec{a} \cdot \vec{b}}{|\vec{a}||\vec{b}|} = \frac{-1}{\sqrt{3} \times \sqrt{3}} = -\frac{1}{3}$$
4. Isolate the final angle expression:
$$\theta = \cos^{-1}\left(-\frac{1}{3}\right)$$

**Example 3:** Find the cross product $\vec{a} \times \vec{b}$ for the vectors $\vec{a} = 2\hat{i} + \hat{j} + 3\hat{k}$ and $\vec{b} = 3\hat{i} + 5\hat{j} - 2\hat{k}$.  
**Solution:**
1. Formulate the matrix determinant layout:
$$\vec{a} \times \vec{b} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ 2 & 1 & 3 \\ 3 & 5 & -2 \end{vmatrix}$$
2. Expand the determinant along the first row containing the basic unit components:
$$\vec{a} \times \vec{b} = \hat{i}\begin{vmatrix} 1 & 3 \\ 5 & -2 \end{vmatrix} - \hat{j}\begin{vmatrix} 2 & 3 \\ 3 & -2 \end{vmatrix} + \hat{k}\begin{vmatrix} 2 & 1 \\ 3 & 5 \end{vmatrix}$$
3. Evaluate the minor $2 \times 2$ diagonal terms:
   * For $\hat{i}$: $(1 \times -2) - (3 \times 5) = -2 - 15 = -17$
   * For $\hat{j}$: $(2 \times -2) - (3 \times 3) = -4 - 9 = -13$
   * For $\hat{k}$: $(2 \times 5) - (1 \times 3) = 10 - 3 = 7$
4. Combine the terms (mind the negative subtraction sign on the $\hat{j}$ term):
$$\vec{a} \times \vec{b} = -17\hat{i} - (-13\hat{j}) + 7\hat{k} = -17\hat{i} + 13\hat{j} + 7\hat{k}$$

---

### Terminal Exercises & Self-Check Questions

1. **Perpendicular Orthogonality Condition:** Find the value of $\lambda$ if the vectors $\vec{u} = 3\hat{i} + 2\hat{j} + 9\hat{k}$ and $\vec{v} = \hat{i} + \lambda\hat{j} + 3\hat{k}$ are given as mutually perpendicular.
   * *Answer Hint:* For perpendicular vectors, set their dot product to zero: $\vec{u} \cdot \vec{v} = 0$.
     $$(3)(1) + (2)(\lambda) + (9)(3) = 0 \implies 3 + 2\lambda + 27 = 0 \implies 2\lambda + 30 = 0 \implies \lambda = -15$$

2. **Geometric Area Problem:** Find the area of a triangle whose adjacent sides are determined by the vectors $\vec{a} = \hat{i} + 4\hat{j}$ and $\vec{b} = 2\hat{i} - 3\hat{j}$.
   * *Step-by-Step Solution:* 1. The area of a triangle is exactly half the area of the corresponding parallelogram: $\text{Area} = \frac{1}{2}|\vec{a} \times \vec{b}|$.
     2. Evaluate the cross product determinant:
        $$\vec{a} \times \vec{b} = \begin{vmatrix} \hat{i} & \hat{j} & \hat{k} \\ 1 & 4 & 0 \\ 2 & -3 & 0 \end{vmatrix} = \hat{k}[(1 \times -3) - (4 \times 2)] = \hat{k}[-3 - 8] = -11\hat{k}$$
     3. Calculate the magnitude: $|-11\hat{k}| = 11$.
     4. Divide by two: $\text{Area} = \frac{11}{2} = 5.5 \text{ sq. units}$.

3. **Direction Angles Validation:** Can a vector have direction angles $\alpha = 45^\circ$, $\beta = 60^\circ$, and $\gamma = 45^\circ$?
   * *Answer Hint:* Check the fundamental metric identity rule $l^2 + m^2 + n^2 = 1$.
     $$\cos^2 45^\circ + \cos^2 60^\circ + \cos^2 45^\circ = \left(\frac{1}{\sqrt{2}}\right)^2 + \left(\frac{1}{2}\right)^2 + \left(\frac{1}{\sqrt{2}}\right)^2 = \frac{1}{2} + \frac{1}{4} + \frac{1}{2} = \frac{5}{4}$$
     Since $\frac{5}{4} \neq 1$, it violates the identity rule. Therefore, a vector **cannot** have these direction angles.