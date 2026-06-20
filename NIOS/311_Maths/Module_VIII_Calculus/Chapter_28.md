# NIOS Senior Secondary Mathematics (311)

## Module VIII: Calculus
### Chapter 28: Differentiation of Exponential and Logarithmic Functions

### Introduction & Key Objectives
In our study of differential calculus so far, we have mastered the derivatives of algebraic functions (using the power rule) and periodic trigonometric functions. However, many real-world systems do not grow at a constant polynomial pace or repeat in cycles. Processes like bacterial population growth, radioactive decay, and compound interest grow or decay at a rate proportional to their current size, which is modeled using **Exponential Functions**. Conversely, scaling massive data spans down into manageable steps requires their inverse counterparts, **Logarithmic Functions**. This chapter covers the specific rules needed to differentiate these transcendental structures.

After studying this chapter, you will be able to:
* Define the natural exponential function ($e^x$) and natural logarithmic function ($\ln x$ or $\log_e x$) from a calculus perspective.
* Master the standard derivatives of exponential and logarithmic functions across both natural and general bases.
* Apply the **Chain Rule** to complex exponential and logarithmic composite expressions.
* Use the technique of **Logarithmic Differentiation** to differentiate variable-base variable-exponent functions ($[f(x)]^{g(x)}$).

---

### Core Concepts & Formulas

#### 1. Foundational Calculus Limits
The derivatives of exponential and logarithmic functions are rooted in two primary mathematical limit limits:
* $$\lim_{x \to 0} \frac{e^x - 1}{x} = 1$$
* $$\lim_{x \to 0} \frac{\log_e(1 + x)}{x} = 1$$

Here, $e$ is Euler's constant, an irrational number approximately equal to $2.71828$. When a logarithm uses base $e$, it is called the **Natural Logarithm**, written as $\log_e x$ or $\ln x$.

#### 2. Standard Derivatives Table
You must memorize these baseline rules for both natural (base $e$) and general (base $a$) scenarios:

> **Exponential Derivatives:**
> * Natural Base: $$\frac{d}{dx}(e^x) = e^x$$
> * General Base ($a > 0$): $$\frac{d}{dx}(a^x) = a^x \cdot \log_e a$$

> **Logarithmic Derivatives:**
> * Natural Base: $$\frac{d}{dx}(\log_e x) = \frac{1}{x}$$
> * General Base ($a > 0, a \neq 1$): $$\frac{d}{dx}(\log_a x) = \frac{1}{x \cdot \log_e a}$$

---

#### 3. Chain Rule and Composite Structures
When an exponential or logarithmic shell wraps around an inner functional argument $u(x)$, the Chain Rule dictates the following operational extensions:



* **Exponential Chain:** $$\frac{d}{dx}[e^{u(x)}] = e^{u(x)} \cdot \frac{du}{dx}$$
* **Logarithmic Chain:** $$\frac{d}{dx}[\log_e(u(x))] = \frac{1}{u(x)} \cdot \frac{du}{dx}$$

---

#### 4. Logarithmic Differentiation Technique
When an expression consists of a variable function in both the base and the exponent, such as $y = [f(x)]^{g(x)}$, standard power rules ($n x^{n-1}$) and standard exponential rules ($a^x \ln a$) cannot be used. We must use **Logarithmic Differentiation**:

> **Step-by-Step Procedure:**
> 1. Take the natural logarithm ($\log_e$) on both sides of the equation: $\log_e y = \log_e([f(x)]^{g(x)})$.
> 2. Use the logarithmic power property ($\log M^n = n \log M$) to pull down the exponent:
>    $$\log_e y = g(x) \cdot \log_e[f(x)]$$
> 3. Differentiate implicitly with respect to $x$ on both sides, applying the **Product Rule** on the right side:
>    $$\frac{1}{y} \cdot \frac{dy}{dx} = g(x) \cdot \frac{d}{dx}(\log_e[f(x)]) + \log_e[f(x)] \cdot g'(x)$$
> 4. Multiply the entire resulting expression by $y$ to isolate $\frac{dy}{dx}$, then substitute back the original definition of $y$.

---

### Step-by-Step Examples

