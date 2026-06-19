# NIOS Senior Secondary Mathematics (311)

## Chapter 4: Trigonometric Functions-II

### Introduction & Key Objectives
In the previous chapter, we defined trigonometric functions for generalized angles and studied their behavior across different quadrants. In this chapter, we extend those concepts to analyze compound angles, multiple and sub-multiple angles, and transformation formulas. These identities are vital for simplifying complex algebraic expressions and are extensively used in Calculus for integration and differentiation.

After studying this chapter, you will be able to:
* Find the trigonometric functions of **negative angles**.
* Express trigonometric functions of **associated angles** (e.g., $\pi/2 \pm \theta$, $\pi \pm \theta$) in terms of $\theta$.
* Apply addition and subtraction formulas for **compound angles**.
* Derive and use formulas for **multiple angles** ($2\theta$ and $3\theta$) and **sub-multiple angles** ($\theta/2$).
* Apply product-to-sum and sum-to-product **transformation formulas**.

---

### Core Concepts & Formulas

#### 1. Functions of Negative Angles
When the terminal ray rotates in a clockwise direction, a negative angle $-\theta$ is formed in Quadrant IV. Following the ASTC rule:
> * $\sin(-\theta) = -\sin\theta$
> * $\cos(-\theta) = \cos\theta$
> * $\tan(-\theta) = -\tan\theta$
> * $\csc(-\theta) = -\csc\theta$
> * $\sec(-\theta) = \sec\theta$
> * $\cot(-\theta) = -\cot\theta$

#### 2. Functions of Associated Angles
Angles like $\frac{\pi}{2} \pm \theta$, $\pi \pm \theta$, $\frac{3\pi}{2} \pm \theta$, and $2\pi \pm \theta$ are called associated angles.
* **Rule 1 (Function Change):** For odd multiples of $\frac{\pi}{2}$ (i.e., $\frac{\pi}{2}, \frac{3\pi}{2}$), the function changes to its co-function ($\sin \leftrightarrow \cos$, $\tan \leftrightarrow \cot$, $\sec \leftrightarrow \csc$).
* **Rule 2 (No Change):** For multiples of $\pi$ (i.e., $\pi, 2\pi$), the function name remains the same.
* **Rule 3 (Sign):** The final sign is determined by the quadrant of the original function.

*Key Examples:*
* $\sin(\frac{\pi}{2} - \theta) = \cos\theta$, $\cos(\frac{\pi}{2} - \theta) = \sin\theta$
* $\sin(\frac{\pi}{2} + \theta) = \cos\theta$, $\cos(\frac{\pi}{2} + \theta) = -\sin\theta$
* $\sin(\pi - \theta) = \sin\theta$, $\cos(\pi - \theta) = -\cos\theta$
* $\sin(\pi + \theta) = -\sin\theta$, $\cos(\pi + \theta) = -\cos\theta$

#### 3. Compound Angle Formulas
Angles expressed as the algebraic sum or difference of two or more angles (e.g., $A + B$, $A - B$) are compound angles.
> **Addition Formulas:**
> * $\sin(A + B) = \sin A\cos B + \cos A\sin B$
> * $\cos(A + B) = \cos A\cos B - \sin A\sin B$
> * $\tan(A + B) = \frac{\tan A + \tan B}{1 - \tan A\tan B}$

> **Subtraction Formulas:**
> * $\sin(A - B) = \sin A\cos B - \cos A\sin B$
> * $\cos(A - B) = \cos A\cos B + \sin A\sin B$
> * $\tan(A - B) = \frac{\tan A - \tan B}{1 + \tan A\tan B}$

#### 4. Multiple Angle Formulas ($2A$ and $3A$)
> **Double Angle Formulas ($2A$):**
> * $\sin 2A = 2\sin A\cos A = \frac{2\tan A}{1 + \tan^2 A}$
> * $\cos 2A = \cos^2 A - \sin^2 A = 2\cos^2 A - 1 = 1 - 2\sin^2 A = \frac{1 - \tan^2 A}{1 + \tan^2 A}$
> * $\tan 2A = \frac{2\tan A}{1 - \tan^2 A}$

> **Triple Angle Formulas ($3A$):**
> * $\sin 3A = 3\sin A - 4\sin^3 A$
> * $\cos 3A = 4\cos^3 A - 3\cos A$
> * $\tan 3A = \frac{3\tan A - \tan^3 A}{1 - 3\tan^2 A}$

#### 5. Sub-Multiple Angle Formulas ($\frac{A}{2}$)
By replacing $A$ with $\frac{A}{2}$ in the double-angle formulas, we obtain:
* $\sin A = 2\sin(\frac{A}{2})\cos(\frac{A}{2})$
* $1 - \cos A = 2\sin^2(\frac{A}{2}) \implies \sin(\frac{A}{2}) = \pm\sqrt{\frac{1 - \cos A}{2}}$
* $1 + \cos A = 2\cos^2(\frac{A}{2}) \implies \cos(\frac{A}{2}) = \pm\sqrt{\frac{1 + \cos A}{2}}$

#### 6. Transformation Formulas
> **Product to Sum/Difference:**
> * $2\sin A\cos B = \sin(A + B) + \sin(A - B)$
> * $2\cos A\sin B = \sin(A + B) - \sin(A - B)$
> * $2\cos A\cos B = \cos(A + B) + \cos(A - B)$
> * $2\sin A\sin B = \cos(A - B) - \cos(A + B)$

