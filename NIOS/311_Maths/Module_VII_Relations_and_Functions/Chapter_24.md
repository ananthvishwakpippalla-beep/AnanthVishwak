# NIOS Senior Secondary Mathematics (311)

## Module VII: Relations and Functions
### Chapter 24: Inverse Trigonometric Functions

### Introduction & Key Objectives
In the preceding chapter, we established that a function can only be inverted if it satisfies the strict bijectivity criterion—meaning it must be both one-to-one (injective) and onto (surjective). Standard trigonometric functions are periodic, meaning they repeat their outputs infinitely and are inherently many-to-one. However, by strategically restricting their domain ranges to specific boundaries, we can force them to become bijective. This chapter introduces **Inverse Trigonometric Functions**, their principal domains, and algebraic identities vital for calculus simplification.

After studying this chapter, you will be able to:
* Understand the concept of restriction of domains for trigonometric functions.
* Define the **Principal Value Branches** of inverse trigonometric functions.
* State and locate the exact **Domain** and **Range** for $\sin^{-1}x$, $\cos^{-1}x$, $\tan^{-1}x$, etc.
* Evaluate the **Principal Value** of various inverse trigonometric expressions.
* Apply core **Properties and Identities** of inverse trigonometric functions to solve algebraic equations.

---

### Core Concepts & Formulas

#### 1. Foundation of Inverse Trigonometric Functions
If $y = \sin x$, then by restricting $x$ to an interval where the function is strictly increasing or decreasing without repeating values (e.g., $[-\frac{\pi}{2}, \frac{\pi}{2}]$), we can uniquely write:
$$x = \sin^{-1}y \quad (\text{or } x = \arcsin y)$$
* *Crucial Alert:* $\sin^{-1}x$ is **not** equal to $(\sin x)^{-1}$. Note that $(\sin x)^{-1} = \frac{1}{\sin x} = \csc x$, which is completely different from the inverse function mapping.

#### 2. Master Principal Value Branches Table
This table is highly emphasized across all public examinations. Any final calculated value **must** fall within these strict range limits to be considered a valid principal value:

| Function | Domain ($x$) | Range / Principal Value Branch ($y$) |
| :--- | :--- | :--- |
| $y = \sin^{-1}x$ | $[-1, 1]$ | $\left[-\frac{\pi}{2}, \frac{\pi}{2}\right]$ |
| $y = \cos^{-1}x$ | $[-1, 1]$ | $[0, \pi]$ |
| $y = \tan^{-1}x$ | $\mathbb{R}$ | $\left(-\frac{\pi}{2}, \frac{\pi}{2}\right)$ |
| $y = \csc^{-1}x$ | $\mathbb{R} - (-1, 1)$ | $\left[-\frac{\pi}{2}, \frac{\pi}{2}\right] - \{0\}$ |
| $y = \sec^{-1}x$ | $\mathbb{R} - (-1, 1)$ | $[0, \pi] - \left\{\frac{\pi}{2}\right\}$ |
| $y = \cot^{-1}x$ | $\mathbb{R}$ | $(0, \pi)$ |



---

#### 3. Primary Algebraic Properties & Identities

> **Negative Argument Identities:**
> * $\sin^{-1}(-x) = -\sin^{-1}x$
> * $\tan^{-1}(-x) = -\tan^{-1}x$
> * $\csc^{-1}(-x) = -\csc^{-1}x$
> * $\cos^{-1}(-x) = \pi - \cos^{-1}x$
> * `\sec^{-1}(-x) = \pi - \sec^{-1}x`
> * $\cot^{-1}(-x) = \pi - \cot^{-1}x$

> **Complementary Angle Pairs:**
> * $\sin^{-1}x + \cos^{-1}x = \frac{\pi}{2} \quad (x \in [-1, 1])$
> * $\tan^{-1}x + \cot^{-1}x = \frac{\pi}{2} \quad (x \in \mathbb{R})$
> * $\sec^{-1}x + \csc^{-1}x = \frac{\pi}{2} \quad (|x| \ge 1)$

> **Sum and Difference of Tangent Operations:**
> * $$\tan^{-1}x + \tan^{-1}y = \tan^{-1}\left(\frac{x + y}{1 - xy}\right) \quad (\text{if } xy < 1)$$
> * $$\tan^{-1}x - \tan^{-1}y = \tan^{-1}\left(\frac{x - y}{1 + xy}\right) \quad (\text{if } xy > -1)$$

> **Double Angle Conversions ($2\tan^{-1}x$):**
> $$2\tan^{-1}x = \sin^{-1}\left(\frac{2x}{1 + x^2}\right) = \cos^{-1}\left(\frac{1 - x^2}{1 + x^2}\right) = \tan^{-1}\left(\frac{2x}{1 - x^2}\right)$$

---

### Step-by-Step Examples

