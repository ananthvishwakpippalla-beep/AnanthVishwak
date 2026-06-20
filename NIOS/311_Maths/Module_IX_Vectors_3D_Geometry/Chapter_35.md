# NIOS Senior Secondary Mathematics (311)

## Module IX: Vectors and Three Dimensional Geometry
### Chapter 35: Plane

### Introduction & Key Objectives
A flat, two-dimensional surface that extends infinitely in all directions is called a **Plane**. In standard coordinate geometry, a straight line is represented by a first-degree linear equation in two variables ($x$ and $y$). When we step into a three-dimensional ($3\text{D}$) spatial system, a first-degree linear equation in three variables ($x, y,$ and $z$) no longer plots a line—instead, it defines a plane. This chapter establishes the vector and Cartesian equations of planes under varying geometric constraints, providing critical tools for multivariable calculus and structural modeling.

After studying this chapter, you will be able to:
* Define a plane and understand the structural role of a **Normal Vector** to a plane.
* Derive and apply the equation of a plane in **Normal Form**.
* Write down the general equation of a plane passing through a point perpendicular to a given vector direction.
* Derive the equation of a plane passing through **three non-collinear points**.
* Convert a general equation of a plane into its standard **Intercept Form**.
* Calculate the **Angle** between two planes and determine the **Perpendicular Distance** from a point to a plane.

---

### Core Concepts & Formulas

#### 1. General Representation of a Plane
The general first-degree linear equation in three variables always structurally defines a plane in space:
> $$Ax + By + Cz + D = 0$$
Where the coefficients $A, B,$ and $C$ are not all zero. Crucially, these values represent the **Direction Ratios (DR)** of a straight line pointing perfectly perpendicular to the plane, known as the **Normal to the Plane**.

#### 2. Vector and Cartesian Equations under Specific Constraints

##### A. Normal Form
Given the perpendicular distance $p$ from the origin to the plane, and a unit vector $\hat{n}$ pointing along this perpendicular normal:



* **Vector Equation:** $$\vec{r} \cdot \hat{n} = p$$
* **Cartesian Equation:** If $l, m,$ and $n$ are the direction cosines of the normal line:
  $$lx + my + nz = p$$

##### B. Plane Passing Through a Fixed Point and Perpendicular to a Normal Vector
Let a plane pass through a fixed point $A$ with position vector $\vec{a}$ (or coordinate $(x_1, y_1, z_1)$) and run perpendicular to a normal vector $\vec{n} = A\hat{i} + B\hat{j} + C\hat{k}$:
* **Vector Equation:** $$(\vec{r} - \vec{a}) \cdot \vec{n} = 0$$
* **Cartesian Equation:**
  $$A(x - x_1) + B(y - y_1) + C(z - z_1) = 0$$

##### C. Intercept Form
If a plane cuts across the positive or negative coordinate axes at distances $a, b,$ and $c$ from the origin respectively, its spatial position simplifies to:
> $$\frac{x}{a} + \frac{y}{b} + \frac{z}{c} = 1$$
*(where the intercept intersection points are given by $(a,0,0), (0,b,0),$ and $(0,0,c)$).*

---

#### 3. Metric and Relational Rules

##### A. Angle Between Two Planes
The angle $\theta$ between two intersecting planes is mathematically identical to the acute angle separating their corresponding perpendicular normal vectors $\vec{n}_1$ and $\vec{n}_2$:
> $$\cos\theta = \frac{|\vec{n}_1 \cdot \vec{n}_2|}{|\vec{n}_1||\vec{n}_2|} = \frac{|A_1A_2 + B_1B_2 + C_1C_2|}{\sqrt{A_1^2 + B_1^2 + C_1^2}\sqrt{A_2^2 + B_2^2 + C_2^2}}$$

* **Perpendicular Planes Condition ($\perp$):** $$A_1A_2 + B_1B_2 + C_1C_2 = 0$$
* **Parallel Planes Condition ($\parallel$):** $$\frac{A_1}{A_2} = \frac{B_1}{B_2} = \frac{C_1}{C_2}$$

##### B. Perpendicular Distance From a Point to a Plane
> The shortest absolute distance from a spatial point $P(x_1, y_1, z_1)$ to the plane $Ax + By + Cz + D = 0$ is evaluated by:
> $$d = \frac{|Ax_1 + By_1 + Cz_1 + D|}{\sqrt{A^2 + B^2 + C^2}}$$

---

### Step-by-Step Examples

**Example 1:** Find the vector and Cartesian equations of a plane whose perpendicular distance from the origin is $6 \text{ units}$, and whose normal vector direction is given by $\vec{n} = 2\hat{i} + 3\hat{j} + 6\hat{k}$.  
**Solution:**
1. Identify baseline parameters: $p = 6$ and $\vec{n} = 2\hat{i} + 3\hat{j} + 6\hat{k}$.
2. Convert the general normal vector into a specialized **Unit Normal Vector ($\hat{n}$)**:
   * Magnitude: $|\vec{n}| = \sqrt{2^2 + 3^2 + 6^2} = \sqrt{4 + 9 + 36} = \sqrt{49} = 7$
   * Unit Normal: $\hat{n} = \frac{\vec{n}}{|\vec{n}|} = \frac{2}{7}\hat{i} + \frac{3}{7}\hat{j} + \frac{6}{7}\hat{k}$
