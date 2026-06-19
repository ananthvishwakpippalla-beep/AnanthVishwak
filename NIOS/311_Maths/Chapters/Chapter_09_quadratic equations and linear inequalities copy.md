# NIOS Senior Secondary Mathematics (311)

## Chapter 9: Quadratic Equations and Linear Inequalities

### Introduction & Key Objectives
In earlier classes, we learned how to solve quadratic equations with real roots. By extending our number system to include complex numbers (as covered in Chapter 8), we can now solve any quadratic equation, even when the discriminant is negative. Additionally, many real-world constraints involve boundary ranges rather than exact equations. This chapter introduces the methods to analyze complex roots of quadratic expressions and solve single-variable linear inequalities.

After studying this chapter, you will be able to:
* Solve a **Quadratic Equation** with real or complex coefficients.
* Determine the nature of roots using the **Discriminant**.
* Establish the relationship between the roots and coefficients of a quadratic equation.
* Form a quadratic equation when its roots are given.
* Solve **Linear Inequalities** in one variable and represent their solution sets on a number line.

---

### Core Concepts & Formulas

#### 1. Quadratic Equations & General Solution
A quadratic equation is a polynomial equation of degree 2. Its standard form is:
$$ax^2 + bx + c = 0 \quad (\text{where } a, b, c \in \mathbb{R} \text{ and } a \neq 0)$$

The roots of this equation are given by the quadratic formula:
> $$x = \frac{-b \pm \sqrt{D}}{2a}$$
> Where $D$ is the **Discriminant**:
> $$D = b^2 - 4ac$$

#### 2. Nature of Roots Based on the Discriminant ($D$)
* If $D > 0$: Two distinct, real roots.
* If $D = 0$: Two equal (repeated), real roots ($x = -b/2a$).
* If $D < 0$: Two distinct, **complex conjugate roots**. 
  $$\text{Roots} = \frac{-b \pm i\sqrt{-D}}{2a}$$

#### 3. Relations Between Roots and Coefficients
Let $\alpha$ and $\beta$ be the two roots of $ax^2 + bx + c = 0$:
> * **Sum of Roots ($\alpha + \beta$):** >   $$\alpha + \beta = -\frac{b}{a}$$
> * **Product of Roots ($\alpha \cdot \beta$):** >   $$\alpha \cdot \beta = \frac{c}{a}$$

#### 4. Formation of a Quadratic Equation
If the roots $\alpha$ and $\beta$ (or their sum $S$ and product $P$) are known, the corresponding quadratic equation is given by:
> $$x^2 - (\alpha + \beta)x + (\alpha\beta) = 0 \implies x^2 - Sx + P = 0$$

#### 5. Linear Inequalities in One Variable
An inequality is a statement involving variables and relational operators such as $<, >, \le, \text{ or } \ge$. 

*Key Operational Rules for Inequalities:*
* **Rule 1:** Adding or subtracting the same number on both sides preserves the inequality sign.
* **Rule 2:** Multiplying or dividing both sides by a **positive** number preserves the inequality sign.
* **Rule 3 (Crucial):** Multiplying or dividing both sides by a **negative** number **reverses** the direction of the inequality sign.
  $$\text{If } -x < 5 \implies x > -5$$

---

### Step-by-Step Examples

**Example 1:** Solve the quadratic equation $x^2 + x + 1 = 0$.  
**Solution:**
1. Identify the coefficients: $a = 1, b = 1, c = 1$.
2. Calculate the Discriminant ($D$):
$$D = b^2 - 4ac = 1^2 - 4(1)(1) = 1 - 4 = -3$$
3. Since $D < 0$, the roots are complex. Apply the quadratic formula:
$$x = \frac{-1 \pm \sqrt{-3}}{2(1)} = \frac{-1 \pm i\sqrt{3}}{2}$$
4. The solution set is: $\left\{ \frac{-1 + i\sqrt{3}}{2}, \frac{-1 - i\sqrt{3}}{2} \right\}$ (These are the imaginary cube roots of unity, often denoted as $\omega$ and $\omega^2$).

**Example 2:** Form a quadratic equation whose roots are $2 + 3i$ and $2 - 3i$.  
**Solution:**
1. Let $\alpha = 2 + 3i$ and $\beta = 2 - 3i$. Calculate the Sum of Roots ($S$):
$$S = \alpha + \beta = (2 + 3i) + (2 - 3i) = 4$$
2. Calculate the Product of Roots ($P$) using the complex identity $(a+ib)(a-ib) = a^2 + b^2$:
$$P = \alpha \cdot \beta = (2 + 3i)(2 - 3i) = 2^2 + 3^2 = 4 + 9 = 13$$
3. Substitute $S$ and $P$ into the standard equation profile $x^2 - Sx + P = 0$:
$$x^2 - 4x + 13 = 0$$



**Example 3:** Solve the linear inequality $\frac{5 - 2x}{3} \le \frac{x}{6} - 5$ for real numbers $x$, and show the solution on a number line.  
**Solution:**
1. Multiply the entire inequality by 6 (the LCM of the denominators) to clear the fractions:
$$2(5 - 2x) \le x - 30$$
2. Expand the left side:
$$10 - 4x \le x - 30$$
3. Move all terms containing $x$ to one side and constants to the other:
$$10 + 30 \le x + 4x \implies 40 \le 5x$$
4. Divide by 5 (since 5 is positive, the sign stays the same):
$$8 \le x \implies x \ge 8$$
5. The solution set in interval notation is $[8, \infty)$. On a number line, this is represented by a solid/closed circle at 8 extending indefinitely to the right.

---

### Terminal Exercises & Self-Check Questions

1. **Discriminant Condition Problem:** Find the value of $k$ for which the quadratic equation $2x^2 + kx + 3 = 0$ has two equal real roots.
   * *Answer Hint:* For equal roots, set $D = 0 \implies k^2 - 4(2)(3) = 0 \implies k^2 - 24 = 0 \implies k = \pm\sqrt{24} = \pm2\sqrt{6}$.

2. **Root Transformation Workout:** If $\alpha$ and $\beta$ are the roots of $x^2 - 5x + 6 = 0$, find an equation whose roots are $\frac{1}{\alpha}$ and $\frac{1}{\beta}$.
   * *Step-by-Step Solution:* 1. From the given equation, $\alpha + \beta = 5$ and $\alpha\beta = 6$.
     2. New Sum $S' = \frac{1}{\alpha} + \frac{1}{\beta} = \frac{\alpha + \beta}{\alpha\beta} = \frac{5}{6}$.
     3. New Product $P' = \frac{1}{\alpha} \cdot \frac{1}{\beta} = \frac{1}{\alpha\beta} = \frac{1}{6}$.
     4. Form the equation: $x^2 - \frac{5}{6}x + \frac{1}{6} = 0 \implies 6x^2 - 5x + 1 = 0$.

3. **Inequality Range Problem:** Solve the system of linear inequalities: $3x - 7 > 2(x - 6)$ and $6 - x > 11 - 2x$. Find the common real solution interval.
   * *Answer Hint:* Solving the first inequality: $3x - 7 > 2x - 12 \implies x > -5$. Solving the second inequality: $6 - x > 11 - 2x \implies x > 5$. The overlapping intersection region of both constraints is $x > 5$, or $(5, \infty)$.