**Example 1:** Find the exact principal value of $\sin^{-1}\left(-\frac{1}{2}\right)$.  
**Solution:**
1. Let $y = \sin^{-1}\left(-\frac{1}{2}\right)$. This means:
$$\sin y = -\frac{1}{2}$$
2. Recall the standard angle value for sine: $\sin\left(\frac{\pi}{6}\right) = \frac{1}{2}$.
3. Apply the negative parameter rule for sine ($\sin(-\theta) = -\sin\theta$):
$$\sin\left(-\frac{\pi}{6}\right) = -\sin\left(\frac{\pi}{6}\right) = -\frac{1}{2}$$
4. Check the range constraint: $-\frac{\pi}{6}$ falls perfectly within the principal branch interval $\left[-\frac{\pi}{2}, \frac{\pi}{2}\right]$.
5. Conclusion: The principal value is $-\frac{\pi}{6}$.

**Example 2:** Evaluate the principal value of $\cos^{-1}\left(-\frac{\sqrt{3}}{2}\right)$.  
**Solution:**
1. Apply the negative parameter formula for cosine directly: $\cos^{-1}(-x) = \pi - \cos^{-1}x$.
$$\cos^{-1}\left(-\frac{\sqrt{3}}{2}\right) = \pi - \cos^{-1}\left(\frac{\sqrt{3}}{2}\right)$$
2. Find the standard acute angle value where cosine yields $\frac{\sqrt{3}}{2}$:
$$\cos\left(\frac{\pi}{6}\right) = \frac{\sqrt{3}}{2} \implies \cos^{-1}\left(\frac{\sqrt{3}}{2}\right) = \frac{\pi}{6}$$
3. Perform the subtraction from $\pi$:
$$\text{Value} = \pi - \frac{\pi}{6} = \frac{6\pi - \pi}{6} = \frac{5\pi}{6}$$
4. Verify the branch limits: $\frac{5\pi}{6}$ (or $150^\circ$) fits inside the standard interval $[0, \pi]$.
5. Conclusion: The principal value is $\frac{5\pi}{6}$.

**Example 3:** Prove that $\tan^{-1}\left(\frac{1}{2}\right) + \tan^{-1}\left(\frac{1}{3}\right) = \frac{\pi}{4}$.  
**Solution:**
1. Identify the parameters for the tangent sum formula: $x = \frac{1}{2}$ and $y = \frac{1}{3}$.
2. Perform the product check to ensure compatibility: $xy = \frac{1}{2} \times \frac{1}{3} = \frac{1}{6}$. Since $\frac{1}{6} < 1$, the standard sum formula is valid.
3. Apply the formula:
$$\tan^{-1}\left(\frac{1}{2}\right) + \tan^{-1}\left(\frac{1}{3}\right) = \tan^{-1}\left( \frac{\frac{1}{2} + \frac{1}{3}}{1 - \frac{1}{2} \cdot \frac{1}{3}} \right)$$
4. Simplify the fractions inside the brackets:
$$\text{Numerator} = \frac{3 + 2}{6} = \frac{5}{6}$$
$$\text{Denominator} = 1 - \frac{1}{6} = \frac{5}{6}$$
5. Divide the numerator by the denominator:
$$\text{Expression} = \tan^{-1}\left( \frac{5/6}{5/6} \right) = \tan^{-1}(1)$$
6. Since $\tan\left(\frac{\pi}{4}\right) = 1$, we know that $\tan^{-1}(1) = \frac{\pi}{4}$.
7. $\text{LHS} = \text{RHS}$. Hence proved.

---

### Terminal Exercises & Self-Check Questions

1. **Boundary Out-of-Range Workout:** Evaluate the value of $\sin^{-1}\left(\sin \frac{2\pi}{3}\right)$.
   * *Answer Hint:* You cannot simply cancel out the terms to get $\frac{2\pi}{3}$ because $\frac{2\pi}{3}$ (or $120^\circ$) falls completely outside the valid principal range branch $\left[-\frac{\pi}{2}, \frac{\pi}{2}\right]$. You must rewrite the inner angle using associated angles: $\sin\left(\frac{2\pi}{3}\right) = \sin\left(\pi - \frac{\pi}{3}\right) = \sin\left(\frac{\pi}{3}\right)$. Now solve: $\sin^{-1}\left(\sin \frac{\pi}{3}\right) = \frac{\pi}{3}$, which is inside the branch.

2. **Complementary Substitution Workout:** Find the value of $\cos\left[\sin^{-1}x + \cos^{-1}x\right]$ for $|x| \le 1$.
   * *Step-by-Step Solution:* 1. Recall the complementary angle sum pair rule: $\sin^{-1}x + \cos^{-1}x = \frac{\pi}{2}$.
     2. Substitute this identity into the expression: $\cos\left[\frac{\pi}{2}\right]$.
     3. Evaluate the exact trigonometric value: $\cos\left(\frac{\pi}{2}\right) = 0$.

3. **Identity Verification Problem:** Find the value of $2\tan^{-1}\left(\frac{1}{3}\right)$.
   * *Answer Hint:* Apply the double angle conversion formula for tangent: $\tan^{-1}\left(\frac{2x}{1-x^2}\right)$.
     $$\text{Output} = \tan^{-1}\left( \frac{2(1/3)}{1 - (1/3)^2} \right) = \tan^{-1}\left( \frac{2/3}{1 - 1/9} \right) = \tan^{-1}\left( \frac{2/3}{8/9} \right) = \tan^{-1}\left( \frac{2}{3} \times \frac{9}{8} \right) = \tan^{-1}\left(\frac{3}{4}\right)$$