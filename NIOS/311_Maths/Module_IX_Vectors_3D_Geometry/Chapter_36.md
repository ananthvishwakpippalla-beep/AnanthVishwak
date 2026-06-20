# NIOS Senior Secondary Mathematics (311)

## Module IX: Vectors and Three Dimensional Geometry
### Chapter 36: Straight Line

### Introduction & Key Objectives
In two-dimensional coordinate geometry, a single linear equation in $x$ and $y$ defines a straight line. However, as we discovered in Chapter 35, when we transition into a three-dimensional ($3\text{D}$) spatial framework, a first-degree linear equation defines a plane, not a line. A straight line in $3\text{D}$ space is structurally defined as the intersection of two unique planes. This final geometry chapter introduces the vector and Cartesian systems used to trace lines under explicit point and directional constraints, as well as methods to calculate intersections and absolute spatial separation.

After studying this chapter, you will be able to:
* Derive and apply the vector and Cartesian equations of a line passing through a **fixed point parallel to a given vector**.
* Derive and apply the equations of a line passing through **two unique fixed points**.
* Convert easily between the **Vector Form** and **Symmetrical Cartesian Form** of a line.
* Calculate the **Angle** between two lines in space.
* Understand the concept of **Skew Lines**.
* Compute the **Shortest Distance** between two parallel or skew lines.

---

### Core Concepts & Formulas

#### 1. Equations under Geometric Constraints

##### A. Line Passing Through a Fixed Point and Parallel to a Given Vector
Let a line pass through a fixed point $A$ with position vector $\vec{a} = x_1\hat{i} + y_1\hat{j} + z_1\hat{k}$ and run perfectly parallel to a direction vector $\vec{b} = a\hat{i} + b\hat{j} + c\hat{k}$ (where $a, b,$ and $c$ are its direction ratios).



* **Vector Equation:** $$\vec{r} = \vec{a} + \lambda\vec{b}$$
  *(where $\lambda$ is a real number scalar parameter).*
* **Symmetrical Cartesian Form:**
  $$\frac{x - x_1}{a} = \frac{y - y_1}{b} = \frac{z - z_1}{c}$$

##### B. Line Passing Through Two Fixed Points
Let a line pass through two distinct points $A(x_1, y_1, z_1)$ and $B(x_2, y_2, z_2)$ with position vectors $\vec{a}$ and $\vec{b}$ respectively:
* **Vector Equation:** $$\vec{r} = \vec{a} + \lambda(\vec{b} - \vec{a})$$
* **Symmetrical Cartesian Form:**
  $$\frac{x - x_1}{x_2 - x_1} = \frac{y - y_1}{y_2 - y_1} = \frac{z - z_1}{z_2 - z_1}$$

---

#### 2. Relational and Metric Rules

##### A. Angle Between Two Lines
The angle $\theta$ between two intersecting lines is identical to the acute angle separating their corresponding direction vectors $\vec{b}_1$ and $\vec{b}_2$:
> $$\cos\theta = \frac{|\vec{b}_1 \cdot \vec{b}_2|}{|\vec{b}_1||\vec{b}_2|} = \frac{|a_1a_2 + b_1b_2 + c_1c_2|}{\sqrt{a_1^2 + b_1^2 + c_1^2}\sqrt{a_2^2 + b_2^2 + c_2^2}}$$

* **Perpendicular Lines Condition ($\perp$):** $$a_1a_2 + b_1b_2 + c_1c_2 = 0$$
* **Parallel Lines Condition ($\parallel$):** $$\frac{a_1}{a_2} = \frac{b_1}{b_2} = \frac{c_1}{c_2}$$

##### B. Shortest Distance Between Two Lines
In a 2D plane, two lines either intersect at a point or run parallel forever. In 3D space, a third configuration exists: lines that are non-parallel but never intersect because they lie in completely different planes. These are called **Skew Lines**.



> **Shortest Distance Between Skew Lines:**
> For the two lines $\vec{r}_1 = \vec{a}_1 + \lambda\vec{b}_1$ and $\vec{r}_2 = \vec{a}_2 + \mu\vec{b}_2$, the shortest straight distance separating them is:
> $$d = \frac{|(\vec{a}_2 - \vec{a}_1) \cdot (\vec{b}_1 \times \vec{b}_2)|}{|\vec{b}_1 \times \vec{b}_2|}$$
* *Condition for Intersection:* If two lines intersect in space, the shortest distance between them drops to zero, meaning: $(\vec{a}_2 - \vec{a}_1) \cdot (\vec{b}_1 \times \vec{b}_2) = 0$.

> **Shortest Distance Between Parallel Lines:**
> For lines sharing a common direction vector ($\vec{r}_1 = \vec{a}_1 + \lambda\vec{b}$ and $\vec{r}_2 = \vec{a}_2 + \mu\vec{b}$):
> $$d = \frac{|(\vec{a}_2 - \vec{a}_1) \times \vec{b}|}{|\vec{b}|}$$

---

### Step-by-Step Examples

