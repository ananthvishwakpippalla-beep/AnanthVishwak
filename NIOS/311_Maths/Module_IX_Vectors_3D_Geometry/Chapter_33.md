# NIOS Senior Secondary Mathematics (311)

## Module IX: Vectors and Three Dimensional Geometry
### Chapter 33: Introduction to Three Dimensional Geometry

### Introduction & Key Objectives
In all our previous coordinate geometry modules (Module IV), we confined our calculations to a flat, two-dimensional ($2\text{D}$) Cartesian plane. However, the physical world we inhabit is fundamentally three-dimensional ($3\text{D}$). To mathematically locate an object in space—such as an airplane in flight or an atom within a crystal lattice—a third directional parameter is required. This chapter extends our analytical geometry foundations into three dimensions, introducing a triad of mutually perpendicular axes, eight directional spatial zones, and fundamental metric spatial formulas.

After studying this chapter, you will be able to:
* Understand the setup of a **Three-Dimensional Coordinate System** using three mutually perpendicular axes.
* Identify the coordinates of a point in space and name its corresponding **Octant**.
* Derive and apply the $3\text{D}$ extension of the **Distance Formula**.
* Apply the $3\text{D}$ **Section Formula** for both internal and external spatial divisions.
* Find the coordinates of the midpoint and the centroid of a triangle in space.

---

### Core Concepts & Formulas

#### 1. Rectangular Coordinate Axes and Planes in Space
To construct a $3\text{D}$ space, take three mutually perpendicular lines intersecting at a common zero-point called the **Origin ($O$)**.
* **Axes:** These lines form the **x-axis** ($X'OX$), **y-axis** ($Y'OY$), and the new **z-axis** ($Z'OZ$).
* **Coordinate Planes:** Taken in pairs, these axes determine three intersecting boundary planes:
  * The **$XY$-plane** (where the $z$-coordinate is always strictly $0$)
  * The **$YZ$-plane** (where the $x$-coordinate is always strictly $0$)
  * The **$ZX$-plane** (where the $y$-coordinate is always strictly $0$)

#### 2. Sign Profiles of the Eight Octants
The three intersecting coordinate planes slice the entire infinite universe into **eight** unique spatial zones called **Octants**. The signs of a point $P(x, y, z)$ depend directly on its octant home:



| Octant | I | II | III | IV | V | VI | VII | VIII |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| **$x$** | $+$ | $-$ | $-$ | $+$ | $+$ | $-$ | $-$ | $+$ |
| **$y$** | $+$ | $+$ | $-$ | $-$ | $+$ | $+$ | $-$ | $-$ |
| **$z$** | $+$ | $+$ | $+$ | $+$ | $-$ | $-$ | $-$ | $-$ |

*Memory Tip:* Notice that the sign patterns for $x$ and $y$ mirror the familiar four quadrants of a $2\text{D}$ plane for the first four octants (where $z$ is positive) and repeat exactly for the last four octants (where $z$ is negative).

---

#### 3. The 3D Distance Formula
> The straight-line distance separating any two spatial coordinates $P(x_1, y_1, z_1)$ and $Q(x_2, y_2, z_2)$ is given by:
> $$d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2 + (z_2 - z_1)^2}$$

* Consequently, the shortest absolute distance from the origin $O(0,0,0)$ to any point $P(x,y,z)$ is:
$$d = \sqrt{x^2 + y^2 + z^2}$$

#### 4. The 3D Section Formula
Let a spatial segment connect endpoints $A(x_1, y_1, z_1)$ and $B(x_2, y_2, z_2)$. If a point $P(x,y,z)$ divides the line segment $AB$ in the ratio $m : n$, its coordinates are:

> **Internal Division:**
> $$x = \frac{mx_2 + nx_1}{m + n}, \quad y = \frac{my_2 + ny_1}{m + n}, \quad z = \frac{mz_2 + nz_1}{m + n}$$

> **External Division:**
> $$x = \frac{mx_2 - nx_1}{m - n}, \quad y = \frac{my_2 - ny_1}{m - n}, \quad z = \frac{mz_2 - nz_1}{m - n}$$

* **Midpoint Coordinates:** Setting $m = n = 1$ yields:
> $$x = \frac{x_1 + x_2}{2}, \quad y = \frac{y_1 + y_2}{2}, \quad z = \frac{z_1 + z_2}{2}$$

#### 5. Centroid of a Spatial Triangle
If a triangle has vertices at $A(x_1, y_1, z_1)$, $B(x_2, y_2, z_2)$, and $C(x_3, y_3, z_3)$, the center of mass intersection (**Centroid $G$**) is:
> $$G = \left( \frac{x_1 + x_2 + x_3}{3}, \frac{y_1 + y_2 + y_3}{3}, \frac{z_1 + z_2 + z_3}{3} \right)$$

