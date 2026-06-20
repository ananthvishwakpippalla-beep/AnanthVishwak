# NIOS Senior Secondary Mathematics (311)

## Module VI: Algebra-II
### Chapter 20: Matrices

### Introduction & Key Objectives
In the middle of the 19th century, the English mathematician Arthur Cayley (1821–1895) introduced matrices as a powerful tool to represent and solve simultaneous systems of linear equations. Today, matrix algebra is an indispensable framework utilized not only across advanced mathematics, but also in economics (input-output tables), computer graphics, game theory, physics, and engineering. This chapter introduces multi-dimensional rectangular arrays, their structural classification, and fundamental algebraic properties.

After studying this chapter, you will be able to:
* Define a **Matrix** and identify its **Order**.
* Classify various types of matrices (Row, Column, Square, Rectangular, Zero, Diagonal, Scalar, and Identity matrices).
* State and apply the conditions for the **Equality of Two Matrices**.
* Perform matrix **Addition**, **Subtraction**, and **Scalar Multiplication**.
* State the compatibility criteria for **Matrix Multiplication** and multiply conforming matrices.
* Define and find the **Transpose** of a matrix.
* Differentiate between **Symmetric** and **Skew-Symmetric Matrices**.

---

### Core Concepts & Formulas

#### 1. Definition and Notation
> **Matrix:** A matrix is a well-defined rectangular arrangement of numbers or functions disposed in horizontal lines called **Rows** and vertical lines called **Columns**.

An $m \times n$ matrix (read as "$m$ by $n$") has exactly $m$ rows and $n$ columns, which defines its **Order**. A general matrix $A$ is represented compactly as:
$$A = [a_{ij}]_{m \times n}$$
*(where $a_{ij}$ represents the individual element located at the intersection of the $i^{\text{th}}$ row and the $j^{\text{th}}$ column, $1 \le i \le m$ and $1 \le j \le n$).*

#### 2. Classification of Matrices
* **Row Matrix:** A matrix having only one single row ($1 \times n$).
* **Column Matrix:** A matrix having only one single column ($m \times 1$).
* **Rectangular Matrix:** A matrix where the number of rows is not equal to the columns ($m \neq n$).
* **Square Matrix:** A matrix where the number of rows equals the columns ($m = n$).
* **Zero (Null) Matrix ($O$):** A matrix in which every individual element is exactly 0.
* **Diagonal Matrix:** A square matrix where all elements outside the principal diagonal are zero ($a_{ij} = 0$ for all $i \neq j$).
* **Scalar Matrix:** A diagonal matrix in which all elements along the principal diagonal are equal to a common constant value.
* **Identity (Unit) Matrix ($I$):** A diagonal matrix in which all elements along the principal diagonal are exactly equal to 1.
  $$I_2 = \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix}, \quad I_3 = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}$$

#### 3. Equality of Matrices
Two matrices $A = [a_{ij}]$ and $B = [b_{ij}]$ are mathematically **equal** ($A = B$) if and only if:
1. They possess the exact same order (same dimensions).
2. Their corresponding elements are identical ($a_{ij} = b_{ij}$ for all values of $i$ and $j$).

---

#### 4. Algebraic Operations
* **Addition and Subtraction:** Two matrices can be added or subtracted if and only if they share the **same order**. The result is obtained by performing the operation on corresponding entries:
  $$A \pm B = [a_{ij} \pm b_{ij}]$$
* **Scalar Multiplication:** Multiplying a matrix by a scalar constant $k$ requires multiplying **every individual element** inside the matrix by $k$:
  $$k \cdot A = [k \cdot a_{ij}]$$

#### 5. Matrix Multiplication (Row-by-Column)
> **Compatibility Rule:** The product $AB$ of two matrices $A$ and $B$ is defined if and only if the **number of columns in matrix $A$ equals the number of rows in matrix $B$**.

If $A$ is of order $m \times p$ and $B$ is of order $p \times n$, then the resulting product matrix $C = AB$ will have an order of **$m \times n$**.



The entry $c_{ij}$ is calculated by taking the sum of the products of the elements from the $i^{\text{th}}$ row of $A$ with the corresponding elements of the $j^{\text{th}}$ column of $B$:
$$c_{ij} = \sum_{k=1}^{p} a_{ik} b_{kj}$$
* *Crucial Note:* Matrix multiplication is generally **non-commutative** ($AB \neq BA$).

---

