# Module III — Algebra I

# NIOS Senior Secondary Mathematics (311)

## Chapter 12: Binomial Theorem

### Introduction & Key Objectives
In algebra, we frequently expand identities like $(x + y)^2 = x^2 + 2xy + y^2$ and $(x + y)^3 = x^3 + 3x^2y + 3xy^2 + y^3$. However, as the power/exponent increases (e.g., $(x + y)^{10}$ or $(x + y)^{n}$), multiplying the algebraic terms manually becomes highly impractical. The Binomial Theorem provides a definitive, systematic formula to expand any positive integral power of a binomial expression using combination coefficients.

After studying this chapter, you will be able to:
* State and prove the **Binomial Theorem** for a positive integral index.
* Write the general term ($T_{r+1}$) and specific terms in a binomial expansion.
* Determine the **Middle Term(s)** of an expansion.
* Apply Pascal's Triangle to analyze the symmetrical nature of binomial coefficients.
* Use the binomial theorem to compute approximate numerical values of decimal powers.

---

### Core Concepts & Formulas

#### 1. Statement of the Binomial Theorem
> For any positive integer $n$ and any real numbers $x$ and $y$, the expansion of $(x + y)^n$ is given by:
> $$(x + y)^n = ^nC_0 x^n + ^nC_1 x^{n-1}y^1 + ^nC_2 x^{n-2}y^2 + \dots + ^nC_r x^{n-r}y^r + \dots + ^nC_n y^n$$
> Using sigma summation notation:
> $$(x + y)^n = \sum_{r=0}^{n} ^nC_r x^{n-r}y^r$$

*Key Observation Properties:*
1. **Total Number of Terms:** The total number of terms in the expansion of $(x + y)^n$ is always **$n + 1$**.
2. **Behavior of Exponents:** The exponent of $x$ decreases progressively by 1 (from $n$ down to 0), while the exponent of $y$ increases progressively by 1 (from 0 up to $n$).
3. **Constant Sum of Indices:** In any given individual term, the sum of the exponents of $x$ and $y$ is always equal to $n$ (since $(n - r) + r = n$).
4. **Symmetrical Coefficients:** The binomial coefficients ($^nC_0, ^nC_1, ^nC_2, \dots$) are symmetrical because $^nC_r = ^nC_{n-r}$.

#### 2. The General Term ($T_{r+1}$)
Instead of writing out the entire expansion, any specific term can be found using the general term formula. Note that the index variable $r$ begins at 0, meaning the $k^{\text{th}}$ term corresponds to $r = k - 1$:
> $$T_{r+1} = ^nC_r x^{n-r}y^r$$

#### 3. Finding the Middle Term
The position of the middle term depends directly on whether the power $n$ is even or odd:

> **Case 1: $n$ is an EVEN number**
> The total number of terms ($n + 1$) is odd, meaning there is exactly **one middle term**:
> $$\text{Middle Term} = T_{\frac{n}{2} + 1}$$

> **Case 2: $n$ is an ODD number**
> The total number of terms ($n + 1$) is even, meaning there are exactly **two middle terms**:
> $$\text{First Middle Term} = T_{\frac{n+1}{2}} \quad \text{and} \quad \text{Second Middle Term} = T_{\frac{n+1}{2} + 1}$$

#### 4. Specialized Binomial Identites
* By replacing $y$ with $-y$:
$$(x - y)^n = ^nC_0 x^n - ^nC_1 x^{n-1}y^1 + ^nC_2 x^{n-2}y^2 - \dots + (-1)^n \cdot ^nC_n y^n$$
* By setting $x = 1$ and $y = x$:
$$(1 + x)^n = ^nC_0 + ^nC_1 x + ^nC_2 x^2 + \dots + ^nC_n x^n$$

---

### Step-by-Step Examples

