# NIOS Senior Secondary Mathematics (311)

## Module VIII: Calculus
### Chapter 26: Differentiation

### Introduction & Key Objectives
In the previous chapter, we explored limits and continuity, which allowed us to observe the behavior of a function as it approaches a specific boundary point. In this chapter, we use limits to define the absolute core operation of Differential Calculus: **Differentiation**. Geometrically, differentiation finds the exact slope of a curve at a single instantaneous point. Physically, it measures the instantaneous rate of change of a dependent variable with respect to an independent variable (such as velocity finding the rate of change of distance over time). 

After studying this chapter, you will be able to:
* Define the **Derivative** of a function at a point using the fundamental limit structure.
* Find the derivative of basic algebraic functions from first principles (**$\delta$-method**).
* Apply core rules of differentiation: **Constant Multiple Rule**, **Sum and Difference Rules**, **Product Rule**, and **Quotient Rule**.
* Find the derivative of a function of a function using the **Chain Rule**.

---

### Core Concepts & Formulas

#### 1. Definition from First Principles ($\delta$-Method)
Let $f(x)$ be a continuous real-valued function. The derivative of $f(x)$ with respect to $x$ is denoted by $f'(x)$, $\frac{dy}{dx}$, or $\frac{d}{dx}[f(x)]$. 

> **The First Principles Formula:**
> $$\frac{dy}{dx} = \lim_{\delta x \to 0} \frac{f(x + \delta x) - f(x)}{\delta x}$$
*(provided this limit exists and is finite).*

Geometrically, this represents the limit of the slope of a secant line passing through points $P(x, f(x))$ and $Q(x+\delta x, f(x+\delta x))$ as $Q$ slides infinitely close to $P$, transforming into a **Tangent Line**.



#### 2. Fundamental Derivatives Table
By evaluating the first principles limit formula for basic functions, we establish standard baseline rules:
* $$\frac{d}{dx}(c) = 0 \quad \text{(where } c \text{ is any constant)}$$
* **The Power Rule:** $$\frac{d}{dx}(x^n) = n \cdot x^{n-1}$$
* $$\frac{d}{dx}(x) = 1$$

#### 3. Fundamental Rules of Differentiation
If $u$ and $v$ are differentiable functions of $x$, and $c$ is a scalar constant:

> **Scalar Multiple Rule:**
> $$\frac{d}{dx}[c \cdot u] = c \cdot \frac{du}{dx}$$

> **Sum and Difference Rules:**
> $$\frac{d}{dx}[u \pm v] = \frac{du}{dx} \pm \frac{dv}{dx}$$