---

### Step-by-Step Examples

**Example 1:** Identify the octants in which the following points lie: $A(2, -3, 4)$ and $B(-1, -4, -5)$.  
**Solution:**
1. Examine the sign matrix of point $A(2, -3, 4)$: Here, $x > 0$ ($+$), $y < 0$ ($-$), and $z > 0$ ($+$). 
2. Matching the sign profile $(+, -, +)$ against our master chart places point $A$ in **Octant IV**.
3. Examine the sign matrix of point $B(-1, -4, -5)$: Here, $x < 0$ ($-$), $y < 0$ ($-$), and $z < 0$ ($-$).
4. Matching the sign profile $(-, -, -)$ against our master chart places point $B$ in **Octant VII**.

**Example 2:** Find the straight-line distance between the spatial points $P(1, -3, 4)$ and $Q(-4, 1, 2)$.  
**Solution:**
1. Map the coordinate variables: $(x_1, y_1, z_1) = (1, -3, 4)$ and $(x_2, y_2, z_2) = (-4, 1, 2)$.
2. Substitute these values into the $3\text{D}$ distance formula:
$$d = \sqrt{[-4 - 1]^2 + [1 - (-3)]^2 + [2 - 4]^2}$$
3. Simplify operations inside the brackets step-by-step:
$$d = \sqrt{[-5]^2 + [4]^2 + [-2]^2}$$
$$d = \sqrt{25 + 16 + 4} = \sqrt{45}$$
4. Factor the radical expression into its cleanest exam-ready form:
$$d = \sqrt{9 \times 5} = 3\sqrt{5} \text{ units}$$

**Example 3:** Find the coordinates of the point $R$ which divides the line segment joining $A(2, 4, 5)$ and $B(3, 5, -4)$ externally in the ratio $3 : 2$.  
**Solution:**
1. Identify the input values: $(x_1, y_1, z_1) = (2, 4, 5)$, $(x_2, y_2, z_2) = (3, 5, -4)$, $m = 3$, and $n = 2$.
2. Since it is an **External Division**, use the subtraction section rules:
   * $$x = \frac{3(3) - 2(2)}{3 - 2} = \frac{9 - 4}{1} = 5$$
   * $$y = \frac{3(5) - 2(4)}{3 - 2} = \frac{15 - 8}{1} = 7$$
   * $$z = \frac{3(-4) - 2(5)}{3 - 2} = \frac{-12 - 10}{1} = -22$$
3. Conclusion: The coordinates of the external dividing point $R$ are **$(5, 7, -22)$**.

---

### Terminal Exercises & Self-Check Questions

1. **Axis Projection Locus Analysis:** A point lies on the x-axis. State its precise y-coordinate and z-coordinate values. What is its general vector form?
   * *Answer Hint:* Any point situated strictly along the x-axis has made zero movement into spatial height or width planes. Therefore, its y-coordinate $= 0$ and its z-coordinate $= 0$, giving it a general coordinate locus form of **$(x, 0, 0)$**.

2. **Collinearity Verification Workout:** Prove using the distance formula that the points $A(1, 2, 3)$, $B(7, 0, 1)$, and $C(-2, 3, 4)$ are collinear.
   * *Step-by-Step Solution:* 1. Calculate length $AB$: $\sqrt{(7-1)^2 + (0-2)^2 + (1-3)^2} = \sqrt{36 + 4 + 4} = \sqrt{44} = 2\sqrt{11}$.
     2. Calculate length $BC$: $\sqrt{(-2-7)^2 + (3-0)^2 + (4-1)^2} = \sqrt{81 + 9 + 9} = \sqrt{99} = 3\sqrt{11}$.
     3. Calculate length $AC$: $\sqrt{(-2-1)^2 + (3-2)^2 + (4-3)^2} = \sqrt{9 + 1 + 1} = \sqrt{11}$.
     4. Check the summation chain: Notice that $AC + AB = \sqrt{11} + 2\sqrt{11} = 3\sqrt{11} = BC$. Since the sum of two smaller segments perfectly matches the longest boundary segment, the points are strictly **collinear**.

3. **Centroid Extraction Workout:** Find the centroid of a triangle whose spatial vertices are given as $A(3, -5, 7)$, $B(5, 4, 2)$, and $C(7, -2, -3)$.
   * *Answer Hint:* Apply the centroid averaging formula:
     $$G = \left( \frac{3+5+7}{3}, \frac{-5+4-2}{3}, \frac{7+2-3}{3} \right) = \left( \frac{15}{3}, \frac{-3}{3}, \frac{6}{3} \right) = (5, -1, 2)$$