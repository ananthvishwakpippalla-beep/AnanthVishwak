# Module II — Sequences and Series

# NIOS Senior Secondary Mathematics (311)

## Chapter 7: Some Special Sequences

### Introduction & Key Objectives
In the preceding chapter, we explored standard progressions where consecutive terms shared a common difference or common ratio. However, many mathematical and natural series do not fall strictly into standard AP or GP patterns. This chapter introduces specialized techniques to calculate the general terms and sum up special series involving the natural numbers, squares, cubes, and arithmetico-geometric combinations.

After studying this chapter, you will be able to:
* Use sigma ($\sum$) notation fluently to represent algebraic sums.
* Recall and apply standard algebraic formulas for the sum of the first $n$ **natural numbers**, their **squares**, and their **cubes**.
* Find the sum of a series by finding its general $n^{\text{th}}$ term ($a_n$).
* Recognize and evaluate an **Arithmetico-Geometric Progression (AGP)**.

---

### Core Concepts & Formulas

#### 1. Properties of Sigma Notations ($\sum$)
The Greek letter $\sum$ (sigma) represents a summation. Let $a_k$ be a general term dependent on an index variable $k$:
$$\sum_{k=1}^{n} a_k = a_1 + a_2 + a_3 + \dots + a_n$$

Key operational properties include:
* **Linearity Rule I:** $\sum_{k=1}^{n} (a_k \pm b_k) = \sum_{k=1}^{n} a_k \pm \sum_{k=1}^{n} b_k$
* **Linearity Rule II:** $\sum_{k=1}^{n} c \cdot a_k = c \sum_{k=1}^{n} a_k \quad$ *(where $c$ is a constant)*
* **Constant Summation:** $\sum_{k=1}^{n} c = c + c + \dots + c = n \cdot c$

#### 2. Three Standard Identities of Summation
These identities are highly emphasized across public examinations for direct or substituted calculations:

> **Sum of the first $n$ Natural Numbers ($\sum n$):**
> $$\sum_{k=1}^{n} k = 1 + 2 + 3 + \dots + n = \frac{n(n + 1)}{2}$$

> **Sum of the Squares of the first $n$ Natural Numbers ($\sum n^2$):**
> $$\sum_{k=1}^{n} k^2 = 1^2 + 2^2 + 3^2 + \dots + n^2 = \frac{n(n + 1)(2n + 1)}{6}$$

> **Sum of the Cubes of the first $n$ Natural Numbers ($\sum n^3$):**
> $$\sum_{k=1}^{n} k^3 = 1^3 + 2^3 + 3^3 + \dots + n^3 = \left[ \frac{n(n + 1)}{2} \right]^2 = \left( \sum_{k=1}^{n} k \right)^2$$

#### 3. Summing a Series via the $n^{\text{th}}$ Term Method
If a series is neither an AP nor a GP, its sum $S_n$ can be derived if the general $n^{\text{th}}$ term $a_n$ can be written as an algebraic function of $n$.
> If $a_n$ can be expanded into polynomial form $a_n = A n^3 + B n^2 + C n + D$, then:
> $$S_n = \sum_{k=1}^{n} a_k = A\sum k^3 + B\sum k^2 + C\sum k + \sum D$$

#### 4. Arithmetico-Geometric Progressions (AGP)
> An **Arithmetico-Geometric Progression** is a sequence in which each term is formed by multiplying the corresponding terms of an Arithmetic Progression (AP) and a Geometric Progression (GP).
> The standard format is: $a, (a + d)r, (a + 2d)r^2, (a + 3d)r^3, \dots$

* **Method of Summation:** The standard strategy to sum an AGP is to write the sum expression $S_n$, multiply the entire equation by the common ratio $r$, shift the series by one term to the right, and subtract the modified equation from the original one. This isolates a standard GP that can be easily resolved.

---

### Step-by-Step Examples

**Example 1:** Find the sum of the first 20 terms of the series whose $n^{\text{th}}$ term is given by $a_n = n(n + 3)$.  
**Solution:**
1. Expand the given expression for the $n^{\text{th}}$ term:
$$a_n = n^2 + 3n$$
2. Express the sum $S_n$ using sigma notation properties:
$$S_n = \sum_{k=1}^{n} a_k = \sum_{k=1}^{n} (k^2 + 3k) = \sum_{k=1}^{n} k^2 + 3\sum_{k=1}^{n} k$$
3. Substitute the standard identities for $\sum k^2$ and $\sum k$:
$$S_n = \frac{n(n + 1)(2n + 1)}{6} + 3 \left[ \frac{n(n + 1)}{2} \right]$$
4. Set $n = 20$ to calculate the final value:
$$S_{20} = \frac{20(21)(41)}{6} + 3 \left[ \frac{20(21)}{2} \right]$$
5. Calculate the individual parts:
   * First part: $\frac{17220}{6} = 2870$
   * Second part: $3 \times 210 = 630$
6. Total Sum: $S_{20} = 2870 + 630 = 3500$.

**Example 2:** Find the sum of the series: $1 \cdot 2 + 2 \cdot 3 + 3 \cdot 4 + \dots$ up to $n$ terms.  
**Solution:**
1. Determine the structure of the general $n^{\text{th}}$ term by inspecting the factors:
   * The first factor in each term forms the sequence $1, 2, 3, \dots$, which has a general term of $n$.
   * The second factor forms the sequence $2, 3, 4, \dots$, which has a general term of $(n + 1)$.
2. Combine them to get the general term: $a_n = n(n + 1) = n^2 + n$.
3. Set up the summation:
$$S_n = \sum_{k=1}^{n} k^2 + \sum_{k=1}^{n} k = \frac{n(n + 1)(2n + 1)}{6} + \frac{n(n + 1)}{2}$$
4. Factor out the common expression $\frac{n(n + 1)}{2}$:
$$S_n = \frac{n(n + 1)}{2} \left[ \frac{2n + 1}{3} + 1 \right] = \frac{n(n + 1)}{2} \left[ \frac{2n + 1 + 3}{3} \right]$$
$$S_n = \frac{n(n + 1)}{2} \left[ \frac{2n + 4}{3} \right] = \frac{n(n + 1) \cdot 2(n + 2)}{6} = \frac{n(n + 1)(n + 2)}{3}$$

---

### Terminal Exercises & Self-Check Questions

1. **Identity Value Calculation:** Evaluate the exact sum of $11^2 + 12^2 + 13^2 + \dots + 20^2$.
   * *Step-by-Step Solution:* 1. Rewrite the expression as a difference between two complete standard series starting from 1:
        $$\text{Output} = (1^2 + 2^2 + \dots + 20^2) - (1^2 + 2^2 + \dots + 10^2)$$
     2. Apply the square summation formula for $n=20$ and $n=10$:
        $$\text{Sum}_{20} = \frac{20(21)(41)}{6} = 2870$$
        $$\text{Sum}_{10} = \frac{10(11)(21)}{6} = 385$$
     3. Subtract the two values: $2870 - 385 = 2485$.

2. **Summation Workout:** Find the sum to $n$ terms of the series whose general term is $a_n = n^3 - n$.
   * *Answer Hint:* $S_n = \sum k^3 - \sum k = \left[\frac{n(n+1)}{2}\right]^2 - \frac{n(n+1)}{2}$. Factorizing out $\frac{n(n+1)}{2}$ yields $\frac{n(n+1)}{2}\left[\frac{n(n+1)}{2} - 1\right] = \frac{n(n+1)(n^2+n-2)}{4} = \frac{(n-1)n(n+1)(n+2)}{4}$.
