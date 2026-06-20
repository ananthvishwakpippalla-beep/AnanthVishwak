# NIOS Senior Secondary Mathematics (311)

## Module VI: Algebra-II
### Chapter 22: Inverse of a Matrix and its Applications

### Introduction & Key Objectives
In real number arithmetic, every non-zero number $x$ has a multiplicative inverse $\frac{1}{x}$ (or $x^{-1}$) such that $x \cdot x^{-1} = 1$. In matrix algebra, a similar concept exists for square matrices. Finding the inverse of a matrix allows us to perform the equivalent of "matrix division" to solve complex multi-variable linear systems. This chapter explores the formal conditions for a matrix to be invertible, the computation of the Adjoint matrix, and practical applications for solving engineering and economic linear systems.

After studying this chapter, you will be able to:
* Differentiate between **Singular** and **Non-Singular Matrices**.
* Define and construct the **Adjoint of a Square Matrix ($\text{adj } A$)**.
* State and apply the conditions for the existence of the **Inverse of a Matrix ($A^{-1}$)**.
* Compute the inverse of $2 \times 2$ and $3 \times 3$ square matrices.
* Use the **Matrix Method** ($X = A^{-1}B$) to solve a simultaneous system of linear equations.

---

### Core Concepts & Formulas

#### 1. Singular and Non-Singular Matrices
The existence of a matrix inverse depends entirely on the numerical value of its determinant:
* **Singular Matrix:** A square matrix whose determinant is exactly equal to zero ($|A| = 0$). A singular matrix **cannot** be inverted.
* **Non-Singular Matrix:** A square matrix whose determinant is not equal to zero ($|A| \neq 0$). A non-singular matrix is **invertible**.

#### 2. Adjoint of a Square Matrix ($\text{adj } A$)
> **Adjoint:** The adjoint of a square matrix $A$ is the **transpose of the cofactor matrix** of $A$.

If $A = [a_{ij}]$ is a square matrix and $A_{ij}$ represents the cofactor of each element $a_{ij}$, then:
$$\text{adj } A = [A_{ij}]^T$$

* **Core Operational Identity:** For any square matrix $A$ of order $n$:
> $$A \cdot (\text{adj } A) = (\text{adj } A) \cdot A = |A| \cdot I_n$$

#### 3. Inverse of a Matrix ($A^{-1}$)
Let $A$ be a non-singular square matrix. If there exists another square matrix $B$ of the same order such that $AB = BA = I$, then $B$ is called the multiplicative inverse of $A$, denoted by $A^{-1}$.

> **The Inverse Formula:**
> $$A^{-1} = \frac{1}{|A|} \cdot \text{adj } A \quad (\text{valid only if } |A| \neq 0)$$

* **Key Properties of Matrix Inverses:**
  * **Uniqueness:** The inverse of a square matrix, if it exists, is completely unique.
  * **Reversal Law:** $(AB)^{-1} = B^{-1}A^{-1}$
  * **Transpose Rule:** $(A^T)^{-1} = (A^{-1})^T$

---

#### 4. The Matrix Method (Solving Linear Equations)
Consider a system of linear equations in three variables:
$$\begin{aligned} a_1x + b_1y + c_1z &= d_1 \\ a_2x + b_2y + c_2z &= d_2 \\ a_3x + b_3y + c_3z &= d_3 \end{aligned}$$

We can re-write this system cleanly as a single matrix product equation:
> $$AX = B$$



