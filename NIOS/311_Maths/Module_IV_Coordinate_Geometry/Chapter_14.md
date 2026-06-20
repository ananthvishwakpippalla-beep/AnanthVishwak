# Module IV — Co-ordinate Geometry

# NIOS Senior Secondary Mathematics (311)

## Chapter 14: Straight Lines

### Introduction & Key Objectives
A straight line is the simplest geometric locus on a coordinate plane. Geometrically, it represents the shortest path connecting two points; algebraically, it is represented by a first-degree linear equation in two variables ($x$ and $y$). Understanding the equations of straight lines is crucial for linear programming, calculus optimization, and coordinate geometry.

After studying this chapter, you will be able to:
* Calculate the **Slope (Gradient)** of a straight line given its inclination or two coordinates.
* Understand the conditions for lines to be **parallel** or **perpendicular** based on their slopes.
* Find the **angle** between two intersecting straight lines.
* Write down the equation of a line across various standard formats (**Slope-Intercept**, **Point-Slope**, **Two-Point**, **Intercept**, and **Normal** forms).
* Convert a general linear equation ($Ax + By + C = 0$) into standard forms.
* Calculate the **perpendicular distance** from a point to a line and the distance between parallel lines.

---

### Core Concepts & Formulas

#### 1. Slope (Gradient) of a Line
The slope $m$ measures the steepness and directional orientation of a line.
* If a line makes an angle of inclination $\theta$ with the positive direction of the x-axis (measured counter-clockwise):
> $$m = \tan\theta \quad (\theta \neq 90^\circ)$$
* If a line passes through two specified coordinates $P(x_1, y_1)$ and $Q(x_2, y_2)$:
> $$m = \frac{y_2 - y_1}{x_2 - x_1}$$

#### 2. Parallel and Perpendicular Slope Conditions
Let two lines have slopes $m_1$ and $m_2$:
* **Parallel Lines ($\parallel$):** They have identical inclinations, so their slopes must be equal.
> $$m_1 = m_2$$
* **Perpendicular Lines ($\perp$):** The product of their slopes equals $-1$ (negative reciprocals).
> $$m_1 \cdot m_2 = -1 \implies m_2 = -\frac{1}{m_1}$$

#### 3. Angle Between Intersecting Lines
The acute angle $\theta$ between two intersecting straight lines with known slopes $m_1$ and $m_2$ is given by:
> $$\tan\theta = \left| \frac{m_2 - m_1}{1 + m_1 m_2} \right|$$



#### 4. Standard Forms of the Equation of a Straight Line
* **Slope-Intercept Form:** Given slope $m$ and y-intercept $c$.
  $$y = mx + c$$
* **Point-Slope Form:** Given slope $m$ and passing through a fixed point $(x_1, y_1)$.
  $$y - y_1 = m(x - x_1)$$
* **Two-Point Form:** Passing through two distinct coordinates $(x_1, y_1)$ and $(x_2, y_2)$.
  $$y - y_1 = \frac{y_2 - y_1}{x_2 - x_1}(x - x_1)$$
* **Intercept Form:** Cutting the x-axis at $(a,0)$ and y-axis at $(0,b)$.
  $$\frac{x}{a} + \frac{y}{b} = 1$$
* **Normal Form:** Given the perpendicular distance $p$ from the origin to the line, where this perpendicular makes an angle $\alpha$ with the positive x-axis.
  $$x\cos\alpha + y\sin\alpha = p$$

#### 5. Distance and Metric Rules
The general equation of a straight line is always expressed as: $Ax + By + C = 0$.
> **Perpendicular Distance from a Point $P(x_1, y_1)$ to a Line:**
> $$d = \frac{|Ax_1 + By_1 + C|}{\sqrt{A^2 + B^2}}$$
> **Distance Between Two Parallel Lines ($Ax + By + C_1 = 0$ and $Ax + By + C_2 = 0$):**
> $$d = \frac{|C_1 - C_2|}{\sqrt{A^2 + B^2}}$$

---

### Step-by-Step Examples