> **Sum/Difference to Product ($C-D$ Formulas):**
> * $\sin C + \sin D = 2\sin\left(\frac{C + D}{2}\right)\cos\left(\frac{C - D}{2}\right)$
> * $\sin C - \sin D = 2\cos\left(\frac{C + D}{2}\right)\sin\left(\frac{C - D}{2}\right)$
> * $\cos C + \cos D = 2\cos\left(\frac{C + D}{2}\right)\cos\left(\frac{C - D}{2}\right)$
> * $\cos C - \cos D = 2\sin\left(\frac{C + D}{2}\right)\sin\left(\frac{D - C}{2}\right)$ or $-2\sin\left(\frac{C + D}{2}\right)\sin\left(\frac{C - D}{2}\right)$

---

### Step-by-Step Examples

**Example 1:** Find the exact value of $\sin 15^\circ$.  
**Solution:**
1. Express $15^\circ$ as a difference of two standard angles whose trigonometric values are well-known:
$$15^\circ = 45^\circ - 30^\circ$$
2. Apply the subtraction formula for sine, $\sin(A - B) = \sin A\cos B - \cos A\sin B$:
$$\sin(45^\circ - 30^\circ) = \sin 45^\circ\cos 30^\circ - \cos 45^\circ\sin 30^\circ$$
3. Substitute the standard values ($\sin 45^\circ = \frac{1}{\sqrt{2}}$, $\cos 30^\circ = \frac{\sqrt{3}}{2}$, $\cos 45^\circ = \frac{1}{\sqrt{2}}$, $\sin 30^\circ = \frac{1}{2}$):
$$\sin 15^\circ = \left(\frac{1}{\sqrt{2}}\right)\left(\frac{\sqrt{3}}{2}\right) - \left(\frac{1}{\sqrt{2}}\right)\left(\frac{1}{2}\right)$$
$$\sin 15^\circ = \frac{\sqrt{3} - 1}{2\sqrt{2}}$$

**Example 2:** Prove that $\frac{\sin 5x + \sin 3x}{\cos 5x + \cos 3x} = \tan 4x$.  
**Solution:**
1. Apply the $C-D$ sum-to-product formulas to both the numerator and the denominator.
   * Numerator: $\sin 5x + \sin 3x = 2\sin\left(\frac{5x + 3x}{2}\right)\cos\left(\frac{5x - 3x}{2}\right) = 2\sin 4x\cos x$
   * Denominator: $\cos 5x + \cos 3x = 2\cos\left(\frac{5x + 3x}{2}\right)\cos\left(\frac{5x - 3x}{2}\right) = 2\cos 4x\cos x$
2. Set up the fraction and cancel out the common terms ($2$ and $\cos x$):
$$\text{LHS} = \frac{2\sin 4x\cos x}{2\cos 4x\cos x} = \frac{\sin 4x}{\cos 4x} = \tan 4x = \text{RHS}$$
3. Hence proved.

**Example 3:** If $\sin A = \frac{3}{5}$ and $A$ is in Quadrant I, find the value of $\sin 2A$ and $\cos 2A$.  
**Solution:**
1. Find $\cos A$ using the fundamental identity. Since $A$ is in Quadrant I, $\cos A$ is positive:
$$\cos A = \sqrt{1 - \sin^2 A} = \sqrt{1 - \left(\frac{3}{5}\right)^2} = \sqrt{\frac{16}{25}} = \frac{4}{5}$$
2. Calculate $\sin 2A$ using the double angle identity:
$$\sin 2A = 2\sin A\cos A = 2\left(\frac{3}{5}\right)\left(\frac{4}{5}\right) = \frac{24}{25}$$
3. Calculate $\cos 2A$ using a double angle identity:
$$\cos 2A = 1 - 2\sin^2 A = 1 - 2\left(\frac{3}{5}\right)^2 = 1 - \frac{18}{25} = \frac{7}{25}$$

---

### Terminal Exercises & Self-Check Questions

1. **Evaluate Expression:** Find the value of $\tan 75^\circ$.
   * *Answer Hint:* Use $\tan(45^\circ + 30^\circ) = \frac{\tan 45^\circ + \tan 30^\circ}{1 - \tan 45^\circ\tan 30^\circ} = \frac{1 + 1/\sqrt{3}}{1 - 1/\sqrt{3}} = \frac{\sqrt{3}+1}{\sqrt{3}-1} = 2 + \sqrt{3}$.

2. **Identity Verification:** Prove that $\frac{1 - \cos 2\theta}{\sin 2\theta} = \tan\theta$.
   * *Step-by-Step Solution:* Substitute $1 - \cos 2\theta = 2\sin^2\theta$ and $\sin 2\theta = 2\sin\theta\cos\theta$:
     $$\text{LHS} = \frac{2\sin^2\theta}{2\sin\theta\cos\theta} = \frac{\sin\theta}{\cos\theta} = \tan\theta = \text{RHS}$$

3. **Product Transformation:** Express the product $2\cos 4\theta\cos 2\theta$ as a sum or difference.
   * *Answer Hint:* Use $2\cos A\cos B = \cos(A+B) + \cos(A-B)$. Here, $A=4\theta$ and $B=2\theta$.
     $$\text{Output} = \cos(4\theta + 2\theta) + \cos(4\theta - 2\theta) = \cos 6\theta + \cos 2\theta$$