Where:
* $A = \begin{bmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{bmatrix}$ (The **Coefficient Matrix**)
* $X = \begin{bmatrix} x \\ y \\ z \end{bmatrix}$ (The **Variable Matrix**)
* $B = \begin{bmatrix} d_1 \\ d_2 \\ d_3 \end{bmatrix}$ (The **Constant Matrix**)

> **The Solution Pathway:**
> If $|A| \neq 0$, the system is consistent and yields a unique solution by multiplying the inverse matrix across the constants:
> $$X = A^{-1}B$$

---

### Step-by-Step Examples

**Example 1:** Find the Adjoint and Inverse of the $2 \times 2$ matrix: $A = \begin{bmatrix} 2 & 3 \\ 1 & 4 \end{bmatrix}$.  
**Solution:**
1. Calculate the determinant to check for invertibility:
$$|A| = \begin{vmatrix} 2 & 3 \\ 1 & 4 \end{vmatrix} = (2 \times 4) - (3 \times 1) = 8 - 3 = 5$$
Since $|A| = 5 \neq 0$, the matrix is non-singular and $A^{-1}$ exists.
2. Find the cofactors of all elements:
   * $A_{11} = (-1)^{1+1}(4) = 4$
   * $A_{12} = (-1)^{1+2}(1) = -1$
   * $A_{21} = (-1)^{2+1}(3) = -3$
   * $A_{22} = (-1)^{2+2}(2) = 2$
3. Assemble the cofactor matrix and take its transpose to get the Adjoint ($\text{adj } A$):
$$\text{Cofactor Matrix} = \begin{bmatrix} 4 & -1 \\ -3 & 2 \end{bmatrix} \implies \text{adj } A = \begin{bmatrix} 4 & -3 \\ -1 & 2 \end{bmatrix}$$
*(Shortcut Rule for $2 \times 2$: Swap principal diagonal elements, flip signs of off-diagonal elements).*
4. Apply the inverse formula:
$$A^{-1} = \frac{1}{|A|} \cdot \text{adj } A = \frac{1}{5} \begin{bmatrix} 4 & -3 \\ -1 & 2 \end{bmatrix} = \begin{bmatrix} \frac{4}{5} & -\frac{3}{5} \\ -\frac{1}{5} & \frac{2}{5} \end{bmatrix}$$

**Example 2:** Solve the system of linear equations using the Matrix Method:
$$\begin{aligned} 5x + 2y &= 4 \\ 7x + 3y &= 5 \end{aligned}$$

**Solution:**
1. Express the system in the matrix form $AX = B$:
$$\begin{bmatrix} 5 & 2 \\ 7 & 3 \end{bmatrix} \begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 4 \\ 5 \end{bmatrix}$$
2. Compute the determinant of the coefficient matrix $A$:
$$|A| = \begin{vmatrix} 5 & 2 \\ 7 & 3 \end{vmatrix} = (5 \times 3) - (2 \times 7) = 15 - 14 = 1$$
3. Find $\text{adj } A$ using the shortcut swapping method:
$$\text{adj } A = \begin{bmatrix} 3 & -2 \\ -7 & 5 \end{bmatrix}$$
4. Compute $A^{-1}$ (since $|A|=1$, $A^{-1} = \text{adj } A$):
$$A^{-1} = \frac{1}{1} \begin{bmatrix} 3 & -2 \\ -7 & 5 \end{bmatrix} = \begin{bmatrix} 3 & -2 \\ -7 & 5 \end{bmatrix}$$
5. Solve for the variables using $X = A^{-1}B$:
$$X = \begin{bmatrix} x \\ y \end{bmatrix} = \begin{bmatrix} 3 & -2 \\ -7 & 5 \end{bmatrix} \begin{bmatrix} 4 \\ 5 \end{bmatrix}$$
6. Perform row-by-column multiplication:
   * $x = (3 \times 4) + (-2 \times 5) = 12 - 10 = 2$
   * $y = (-7 \times 4) + (5 \times 5) = -28 + 25 = -3$
7. Conclusion: $x = 2, y = -3$.

---

### Terminal Exercises & Self-Check Questions

1. **Singular Matrix Analysis:** Find the value of $k$ for which the matrix $M = \begin{bmatrix} 4 & k \\ 2 & 3 \end{bmatrix}$ is a singular matrix.
   * *Answer Hint:* For a matrix to be singular, its determinant must equal 0. Set $|M| = 0 \implies (4 \times 3) - (2 \times k) = 0 \implies 12 - 2k = 0 \implies 2k = 12 \implies k = 6$.

2. **Inverse Rule Workout:** Given a non-singular matrix $A$ where $|A| = 3$ and $\text{adj } A = \begin{bmatrix} 1 & 2 \\ 0 & 3 \end{bmatrix}$, state the matrix expression for $A^{-1}$.
   * *Step-by-Step Solution:* Apply the definition directly: $A^{-1} = \frac{1}{|A|} \cdot \text{adj } A$. Substitute the known metrics: $A^{-1} = \frac{1}{3} \begin{bmatrix} 1 & 2 \\ 0 & 3 \end{bmatrix} = \begin{bmatrix} \frac{1}{3} & \frac{2}{3} \\ 0 & 1 \end{bmatrix}$.

3. **Reversal Law Application:** If $A^{-1} = \begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix}$ and $B^{-1} = \begin{bmatrix} 0 & 1 \\ 4 & -2 \end{bmatrix}$, compute the matrix product value of $(AB)^{-1}$.
   * *Answer Hint:* Apply the reversal law property: $(AB)^{-1} = B^{-1}A^{-1}$. Perform the row-by-column product of the given matrices:
     $$(AB)^{-1} = \begin{bmatrix} 0 & 1 \\ 4 & -2 \end{bmatrix} \begin{bmatrix} 1 & -1 \\ 2 & 3 \end{bmatrix} = \begin{bmatrix} (0+2) & (0+3) \\ (4-4) & (-4-6) \end{bmatrix} = \begin{bmatrix} 2 & 3 \\ 0 & -10 \end{bmatrix}$$