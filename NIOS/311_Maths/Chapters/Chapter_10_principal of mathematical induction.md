# NIOS Senior Secondary Mathematics (311)

## Chapter 10: Principle of Mathematical Induction

### Introduction & Key Objectives
In mathematics, we often discover general properties or patterns by examining specific cases. However, checking a finite number of cases is not sufficient to prove that a statement is universally true for all natural numbers. The Principle of Mathematical Induction (PMI) provides a rigorous deductive technique to prove mathematical propositions, identities, and inequalities for the infinite set of natural numbers $\mathbb{N}$.

After studying this chapter, you will be able to:
* Understand the concept of a mathematical statement $P(n)$.
* Comprehend the logical structure of inductive proofs.
* Apply the **Principle of Mathematical Induction** to prove summation identities.
* Apply PMI to verify divisibility properties of algebraic expressions.

---

### Core Concepts & Formulas

#### 1. What is a Mathematical Statement?
A statement or proposition $P(n)$ is a declarative sentence involving a natural number variable $n$ which can be classified as either uniquely true or false for any specific value of $n \in \mathbb{N}$.
* *Example:* Let $P(n): 1 + 2 + 3 + \dots + n = \frac{n(n+1)}{2}$.
* To test $P(1)$, substitute $n=1$: $\text{LHS} = 1$, $\text{RHS} = \frac{1(1+1)}{2} = 1$. Thus, $P(1)$ is true.

#### 2. The Two Core Steps of PMI
To prove that a mathematical statement $P(n)$ is true for all natural numbers $n \in \mathbb{N}$, we follow a strict two-step proof procedure:

> **Step 1: The Base Step (Inductive Base)**
> Prove that the statement is true for the first natural number, i.e., $P(1)$ is true. (In some problem contexts, if the domain specifies $n \ge \text{constant}$, check the lowest valid value instead).

> **Step 2: The Inductive Step**
> * **Assumption:** Assume that the statement is true for a general positive integer $k$, i.e., assume $P(k)$ is true. This assumption is called the **Inductive Hypothesis**.
> * **Proof:** Using the inductive hypothesis as a true mathematical fact, prove that the statement must logically be true for the next subsequent integer $k + 1$, i.e., prove $P(k+1)$ is true.

If both the Base Step and the Inductive Step are successfully completed, then by the Principle of Mathematical Induction, $P(n)$ is true for all $n \in \mathbb{N}$.



---

### Step-by-Step Examples

**Example 1 (Summation Identity):** Prove by mathematical induction that for all $n \in \mathbb{N}$:
$$1 + 3 + 5 + \dots + (2n - 1) = n^2$$

**Solution:**
Let the given statement be $P(n): 1 + 3 + 5 + \dots + (2n - 1) = n^2$.

1. **Base Step ($n = 1$):**
   * $\text{LHS} = 2(1) - 1 = 1$
   * $\text{RHS} = 1^2 = 1$
   * Since $\text{LHS} = \text{RHS}$, $P(1)$ is **true**.

2. **Inductive Step:**
   * **Hypothesis:** Assume $P(k)$ is true for some $k \in \mathbb{N}$. This means we assume:
     $$1 + 3 + 5 + \dots + (2k - 1) = k^2 \quad \text{--- (Equation 1)}$$
   * **Goal:** We need to prove that $P(k+1)$ is true. Let's look at the expression for $P(k+1)$:
     $$1 + 3 + 5 + \dots + (2k - 1) + [2(k + 1) - 1] = (k + 1)^2$$
   * **Proof:** Take the left-hand side ($\text{LHS}$) of $P(k+1)$:
     $$\text{LHS} = \underbrace{1 + 3 + 5 + \dots + (2k - 1)}_{\text{Substitute from Equation 1}} + (2k + 2 - 1)$$
     $$\text{LHS} = k^2 + (2k + 1)$$
     $$\text{LHS} = k^2 + 2k + 1$$
   * Recognizing the perfect square binomial expansion:
     $$\text{LHS} = (k + 1)^2 = \text{RHS of } P(k+1)$$
   * Thus, $P(k+1)$ is true whenever $P(k)$ is true.

3. **Conclusion:** Both steps are satisfied. Therefore, by the Principle of Mathematical Induction, the statement is true for all $n \in \mathbb{N}$.

**Example 2 (Divisibility Property):** Prove by mathematical induction that $7^n - 3^n$ is divisible by 4 for all $n \in \mathbb{N}$.

**Solution:**
Let $P(n): 7^n - 3^n \text{ is divisible by } 4$.

1. **Base Step ($n = 1$):**
   * $P(1) = 7^1 - 3^1 = 7 - 3 = 4$
   * Since 4 is divisible by 4, $P(1)$ is **true**.

2. **Inductive Step:**
   * **Hypothesis:** Assume $P(k)$ is true. This means $7^k - 3^k$ is a multiple of 4:
     $$7^k - 3^k = 4m \quad (\text{where } m \in \mathbb{Z}) \implies 7^k = 4m + 3^k \quad \text{--- (Equation 2)}$$
   * **Goal:** Prove $P(k+1)$ is true, i.e., $7^{k+1} - 3^{k+1}$ is a multiple of 4.
   * **Proof:** Write out the expression for $k+1$:
     $$7^{k+1} - 3^{k+1} = 7^1 \cdot 7^k - 3^{k+1}$$
   * Substitute the expression for $7^k$ from Equation 2:
     $$= 7(4m + 3^k) - 3^{k+1}$$
     $$= 28m + 7 \cdot 3^k - 3 \cdot 3^k$$
   * Factor out $3^k$ from the last two terms:
     $$= 28m + (7 - 3) \cdot 3^k$$
     $$= 28m + 4 \cdot 3^k$$
   * Factor out 4 from the entire expression:
     $$= 4(7m + 3^k)$$
   * Since $(7m + 3^k)$ is an integer, $4(7m + 3^k)$ is clearly a multiple of 4. Thus, $P(k+1)$ is **true**.

3. **Conclusion:** By PMI, $7^n - 3^n$ is divisible by 4 for all $n \in \mathbb{N}$.

---

### Terminal Exercises & Self-Check Questions

1. **Identity Verification Workout:** Use PMI to prove that $1^2 + 2^2 + 3^2 + \dots + n^2 = \frac{n(n+1)(2n+1)}{6}$.
   * *Strategy Hint:* Assume the equation is valid for $k$. For $k+1$, add $(k+1)^2$ to both sides of the inductive equation: $\frac{k(k+1)(2k+1)}{6} + (k+1)^2$. Factor out $(k+1)$ and find a common denominator to simplify the expression to $\frac{(k+1)(k+2)(2k+3)}{6}$.

2. **Divisibility Problem:** Prove using mathematical induction that $n(n+1)(n+2)$ is divisible by 6 for all natural numbers.
   * *Strategy Hint:* Verify for $n=1 \implies 1(2)(3) = 6$ (True). Assume for $k$: $k(k+1)(k+2) = 6m$. For $k+1$, the expression becomes $(k+1)(k+2)(k+3) = (k+1)(k+2)k + 3(k+1)(k+2) = 6m + 3(k+1)(k+2)$. Since either $(k+1)$ or $(k+2)$ must be an even number, their product is a multiple of 2, making $3(k+1)(k+2)$ divisible by 6.