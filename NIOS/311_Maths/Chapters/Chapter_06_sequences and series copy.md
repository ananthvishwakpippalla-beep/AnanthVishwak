# NIOS Senior Secondary Mathematics (311)

## Chapter 6: Sequences and Series

### Introduction & Key Objectives
In mathematics, identifying patterns in numbers is fundamental to solving complex real-world progression problems, such as calculating compound interest, financial multi-year returns, or analyzing structural spacing. A sequence is a collection of numbers arranged in a definite, rule-based order, while a series represents the sum of those elements. This chapter establishes the rigorous framework for Arithmetic Progressions (AP) and Geometric Progressions (GP).

After studying this chapter, you will be able to:
* Distinguish between a finite sequence, an infinite sequence, and a series.
* Define and recognize an **Arithmetic Progression (AP)**.
* Compute the **$n^{\text{th}}$ term** and the **sum of the first $n$ terms** of an AP.
* Define and insert **Arithmetic Means (AM)** between two given numbers.
* Define and recognize a **Geometric Progression (GP)**.
* Compute the **$n^{\text{th}}$ term** and the **sum of the first $n$ terms** of a GP.
* Calculate the sum of an **infinite GP** when the common ratio $|r| < 1$.
* Define and insert **Geometric Means (GM)** between two numbers, and understand the core relation between AM and GM.

---

### Core Concepts & Formulas

#### 1. General Concepts
* **Sequence:** A successive arrangement of numbers followed by a specific law or functional rule: $a_1, a_2, a_3, \dots, a_n$.
* **Series:** The algebraic sum expression connecting the terms of a sequence: $a_1 + a_2 + a_3 + \dots + a_n$. It is concisely expressed using sigma notation $\sum_{k=1}^{n} a_k$.

#### 2. Arithmetic Progressions (AP)
> **Arithmetic Progression:** A progression where each subsequent term is obtained by adding a constant fixed number $d$ (called the **common copy ratio / difference**) to its preceding term.
> $$a_n = a_{n-1} + d$$

Let $a$ be the first term, and $d$ be the common difference. The standard AP is represented as: $a, a+d, a+2d, a+3d, \dots$

> **$n^{\text{th}}$ Term of an AP ($a_n$ or $t_n$):**
> $$a_n = a + (n - 1)d$$

> **Sum of $n$ Terms of an AP ($S_n$):**
> * $$S_n = \frac{n}{2} [2a + (n - 1)d]$$
> * $$S_n = \frac{n}{2} [a + l]$$ *(where $l$ is the final terminal term $a_n$)*

#### 3. Arithmetic Mean (AM)
* If three terms $a, b, c$ are in AP, then $b$ is the Arithmetic Mean between $a$ and $c$:
$$b = \frac{a + c}{2}$$
* **Inserting $n$ Arithmetic Means:** To insert $n$ terms $A_1, A_2, \dots, A_n$ between numbers $a$ and $b$ such that the sequence becomes an AP, the common difference $d$ must satisfy:
> $$d = \frac{b - a}{n + 1}$$

#### 4. Geometric Progressions (GP)
> **Geometric Progression:** A sequence where each non-zero term is obtained by multiplying the preceding term by a fixed, constant factor $r$ (called the **common ratio**).
> $$\frac{a_n}{a_{n-1}} = r$$

Let $a$ be the first term, and $r$ be the common ratio. The standard GP is represented as: $a, ar, ar^2, ar^3, \dots$

> **$n^{\text{th}}$ Term of a GP ($a_n$ or $t_n$):**
> $$a_n = ar^{n-1}$$

> **Sum of $n$ Terms of a GP ($S_n$):**
> * $$S_n = \frac{a(r^n - 1)}{r - 1} \quad \text{for } r > 1$$
> * $$S_n = \frac{a(1 - r^n)}{1 - r} \quad \text{for } r < 1$$
> * $$S_n = na \quad \text{for } r = 1$$

> **Sum of an Infinite GP ($S_\infty$):**
> If the common ratio lies within the strict boundary $-1 < r < 1$ (or $|r| < 1$), the sum of an infinite number of terms converges to a definitive constant:
> $$S_\infty = \frac{a}{1 - r}$$

