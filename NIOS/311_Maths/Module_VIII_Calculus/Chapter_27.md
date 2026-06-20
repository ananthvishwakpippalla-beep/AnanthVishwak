# NIOS Senior Secondary Mathematics (311)

## Module VIII: Calculus
### Chapter 27: Differentiation of Trigonometric Functions

### Introduction & Key Objectives
In Chapter 26, we established the fundamental rules of differentiation from first principles and applied them primarily to algebraic functions. However, many physical and mathematical systems—such as alternating electrical currents, sound waves, and planetary movements—are periodic. These systems are modeled using circular trigonometric functions. This chapter extends our differentiation toolkit to the six basic trigonometric functions, exploring their derivatives and structural behavior under composite combinations.

After studying this chapter, you will be able to:
* Derive the derivatives of standard trigonometric functions ($\sin x$, $\cos x$, $\tan x$) from first principles.
* Master the standard derivatives table for all six circular trigonometric functions.
* Apply product, quotient, and chain rules to complex trigonometric expressions.
* Differentiate trigonometric functions with respect to other functional parameters.

---

### Core Concepts & Formulas

#### 1. Derivatives of Trigonometric Functions from First Principles
To find the derivative of a trigonometric function like $f(x) = \sin x$ using the first principles definition, we rely heavily on standard trigonometric sum-to-product identities ($C-D$ formulas) and the fundamental limit identity $\lim_{\theta \to 0} \frac{\sin\theta}{\theta} = 1$:

$$\frac{d}{dx}(\sin x) = \lim_{\delta x \to 0} \frac{\sin(x + \delta x) - \sin x}{\delta x}$$
Applying the transformation identity $\sin C - \sin D = 2 \cos\left(\frac{C+D}{2}\right)\sin\left(\frac{C-D}{2}\right)$ expands the numerator to let us cleanly evaluate the limit as $\cos x$.

#### 2. Master Trigonometric Derivatives Table
Memorizing these six baseline derivatives is critical for computational speed in the examination:

> * $$\frac{d}{dx}(\sin x) = \cos x$$
> * $$\frac{d}{dx}(\cos x) = -\sin x$$
> * $$\frac{d}{dx}(\tan x) = \sec^2 x$$
> * $$\frac{d}{dx}(\cot x) = -\csc^2 x$$
> * $$\frac{d}{dx}(\sec x) = \sec x \tan x$$
> * $$\frac{d}{dx}(\csc x) = -\csc x \cot x$$

*Memory Strategy:* Notice that the derivative of every trigonometric function starting with the letter **"C"** ($\cos$, $\cot$, $\csc$) always yields a **negative** result.

---

#### 3. Trigonometric Chain Rule Structures
When a trigonometric function wraps around a non-trivial inner algebraic angle $u(x)$, we combine the standard trigonometric derivative with the derivative of that inner angle:



> * $$\frac{d}{dx}[\sin(u)] = \cos(u) \cdot \frac{du}{dx}$$
> * $$\frac{d}{dx}[\cos(u)] = -\sin(u) \cdot \frac{du}{dx}$$
> * $$\frac{d}{dx}[\tan(u)] = \sec^2(u) \cdot \frac{du}{dx}$$

Similarly, if the entire trigonometric function is raised to an exponential power $n$, we apply the power rule first, followed by the inner trigonometric derivative:
> $$\frac{d}{dx}(\sin^n x) = n \cdot \sin^{n-1} x \cdot \frac{d}{dx}(\sin x) = n \sin^{n-1} x \cos x$$

---

### Step-by-Step Examples

**Example 1:** Differentiate $y = x^3 \tan x$ with respect to $x$.  
**Solution:**
1. Identify the structural format: This expression is a product of an algebraic function ($u = x^3$) and a trigonometric function ($v = \tan x$). We must apply the **Product Rule**.
2. Find individual component derivatives:
   * $\frac{du}{dx} = \frac{d}{dx}(x^3) = 3x^2$
   * $\frac{dv}{dx} = \frac{d}{dx}(\tan x) = \sec^2 x$
