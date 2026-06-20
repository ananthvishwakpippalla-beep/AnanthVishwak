# NIOS Senior Secondary Mathematics (311)

## Module VIII: Calculus
### Chapter 25: Limits and Continuity

### Introduction & Key Objectives
Calculus is the mathematical study of continuous change. The absolute cornerstone of all calculus—including differentiation and integration—is the concept of a **Limit**. In elementary algebra, we evaluate functions at exact, static values (e.g., what is $f(x)$ when $x = 2$). Limits allow us to analyze dynamic behavior *near* a point, observing what value a function approaches as the input gets infinitely close to a boundary value. This chapter formalizes limits and explores **Continuity**, which mathematically describes unbroken paths and surfaces.

After studying this chapter, you will be able to:
* Understand the intuitive and formal meaning of a **Limit**.
* Evaluate **Left-Hand Limits (LHL)** and **Right-Hand Limits (RHL)** to determine if a limit exists.
* Apply core algebraic limit theorems to evaluate indeterminate forms ($\frac{0}{0}$).
* Recognize and use standard standard limit theorems (algebraic and trigonometric).
* Define **Continuity** at a specific point and over an interval, and test functions for points of discontinuity.

---

### Core Concepts & Formulas

#### 1. Intuitive Definition and Existence of a Limit
Let $f(x)$ be a function defined in an open interval around a real number $a$ (though not necessarily at $a$ itself). We say that the limit of $f(x)$ as $x$ approaches $a$ is the finite real number $L$:
$$\lim_{x \to a} f(x) = L$$
This statement is true if and only if both one-sided approaches converge onto the exact same finite value:

> **Criteria for Existence of a Limit:**
> * **Left-Hand Limit (LHL):** The value approached by $f(x)$ as $x$ moves toward $a$ from values strictly smaller than $a$.
>   $$\text{LHL} = \lim_{x \to a^-} f(x) = \lim_{h \to 0} f(a - h) \quad (h > 0)$$
> * **Right-Hand Limit (RHL):** The value approached by $f(x)$ as $x$ moves toward $a$ from values strictly larger than $a$.
>   $$\text{RHL} = \lim_{x \to a^+} f(x) = \lim_{h \to 0} f(a + h) \quad (h > 0)$$
> $$\lim_{x \to a} f(x) \text{ exists} \iff \text{LHL} = \text{RHL} = L$$



#### 2. Core Theorems on Limits
If $\lim_{x \to a} f(x) = L$ and $\lim_{x \to a} g(x) = M$, then:
* **Sum/Difference Rule:** $\lim_{x \to a} [f(x) \pm g(x)] = L \pm M$
* **Product Rule:** $\lim_{x \to a} [f(x) \cdot g(x)] = L \cdot M$
* **Quotient Rule:** $\lim_{x \to a} \left[\frac{f(x)}{g(x)}\right] = \frac{L}{M} \quad (\text{provided } M \neq 0)$
* **Constant Multiplier Rule:** $\lim_{x \to a} [c \cdot f(x)] = c \cdot L$

#### 3. Standard Standard Limit Identites
These formulas are heavily utilized to quickly resolve limits across public examinations:

> **Algebraic Standard Form:**
> $$\lim_{x \to a} \frac{x^n - a^n}{x - a} = n \cdot a^{n-1}$$

> **Trigonometric Standard Forms (Angles strictly in Radians):**
> * $$\lim_{\theta \to 0} \frac{\sin\theta}{\theta} = 1$$
> * $$\lim_{\theta \to 0} \frac{\tan\theta}{\theta} = 1$$
> * $$\lim_{\theta \to 0} \cos\theta = 1$$

---

#### 4. Continuity of a Function
In simple terms, a function is continuous if you can draw its graph completely without lifting your pen from the paper. 

> **Formal Definition of Continuity at a Point:**
> A function $f(x)$ is continuous at a specific point $x = a$ if and only if it satisfies three strict criteria:
> 1. $f(a)$ is completely defined (meaning $a$ lies within the domain of the function).
> 2. $\lim_{x \to a} f(x)$ exists (meaning $\text{LHL} = \text{RHL}$).
> 3. The limit value matches the exact value of the function at that point:
>    $$\lim_{x \to a} f(x) = f(a)$$



If any of these conditions are violated, the function is said to be **discontinuous** at $x = a$.

---

### Step-by-Step Examples

**Example 1:** Evaluate the limit: $\lim_{x \to 2} \frac{x^2 - 4}{x - 2}$.  
**Solution:**
1. Test for direct substitution: Substituting $x = 2$ directly into the expression yields $\frac{2^2 - 4}{2 - 2} = \frac{0}{0}$, which is an **indeterminate form**. We must manipulate the algebra.
2. Factorize the numerator using the difference of squares identity ($a^2 - b^2 = (a-b)(a+b)$):
$$x^2 - 4 = (x - 2)(x + 2)$$
3. Rewrite the limit expression and cancel out the common factor $(x - 2)$ (this is valid because as $x \to 2$, $x \neq 2$, so $x - 2 \neq 0$):
$$\lim_{x \to 2} \frac{(x - 2)(x + 2)}{x - 2} = \lim_{x \to 2} (x + 2)$$
4. Now substitute $x = 2$ safely into the simplified expression:
$$\text{Limit Value} = 2 + 2 = 4$$

