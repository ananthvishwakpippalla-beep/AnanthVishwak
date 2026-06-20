# NIOS Senior Secondary Mathematics (311)

## Module VIII: Calculus
### Chapter 29: Application of Derivatives

### Introduction & Key Objectives
In the preceding chapters of this module, we mastered the core operational mechanics of differentiation across algebraic, trigonometric, exponential, and logarithmic expressions. In this chapter, we transition from pure computation to real-world applications. By treating the derivative $\frac{dy}{dx}$ as an instantaneous rate-of-change engine, we can geometrically locate the exact pathways of **Tangents and Normals**, determine whether a function is climbing or falling (**Increasing and Decreasing Functions**), and optimize systems to locate absolute limits via **Maxima and Minima**.

After studying this chapter, you will be able to:
* Calculate the **Rate of Change** of varying geometric and physical quantities.
* Find the equations of the **Tangent** and **Normal** to a curve at a given point.
* Identify intervals in which a function is strictly **Increasing** or **Decreasing**.
* Locate turning points and apply the **First and Second Derivative Tests** to find local **Maxima and Minima**.
* Solve real-world optimization problems (maximizing area, minimizing costs, etc.).

---

### Core Concepts & Formulas

#### 1. Rate of Change of Quantities
If a variable $y$ varies continuously with respect to another variable $x$, the derivative $\frac{dy}{dx}$ represents the instantaneous rate of change of $y$ with respect to $x$. 
* If two variables $x$ and $y$ are both changing with respect to a time parameter $t$, we link them using the Chain Rule:
> $$\frac{dy}{dt} = \frac{dy}{dx} \times \frac{dx}{dt}$$

#### 2. Tangents and Normals to a Curve
Let a curve be defined by $y = f(x)$, and let $P(x_1, y_1)$ be a specific target point lying on this curve.



* **Slope of Tangent ($m_t$):** Evaluated by finding the numerical value of the derivative at that specific coordinate point:
> $$m_t = \left[ \frac{dy}{dx} \right]_{(x_1, y_1)} = f'(x_1)$$
* **Slope of Normal ($m_n$):** Since the normal line is strictly perpendicular to the tangent line, its slope is the negative reciprocal ($m_t \cdot m_n = -1$):
> $$m_n = -\frac{1}{m_t} = -\frac{1}{f'(x_1)} \quad (\text{if } f'(x_1) \neq 0)$$

