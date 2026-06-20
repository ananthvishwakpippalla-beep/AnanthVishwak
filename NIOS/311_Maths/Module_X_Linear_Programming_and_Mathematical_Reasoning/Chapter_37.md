# NIOS Senior Secondary Mathematics (311)

## Module X: Linear Programming and Mathematical Reasoning
### Chapter 37: Linear Programming

### Introduction & Key Objectives
In real-world business, engineering, and economics, data-driven decisions are constrained by limited resources—such as finite capital, restricted factory hours, limited raw materials, or workforce caps. **Linear Programming (LP)** is a powerful mathematical optimization technique developed to determine the best possible outcome (such as maximizing profits or minimizing structural costs) under a strict system of linear constraints. This chapter introduces the formulation of linear programming problems (LPP) and their geometric solution via the graphical method.

After studying this chapter, you will be able to:
* Define a **Linear Programming Problem (LPP)** and identify its structural components.
* Formulate an LPP mathematically from a real-world descriptive problem.
* Graphically map linear inequalities to identify the **Feasible Region**.
* Differentiate between bounded and unbounded feasible regions.
* Apply the **Corner Point Method** to find the optimal solution (Maximum or Minimum values).

---

### Core Concepts & Formulas

#### 1. Core Terminology of LPP
An LPP structurally consists of three distinct mathematical components:
* **Objective Function ($Z$):** The linear function that needs to be optimized (maximized or minimized). It is typically expressed in the form:
  $$Z = ax + by$$
  *(where $a$ and $b$ are constant cost/profit coefficients, and $x$ and $y$ are called **Decision Variables**).*
* **Constraints:** A system of linear inequalities or equations that restrict the decision variables based on resource limitations (e.g., $gx + hy \le k$).
* **Non-Negative Restrictions:** Physical quantities cannot be negative, which enforces the quadrant constraint:
  $$x \ge 0, \quad y \ge 0$$

#### 2. Geometric Definitions
* **Feasible Region:** The common region determined by all the given constraints and non-negative restrictions simultaneously. Any point inside or on the boundary of this region is a **Feasible Solution**.
* **Infeasible Region:** Any area outside the feasible region where constraints are violated.
* **Optimal Solution:** A feasible solution that achieves the absolute highest possible maximum profit or lowest possible minimum cost for the objective function $Z$.

---

#### 3. The Corner Point Theorem
> **Fundamental Theorem:** If an optimal solution to an LPP exists, it **must occur at one of the corner points (vertices)** of the feasible region.



> **The Corner Point Method Protocol:**
> 1. Formulate the mathematical constraints and graph them on a Cartesian plane.
> 2. Shade the overlapping area to isolate the **Feasible Region**.
> 3. Identify and calculate the exact coordinates $(x, y)$ of all **Corner Points (Vertices)** of the region by solving the corresponding system of intersecting line equations.
> 4. Substitute the coordinates of each corner point into the objective function $Z = ax + by$.
> 5. Select the largest resulting value (for maximization problems) or the smallest value (for minimization problems) to establish your final optimal solution.

---

### Step-by-Step Formulation & Solution

**Example 1:** A manufacturer produces two items: Product X and Product Y. Each unit of Product X yields a profit of $40 \text{ INR}$, while Product Y yields $30 \text{ INR}$. Product X requires 2 hours of machine processing, and Product Y requires 1 hour. The total available machine runtime is 60 hours per week. Formulate this scenario as a mathematical Linear Programming Problem.  
**Solution:**
1. Identify the decision variables: Let $x$ be the number of units of Product X produced per week, and $y$ be the number of units of Product Y.
2. Formulate the Objective Function ($Z$) to maximize weekly profit:
$$\text{Maximize } Z = 40x + 30y$$
3. Formulate the linear resource constraints based on machine processing time limits:
$$2x + 1y \le 60$$
4. Append the non-negative baseline constraints since manufacturing counts cannot drop below zero:
$$x \ge 0, \quad y \ge 0$$
5. Assembled LPP Framework:
$$\begin{aligned} \text{Maximize } &Z = 40x + 30y \\ \text{Subject to: } &2x + y \le 60 \\ &x \ge 0, \quad y \ge 0 \end{aligned}$$

