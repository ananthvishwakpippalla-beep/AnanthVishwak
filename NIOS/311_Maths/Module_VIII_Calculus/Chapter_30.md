# NIOS Senior Secondary Mathematics (311)

## Module VIII: Calculus
### Chapter 30: Integration

### Introduction & Key Objectives
In the preceding chapters, we focused on differential calculus—the process of breaking down a function to find its instantaneous rate of change (the derivative). In this chapter, we introduce **Integral Calculus**, which is fundamentally the reverse operation of differentiation. Historically, integration arose from the geometric problem of finding the exact area bounded by curved shapes. This chapter introduces **Indefinite Integration**, establishing standard algebraic tracking forms, substitution methods, and structural integration rules heavily emphasized in examinations.

After studying this chapter, you will be able to:
* Define **Integration** as the inverse process of differentiation (Anti-derivative).
* Understand the role of the **Constant of Integration ($C$)**.
* Master standard integration formulas for algebraic, trigonometric, and exponential functions.
* Apply properties of integrals (Sum, Difference, and Scalar Multiples).
* Solve complex integrals using the **Method of Substitution**.
* Apply the method of **Integration by Parts** for products of two functions.
* Integrate rational functions using **Partial Fractions**.

---

### Core Concepts & Formulas

#### 1. Integration as the Inverse of Differentiation
If the derivative of a function $F(x)$ is $f(x)$, then the anti-derivative or **integral** of $f(x)$ with respect to $x$ is written as:
> $$\frac{d}{dx}[F(x)] = f(x) \iff \int f(x) \, dx = F(x) + C$$

* **The Integrand:** The function $f(x)$ being integrated.
* **Constant of Integration ($C$):** Since the derivative of any constant is zero ($\frac{d}{dx}[F(x) + C] = f(x)$), an indefinite integral always includes an arbitrary constant $C$ to represent the entire family of parallel curves.

#### 2. Master Table of Standard Integrals
By reversing our standard derivative identities, we establish the core baseline integration formulas:

> **Algebraic Integrals:**
> * **The Power Rule:** $$\int x^n \, dx = \frac{x^{n+1}}{n+1} + C \quad (n \neq -1)$$
> * $$\int \frac{1}{x} \, dx = \log_e |x| + C$$

> **Trigonometric Integrals:**
> * $$\int \sin x \, dx = -\cos x + C$$
> * $$\int \cos x \, dx = \sin x + C$$
> * $$\int \sec^2 x \, dx = \tan x + C$$
> * $$\int \csc^2 x \, dx = -\cot x + C$$
> * $$\int \sec x \tan x \, dx = \sec x + C$$
> * $$\int \csc x \cot x \, dx = -\csc x + C$$

> **Exponential Integrals:**
> * $$\int e^x \, dx = e^x + C$$
> * $$\int a^x \, dx = \frac{a^x}{\log_e a} + C$$

---

#### 3. Core Methods of Advanced Integration

##### A. Method of Substitution
When an integrand contains a function along with its internal derivative, we simplify it by substituting a new variable $t$:
$$\int f(g(x)) \cdot f'(x) \, dx$$
Let $g(x) = t \implies f'(x) \, dx = dt$. The integral transforms cleanly into $\int f(t) \, dt$.

##### B. Integration by Parts (Product Rule for Integrals)
When integrating the product of two distinct functions, we apply the integration by parts formula:
> $$\int (u \cdot v) \, dx = u \int v \, dx - \int \left[ \frac{du}{dx} \cdot \int v \, dx \right] dx$$

* **ILATE Rule:** To decide which function to treat as the first function ($u$), follow the priority order of this acronym:
  1. **I** - Inverse Trigonometric (e.g., $\sin^{-1}x$)
  2. **L** - Logarithmic (e.g., $\log x$)
  3. **A** - Algebraic (e.g., $x^2, 3x$)
  4. **T** - Trigonometric (e.g., $\sin x, \cos x$)
  5. **E** - Exponential (e.g., $e^x$)

##### C. Integration using Partial Fractions
If the integrand is a rational fraction $\frac{P(x)}{Q(x)}$ where the degree of the numerator polynomial is less than the denominator, we break it down into simpler linear or quadratic fractional sums before integrating:
$$\frac{1}{(x-a)(x-b)} = \frac{A}{x-a} + \frac{B}{x-b}$$

---

### Step-by-Step Examples

