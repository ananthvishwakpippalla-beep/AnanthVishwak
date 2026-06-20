# NIOS Senior Secondary Mathematics (311)

## Module VI: Algebra-II
### Chapter 21: Determinants

### Introduction & Key Objectives
To every square matrix, we can associate a unique scalar number or algebraic value known as its determinant. While matrices represent structured systems of operations, determinants provide an immediate diagnostic test to see if those operations can be mathematically reversed or inverted. Determinants are heavily utilized to compute areas of polygons, test for point collinearity, and evaluate the existence of solutions for systems of simultaneous linear equations.

After studying this chapter, you will be able to:
* Define a **Determinant** and distinguish it from a matrix.
* Evaluate determinants of **Order 2** and **Order 3**.
* Understand and locate the **Minors** and **Cofactors** of any element in a determinant.
* Apply core **Properties of Determinants** to simplify expansions and solve algebraic equations.
* Apply **Cramer's Rule** to solve a system of simultaneous linear equations in two or three variables.

---

### Core Concepts & Formulas

#### 1. Definition and Notation
A determinant is a scalar value associated strictly with a **Square Matrix**. If $A$ is a square matrix, its determinant is denoted by $|A|$, $\det(A)$, or $\Delta$ (Delta). 
* *Crucial Difference:* A matrix is an arrangement enclosed in brackets `[]` and has no numerical value. A determinant is a scalar value enclosed inside vertical bars `||`.

#### 2. Evaluation of Determinants
> **Order 2 ($2 \times 2$):**
> $$\Delta = \begin{vmatrix} a_{11} & a_{12} \\ a_{21} & a_{22} \end{vmatrix} = a_{11}a_{22} - a_{12}a_{21}$$