**Example 1:** Find the equation of the straight line passing through the points $A(2, 5)$ and $B(4, 9)$.  
**Solution:**
1. Identify the given endpoints: $(x_1, y_1) = (2, 5)$ and $(x_2, y_2) = (4, 9)$.
2. Calculate the slope $m$ using the two-point gradient rule:
$$m = \frac{9 - 5}{4 - 2} = \frac{4}{2} = 2$$
3. Use the point-slope form with the first point $A(2,5)$:
$$y - 5 = 2(x - 2)$$
4. Expand and simplify into general linear form:
$$y - 5 = 2x - 4 \implies 2x - y + 1 = 0$$

**Example 2:** Find the acute angle between the two lines given by equations $y = 3x + 5$ and $y = \frac{1}{2}x - 2$.  
**Solution:**
1. Extract the individual slopes directly from their slope-intercept profiles ($y=mx+c$):
   * First slope $m_1 = 3$
   * Second slope $m_2 = \frac{1}{2}$
2. Substitute these slopes into the angle tangent formula:
$$\tan\theta = \left| \frac{\frac{1}{2} - 3}{1 + 3\left(\frac{1}{2}\right)} \right| = \left| \frac{-\frac{5}{2}}{1 + \frac{3}{2}} \right| = \left| \frac{-\frac{5}{2}}{\frac{5}{2}} \right| = |-1| = 1$$
3. Since $\tan\theta = 1$, the acute angle is:
$$\theta = \tan^{-1}(1) = 45^\circ \text{ (or } \frac{\pi}{4} \text{ radians)}$$

**Example 3:** Find the perpendicular distance from the point $P(2, 3)$ to the line $3x + 4y - 8 = 0$.  
**Solution:**
1. Identify parameters: $A = 3$, $B = 4$, $C = -8$, and the target point $(x_1, y_1) = (2, 3)$.
2. Substitute these numbers directly into the perpendicular distance formula:
$$d = \frac{|3(2) + 4(3) - 8|}{\sqrt{3^2 + 4^2}}$$
3. Simplify the numerator and denominator:
$$d = \frac{|6 + 12 - 8|}{\sqrt{9 + 16}} = \frac{|10|}{\sqrt{25}} = \frac{10}{5} = 2 \text{ units}$$

---

### Terminal Exercises & Self-Check Questions

1. **Slope Conditioning:** Find the equation of a straight line passing through the point $(3, -2)$ and perpendicular to the line $x - 2y + 4 = 0$.
   * *Answer Hint:* Convert the target reference line to find its baseline slope: $2y = x + 4 \implies y = \frac{1}{2}x + 2$, so $m_{\text{ref}} = \frac{1}{2}$. The perpendicular line must have a slope $m = -1 / (\frac{1}{2}) = -2$. Apply the point-slope form: $y - (-2) = -2(x - 3) \implies y + 2 = -2x + 6 \implies 2x + y - 4 = 0$.

2. **Intercept Extraction Workout:** Find the x and y intercepts cut off by the line $4x - 3y + 12 = 0$.
   * *Step-by-Step Solution:* 1. Move the constant to the right-hand side: $4x - 3y = -12$.
     2. Divide the entire equation by $-12$ to set the right side to 1: $\frac{4x}{-12} - \frac{3y}{-12} = 1$.
     3. Simplify terms into intercept form ($\frac{x}{a} + \frac{y}{b} = 1$): $\frac{x}{-3} + \frac{y}{4} = 1$.
     4. The x-intercept is $a = -3$, and the y-intercept is $b = 4$.

3. **Parallel Metric Tracking:** Calculate the exact shortest distance separating the parallel lines $5x + 12y - 7 = 0$ and $5x + 12y + 19 = 0$.
   * *Answer Hint:* Use $d = \frac{|C_1 - C_2|}{\sqrt{A^2 + B^2}}$. Here, $C_1 = -7$, $C_2 = 19$, $A = 5$, $B = 12$.
     $$d = \frac{|-7 - 19|}{\sqrt{5^2 + 12^2}} = \frac{|-26|}{\sqrt{25 + 144}} = \frac{26}{\sqrt{169}} = \frac{26}{13} = 2 \text{ units}$$
