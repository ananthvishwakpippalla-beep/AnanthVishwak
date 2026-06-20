# Module IV — Co-ordinate Geometry

# NIOS Senior Secondary Mathematics (311)

## Chapter 13: Cartesian System of Rectangular Coordinates

### Introduction & Key Objectives
René Descartes (1596–1650), a French philosopher and mathematician, revolutionized mathematics by introducing an algebraic approach to geometry. By defining a coordinate grid system using two perpendicular lines, he provided a method to pin down any geometric point using real number pairs. This chapter forms the structural foundation for all of Analytical Geometry, introducing point plotting, distance computation, and sectional divisions.

After studying this chapter, you will be able to:
* Define and set up a **Cartesian Coordinate System** with axes, origin, and quadrants.
* Plot points on a 2D plane using dynamic rectangular coordinates.
* Derive and apply the **Distance Formula** between two given points.
* Calculate the area of a triangle given its vertices on a coordinate grid.
* Apply the **Section Formula** to find the coordinates of a point dividing a line segment internally or externally in a given ratio.

---

### Core Concepts & Formulas

#### 1. Rectangular Cartesian Coordinates
The system consists of two mutually perpendicular real number lines intersecting at their respective zero points.
* **Axes:** The horizontal line is the **x-axis** ($X'OX$), and the vertical line is the **y-axis** ($Y'OY$).
* **Origin ($O$):** The point of intersection, denoted by coordinates $(0,0)$.
* **Coordinates:** For any point $P(x,y)$, $x$ is the **Abscissa** (perpendicular distance from the y-axis), and $y$ is the **Ordinate** (perpendicular distance from the x-axis).

[Image of a 2D Cartesian coordinate plane showing the four quadrants and an arbitrary point P with coordinates x and y]

#### 2. Quadrants and Signs
The coordinate axes divide the plane into four infinite regions called **Quadrants**:
* **Quadrant I:** Top Right | $x > 0, y > 0 \implies (+, +)$
* **Quadrant II:** Top Left | $x < 0, y > 0 \implies (-, +)$
* **Quadrant III:** Bottom Left | $x < 0, y < 0 \implies (-, -)$
* **Quadrant IV:** Bottom Right | $x > 0, y < 0 \implies (+, -)$

#### 3. The Distance Formula
> The straight-line distance between any two geometric points $P(x_1, y_1)$ and $Q(x_2, y_2)$ on the Cartesian plane is given by:
> $$d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$$

* Distance from the origin $O(0,0)$ to a point $P(x,y)$ simplifies directly to:
$$d = \sqrt{x^2 + y^2}$$

#### 4. The Section Formula
Let $A(x_1, y_1)$ and $B(x_2, y_2)$ be two distinct endpoints of a straight line segment. Let a point $P(x,y)$ divide the line segment $AB$ in the explicit numerical ratio $m : n$.

> **Internal Division:** (Point $P$ lies strictly *between* $A$ and $B$)
> $$x = \frac{mx_2 + nx_1}{m + n}, \quad y = \frac{my_2 + ny_1}{m + n}$$

> **External Division:** (Point $P$ lies on the extended line *outside* segment $AB$)
> $$x = \frac{mx_2 - nx_1}{m - n}, \quad y = \frac{my_2 - ny_1}{m - n}$$

* **Mid-point Rule:** If $P$ is exactly the halfway point, it divides the segment in a $1:1$ ratio ($m=n=1$):
> $$x = \frac{x_1 + x_2}{2}, \quad y = \frac{y_1 + y_2}{2}$$

#### 5. Area of a Triangle
> If a triangle has vertices at coordinates $A(x_1, y_1)$, $B(x_2, y_2)$, and $C(x_3, y_3)$, the absolute bounded area is:
> $$\text{Area} = \frac{1}{2} |x_1(y_2 - y_3) + x_2(y_3 - y_1) + x_3(y_1 - y_2)|$$

* **Condition for Collinearity:** If three points $A$, $B$, and $C$ lie on a single continuous straight line, they cannot enclose space. Therefore:
> $$\text{Points are Collinear} \iff \text{Area of Triangle } ABC = 0$$

---

### Step-by-Step Examples

**Example 1:** Find the distance between the points $A(-3, 4)$ and $B(2, -1)$.  
**Solution:**
1. Assign the coordinate indexes: $(x_1, y_1) = (-3, 4)$ and $(x_2, y_2) = (2, -1)$.
2. Substitute these values into the distance formula:
$$d = \sqrt{[2 - (-3)]^2 + [-1 - 4]^2}$$
3. Simplify the values inside the brackets:
$$d = \sqrt{[2 + 3]^2 + [-5]^2} = \sqrt{5^2 + (-5)^2}$$
$$d = \sqrt{25 + 25} = \sqrt{50}$$
4. Simplify the radical expression:
$$d = \sqrt{25 \times 2} = 5\sqrt{2} \text{ units}$$

**Example 2:** Find the coordinates of the point $P$ which divides the line segment joining $A(1, 3)$ and $B(4, 6)$ internally in the ratio $2 : 1$.  
**Solution:**
1. Identify the given parameters: $(x_1, y_1) = (1, 3)$, $(x_2, y_2) = (4, 6)$, $m = 2$, and $n = 1$.
2. Apply the internal section formula for $x$:
$$x = \frac{mx_2 + nx_1}{m + n} = \frac{2(4) + 1(1)}{2 + 1} = \frac{8 + 1}{3} = \frac{9}{3} = 3$$
3. Apply the internal section formula for $y$:
$$y = \frac{my_2 + ny_1}{m + n} = \frac{2(6) + 1(3)}{2 + 1} = \frac{12 + 3}{3} = \frac{15}{3} = 5$$
4. Conclusion: The coordinates of point $P$ are $(3, 5)$.

**Example 3:** Check whether the three points $A(1, 1)$, $B(2, 3)$, and $C(3, 5)$ are collinear.  
**Solution:**
1. Calculate the area of the triangle formed by these three points as vertices:
$$\text{Area} = \frac{1}{2} |1(3 - 5) + 2(5 - 1) + 3(1 - 3)|$$
2. Simplify the operations inside the brackets step-by-step:
$$\text{Area} = \frac{1}{2} |1(-2) + 2(4) + 3(-2)|$$
$$\text{Area} = \frac{1}{2} |-2 + 8 - 6|$$
$$\text{Area} = \frac{1}{2} |0| = 0$$
3. Conclusion: Since the computed area is exactly $0$, the points do not form a triangle. Thus, $A$, $B$, and $C$ are strictly **collinear**.

---

### Terminal Exercises & Self-Check Questions

1. **Quadrant Mapping Analysis:** Identify the respective quadrants for the following coordinate points: $P(-2, -5)$, $Q(3, -4)$, and $R(-1, 7)$.
   * *Answer Hint:* $P(-,-)$ lies in Quadrant III; $Q(+,-)$ lies in Quadrant IV; $R(-,+)$ lies in Quadrant II.

2. **Ratio Extraction Workout:** Find the ratio in which the y-axis divides the line segment joining the points $A(-4, 2)$ and $
