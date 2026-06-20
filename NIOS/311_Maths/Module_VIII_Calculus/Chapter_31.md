# NIOS Senior Secondary Mathematics (311)

## Module VIII: Calculus
### Chapter 31: Definite Integrals

### Introduction & Key Objectives
In Chapter 30, we introduced indefinite integration, which acts as the inverse operation of differentiation and yields a family of parallel curves parameterized by an arbitrary constant $C$. In this chapter, we explore **Definite Integrals**, where the integration process is bound between two strict real numerical limits. Geometrically, a definite integral evaluates the exact net signed area enclosed between a curve and the horizontal axis. This chapter covers the Fundamental Theorem of Calculus and a set of structural properties that allow us to evaluate highly complex definite equations efficiently.

After studying this chapter, you will be able to:
* Define a **Definite Integral** and interpret its geometric meaning as an area under a curve.
* State and apply the **First and Second Fundamental Theorems of Calculus**.
* Evaluate basic definite integrals by applying boundary limits to anti-derivatives.
* Master the primary **Properties of Definite Integrals** used to simplify calculations.
* Evaluate integrals involving absolute values (modulus functions) and piecewise functions by partitioning intervals.

---

### Core Concepts & Formulas

#### 1. Geometric Interpretation & Notation
The definite integral of a continuous function $f(x)$ over the closed interval $[a, b]$ is written as:
> $$\int_{a}^{b} f(x) \, dx$$
* **$a$:** The Lower Limit of integration.
* **$b$:** The Upper Limit of integration.

Geometrically, if $f(x) \ge 0$, the integral represents the exact area of the region bounded by the curve $y = f(x)$, the x-axis, and the vertical lines $x = a$ and $x = b$. Notice that because it represents a specific physical quantity, a definite integral evaluates to a **unique numerical constant** and does not require the arbitrary constant of integration $C$.



#### 2. The Fundamental Theorem of Calculus
> **The Second Fundamental Theorem:**
> If $F(x)$ is the anti-derivative of a continuous function $f(x)$ such that $\int f(x) \, dx = F(x)$, then the definite integral is evaluated by subtracting the function value at the lower boundary from the value at the upper boundary:
> $$\int_{a}^{b} f(x) \, dx = [F(x)]_{a}^{b} = F(b) - F(a)$$

---

#### 3. Primary Properties of Definite Integrals
These structural rules are highly emphasized in public examinations for simplifying complicated integration terms:

* **Property 1 (Variable Invariance):** Changing the dummy variable of integration does not alter the value:
  $$\int_{a}^{b} f(x) \, dx = \int_{a}^{b} f(t) \, dt$$
* **Property 2 (Limits Reversal):** Interchanging the boundary integration limits changes the sign of the integral:
  $$\int_{a}^{b} f(x) \, dx = -\int_{b}^{a} f(x) \, dx$$
* **Property 3 (Interval Partitioning):** An integration interval can be broken up into a sum of sub-intervals using an intermediate point $c$:
  $$\int_{a}^{b} f(x) \, dx = \int_{a}^{c} f(x) \, dx + \int_{c}^{b} f(x) \, dx \quad (\text{where } a < c < b)$$
  *(Essential for resolving absolute value modulus or split piecewise functions).*
* **Property 4 (The Reflection Property):**
  $$\int_{a}^{b} f(x) \, dx = \int_{a}^{b} f(a + b - x) \, dx \quad \implies \int_{0}^{a} f(x) \, dx = \int_{0}^{a} f(a - x) \, dx$$
* **Property 5 (Even/Odd Functions):** For symmetric intervals around zero ($[-a, a]$):
  $$\int{-a}^{a} f(x) \, dx = \begin{cases} 2\int_{0}^{a} f(x) \, dx, & \text{if } f(x) \text{ is an Even Function } (f(-x) = f(x)) \\ 0, & \text{if } f(x) \text{ is an Odd Function } (f(-x) = -f(x)) \end{cases}$$

---

### Step-by-Step Examples

**Example 1:** Evaluate the definite integral: $\int_{1}^{3} (3x^2 + 2x) \, dx$.  
**Solution:**
1. Find the indefinite anti-derivative $F(x)$ using standard power rules:
$$F(x) = \int (3x^2 + 2x) \, dx = 3\left(\frac{x^3}{3}\right) + 2\left(\frac{x^2}{2}\right) = x^3 + x^2$$
2. Apply the Fundamental Theorem of Calculus across the boundary values $[1, 3]$:
$$\int_{1}^{3} (3x^2 + 2x) \, dx = [x^3 + x^2]_{1}^{3}$$
3. Substitute the upper limit ($x = 3$):
$$F(3) = (3)^3 + (3)^2 = 27 + 9 = 36$$
4. Substitute the lower limit ($x = 1$):
$$F(1) = (1)^3 + (1)^2 = 1 + 1 = 2$$
5. Perform the final subtraction:
$$\text{Output} = F(3) - F(1) = 36 - 2 = 34$$