3. Substitute components into the Product Rule formula $\frac{dy}{dx} = u\frac{dv}{dx} + v\frac{du}{dx}$:
$$\frac{dy}{dx} = (x^3)(\sec^2 x) + (\tan x)(3x^2)$$
4. Factor out common algebraic terms to simplify into final clean exam form:
$$\frac{dy}{dx} = x^2(x \sec^2 x + 3 \tan x)$$

**Example 2:** Find the derivative of $y = \sin(5x^2 + 4)$ with respect to $x$.  
**Solution:**
1. Recognize this as a composite function where the outer shell function is $\sin(u)$ and the inner angle function is $u = 5x^2 + 4$. We must apply the **Chain Rule**.
2. Calculate the derivative of the inner angle parameter:
$$\frac{du}{dx} = \frac{d}{dx}(5x^2 + 4) = 10x + 0 = 10x$$
3. Differentiate the outer function shell, leaving the inner argument completely untouched, then multiply by $\frac{du}{dx}$:
$$\frac{dy}{dx} = \cos(5x^2 + 4) \cdot \frac{d}{dx}(5x^2 + 4)$$
$$\frac{dy}{dx} = \cos(5x^2 + 4) \cdot (10x)$$
4. Rearrange terms to avoid algebraic confusion:
$$\frac{dy}{dx} = 10x \cos(5x^2 + 4)$$

**Example 3:** Find $\frac{dy}{dx}$ if $y = \frac{\cos x}{1 + \sin x}$.  
**Solution:**
1. Identify the structural format: This is a fractional distribution, so we must use the **Quotient Rule**. Let $u = \cos x$ and $v = 1 + \sin x$.
2. Compute individual components:
   * $\frac{du}{dx} = -\sin x$
   * $\frac{dv}{dx} = 0 + \cos x = \cos x$
3. Apply the Quotient Rule formula $\frac{dy}{dx} = \frac{v \frac{du}{dx} - u \frac{dv}{dx}}{v^2}$:
$$\frac{dy}{dx} = \frac{(1 + \sin x)(-\sin x) - (\cos x)(\cos x)}{(1 + \sin x)^2}$$
4. Expand the terms in the numerator:
$$\text{Numerator} = -\sin x - \sin^2 x - \cos^2 x = -\sin x - (\sin^2 x + \cos^2 x)$$
5. Substitute the fundamental Pythagorean trigonometric identity $\sin^2 x + \cos^2 x = 1$:
$$\text{Numerator} = -\sin x - 1 = -(1 + \sin x)$$
6. Reassemble the full fraction over the denominator and cancel out matching factors:
$$\frac{dy}{dx} = \frac{-(1 + \sin x)}{(1 + \sin x)^2} = \frac{-1}{1 + \sin x}$$

---

### Terminal Exercises & Self-Check Questions

1. **Composite Power Workout:** Differentiate $y = \cos^4 x$ with respect to $x$.
   * *Answer Hint:* Treat this expression structurally as $y = (\cos x)^4$. Apply the power chain rule:
     $$\frac{dy}{dx} = 4(\cos x)^3 \cdot \frac{d}{dx}(\cos x) = 4\cos^3 x \cdot (-\sin x) = -4\cos^3 x \sin x$$

2. **Combined Product/Chain Problem:** Find the derivative of $y = \sin 2x \cos 3x$.
   * *Step-by-Step Solution:* 1. Apply the product rule first: $\frac{dy}{dx} = \sin 2x \frac{d}{dx}(\cos 3x) + \cos 3x \frac{d}{dx}(\sin 2x)$.
     2. Evaluate inner chain angles: $\frac{d}{dx}(\cos 3x) = -3\sin 3x$ and $\frac{d}{dx}(\sin 2x) = 2\cos 2x$.
     3. Substitute back and combine terms: $\frac{dy}{dx} = -3\sin 2x \sin 3x + 2\cos 2x \cos 3x$.

3. **Trigonometric Parameter Division:** Differentiate $y = \sqrt{\tan x}$ with respect to $x$.
   * *Answer Hint:* Write the radical expression as a fractional power: $y = (\tan x)^{1/2}$.
     $$\frac{dy}{dx} = \frac{1}{2}(\tan x)^{-1/2} \cdot \frac{d}{dx}(\tan x) = \frac{1}{2\sqrt{\tan x}} \cdot \sec^2 x = \frac{\sec^2 x}{2\sqrt{\tan x}}$$