**Example 2:** Solve the following LPP graphically using the Corner Point Method:
$$\begin{aligned} \text{Maximize } &Z = 3x + 5y \\ \text{Subject to: } &x + 2y \le 8 \\ &3x + 2y \le 12 \\ &x \ge 0, \quad y \ge 0 \end{aligned}$$

**Solution:**
1. Plot the boundary lines by treating the inequalities as strict equations:
   * **Line 1:** $x + 2y = 8 \implies$ Passes through intercept points $(8, 0)$ and $(0, 4)$.
   * **Line 2:** $3x + 2y = 12 \implies$ Passes through intercept points $(4, 0)$ and $(0, 6)$.
2. Determine the valid direction of the shaded inequalities by testing the origin $(0,0)$:
   * $0 + 2(0) = 0 \le 8$ (True $\implies$ Shade inward toward the origin)
   * $3(0) + 2(0) = 0 \le 12$ (True $\implies$ Shade inward toward the origin)
3. Identify the enclosed intersection vertices of the bounded feasible region. The region is a four-sided polygon with corner points at:
   * $O(0, 0)$
   * $A(4, 0)$
   * $B$: The intersection point of the two lines. Solve the system:
     $$(3x + 2y) - (x + 2y) = 12 - 8 \implies 2x = 4 \implies x = 2$$
     Substitute $x = 2$ back into Line 1: $2 + 2y = 8 \implies 2y = 6 \implies y = 3$. This gives point $B(2, 3)$.
   * $C(0, 4)$
4. Evaluate the Objective Function $Z = 3x + 5y$ at each vertex position:

| Corner Point Vertex | Coordinates $(x, y)$ | Value of $Z = 3x + 5y$ |
| :--- | :--- | :--- |
| $O$ | $(0, 0)$ | $Z = 3(0) + 5(0) = 0$ |
| $A$ | $(4, 0)$ | $Z = 3(4) + 5(0) = 12$ |
| **$B$ (Optimal)** | **$(2, 3)$** | **$Z = 3(2) + 5(3) = 6 + 15 = 21$** |
| $C$ | $(0, 4)$ | $Z = 3(0) + 5(4) = 20$ |

5. Conclusion: The objective function achieves its absolute **Maximum value of 21** at the coordinate point **$(2, 3)$**.

---

### Terminal Exercises & Self-Check Questions

1. **Constraint Parameter Evaluation:** Graph the linear inequality $x - y \ge 0$. Does the origin verification point $(0,0)$ help determine the shaded half-plane side?
   * *Answer Hint:* No. Because the boundary line $x = y$ passes directly through the origin, substituting $(0,0)$ yields $0 \ge 0$, which does not isolate a specific half-plane side. You must choose an alternative verification point off the line, such as $(2,1) \implies 2 - 1 = 1 \ge 0$ (True), to show the region lies on the lower-right side of the boundary line.

2. **Feasible Region Verification:** Consider an LPP constraint profile given as $x + y \le 4$ and $x + y \ge 6$ under $x, y \ge 0$. Describe its feasible region.
   * *Step-by-Step Solution:* 1. Plot line $x + y = 4$ and shade inward toward the origin.
     2. Plot line $x + y = 6$ and shade outward away from the origin.
     3. Observe that these two parallel lines run away from each other, creating zero spatial overlap.
     4. Since no coordinate space satisfies both parameters simultaneously, the problem has **No Feasible Region** and zero solutions can be evaluated.

3. **Multiple Optimal Solutions Identity:** Under what geometric condition can an LPP objective function achieve the exact same maximum value at two distinct corner points?
   * *Answer Hint:* If the objective function yields the identical optimal value at two different vertices, it will achieve that exact same value at **every single point lying along the straight line segment joining those two vertices**. This scenario is called an LPP with infinitely many optimal solutions.