**Example 2:** Evaluate the absolute value modulus integral: $\int_{1}^{4} |x - 2| \, dx$.  
**Solution:**
1. Identify the critical turning point where the modulus function changes its algebraic behavior: $x - 2 = 0 \implies x = 2$.
2. Define the piece-wise nature of the function around $x = 2$:
$$|x - 2| = \begin{cases} -(x - 2) = 2 - x, & \text{if } x < 2 \\ x - 2, & \text{if } x \ge 2 \end{cases}$$
3. Use the **Interval Partitioning Property** to split the integral at $x = 2$:
$$\int_{1}^{4} |x - 2| \, dx = \int_{1}^{2} (2 - x) \, dx + \int_{2}^{4} (x - 2) \, dx$$
4. Integrate each section independently:
   * **First Section:** $\left[ 2x - \frac{x^2}{2} \right]_{1}^{2} = \left( 2(2) - \frac{2^2}{2} \right) - \left( 2(1) - \frac{1^2}{2} \right) = (4 - 2) - (2 - 0.5) = 2 - 1.5 = 0.5$
   * **Second Section:** $\left[ \frac{x^2}{2} - 2x \right]_{2}^{4} = \left( \frac{4^2}{2} - 2(4) \right) - \left( \frac{2^2}{2} - 2(2) \right) = (8 - 8) - (2 - 4) = 0 - (-2) = 2$
5. Add the values from both sections together:
$$\text{Total Output} = 0.5 + 2 = 2.5 \quad (\text{or } \frac{5}{2})$$

**Example 3:** Evaluate the complex trigonometric integral: $I = \int_{0}^{\pi/2} \frac{\sin x}{\sin x + \cos x} \, dx$.  
**Solution:**
1. Let the original equation layout be labeled as **Equation 1**:
$$I = \int_{0}^{\pi/2} \frac{\sin x}{\sin x + \cos x} \, dx \quad \text{--- (Equation 1)}$$
2. Apply the reflection property $\int_{0}^{a} f(x) \, dx = \int_{0}^{a} f(a - x) \, dx$ by replacing $x$ with $\left(\frac{\pi}{2} - x\right)$:
$$I = \int_{0}^{\pi/2} \frac{\sin(\frac{\pi}{2} - x)}{\sin(\frac{\pi}{2} - x) + \cos(\frac{\pi}{2} - x)} \, dx$$
3. Simplify using standard complementary trigonometric identities ($\sin(\frac{\pi}{2}-x) = \cos x$ and $\cos(\frac{\pi}{2}-x) = \sin x$):
$$I = \int_{0}^{\pi/2} \frac{\cos x}{\cos x + \sin x} \, dx \quad \text{--- (Equation 2)}$$
4. Add Equation 1 and Equation 2 together:
$$2I = \int_{0}^{\pi/2} \frac{\sin x}{\sin x + \cos x} \, dx + \int_{0}^{\pi/2} \frac{\cos x}{\sin x + \cos x} \, dx$$
$$2I = \int_{0}^{\pi/2} \frac{\sin x + \cos x}{\sin x + \cos x} \, dx = \int_{0}^{\pi/2} 1 \, dx$$
5. Evaluate the simplified integration:
$$2I = [x]_{0}^{\pi/2} = \frac{\pi}{2} - 0 = \frac{\pi}{2}$$
6. Isolate $I$ by dividing by 2:
$$I = \frac{\pi}{4}$$

---

### Terminal Exercises & Self-Check Questions

1. **Exponential Evaluation Exercise:** Evaluate the definite boundary integral: $\int_{0}^{1} e^{2x} \, dx$.
   * *Answer Hint:* The anti-derivative is $\frac{e^{2x}}{2}$. Substitute limits:
     $$\text{Output} = \left[ \frac{e^{2x}}{2} \right]_{0}^{1} = \frac{e^{2(1)}}{2} - \frac{e^{2(0)}}{2} = \frac{e^2 - 1}{2}$$

2. **Odd Function Property Problem:** Without expanding, find the exact numerical value of $\int_{-\pi}^{\pi} \sin^5 x \, dx$.
   * *Step-by-Step Solution:* 1. Check the symmetry of the interval: it is bound from $-a$ to $+a$ where $a = \pi$.
     2. Identify the nature of the function: let $f(x) = \sin^5 x$.
     3. Test for even/odd structure: $f(-x) = \sin^5(-x) = (-\sin x)^5 = -\sin^5 x = -f(x)$.
     4. Since $f(-x) = -f(x)$, the integrand is an **Odd Function**.
     5. By Property 5, the definite integral of any odd function over a symmetric interval around zero is exactly **0**.

3. **Logarithmic Property Application:** Find the value of $\int_{0}^{\pi/2} \log_e(\tan x) \, dx$.
   * *Answer Hint:* Apply the reflection rule to get $I = \int_{0}^{\pi/2} \log_e(\cot x) \, dx$. Add both forms together: $2I = \int_{0}^{\pi/2} [\log_e(\tan x) + \log_e(\cot x)] \, dx$. Apply logarithmic product rules: $\log(\tan x \cdot \cot x) = \log(1) = 0$. Therefore, $2I = 0 \implies I = 0$.