**Example 1:** Find the vector and Cartesian equations of a line passing through the point $P(2, -1, 4)$ and running parallel to the direction vector $\vec{b} = 3\hat{i} + 5\hat{j} - 2\hat{k}$.  
**Solution:**
1. Identify components: $\vec{a} = 2\hat{i} - \hat{j} + 4\hat{k}$ and direction ratios $a = 3, b = 5, c = -2$.
2. Assemble the Vector form ($\vec{r} = \vec{a} + \lambda\vec{b}$):
$$\vec{r} = (2\hat{i} - \hat{j} + 4\hat{k}) + \lambda(3\hat{i} + 5\hat{j} - 2\hat{k})$$
3. Assemble the Symmetrical Cartesian form ($\frac{x-x_1}{a} = \frac{y-y_1}{b} = \frac{z-z_1}{c}$):
$$\frac{x - 2}{3} = \frac{y - (-1)}{5} = \frac{z - 4}{-2} \implies \frac{x - 2}{3} = \frac{y + 1}{5} = \frac{z - 4}{-2}$$

**Example 2:** Convert the following Cartesian line equation into standard Vector format:
$$\frac{x - 5}{3} = \frac{y + 4}{7} = \frac{z - 6}{2}$$

**Solution:**
1. Extract the fixed point coordinates $(x_1, y_1, z_1)$ from the numerators. Note the sign rules:
   * $x - 5 = 0 \implies x_1 = 5$
   * $y + 4 = 0 \implies y_1 = -4$
   * $z - 6 = 0 \implies z_1 = 6$
   * This yields the initial position vector: $\vec{a} = 5\hat{i} - 4\hat{j} + 6\hat{k}$.
2. Extract the direction ratios from the denominators: $a = 3, b = 7, c = 2$.
   * This yields the parallel direction vector: $\vec{b} = 3\hat{i} + 7\hat{j} + 2\hat{k}$.
3. Combine into the final vector form equation:
$$\vec{r} = (5\hat{i} - 4\hat{j} + 6\hat{k}) + \lambda(3\hat{i} + 7\hat{j} + 2\hat{k})$$

**Example 3:** Calculate the acute angle $\theta$ between the two lines:
$$\frac{x - 2}{2} = \frac{y + 1}{2} = \frac{z - 3}{1} \quad \text{and} \quad \frac{x + 1}{4} = \frac{y - 4}{1} = \frac{z - 1}{8}$$

**Solution:**
1. Extract the directional ratios from the denominators of both equations:
   * Line 1: $\vec{b}_1 = 2\hat{i} + 2\hat{j} + \hat{k}$
   * Line 2: $\vec{b}_2 = 4\hat{i} + \hat{j} + 8\hat{k}$
2. Compute the scalar dot product ($\vec{b}_1 \cdot \vec{b}_2$):
$$\vec{b}_1 \cdot \vec{b}_2 = (2 \times 4) + (2 \times 1) + (1 \times 8) = 8 + 2 + 8 = 18$$
3. Compute the magnitude profiles:
   * $|\vec{b}_1| = \sqrt{2^2 + 2^2 + 1^2} = \sqrt{4 + 4 + 1} = \sqrt{9} = 3$
   * $|\vec{b}_2| = \sqrt{4^2 + 1^2 + 8^2} = \sqrt{16 + 1 + 64} = \sqrt{81} = 9$
4. Substitute values into the cosine angle equation:
$$\cos\theta = \frac{|\vec{b}_1 \cdot \vec{b}_2|}{|\vec{b}_1||\vec{b}_2|} = \frac{18}{3 \times 9} = \frac{18}{27} = \frac{2}{3}$$
5. Isolate the final angle:
$$\theta = \cos^{-1}\left(\frac{2}{3}\right)$$

---

### Terminal Exercises & Self-Check Questions

1. **Two-Point Equation Workout:** Find the Cartesian equations of the straight line passing through the points $M(1, -2, 3)$ and $N(4, 5, -1)$.
   * *Answer Hint:* Use the two-point layout template $\frac{x-x_1}{x_2-x_1} = \frac{y-y_1}{y_2-y_1} = \frac{z-z_1}{z_2-z_1}$:
     $$\frac{x - 1}{4 - 1} = \frac{y - (-2)}{5 - (-2)} = \frac{z - 3}{-1 - 3} \implies \frac{x - 1}{3} = \frac{y + 2}{7} = \frac{z - 3}{-4}$$

2. **Orthogonal Parameter Tracking:** Find the value of variable $k$ if the line $\frac{x-1}{3} = \frac{y+2}{2k} = \frac{z-5}{2}$ and the line $\frac{x+2}{k} = \frac{y-1}{3} = \frac{z+1}{-4}$ are given as perpendicular.
   * *Step-by-Step Solution:* 1. Isolate directions: $\vec{b}_1 = [3, 2k, 2]$ and $\vec{b}_2 = [k, 3, -4]$.
     2. For perpendicular lines, set the dot product to 0: $a_1a_2 + b_1b_2 + c_1c_2 = 0$.
     3. Apply values: $(3)(k) + (2k)(3) + (2)(-4) = 0 \implies 3k + 6k - 8 = 0$.
     4. Solve the expression: $9k = 8 \implies k = \frac{8}{9}$.

3. **Parallel Line Separation Metric:** If the shortest distance between two skew lines evaluates to exactly zero, what physical conclusion can be drawn about their interaction?
   * *Answer Hint:* When the shortest distance drops to exactly zero ($d = 0$), it means there is no spatial separation between them at their closest point. Therefore, the two lines **intersect at a single point** in space.