**Example 2:** Evaluate the trigonometric limit: $\lim_{x \to 0} \frac{\sin 5x}{3x}$.  
**Solution:**
1. Observe that direct substitution yields the indeterminate form $\frac{0}{0}$.
2. To apply the standard identity $\lim_{\theta \to 0} \frac{\sin\theta}{\theta} = 1$, the expression inside the sine function must match the denominator exactly.
3. Multiply and divide the expression by $5$ to structurally adjust the denominator:
$$\lim_{x \to 0} \frac{\sin 5x}{3x} = \lim_{x \to 0} \left( \frac{\sin 5x}{5x} \times \frac{5}{3} \right)$$
4. Pull out the constant fraction factor $\frac{5}{3}$ using limit theorems:
$$= \frac{5}{3} \times \lim_{x \to 0} \left( \frac{\sin 5x}{5x} \right)$$
5. As $x \to 0$, it follows that $5x \to 0$. Apply the standard identity:
$$= \frac{5}{3} \times 1 = \frac{5}{3}$$

**Example 3:** Discuss the continuity of the following function at $x = 2$:
$$f(x) = \begin{cases} 2x + 3, & \text{if } x \le 2 \\ x^2 + 3, & \text{if } x > 2 \end{cases}$$

**Solution:**
1. Find the exact value of the function at the boundary point using the inequality rule ($x \le 2$):
$$f(2) = 2(2) + 3 = 4 + 3 = 7$$
2. Calculate the Left-Hand Limit ($\text{LHL}$):
$$\text{LHL} = \lim_{x \to 2^-} f(x) = \lim_{x \to 2} (2x + 3) = 2(2) + 3 = 7$$
3. Calculate the Right-Hand Limit ($\text{RHL}$):
$$\text{RHL} = \lim_{x \to 2^+} f(x) = \lim_{x \to 2} (x^2 + 3) = 2^2 + 3 = 4 + 3 = 7$$
4. Check the continuity criteria: Since $\text{LHL} = \text{RHL} = 7$, the limit exists and $\lim_{x \to 2} f(x) = 7$.
5. Finally, observe that $\lim_{x \to 2} f(x) = f(2) = 7$.
6. Conclusion: The function satisfies all conditions and is strictly **continuous** at $x = 2$.

---

### Terminal Exercises & Self-Check Questions

1. **Standard Algebraic Form Workout:** Evaluate the limit: $\lim_{x \to 3} \frac{x^4 - 81}{x - 3}$.
   * *Answer Hint:* Rewrite 81 as $3^4$. The expression matches the standard profile $\lim_{x \to a} \frac{x^n - a^n}{x - a}$ where $n = 4$ and $a = 3$.
     $$\text{Output} = n \cdot a^{n-1} = 4 \cdot 3^{4-1} = 4 \cdot 3^3 = 4 \times 27 = 108$$

2. **Trigonometric Expression Problem:** Evaluate the limit: $\lim_{x \to 0} \frac{1 - \cos x}{x^2}$.
   * *Step-by-Step Solution:* 1. Substitute the trigonometric identity $1 - \cos x = 2\sin^2\left(\frac{x}{2}\right)$:
        $$\lim_{x \to 0} \frac{2\sin^2(x/2)}{x^2}$$
     2. Adjust the denominator to match the square fraction template $\left[\frac{\sin(x/2)}{x/2}\right]^2$:
        $$= \lim_{x \to 0} \frac{2\sin^2(x/2)}{4 \cdot (x/2)^2} = \frac{2}{4} \times \lim_{x \to 0} \left[ \frac{\sin(x/2)}{x/2} \right]^2$$
     3. Apply the core standard limit value: $\frac{1}{2} \times (1)^2 = \frac{1}{2}$.

3. **Continuity Optimization Problem:** Find the value of constant $k$ if the function $f(x) = \begin{cases} kx + 1, & \text{if } x \le 5 \\ 3x - 5, & \text{if } x > 5 \end{cases}$ is given as continuous at $x = 5$.
   * *Answer Hint:* For continuity, $\text{LHL} = \text{RHL} \implies \lim_{x \to 5^-} (kx + 1) = \lim_{x \to 5^+} (3x - 5)$. 
     Evaluate limits: $5k + 1 = 3(5) - 5 \implies 5k + 1 = 15 - 5 \implies 5k + 1 = 10 \implies 5k = 9 \implies k = \frac{9}{5}$.