3. Substitute into the Vector Normal Form ($\vec{r} \cdot \hat{n} = p$):
$$\vec{r} \cdot \left(\frac{2}{7}\hat{i} + \frac{3}{7}\hat{j} + \frac{6}{7}\hat{k}\right) = 6 \implies \vec{r} \cdot (2\hat{i} + 3\hat{j} + 6\hat{k}) = 42$$
4. Write out the corresponding Cartesian equation ($lx + my + nz = p$):
$$\frac{2}{7}x + \frac{3}{7}y + \frac{6}{7}z = 6 \implies 2x + 3y + 6z = 42$$

**Example 2:** Find the equation of the plane passing through the coordinate point $P(1, 4, -2)$ and running perfectly perpendicular to a line with direction ratios $[2, -3, 5]$.  
**Solution:**
1. Map out the spatial variables: $(x_1, y_1, z_1) = (1, 4, -2)$ and normal direction ratios $A = 2, B = -3, C = 5$.
2. Apply the single-point Cartesian equation structure $A(x - x_1) + B(y - y_1) + C(z - z_1) = 0$:
$$2(x - 1) - 3(y - 4) + 5(z - (-2)) = 0$$
3. Expand and simplify the operations inside the brackets:
$$2x - 2 - 3y + 12 + 5z + 10 = 0$$
4. Group variables and constants into the final standard layout form:
$$2x - 3y + 5z + 20 = 0$$

**Example 3:** Find the shortest perpendicular distance from the spatial coordinate point $A(2, 5, -3)$ to the plane $6x - 3y + 2z - 4 = 0$.  
**Solution:**
1. Identify individual parameters from the given target definitions:
   * Point: $x_1 = 2, y_1 = 5, z_1 = -3$
   * Plane: $A = 6, B = -3, C = 2, D = -4$
2. Substitute these parameters into the distance formula:
$$d = \frac{|6(2) - 3(5) + 2(-3) - 4|}{\sqrt{6^2 + (-3)^2 + 2^2}}$$
3. Simplify the numerator and denominator step-by-step:
$$d = \frac{|12 - 15 - 6 - 4|}{\sqrt{36 + 9 + 4}} = \frac{|-13|}{\sqrt{49}} = \frac{13}{7} \text{ units}$$

---

### Terminal Exercises & Self-Check Questions

1. **Intercept Transformation Workout:** Find the lengths of the intercepts cut off from the coordinate axes by the plane equation $2x + 3y - z = 6$.
   * *Step-by-Step Solution:* 1. Divide the entire linear plane equation by the constant term $6$ to set the right side to 1:
        $$\frac{2x}{6} + \frac{3y}{6} - \frac{z}{6} = 1$$
     2. Simplify the individual fractional terms to match Intercept Form ($\frac{x}{a} + \frac{y}{b} + \frac{z}{c} = 1$):
        $$\frac{x}{3} + \frac{y}{2} + \frac{z}{-6} = 1$$
     3. The respective axis intercepts are **$a = 3$, $b = 2$, and $c = -6$**.

2. **Orthogonal Parameter Problem:** Find the value of constant $\alpha$ if the two planes given by equations $2x - y + 3z - 5 = 0$ and $\alpha x + 2y - z + 7 = 0$ are given as mutually perpendicular.
   * *Answer Hint:* For perpendicular planes, their direction ratio products must sum to zero: $A_1A_2 + B_1B_2 + C_1C_2 = 0$.
     $$(2)(\alpha) + (-1)(2) + (3)(-1) = 0 \implies 2\alpha - 2 - 3 = 0 \implies 2\alpha = 5 \implies \alpha = \frac{5}{2}$$

3. **Parallel Planes Metric Tracking:** Find the shortest distance separating the two parallel planes given by equations $2x - 3y + 6z + 4 = 0$ and $2x - 3y + 6z - 10 = 0$.
   * *Answer Hint:* Choose any convenient point lying on the first plane (e.g., set $x=0, y=0 \implies 6z+4=0 \implies z = -\frac{4}{6} = -\frac{2}{3}$, giving point $P(0,0,-\frac{2}{3})$). Now calculate the perpendicular distance from point $P$ to the second plane using the distance formula:
     $$d = \frac{|2(0) - 3(0) + 6(-2/3) - 10|}{\sqrt{2^2 + (-3)^2 + 6^2}} = \frac{|-4 - 10|}{\sqrt{4 + 9 + 36}} = \frac{|-14|}{\sqrt{49}} = \frac{14}{7} = 2 \text{ units}$$