**Example 1:** Evaluate the algebraic integral: $\int (3x^5 - 2x^2 + 5) \, dx$.  
**Solution:**
1. Split the expression term-by-term using standard linearity properties:
$$\int (3x^5 - 2x^2 + 5) \, dx = 3\int x^5 \, dx - 2\int x^2 \, dx + 5\int 1 \, dx$$
2. Apply the Power Rule ($\frac{x^{n+1}}{n+1}$) individually to each term:
   * $\int x^5 \, dx = \frac{x^6}{6}$
   * $\int x^2 \, dx = \frac{x^3}{3}$
   * $\int 1 \, dx = x$
3. Combine the expressions and add the final shared constant $C$:
$$\text{Output} = 3\left(\frac{x^6}{6}\right) - 2\left(\frac{x^3}{3}\right) + 5x + C$$
$$\text{Output} = \frac{x^6}{2} - \frac{2x^3}{3} + 5x + C$$

**Example 2:** Evaluate the integral using substitution: $\int 2x \cos(x^2 + 1) \, dx$.  
**Solution:**
1. Notice that the derivative of the inner angle $(x^2 + 1)$ is exactly $2x$, which is present outside as a multiplier. Let's substitute a placeholder variable $t$:
$$t = x^2 + 1$$
2. Differentiate both sides to find the differential mapping:
$$\frac{dt}{dx} = 2x \implies dt = 2x \, dx$$
3. Substitute $t$ and $dt$ back into the original integral expression:
$$\int 2x \cos(x^2 + 1) \, dx = \int \cos(t) \, dt$$
4. Integrate using standard trigonometric rules:
$$\int \cos(t) \, dt = \sin(t) + C$$
5. Substitute the original expression for $t$ back to find the final answer in terms of $x$:
$$\text{Output} = \sin(x^2 + 1) + C$$

**Example 3:** Evaluate the integral using integration by parts: $\int x \log_e x \, dx$.  
**Solution:**
1. Identify the functions using the **ILATE** priority rule:
   * Logarithmic function $\log_e x$ comes before Algebraic function $x$.
   * Set $u = \log_e x$ (First function) and $v = x$ (Second function).
2. Compute individual components:
   * $\frac{du}{dx} = \frac{1}{x}$
   * $\int v \, dx = \int x \, dx = \frac{x^2}{2}$
3. Apply the Integration by Parts formula:
$$\int x \log_e x \, dx = (\log_e x) \cdot \left(\frac{x^2}{2}\right) - \int \left[ \frac{1}{x} \cdot \frac{x^2}{2} \right] dx$$
4. Simplify the integrand in the trailing section:
$$= \frac{x^2}{2}\log_e x - \int \frac{x}{2} \, dx$$
$$= \frac{x^2}{2}\log_e x - \frac{1}{2}\left(\frac{x^2}{2}\right) + C$$
$$\text{Output} = \frac{x^2}{2}\log_e x - \frac{x^2}{4} + C$$

---

### Terminal Exercises & Self-Check Questions

1. **Trigonometric Identity Workout:** Evaluate the integral: $\int \tan^2 x \, dx$.
   * *Answer Hint:* There is no direct standard formula for $\tan^2 x$. Substitute the fundamental Pythagorean trigonometric identity $\tan^2 x = \sec^2 x - 1$:
     $$\int \tan^2 x \, dx = \int (\sec^2 x - 1) \, dx = \int \sec^2 x \, dx - \int 1 \, dx = \tan x - x + C$$

2. **Logarithmic Substitution Problem:** Find the value of $\int \frac{(\log_e x)^2}{x} \, dx$.
   * *Step-by-Step Solution:* 1. Substitute $t = \log_e x \implies dt = \frac{1}{x} \, dx$.
     2. Rewrite the expression in terms of $t$: $\int t^2 \, dt$.
     3. Integrate using the power rule: $\frac{t^3}{3} + C$.
     4. Substitute back the original function: $\frac{(\log_e x)^3}{3} + C$.

3. **Special Algebraic Form:** Evaluate $\int \frac{1}{x^2 - 9} \, dx$.
   * *Answer Hint:* Use the standard special fraction identity $\int \frac{1}{x^2 - a^2} \, dx = \frac{1}{2a} \log_e \left| \frac{x-a}{x+a} \right| + C$. Here $a^2 = 9 \implies a = 3$.
     $$\text{Output} = \frac{1}{2(3)} \log_e \left| \frac{x-3}{x+3} \right| + C = \frac{1}{6} \log_e \left| \frac{x-3}{x+3} \right| + C$$