> **The Product Rule (Leibniz's Rule):**
> $$\frac{d}{dx}[u \cdot v] = u \cdot \frac{dv}{dx} + v \cdot \frac{du}{dx}$$

> **The Quotient Rule:**
> $$\frac{d}{dx}\left[\frac{u}{v}\right] = \frac{v \cdot \frac{du}{dx} - u \cdot \frac{dv}{dx}}{v^2} \quad (v \neq 0)$$

#### 4. The Chain Rule (Function of a Function)
If $y$ is a differentiable function of $t$, and $t$ is itself a differentiable function of $x$, then $y$ can be differentiated with respect to $x$ by linking them together:
> $$\frac{dy}{dx} = \frac{dy}{dt} \times \frac{dt}{dx}$$

---

### Step-by-Step Examples

**Example 1:** Find the derivative of $f(x) = x^2$ from first principles ($\delta$-method).  
**Solution:**
1. State the component parts of the formula: $f(x) = x^2$ and $f(x + \delta x) = (x + \delta x)^2$.
2. Substitute these terms into the first principles definition:
$$\frac{dy}{dx} = \lim_{\delta x \to 0} \frac{(x + \delta x)^2 - x^2}{\delta x}$$
3. Expand the algebraic binomial in the numerator:
$$(x + \delta x)^2 = x^2 + 2x(\delta x) + (\delta x)^2$$
4. Set up the simplified numerator fraction (notice that $x^2$ cancels out):
$$\frac{dy}{dx} = \lim_{\delta x \to 0} \frac{x^2 + 2x(\delta x) + (\delta x)^2 - x^2}{\delta x} = \lim_{\delta x \to 0} \frac{2x(\delta x) + (\delta x)^2}{\delta x}$$
5. Factor out $\delta x$ from the numerator and cancel it out from the denominator (valid since $\delta x \to 0 \implies \delta x \neq 0$):
$$\frac{dy}{dx} = \lim_{\delta x \to 0} \frac{\delta x (2x + \delta x)}{\delta x} = \lim_{\delta x \to 0} (2x + \delta x)$$
6. Evaluate the limit by setting $\delta x = 0$:
$$\frac{dy}{dx} = 2x$$

**Example 2:** Differentiate $y = (3x^2 + 5)(2x - 1)$ with respect to $x$ using the Product Rule.  
**Solution:**
1. Assign the component functions: $u = 3x^2 + 5$ and $v = 2x - 1$.
2. Differentiate each component individually using basic power rules:
   * $\frac{du}{dx} = \frac{d}{dx}(3x^2 + 5) = 6x + 0 = 6x$
   * $\frac{dv}{dx} = \frac{d}{dx}(2x - 1) = 2 - 0 = 2$
3. Apply the Product Rule formula $\frac{dy}{dx} = u\frac{dv}{dx} + v\frac{du}{dx}$:
$$\frac{dy}{dx} = (3x^2 + 5)(2) + (2x - 1)(6x)$$
4. Expand and combine like algebraic terms:
$$\frac{dy}{dx} = (6x^2 + 10) + (12x^2 - 6x) = 18x^2 - 6x + 10$$

**Example 3:** Find the derivative of $y = (2x^3 + 4)^5$ using the Chain Rule.  
**Solution:**
1. Recognize that this is a composite function. Let the inner function expression be a placeholder variable $t$:
$$t = 2x^3 + 4 \implies y = t^5$$
2. Differentiate both parts separately with respect to their independent variables:
   * $\frac{dy}{dt} = \frac{d}{dt}(t^5) = 5t^4$
   * $\frac{dt}{dx} = \frac{d}{dx}(2x^3 + 4) = 6x^2$
3. Apply the Chain Rule formula $\frac{dy}{dx} = \frac{dy}{dt} \times \frac{dt}{dx}$:
$$\frac{dy}{dx} = (5t^4) \times (6x^2) = 30x^2 \cdot t^4$$
4. Substitute the expression for $t$ back into the final equation to get your answer in terms of $x$:
$$\frac{dy}{dx} = 30x^2(2x^3 + 4)^4$$

---

### Terminal Exercises & Self-Check Questions

1. **Power Rule Combined Workout:** Differentiate the expression $y = 4x^3 - 2x^2 + 5x - 7$ with respect to $x$.
   * *Answer Hint:* Apply the power rule term-by-term:
     $$\frac{dy}{dx} = 4(3x^2) - 2(2x) + 5(1) - 0 = 12x^2 - 4x + 5$$

2. **Quotient Rule Workout:** Find $\frac{dy}{dx}$ if $y = \frac{x^2}{x + 1}$.
   * *Step-by-Step Solution:* 1. Let $u = x^2 \implies \frac{du}{dx} = 2x$ and let $v = x + 1 \implies \frac{dv}{dx} = 1$.
     2. Apply the Quotient Rule:
        $$\frac{dy}{dx} = \frac{(x + 1)(2x) - (x^2)(1)}{(x + 1)^2}$$
     3. Expand and simplify the numerator:
        $$\frac{dy}{dx} = \frac{2x^2 + 2x - x^2}{(x + 1)^2} = \frac{x^2 + 2x}{(x + 1)^2}$$

3. **Composite Fraction Problem:** Differentiate $y = \frac{1}{(5x^2 + 3)^2}$ with respect to $x$.
   * *Answer Hint:* Rewrite using a negative index: $y = (5x^2 + 3)^{-2}$. Apply the Chain Rule directly:
     $$\frac{dy}{dx} = -2(5x^2 + 3)^{-3} \cdot \frac{d}{dx}(5x^2 + 3) = -2(5x^2 + 3)^{-3} \cdot (10x) = \frac{-20x}{(5x^2 + 3)^3}$$