#### 6. Transpose and Symmetry
> **Transpose of a Matrix ($A^T$ or $A'$):** The matrix obtained by interchanging the rows and columns of a given matrix $A$. If $A$ is $m \times n$, then $A^T$ is $n \times m$.

* **Symmetric Matrix:** A square matrix $A$ is symmetric if it is identical to its transpose:
> $$A^T = A \quad (\text{meaning } a_{ij} = a_{ji})$$

* **Skew-Symmetric Matrix:** A square matrix $A$ is skew-symmetric if it equals its negative transpose:
> $$A^T = -A \quad (\text{meaning } a_{ij} = -a_{ji})$$
* *Property Rule:* All principal diagonal elements of a skew-symmetric matrix are always strictly **zero** ($a_{ii} = 0$).

---

### Step-by-Step Examples

**Example 1:** Find the values of variables $x, y, z,$ and $a$ if the two matrices are equal:
$$\begin{bmatrix} x + 3 & 2z \\ y - 1 & 4a \end{bmatrix} = \begin{bmatrix} 5 & 6 \\ -2 & 12 \end{bmatrix}$$

**Solution:**
1. Since the matrices are equal, equate their corresponding positions to set up individual equations:
   * Position (1,1): $x + 3 = 5 \implies x = 5 - 3 = 2$
   * Position (1,2): $2z = 6 \implies z = \frac{6}{2} = 3$
   * Position (2,1): $y - 1 = -2 \implies y = -2 + 1 = -1$
   * Position (2,2): $4a = 12 \implies a = \frac{12}{4} = 3$
2. Conclusion: $x = 2, y = -1, z = 3, a = 3$.

**Example 2:** Given matrices $A = \begin{bmatrix} 1 & 3 \\ 2 & 4 \end{bmatrix}$ and $B = \begin{bmatrix} 5 & -1 \\ 0 & 2 \end{bmatrix}$, calculate the product matrix $AB$.  
**Solution:**
1. Check compatibility: Order of $A$ is $2 \times 2$, order of $B$ is $2 \times 2$. Since columns of $A$ (2) equals rows of $B$ (2), multiplication is valid. The output will be $2 \times 2$.
2. Apply the row-by-column tracking method:
   * **Row 1 $\times$ Col 1:** $(1 \times 5) + (3 \times 0) = 5 + 0 = 5$
   * **Row 1 $\times$ Col 2:** $(1 \times -1) + (3 \times 2) = -1 + 6 = 5$
   * **Row 2 $\times$ Col 1:** $(2 \times 5) + (4 \times 0) = 10 + 0 = 10$
   * **Row 2 $\times$ Col 2:** $(2 \times -1) + (4 \times 2) = -2 + 8 = 6$
3. Assemble the product matrix:
$$AB = \begin{bmatrix} 5 & 5 \\ 10 & 6 \end{bmatrix}$$

**Example 3:** Prove that for any square matrix $A$, the matrix $A + A^T$ is always symmetric.  
**Solution:**
1. Let a placeholder matrix be defined as $Y = A + A^T$.
2. Take the transpose of both sides:
$$Y^T = (A + A^T)^T$$
3. Apply the reversal/distribution law of matrix transpose geometry ($(A + B)^T = A^T + B^T$ and $(A^T)^T = A$):
$$Y^T = A^T + (A^T)^T = A^T + A$$
4. Since matrix addition is commutative ($A^T + A = A + A^T$):
$$Y^T = A + A^T = Y$$
5. Since $Y^T = Y$, the combined expression matrix $A + A^T$ is successfully proven to be **symmetric**.

---

### Terminal Exercises & Self-Check Questions

1. **Order Matrix Analysis:** If a matrix has exactly 12 individual elements, write out all the possible unique structural orders it could possess.
   * *Answer Hint:* List all unique positive integer factor pairs multiplying to 12: $1 \times 12$, $12 \times 1$, $2 \times 6$, $6 \times 2$, $3 \times 4$, and $4 \times 3$. There are 6 possible structural orders.

2. **Algebraic Identity Workout:** Given matrix $M = \begin{bmatrix} 2 & -3 \\ 1 & 5 \end{bmatrix}$, compute the matrix value of $3M - 2I_2$.
   * *Step-by-Step Solution:* 1. Calculate the scalar product $3M$:
        $$3M = \begin{bmatrix} 3(2) & 3(-3) \\ 3(1) & 3(5) \end{bmatrix} = \begin{bmatrix} 6 & -9 \\ 3 & 15 \end{bmatrix}$$
     2. Calculate the scalar identity matrix $2I_2$:
        $$2I_2 = \begin{bmatrix} 2 & 0 \\ 0 & 2 \end{bmatrix}$$
     3. Perform the subtraction:
        $$3M - 2I_2 = \begin{bmatrix} 6-2 & -9-0 \\ 3-0 & 15-2 \end{bmatrix} = \begin{bmatrix} 4 & -9 \\ 3 & 13 \end{bmatrix}$$

3. **Multiplication Constraints Verification:** If matrix $X$ has an order of $3 \times 4$ and matrix $Y$ has an order of $4 \times 2$, check if products $XY$ and $YX$ are valid.
   * *Answer Hint:* For $XY$, columns of $X$ (4) equals rows of $Y$ (4), so **$XY$ is valid** (resulting in a $3 \times 2$ matrix). For $YX$, columns of $Y$ (2) does not equal rows of $X$ (3), so **$YX$ is invalid** and cannot be computed.