# NIOS Senior Secondary Mathematics (311)

## Module VIII: Calculus
### Chapter 32: Differential Equations

### Introduction & Key Objectives
Throughout our study of calculus, we have looked at functions and discovered their derivatives ($\frac{dy}{dx}$), and conversely, taken derivatives and Integrated them back to find the original functions. In real-world physics, engineering, and economics, relationships are rarely given as direct functional formulas. Instead, laws of nature dictate how a system changes—meaning equations naturally involve independent variables, dependent variables, and their derivatives. Such equations are called **Differential Equations**. This final calculus chapter covers how to classify these equations and solve standard first-order, first-degree differential forms.

After studying this chapter, you will be able to:
* Define a **Differential Equation** and distinguish it from standard algebraic equations.
* Determine the **Order** and **Degree** of a differential equation.
* Understand the difference between a **General Solution** and a **Particular Solution**.
* Form a differential equation by eliminating arbitrary constants from a family of curves.
* Solve first-order, first-degree differential equations using the **Method of Variable Separable**.

---

### Core Concepts & Formulas

#### 1. Definition, Order, and Degree
> **Differential Equation (DE):** An equation containing an independent variable ($x$), a dependent variable ($y$), and the derivatives of the dependent variable with respect to the independent variable ($\frac{dy}{dx}, \frac{d^2y}{dx^2}$, etc.).

* **Order:** The order of a differential equation is the order of the **highest-order derivative** appearing in the equation.
* **Degree:** The degree of a differential equation is the **highest power (positive integral exponent)** of the highest-order derivative, provided the equation is expressible as a polynomial equation in terms of its derivatives. If derivatives are trapped inside transcendental functions (like $\sin(\frac{dy}{dx})$ or $e^{dy/dx}$), the degree is **not defined**.

*Example:* For the equation $\left(\frac{d^2y}{dx^2}\right)^3 + \left(\frac{dy}{dx}\right)^4 + y = 0$:
$$\text{Highest Derivative} = \frac{d^2y}{dx^2} \implies \text{Order} = 2$$
$$\text{Power of Highest Derivative} = 3 \implies \text{Degree} = 3$$

#### 2. General vs. Particular Solutions
* **General Solution (Complete Primitive):** A solution which contains as many arbitrary constants ($C_1, C_2$, etc.) as the order of the differential equation.
* **Particular Solution:** A solution obtained from the general solution by giving specific values to the arbitrary constants based on given boundary/initial conditions (e.g., finding the exact constant $C$ when $x=0, y=1$).

#### 3. Method of Variable Separable
This is the primary equation-solving method emphasized in the NIOS examination for first-order, first-degree equations. If a differential equation can be algebraically rearranged such that all terms containing $y$ (including $dy$) cluster on one side, and all terms containing $x$ (including $dx$) cluster on the other side, it can be solved by direct integration:

> $$\frac{dy}{dx} = f(x) \cdot g(y) \implies \frac{1}{g(y)} \, dy = f(x) \, dx$$
> Now integrate both sides to find the solution:
> $$\int \frac{1}{g(y)} \, dy = \int f(x) \, dx + C$$



---

### Step-by-Step Examples

**Example 1:** Find the order and degree of the differential equation: $x \left(\frac{d^2y}{dx^2}\right)^2 + y \left(\frac{dy}{dx}\right)^4 - \frac{dy}{dx} = 0$.  
**Solution:**
1. Identify the highest-order derivative present in the expression: $\frac{d^2y}{dx^2}$ (a second derivative). Therefore:
$$\text{Order} = 2$$
2. Identify the exponent power raised on that highest derivative: $\left(\frac{d^2y}{dx^2}\right)^2$. Therefore:
$$\text{Degree} = 2$$