**Example 1:** Differentiate $y = e^{x^2 + 5x}$ with respect to $x$.  
**Solution:**
1. Recognize this as an exponential composite function where the inner argument is $u = x^2 + 5x$.
2. Differentiate the inner argument: $\frac{du}{dx} = \frac{d}{dx}(x^2 + 5x) = 2x + 5$.
3. Apply the exponential chain rule:
$$\frac{dy}{dx} = e^{x^2 + 5x} \cdot \frac{d}{dx}(x^2 + 5x)$$
$$\frac{dy}{dx} = (2x + 5)e^{x^2 + 5x}$$

**Example 2:** Find the derivative of $y = \log_e(\sin x)$ with respect to $x$.  
**Solution:**
1. This is a logarithmic composite function where the inner function is $u = \sin x$.
2. Apply the logarithmic chain rule ($\frac{1}{u} \cdot \frac{du}{dx}$):
$$\frac{dy}{dx} = \frac{1}{\sin x} \cdot \frac{d}{dx}(\sin x)$$
3. Substitute the standard derivative $\frac{d}{dx}(\sin x) = \cos x$:
$$\frac{dy}{dx} = \frac{1}{\sin x} \cdot \cos x = \frac{\cos x}{\sin x}$$
4. Simplify using standard trigonometric ratios:
$$\frac{dy}{dx} = \cot x$$

**Example 3:** Differentiate $y = x^x$ with respect to $x$.  
**Solution:**
1. Since both the base and exponent are variables ($x$), take the natural logarithm on both sides:
$$\log_e y = \log_e(x^x)$$
2. Apply the power property of logarithms to simplify the right-hand side:
$$\log_e y = x \cdot \log_e x$$
3. Differentiate both sides with respect to $x$. Use implicit differentiation on the left ($\frac{1}{y}\frac{dy}{dx}$) and the **Product Rule** on the right ($u = x, v = \log_e x$):
$$\frac{1}{y} \cdot \frac{dy}{dx} = x \cdot \frac{d}{dx}(\log_e x) + (\log_e x) \cdot \frac{d}{dx}(x)$$
$$\frac{1}{y} \cdot \frac{dy}{dx} = x \cdot \left(\frac{1}{x}\right) + (\log_e x) \cdot (1)$$
$$\frac{1}{y} \cdot \frac{dy}{dx} = 1 + \log_e x$$
4. Multiply through by $y$ to cleanly isolate the derivative:
$$\frac{dy}{dx} = y(1 + \log_e x)$$
5. Substitute the original expression $y = x^x$ back into the equation:
$$\frac{dy}{dx} = x^x(1 + \log_e x)$$

---

### Terminal Exercises & Self-Check Questions

1. **General Base Exponential Workout:** Differentiate $y = 5^{x^3}$ with respect to $x$.
   * *Answer Hint:* This matches the general base formula $\frac{d}{dx}(a^u) = a^u \ln a \cdot \frac{du}{dx}$ where $a = 5$ and $u = x^3$.
     $$\frac{dy}{dx} = 5^{x^3} \cdot \log_e 5 \cdot \frac{d}{dx}(x^3) = 3x^2 \cdot 5^{x^3} \cdot \log_e 5$$

2. **Combined Product/Logarithmic Problem:** Find $\frac{dy}{dx}$ if $y = x^2 \log_e x$.
   * *Step-by-Step Solution:* 1. Apply the Product Rule: $\frac{dy}{dx} = x^2 \frac{d}{dx}(\log_e x) + (\log_e x) \frac{d}{dx}(x^2)$.
     2. Substitute standard derivatives: $\frac{dy}{dx} = x^2 \left(\frac{1}{x}\right) + (\log_e x)(2x)$.
     3. Simplify the terms: $\frac{dy}{dx} = x + 2x \log_e x = x(1 + 2\log_e x)$.

3. **Complex Quotient Logarithmic Simplification:** Differentiate $y = \log_e \left( \frac{x^2+1}{x^2-1} \right)$ with respect to $x$.
   * *Answer Hint:* Do not use the chain rule immediately. Simplify the expression first using the logarithmic quotient identity $\log\left(\frac{M}{N}\right) = \log M - \log N$:
     $$y = \log_e(x^2 + 1) - \log_e(x^2 - 1)$$
     Now differentiate term-by-term using the chain rule:
     $$\frac{dy}{dx} = \frac{2x}{x^2 + 1} - \frac{2x}{x^2 - 1} = \frac{2x(x^2 - 1) - 2x(x^2 + 1)}{(x^2 + 1)(x^2 - 1)} = \frac{-4x}{x^4 - 1} = \frac{4x}{1 - x^4}$$