> **Equations of Lines (Using Point-Slope Form):**
> * **Equation of Tangent:** $$y - y_1 = m_t(x - x_1)$$
> * **Equation of Normal:** $$y - y_1 = m_n(x - x_1) \implies y - y_1 = -\frac{1}{f'(x_1)}(x - x_1)$$

---

#### 3. Increasing and Decreasing Functions
Let $f(x)$ be a continuous function differentiable on an open interval $(a, b)$:
* **Strictly Increasing:** The function climbs steadily from left to right. Its tangent slope is consistently positive:
> $$f'(x) > 0 \quad \text{for all } x \in (a, b)$$
* **Strictly Decreasing:** The function falls steadily from left to right. Its tangent slope is consistently negative:
> $$f'(x) < 0 \quad \text{for all } x \in (a, b)$$

---

#### 4. Maxima and Minima (Optimization)
Points where a smooth curve peaks or bottoms out are called local maximum or minimum turning points. At these local extrema, the tangent line becomes completely horizontal, meaning the first derivative is zero.

> **Critical Points Condition:** Points in the domain where $f'(x) = 0$ are called **Critical Points** (or stationary points).

To verify whether a critical point $x = c$ is a maximum or a minimum, we use the **Second Derivative Test** (highly emphasized in exams):



> **The Second Derivative Test Protocol:**
> 1. Find $f'(x)$ and solve the equation $f'(x) = 0$ to extract the critical values ($x = c$).
> 2. Calculate the second derivative: $f''(x) = \frac{d^2y}{dx^2}$.
> 3. Substitute the critical value $c$ into the second derivative:
>    * **If $f''(c) < 0$:** The curve is concave down. Therefore, $x = c$ is a point of **Local Maximum**.
>    * **If $f''(c) > 0$:** The curve is concave up. Therefore, $x = c$ is a point of **Local Minimum**.
>    * **If $f''(c) = 0$:** The test fails. You must revert to the First Derivative Test to check sign changes around $c$.

---

### Step-by-Step Examples

**Example 1:** The radius of a circular metal plate is expanding uniformly at a rate of $3 \text{ cm/s}$. Find the rate at which the total area of the plate is increasing when the radius is exactly $10 \text{ cm}$.  
**Solution:**
1. State the given rates and geometric equations:
   * Rate of radius growth: $\frac{dr}{dt} = 3 \text{ cm/s}$
   * Target radius condition: $r = 10 \text{ cm}$
   * Area of a circle: $A = \pi r^2$
2. Differentiate the area formula with respect to time ($t$) using the Chain Rule:
$$\frac{dA}{dt} = \frac{d}{dt}(\pi r^2) = \pi \cdot (2r) \cdot \frac{dr}{dt} = 2\pi r \frac{dr}{dt}$$
3. Substitute the known parameters into the rate equation:
$$\frac{dA}{dt} = 2 \cdot \pi \cdot (10) \cdot (3) = 60\pi$$
4. Conclusion: The area of the plate is increasing at a rate of **$60\pi \text{ cm}^2\text{/s}$**.

**Example 2:** Find the equations of the tangent and normal to the curve $y = x^3 - 2x + 5$ at the coordinate point $P(2, 9)$.  
**Solution:**
1. Compute the first derivative to establish a general slope equation:
$$\frac{dy}{dx} = \frac{d}{dx}(x^3 - 2x + 5) = 3x^2 - 2$$
2. Evaluate the precise slope of the tangent ($m_t$) at the point $P(2,9)$ by substituting $x = 2$:
$$m_t = 3(2)^2 - 2 = 3(4) - 2 = 12 - 2 = 10$$
3. Compute the perpendicular slope of the normal ($m_n$):
$$m_n = -\frac{1}{m_t} = -\frac{1}{10}$$
4. Formulate the equation of the tangent line using point-slope form ($y - y_1 = m_t(x - x_1)$):
$$y - 9 = 10(x - 2) \implies y - 9 = 10x - 20 \implies 10x - y - 11 = 0$$
5. Formulate the equation of the normal line using point-slope form ($y - y_1 = m_n(x - x_1)$):
$$y - 9 = -\frac{1}{10}(x - 2) \implies 10(y - 9) = -(x - 2)$$
$$10y - 90 = -x + 2 \implies x + 10y - 92 = 0$$

**Example 3:** Find two positive numbers whose sum is 15 and the square of one multiplied by the other is a maximum.  
**Solution:**
1. Let the two positive numbers be $x$ and $y$. We are given their sum constraint:
$$x + y = 15 \implies y = 15 - x$$
2. Set up the function $P(x)$ to be maximized (the product of the square of one number and the other):
$$P(x) = x^2 \cdot y = x^2(15 - x) = 15x^2 - x^3$$
3. Find the first derivative $P'(x)$ and set it to zero to isolate critical values:
$$P'(x) = \frac{d}{dx}(15x^2 - x^3) = 30x - 3x^2$$
$$30x - 3x^2 = 0 \implies 3x(10 - x) = 0 \implies x = 0 \text{ or } x = 10$$
Since the numbers must be positive, choose the critical point $x = 10$.
4. Apply the second derivative test to confirm it is a maximum:
$$P''(x) = \frac{d}{dx}(30x - 3x^2) = 30 - 6x$$
$$P''(10) = 30 - 6(10) = 30 - 60 = -30$$
Since $P''(10) = -30 < 0$, the function achieves a local maximum at $x = 10$.
5. Compute the corresponding value for $y$:
$$y = 15 - 10 = 5$$
6. Conclusion: The two required numbers are **10 and 5**.

---

### Terminal Exercises & Self-Check Questions

1. **Increasing Interval Workout:** Determine the real number intervals in which the function $f(x) = 2x^2 - 4x + 7$ is strictly increasing.
   * *Answer Hint:* Find the first derivative: $f'(x) = 4x - 4$. For the function to be strictly increasing, set $f'(x) > 0 \implies 4x - 4 > 0 \implies 4x > 4 \implies x > 1$. Therefore, the function is strictly increasing on the interval **$(1, \infty)$**.

2. **Parallel Tangent Condition:** Find the points on the curve $y = x^2 - 4x + 5$ where the tangent line is completely parallel to the x-axis.
   * *Step-by-Step Solution:* 1. A line parallel to the x-axis has a slope of zero ($m = 0$).
     2. Differentiate the curve equation: $\frac{dy}{dx} = 2x - 4$.
     3. Equate the derivative to the target slope: $2x - 4 = 0 \implies 2x = 4 \implies x = 2$.
     4. Substitute $x=2$ back into the original curve equation to find the corresponding y-coordinate: $y = 2^2 - 4(2) + 5 = 4 - 8 + 5 = 1$.
     5. The required coordinate point is **$(2, 1)$**.

3. **Optimization Cost Tracking:** Divide the number 20 into two parts such that the sum of their squares is a minimum value.
   * *Answer Hint:* Let the parts be $x$ and $(20-x)$. Form the function $S(x) = x^2 + (20-x)^2 = x^2 + 400 - 40x + x^2 = 2x^2 - 40x + 400$. Find the derivative: $S'(x) = 4x - 40$. Set it to zero: $4x - 40 = 0 \implies x = 10$. Check second derivative: $S''(x) = 4 > 0$ (confirming a minimum). The two parts are **10 and 10**.