**Example 2:** Form the differential equation representing the family of curves given by $y = A e^{2x} + B e^{-2x}$, where $A$ and $B$ are arbitrary constants.  
**Solution:**
1. Count the arbitrary constants: There are two constants ($A$ and $B$). This means we must differentiate the equation exactly **twice** to set up a substitution network to eliminate them.
2. Differentiate the equation the first time with respect to $x$:
$$\frac{dy}{dx} = 2A e^{2x} - 2B e^{-2x} \quad \text{--- (Equation 1)}$$
3. Differentiate a second time with respect to $x$:
$$\frac{d^2y}{dx^2} = 4A e^{2x} + 4B e^{-2x}$$
4. Factor out the common scalar constant 4 from the right-hand expression:
$$\frac{d^2y}{dx^2} = 4(A e^{2x} + B e^{-2x})$$
5. Notice that the expression inside the brackets matches our original definition of $y$. Substitute $y$ back in to eliminate $A$ and $B$:
$$\frac{d^2y}{dx^2} = 4y \implies \frac{d^2y}{dx^2} - 4y = 0$$

**Example 3:** Solve the differential equation $\frac{dy}{dx} = \frac{1 + y^2}{1 + x^2}$ given the initial boundary condition that $y = 1$ when $x = 0$.  
**Solution:**
1. Separate the variables by cross-multiplying $dx$ and dividing by $(1 + y^2)$:
$$\frac{1}{1 + y^2} \, dy = \frac{1}{1 + x^2} \, dx$$
2. Integrate both sides using standard inverse trigonometric integration formulas ($\int \frac{1}{1+x^2}dx = \tan^{-1}x$):
$$\int \frac{1}{1 + y^2} \, dy = \int \frac{1}{1 + x^2} \, dx$$
$$\tan^{-1}y = \tan^{-1}x + C \quad \text{--- (General Solution)}$$
3. Substitute the given initial conditions ($x = 0$ and $y = 1$) to locate the exact value of the **Particular Constant ($C$)**:
$$\tan^{-1}(1) = \tan^{-1}(0) + C$$
$$\frac{\pi}{4} = 0 + C \implies C = \frac{\pi}{4}$$
4. Substitute the value of $C$ back into the general solution equation:
$$\tan^{-1}y = \tan^{-1}x + \frac{\pi}{4} \quad \text{--- (Particular Solution)}$$

---

### Terminal Exercises & Self-Check Questions

1. **Transcendental Degree Analysis:** State the order and degree of the differential equation: $\frac{d^2y}{dx^2} + \sin\left(\frac{dy}{dx}\right) = 0$.
   * *Answer Hint:* The highest derivative is $\frac{d^2y}{dx^2}$, so **Order = 2**. However, the first derivative is trapped inside a sine wave function expansion. Because the equation cannot be written as a standard polynomial in terms of its derivatives, the **Degree is Not Defined**.

2. **Basic Separation Workout:** Find the general solution of the differential equation $\frac{dy}{dx} = 3x^2 y$.
   * *Step-by-Step Solution:* 1. Separate variables: $\frac{1}{y} \, dy = 3x^2 \, dx$.
     2. Integrate both sides: $\int \frac{1}{y} \, dy = \int 3x^2 \, dx$.
     3. Apply standard rules: $\log_e |y| = \frac{3x^3}{3} + C \implies \log_e |y| = x^3 + C$.
     4. Express explicitly by raising to base $e$: $y = e^{x^3 + C} = e^C \cdot e^{x^3} \implies y = A e^{x^3}$ (where $A = e^C$).

3. **Particular Constant Extraction:** Solve the equation $\frac{dy}{dx} = e^{-2y}$ given that $y = 0$ when $x = 0$.
   * *Answer Hint:* Separate variables to get $e^{2y} \, dy = dx$. Integrate both sides: $\frac{e^{2y}}{2} = x + C$. Substitute initial values ($x=0, y=0$) to find $C$: $\frac{e^0}{2} = 0 + C \implies C = \frac{1}{2}$. Write the final particular solution: $\frac{e^{2y}}{2} = x + \frac{1}{2} \implies e^{2y} = 2x + 1 \implies y = \frac{1}{2}\log_e(2x+1)$.