#### 5. Geometric Mean (GM)
* If three terms $a, b, c$ are in GP, then $b$ is the Geometric Mean between $a$ and $c$:
$$b^2 = ac \implies b = \sqrt{ac}$$
* **Inserting $n$ Geometric Means:** To insert $n$ terms $G_1, G_2, \dots, G_n$ between numbers $a$ and $b$ such that the sequence forms a valid GP, the common ratio $r$ is:
> $$r = \left(\frac{b}{a}\right)^{\frac{1}{n+1}}$$

#### 6. Fundamental Inequality Relationship Between AM and GM
> For any two distinct positive real numbers $a$ and $b$, their Arithmetic Mean is strictly greater than or equal to their Geometric Mean:
> $$\text{AM} \ge \text{GM} \implies \frac{a + b}{2} \ge \sqrt{ac \text{ (or } ab\text{)}}$$

---

### Step-by-Step Examples

**Example 1:** Find the $15^{\text{th}}$ term and the sum of the first 20 terms of the AP: $3, 8, 13, 18, \dots$  
**Solution:**
1. Identify the given parameters: first term $a = 3$, common difference $d = 8 - 3 = 5$.
2. Compute the $15^{\text{th}}$ term using $a_n = a + (n-1)d$:
$$a_{15} = 3 + (15 - 1)5 = 3 + (14 \times 5) = 3 + 70 = 73$$
3. Compute the sum of the first 20 terms using $S_n = \frac{n}{2}[2a + (n-1)d]$:
$$S_{20} = \frac{20}{2} [2(3) + (20 - 1)5] = 10 [6 + 19 \times 5]$$
$$S_{20} = 10 [6 + 95] = 10 \times 101 = 1010$$

**Example 2:** Find the $6^{\text{th}}$ term of the GP: $2, 6, 18, 54, \dots$  
**Solution:**
1. Identify parameters: first term $a = 2$, common ratio $r = \frac{6}{2} = 3$.
2. Use the standard $n^{\text{th}}$ term formula $a_n = ar^{n-1}$ for $n=6$:
$$a_6 = 2 \times 3^{6-1} = 2 \times 3^5$$
3. Simplify the calculation ($3^5 = 243$):
$$a_6 = 2 \times 243 = 486$$



**Example 3:** Find the sum of the infinite geometric series: $1 + \frac{1}{3} + \frac{1}{9} + \frac{1}{27} + \dots$  
**Solution:**
1. Check the criteria: first term $a = 1$, common ratio $r = \frac{1/3}{1} = \frac{1}{3}$.
2. Verify convergence: since $|r| = \frac{1}{3} < 1$, an infinite sum converges.
3. Apply the infinite sum formula:
$$S_\infty = \frac{a}{1 - r} = \frac{1}{1 - \frac{1}{3}} = \frac{1}{\frac{2}{3}} = \frac{3}{2} = 1.5$$

---

### Terminal Exercises & Self-Check Questions

1. **Missing Element Evaluation:** In an AP, if the $3^{\text{th}}$ term is 7 and the $7^{\text{th}}$ term is 15, calculate the first term $a$ and the common difference $d$.
   * *Answer Hint:* Setup linear equations: $a + 2d = 7$ and $a + 6d = 15$. Subtracting them yields $4d = 8 \implies d = 2$. Substituting back gives $a = 3$.

2. **Ratio Insertion Workout:** Insert 3 Arithmetic Means between 4 and 20.
   * *Step-by-Step Solution:* 1. Number of inserted means $n = 3$, boundary values $a = 4, b = 20$.
     2. Calculate common difference: $d = \frac{20 - 4}{3 + 1} = \frac{16}{4} = 4$.
     3. Generate terms: $A_1 = 4+4=8$, $A_2 = 8+4=12$, $A_3 = 12+4=16$.
     4. Final progressing series sequence: $4, \mathbf{8, 12, 16}, 20$.

3. **GP Term Position Problem:** Which term of the geometric progression $5, 10, 20, 40, \dots$ is equal to 1280?
   * *Answer Hint:* Use $1280 = 5 \times 2^{n-1} \implies 256 = 2^{n-1}$. Since $256 = 2^8$, we equate powers: $n - 1 = 8 \implies n = 9$. It is the $9^{\text{th}}$ term.