# Module III — Algebra I

# NIOS Senior Secondary Mathematics (311)

## Chapter 8: Complex Numbers

### Introduction & Key Objectives
In our study of algebra so far, we have worked extensively within the real number system ($\mathbb{R}$). However, the real number system is inadequate when dealing with quadratic equations that have negative discriminants (such as $x^2 + 1 = 0$). To overcome this limitation, mathematicians introduced an imaginary unit $i$, extending the number system to include Complex Numbers. This chapter establishes the properties, algebraic operations, and geometric representations of complex numbers.

After studying this chapter, you will be able to:
* Define the imaginary unit $i$ and evaluate its integral powers.
* Understand the definition, real part, and imaginary part of a **Complex Number**.
* Perform fundamental operations: **addition**, **subtraction**, **multiplication**, and **division** of complex numbers.
* Find the **conjugate** and **modulus** of a complex number and understand their properties.
* Represent a complex number geometrically on an **Argand Plane**.
* Find the **square root** of a complex number.

---

### Core Concepts & Formulas

#### 1. The Imaginary Unit ($i$)
The symbol $i$ (called iota) is defined such that:
> $$i = \sqrt{-1} \implies i^2 = -1$$

* **Powers of $i$:** The powers of $i$ repeat in a cycle of 4:
  * $i^1 = i$
  * $i^2 = -1$
  * $i^3 = i^2 \cdot i = -i$
  * $i^4 = (i^2)^2 = 1$
* For any integer $n$, $i^{4n} = 1$, $i^{4n+1} = i$, $i^{4n+2} = -1$, and $i^{4n+3} = -i$.

#### 2. Definition of a Complex Number
> A number of the form $z = a + ib$, where $a$ and $b$ are real numbers, is called a **Complex Number**.
> * $a$ is called the **Real Part** of $z$, denoted by $\text{Re}(z)$.
> * $b$ is called the **Imaginary Part** of $z$, denoted by $\text{Im}(z)$.

* **Purely Real:** If $\text{Im}(z) = 0 \implies z = a$.
* **Purely Imaginary:** If $\text{Re}(z) = 0 \implies z = ib$.
* **Equality Rule:** Two complex numbers $z_1 = a + ib$ and $z_2 = c + id$ are equal if and only if their corresponding real and imaginary parts are identical:
$$z_1 = z_2 \iff a = c \text{ and } b = d$$

#### 3. Algebraic Operations
Let $z_1 = a + ib$ and $z_2 = c + id$:
* **Addition:** $z_1 + z_2 = (a + c) + i(b + d)$
* **Subtraction:** $z_1 - z_2 = (a - c) + i(b - d)$
* **Multiplication:** $z_1 \cdot z_2 = (ac - bd) + i(ad + bc)$
* **Division:** To divide $z_1$ by $z_2$, multiply both the numerator and the denominator by the conjugate of the denominator ($c - id$).

#### 4. Conjugate and Modulus
Let $z = a + ib$ be a complex number.
> **Conjugate ($\bar{z}$):** Obtained by changing the sign of the imaginary part.
> $$\bar{z} = a - ib$$

> **Modulus ($|z|$):** The non-negative real number representing the absolute absolute distance from the origin.
> $$|z| = \sqrt{a^2 + b^2}$$

* **Core Identity:**
> $$z \cdot \bar{z} = (a + ib)(a - ib) = a^2 + b^2 = |z|^2$$

#### 5. Geometrical Representation (Argand Plane)
A complex number $z = a + ib$ can be uniquely represented as a point $P(a, b)$ in a coordinate plane called the **Argand Plane** (or Complex Plane).
* The x-axis is called the **Real Axis**.
* The y-axis is called the **Imaginary Axis**.



---

### Step-by-Step Examples

**Example 1:** Simplify and evaluate the expression: $i^{37} + \frac{1}{i^{67}}$.  
**Solution:**
1. Divide the powers by 4 to find their remainders:
   * For 37: $37 = 4(9) + 1 \implies i^{37} = i^1 = i$
   * For 67: $67 = 4(16) + 3 \implies i^{67} = i^3 = -i$
2. Substitute these back into the expression:
$$\text{Output} = i + \frac{1}{-i}$$
3. Multiply the numerator and denominator of the fraction by $i$ to eliminate it from the denominator:
$$\frac{1}{-i} = \frac{1 \cdot i}{-i \cdot i} = \frac{i}{-(-1)} = \frac{i}{1} = i$$
4. Complete the sum:
$$\text{Total} = i + i = 2i$$

**Example 2:** Express the complex number $z = \frac{2 + 3i}{1 - 2i}$ in the standard form $a + ib$.  
**Solution:**
1. Multiply both the numerator and denominator by the conjugate of the denominator ($1 + 2i$):
$$z = \frac{(2 + 3i)(1 + 2i)}{(1 - 2i)(1 + 2i)}$$
2. Expand the numerator using FOIL/multiplication rules:
$$\text{Numerator} = 2(1) + 2(2i) + 3i(1) + 3i(2i) = 2 + 4i + 3i + 6i^2$$
$$\text{Since } i^2 = -1 \implies 2 + 7i - 6 = -4 + 7i$$
3. Expand the denominator using $z\bar{z} = a^2 + b^2$:
$$\text{Denominator} = 1^2 + (-2)^2 = 1 + 4 = 5$$
4. Split the real and imaginary parts:
$$z = \frac{-4 + 7i}{5} = -\frac{4}{5} + i\frac{7}{5}$$

**Example 3:** Find the modulus and conjugate of $z = 3 - 4i$.  
**Solution:**
1. Identify the real and imaginary parts: $a = 3$, $b = -4$.
2. Compute the conjugate by flipping the imaginary sign:
$$\bar{z} = 3 - (-4i) = 3 + 4i$$
3. Compute the modulus using $|z| = \sqrt{a^2 + b^2}$:
$$|z| = \sqrt{3^2 + (-4)^2} = \sqrt{9 + 16} = \sqrt{25} = 5$$

---

### Terminal Exercises & Self-Check Questions

1. **Equality Workout:** Find the values of real numbers $x$ and $y$ if $(x + iy)(2 - 3i) = 4 - i$.
   * *Answer Hint:* Expand the left hand side to get $(2x + 3y) + i(2y - 3x) = 4 - i$. Create the system of equations: $2x + 3y = 4$ and $2y - 3x = -1$. Solving simultaneously gives $x = \frac{11}{13}$ and $y = \frac{10}{13}$.

2. **Multiplicative Inverse Problem:** Find the multiplicative inverse of $z = 4 - 3i$.
   * *Step-by-Step Solution:* 1. The multiplicative inverse is $z^{-1} = \frac{1}{z} = \frac{1}{4 - 3i}$.
     2. Rationalize using the conjugate $4 + 3i$:
        $$\frac{1}{4 - 3i} \times \frac{4 + 3i}{4 + 3i} = \frac{4 + 3i}{4^2 + (-3)^2} = \frac{4 + 3i}{16 + 9} = \frac{4 + 3i}{25}$$
     3. Separate the components: $z^{-1} = \frac{4}{25} + i\frac{3}{25}$.
