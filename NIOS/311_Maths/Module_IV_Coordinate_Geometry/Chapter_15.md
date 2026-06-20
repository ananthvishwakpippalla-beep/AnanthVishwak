# NIOS Senior Secondary Mathematics (311)

## Module IV: Co-ordinate Geometry
### Chapter 15: Circles

### Introduction & Key Objectives
A circle is one of the most fundamental curved shapes in geometry. In standard Euclidean geometry, we define it as a collection of points equidistant from a fixed center. In analytical coordinate geometry, we translate this property into a second-degree algebraic equation. Understanding the equations of circles allows us to analyze tangent lines, intersections, and system boundaries, which form a vital bridge into advanced calculus and physics.

After studying this chapter, you will be able to:
* Define a **Circle** from a coordinate perspective.
* Write down the **Standard Form** and **Central Form** of a circle's equation given its center and radius.
* Identify the center and radius from the **General Equation of a Circle** ($x^2 + y^2 + 2gx + 2fy + c = 0$).
* Find the equation of a circle given its **Diameter Endpoints**.
* Deduce the conditions under which a straight line becomes a **Tangent** to a circle.

---

### Core Concepts & Formulas

#### 1. Definition and Standard Forms
> **Circle:** The locus of a point which moves in a plane such that its distance from a fixed point (the **Center**) is always constant (the **Radius**).

* **Central Form:** For a circle with its center at the coordinates $(h, k)$ and a radius of length $r$:
> $$(x - h)^2 + (y - k)^2 = r^2$$

* **Standard Form (Center at Origin):** If the center is located exactly at the origin $O(0, 0)$, the equation simplifies to:
> $$x^2 + y^2 = r^2$$



#### 2. General Equation of a Circle
The general second-degree equation representing a circle is written as:
> $$x^2 + y^2 + 2gx + 2fy + c = 0$$

To extract its primary geometric metrics:
* **Center Coordinates:** $$(-g, -f)$$
* **Radius Length:** $$r = \sqrt{g^2 + f^2 - c}$$

*Real-World Roots Conditions:*
1. If $g^2 + f^2 - c > 0$: It represents a **Real Circle**.
2. If $g^2 + f^2 - c = 0$: It represents a **Point Circle** (a circle with radius 0 located at the center point).
3. If $g^2 + f^2 - c < 0$: It represents an **Imaginary Circle** (no real coordinate locus exists).

#### 3. Diametric Form
> If the coordinates of the two endpoints of a circle's diameter are explicitly given as $A(x_1, y_1)$ and $B(x_2, y_2)$, the equation of the circle can be directly written as:
> $$(x - x_1)(x - x_2) + (y - y_1)(y - y_2) = 0$$

#### 4. Condition of Tangency
Let a straight line be given by $y = mx + c$ and a standard circle by $x^2 + y^2 = r^2$.
For the straight line to touch the circle at exactly one single point (making it a **Tangent**), the perpendicular distance from the center $(0,0)$ to the line must be exactly equal to the radius $r$.

> **Condition of Tangency Identity:**
> $$c^2 = r^2(1 + m^2) \implies c = \pm r\sqrt{1 + m^2}$$
* Therefore, any line of the form $y = mx \pm r\sqrt{1 + m^2}$ is always a tangent to the circle $x^2 + y^2 = r^2$.

---

### Step-by-Step Examples

**Example 1:** Find the equation of the circle whose center is located at $(2, -3)$ and whose radius is $5 \text{ units}$.  
**Solution:**
1. Identify the central variables: $h = 2$, $k = -3$, and $r = 5$.
2. Substitute these variables into the Central Form equation:
$$(x - 2)^2 + [y - (-3)]^2 = 5^2$$
$$(x - 2)^2 + (y + 3)^2 = 25$$
3. Expand the algebraic binomials:
$$(x^2 - 4x + 4) + (y^2 + 6y + 9) = 25$$
4. Rearrange terms into standard descending order:
$$x^2 + y^2 - 4x + 6y + 13 - 25 = 0 \implies x^2 + y^2 - 4x + 6y - 12 = 0$$

**Example 2:** Find the center and radius of the circle given by the equation: $x^2 + y^2 - 6x + 4y - 12 = 0$.  
**Solution:**
1. Compare the given equation with the general equation $x^2 + y^2 + 2gx + 2fy + c = 0$:
   * $2g = -6 \implies g = -3$
   * $2f = 4 \implies f = 2$
   * $c = -12$
2. Find the center coordinates using $\text{Center} = (-g, -f)$:
$$\text{Center} = (-(-3), -2) = (3, -2)$$
3. Compute the radius using $r = \sqrt{g^2 + f^2 - c}$:
$$r = \sqrt{(-3)^2 + (2)^2 - (-12)}$$
$$r = \sqrt{9 + 4 + 12} = \sqrt{25} = 5 \text{ units}$$

**Example 3:** Find the equation of the circle drawn with the line segment joining $A(1, 2)$ and $B(3, 4)$ as its diameter.  
**Solution:**
1. Identify diameter coordinates: $(x_1, y_1) = (1, 2)$ and $(x_2, y_2) = (3, 4)$.
2. Substitute these numbers directly into the Diametric Form equation:
$$(x - 1)(x - 3) + (y - 2)(y - 4) = 0$$
3. Expand both products:
$$(x^2 - 4x + 3) + (y^2 - 6y + 8) = 0$$
4. Combine constants into final general order:
$$x^2 + y^2 - 4x - 6y + 11 = 0$$

---

### Terminal Exercises & Self-Check Questions

1. **Equation Verification Workout:** Find the equation of a circle centered at the origin that passes through the point $(3, 4)$.
   * *Answer Hint:* Since the center is at $O(0,0)$, use $x^2 + y^2 = r^2$. The radius squared is the distance to the given point: $r^2 = 3^2 + 4^2 = 9 + 16 = 25$. The final equation is $x^2 + y^2 = 25$.

2. **Intercept Metric Problem:** Find the equation of the circle passing through the origin and cutting off intercepts of length $6$ and $8$ from the positive x and y axes respectively.
   * *Step-by-Step Solution:* 1. The circle passes through the origin $(0,0)$, the x-intercept point $(6,0)$, and the y-intercept point $(0,8)$.
     2. Since the angle subtended by an intercept in a semi-circle is $90^\circ$, the line segment connecting $(6,0)$ and $(0,8)$ forms a diameter of the circle.
     3. Apply the diametric form: $(x - 6)(x - 0) + (y - 0)(y - 8) = 0$.
     4. Expand to find the final equation: $x^2 + y^2 - 6x - 8y = 0$.

3. **Tangency Constraint Problem:** Find the value of $c$ if the straight line $y = 2x + c$ is a tangent to the circle $x^2 + y^2 = 5$.
   * *Answer Hint:* Use the condition of tangency $c^2 = r^2(1 + m^2)$. Here, $r^2 = 5$ and $m = 2$.
     $$c^2 = 5(1 + 2^2) = 5(1 + 4) = 5(5) = 25 \implies c = \pm 5$$