**Example 1:** Expand the expression $\left(x + \frac{1}{x}\right)^4$ completely using the Binomial Theorem.  
**Solution:**
1. Identify the parameters: $n = 4$, the first term is $x$, and the second term is $\frac{1}{x}$.
2. Write out the expansion based on the standard formula:
$$\left(x + \frac{1}{x}\right)^4 = ^4C_0 x^4 + ^4C_1 x^3\left(\frac{1}{x}\right)^1 + ^4C_2 x^2\left(\frac{1}{x}\right)^2 + ^4C_3 x^1\left(\frac{1}{x}\right)^3 + ^4C_4\left(\frac{1}{x}\right)^4$$
3. Calculate the binomial coefficients ($^4C_0 = 1, ^4C_1 = 4, ^4C_2 = 6, ^4C_3 = 4, ^4C_4 = 1$):
$$\left(x + \frac{1}{x}\right)^4 = 1(x^4) + 4\left(x^3 \cdot \frac{1}{x}\right) + 6\left(x^2 \cdot \frac{1}{x^2}\right) + 4\left(x \cdot \frac{1}{x^3}\right) + 1\left(\frac{1}{x^4}\right)$$
4. Simplify the algebraic variables:
$$\left(x + \frac{1}{x}\right)^4 = x^4 + 4x^2 + 6 + \frac{4}{x^2} + \frac{1}{x^4}$$



**Example 2:** Find the $4^{\text{th}}$ term in the expansion of $(2x - 3y)^7$.  
**Solution:**
1. Identify the parameters: $n = 7$, first term $= 2x$, second term $= -3y$.
2. To find the $4^{\text{th}}$ term ($T_4$), set $r + 1 = 4 \implies r = 3$.
3. Substitute these values into the general term formula $T_{r+1} = ^nC_r x^{n-r}y^r$:
$$T_4 = ^7C_3 (2x)^{7-3} (-3y)^3$$
4. Calculate the individual components:
   * Coefficient: $^7C_3 = \frac{7 \times 6 \times 5}{3 \times 2 \times 1} = 35$
   * First variable power: $(2x)^4 = 16x^4$
   * Second variable power: $(-3y)^3 = -27y^3$
5. Multiply all values together:
$$T_4 = 35 \times 16x^4 \times (-27y^3) = (35 \times 16 \times -27) \cdot x^4y^3$$
$$T_4 = -15120x^4y^3$$

**Example 3:** Find the middle term in the expansion of $(x + 2y)^6$.  
**Solution:**
1. Identify parameters: $n = 6$. Since $n$ is an **even** number, there is only one middle term.
2. Calculate the position of the middle term: $\frac{n}{2} + 1 = \frac{6}{2} + 1 = 3 + 1 = 4$. So, the $4^{\text{th}}$ term ($T_4$) is the middle term.
3. For $T_4$, set $r = 3$. Apply the general term formula:
$$T_4 = ^6C_3 (x)^{6-3} (2y)^3$$
4. Evaluate individual components ($^6C_3 = 20$, $x^3$, and $(2y)^3 = 8y^3$):
$$T_4 = 20 \cdot x^3 \cdot 8y^3 = 160x^3y^3$$

---

### Terminal Exercises & Self-Check Questions

1. **Independent Term Problem:** Find the term independent of $x$ (the constant term) in the expansion of $\left(3x^2 - \frac{1}{3x}\right)^9$.
   * *Answer Hint:* Write the general term $T_{r+1} = ^9C_r (3x^2)^{9-r} \left(-\frac{1}{3x}\right)^r$. Group the powers of $x$ together: $x^{2(9-r)-r} = x^{18-3r}$. For a term to be independent of $x$, its exponent must equal 0. Set $18 - 3r = 0 \implies r = 6$. Substitute $r=6$ back into the formula to compute the final numerical constant: $^9C_6 \cdot 3^3 \cdot \left(-\frac{1}{3}\right)^6 = 84 \cdot 27 \cdot \frac{1}{729} = \frac{84}{27} = \frac{28}{9}$.

2. **Numerical Value Calculation:** Evaluate $(1.01)^5$ correct to four decimal places using the Binomial Theorem.
   * *Step-by-Step Solution:* 1. Rewrite the decimal value as a binomial combination: $(1 + 0.01)^5$.
     2. Expand using the first few terms of the theorem (terms with tiny values can be ignored):
        $$(1 + 0.01)^5 = ^5C_0(1)^5 + ^5C_1(1)^4(0.01)^1 + ^5C_2(1)^3(0.01)^2 + ^5C_3(1)^2(0.01)^3 + \dots$$
     3. Calculate the numerical expansion:
        $$= 1 + 5(0.01) + 10(0.0001) + 10(0.000001)$$
        $$= 1 + 0.05 + 0.001 + 0.00001 = 1.05101$$
     4. Rounding to four decimal places gives **1.0510**.