> **Order 3 ($3 \times 3$):**
> Evaluated by expanding along any row or column (typically the first row $R_1$), matching elements with their respective chess-board pattern signs: $\begin{vmatrix} + & - & + \\ - & + & - \\ + & - & + \end{vmatrix}$.
> $$\Delta = \begin{vmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{vmatrix} = a_1\begin{vmatrix} b_2 & c_2 \\ b_3 & c_3 \end{vmatrix} - b_1\begin{vmatrix} a_2 & c_2 \\ a_3 & c_3 \end{vmatrix} + c_1\begin{vmatrix} a_2 & b_2 \\ a_3 & b_3 \end{vmatrix}$$

#### 3. Minors and Cofactors
Let $a_{ij}$ be an element inside a determinant:
* **Minor ($M_{ij}$):** The determinant of the sub-matrix left behind after deleting the $i^{\text{th}}$ row and $j^{\text{th}}$ column containing $a_{ij}$.
* **Cofactor ($A_{ij}$ or $C_{ij}$):** The minor multiplied by its quadrant position sign:
> $$A_{ij} = (-1)^{i+j} \cdot M_{ij}$$

---

#### 4. Primary Properties of Determinants
These rules are highly emphasized in public exams to evaluate complex determinants without expansion:
* **Reflection Property:** The value of a determinant remains unchanged if rows and columns are completely interchanged ($|A| = |A^T|$).
* **All-Zero Property:** If all elements of any single row or column are strictly zero, the value of the determinant is $0$.
* **Proportionality/Identity Property:** If any two rows (or columns) are identical or proportional, the value of the determinant is $0$.
* **Switching Property:** If any two adjacent rows (or columns) are swapped, the sign of the determinant changes, but its absolute magnitude stays the same.
* **Scalar Multiplication Property:** Multiplying a single row or column by a scalar constant $k$ multiplies the value of the entire determinant by $k$.
* **Invariance Property:** The value of a determinant remains unchanged if a multiple of one row/column is added to another row/column ($R_i \rightarrow R_i + kR_j$).

---

#### 5. Cramer's Rule (System of Linear Equations)
For a non-singular system of equations in three variables ($x, y, z$):
$$\begin{aligned} a_1x + b_1y + c_1z &= d_1 \\ a_2x + b_2y + c_2z &= d_2 \\ a_3x + b_3y + c_3z &= d_3 \end{aligned}$$



We define four unique determinants:
* $\Delta$: The baseline coefficient determinant ($\begin{vmatrix} a_1 & b_1 & c_1 \\ a_2 & b_2 & c_2 \\ a_3 & b_3 & c_3 \end{vmatrix}$)
* $\Delta_x$: Formed by replacing the $x$-coefficients column with the constant vector column ($d_1, d_2, d_3$).
* $\Delta_y$: Formed by replacing the $y$-coefficients column with the constant vector column.
* $\Delta_z$: Formed by replacing the $z$-coefficients column with the constant vector column.

> **Solutions Criterion ($\Delta \neq 0$):**
> $$x = \frac{\Delta_x}{\Delta}, \quad y = \frac{\Delta_y}{\Delta}, \quad z = \frac{\Delta_z}{\Delta}$$

---

### Step-by-Step Examples

**Example 1:** Evaluate the $2 \times 2$ determinant: $\Delta = \begin{vmatrix} 2 & 4 \\ -1 & 5 \end{vmatrix}$.  
**Solution:**
1. Cross-multiply the main principal diagonal elements: $2 \times 5 = 10$.
2. Multiply the secondary off-diagonal elements: $4 \times (-1) = -4$.
3. Compute the subtraction:
$$\Delta = (2 \times 5) - (4 \times -1) = 10 - (-4) = 10 + 4 = 14$$

**Example 2:** Find the Minor and Cofactor of the element $4$ in the determinant: $\Delta = \begin{vmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \\ 7 & 8 & 9 \end{vmatrix}$.  
**Solution:**
1. Locate element $4$: It is in Row 2, Column 1 ($a_{21} = 4$).
2. Cross out Row 2 and Column 1 to isolate the remaining sub-determinant for the **Minor ($M_{21}$)**:
$$M_{21} = \begin{vmatrix} 2 & 3 \\ 8 & 9 \end{vmatrix} = (2 \times 9) - (3 \times 8) = 18 - 24 = -6$$
3. Apply the positional sign multiplier to find the **Cofactor ($A_{21}$)**:
$$A_{21} = (-1)^{2+1} \cdot M_{21} = (-1)^3 \cdot (-6) = (-1) \times (-6) = 6$$

**Example 3:** Solve the following system of linear equations using Cramer's Rule:
$$\begin{aligned} 2x + 3y &= 7 \\ 3x - y &= 5 \end{aligned}$$

**Solution:**
1. Form the baseline coefficient determinant $\Delta$:
$$\Delta = \begin{vmatrix} 2 & 3 \\ 3 & -1 \end{vmatrix} = (2 \times -1) - (3 \times 3) = -2 - 9 = -11$$
Since $\Delta \neq 0$, a unique solution exists.
2. Form $\Delta_x$ by replacing the first column with the constants vector $\begin{bmatrix} 7 \\ 5 \end{bmatrix}$:
$$\Delta_x = \begin{vmatrix} 7 & 3 \\ 5 & -1 \end{vmatrix} = (7 \times -1) - (3 \times 5) = -7 - 15 = -22$$
3. Form $\Delta_y$ by replacing the second column with the constants vector:
$$\Delta_y = \begin{vmatrix} 2 & 7 \\ 3 & 5 \end{vmatrix} = (2 \times 5) - (7 \times 3) = 10 - 21 = -11$$
4. Compute variables using the ratio parameters:
$$x = \frac{\Delta_x}{\Delta} = \frac{-22}{-11} = 2, \quad y = \frac{\Delta_y}{\Delta} = \frac{-11}{-11} = 1$$
5. Conclusion: $x = 2, y = 1$.

---

### Terminal Exercises & Self-Check Questions

1. **Equation Verification Workout:** Find the value of $x$ if $\begin{vmatrix} x & 2 \\ 4 & x \end{vmatrix} = 0$.
   * *Answer Hint:* Expand the equation layout: $x^2 - 8 = 0 \implies x^2 = 8 \implies x = \pm\sqrt{8} = \pm2\sqrt{2}$.

2. **Property Application Exercise:** Without expanding, show that $\begin{vmatrix} 2 & 3 & 5 \\ 7 & 8 & 9 \\ 4 & 6 & 10 \end{vmatrix} = 0$.
   * *Step-by-Step Solution:* 1. Look closely at Row 1 ($R_1 = [2, 3, 5]$) and Row 3 ($R_3 = [4, 6, 10]$).
     2. Factor out a common scalar constant of 2 from Row 3:
        $$\Delta = 2 \times \begin{vmatrix} 2 & 3 & 5 \\ 7 & 8 & 9 \\ 2 & 3 & 5 \end{vmatrix}$$
     3. Notice that Row 1 and Row 3 are now completely identical ($R_1 = R_3$).
     4. By the Identity Property of determinants, any determinant with two identical rows equals 0. Thus, $\Delta = 2 \times 0 = 0$.

3. **Consistency Parameter Analysis:** Under what condition will a system of equations handled via Cramer's Rule fail to yield a single unique solution?
   * *Answer Hint:* The calculation fails to produce a unique solution when the baseline coefficient determinant is zero ($\Delta = 0$). If $\Delta = 0$ and any numerator $\Delta_x, \Delta_y, \Delta_z \neq 0$, the system is inconsistent and has no solution. If all determinants equal zero, the system has infinitely many solutions.