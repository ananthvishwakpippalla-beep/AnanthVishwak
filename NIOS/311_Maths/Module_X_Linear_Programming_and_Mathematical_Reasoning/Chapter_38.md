# NIOS Senior Secondary Mathematics (311)

## Module X: Linear Programming and Mathematical Reasoning
### Chapter 38: Mathematical Reasoning

### Introduction & Key Objectives
In everyday language, we use sentences of various types—declarative, interrogative, exclamatory, and imperative. However, human language can be ambiguous, subjective, or dependent on context. Mathematics requires an absolute, unambiguous foundation where statements are strictly objective. This final chapter introduces **Mathematical Reasoning**, a branch of formal logic that establishes how mathematical propositions are constructed, combined using logical connectives, and rigorously proven.

After studying this chapter, you will be able to:
* Identify whether a given sentence is a mathematically valid **Statement**.
* Understand and construct the **Negation** of a statement.
* Define and use logical connectives to form **Compound Statements** ("And", "Or").
* Interpret conditional statements involving implications like **"If-then"** and **"Only if"**.
* Write and distinguish between the **Converse**, **Inverse**, and **Contrapositive** of a conditional statement.
* Understand fundamental methods of proof, including the **Method of Contradiction**.

---

### Core Concepts & Formulas

#### 1. Mathematically Acceptable Statements
> **Mathematical Statement:** A declarative sentence is a mathematically acceptable statement if it is **either strictly true or strictly false, but not both simultaneously**. 

Sentences that are subjective, exclamatory, interrogative, commands, or involve variable time/space anchors (like "Tomorrow is a sunny day" or "Mathematics is a difficult subject") are **not** mathematical statements.

#### 2. Negation of a Statement
The denial of a statement is called its **Negation**. If a statement is denoted by $p$, its negation is denoted by $\sim p$ (read as "not $p$").
* If $p$ is True ($\text{T}$), then $\sim p$ is strictly False ($\text{F}$).
* If $p$ is False ($\text{F}$), then $\sim p$ is strictly True ($\text{T}$).

---

#### 3. Compound Statements and Connectives
A compound statement is formed by combining two or more simple statements (called **Component Statements**) using logical connecting words.

##### A. The Connective "AND" ($\wedge$)
A compound statement joined by "And" is mathematically true **if and only if all its component statements are simultaneously true**. If even one component is false, the entire statement is false.

##### B. The Connective "OR" ($\vee$)
A compound statement joined by "Or" is mathematically true **if at least one of its component statements is true**. It only evaluates to false if every single component is false.
* *Inclusive OR:* Both components can happen at the same time (e.g., "To get a driving license, you must have an Aadhaar card or a Passport").
* *Exclusive OR:* Both components cannot happen together (e.g., "A number is either even or odd").

---

#### 4. Conditional Implications ("If-then")
A conditional statement matches the template **"If $p$, then $g$"**, denoted as $p \implies q$. From this baseline implication, we can derive three related conditional variations:



* **Converse:** Formed by swapping the hypothesis and the conclusion.
  $$\text{If } q, \text{ then } p \quad (q \implies p)$$
* **Inverse:** Formed by negating both the hypothesis and the conclusion.
  $$\text{If } \sim p, \text{ then } \sim q \quad (\sim p \implies \sim q)$$
* **Contrapositive:** Formed by swapping and negating both components.
  $$\text{If } \sim q, \text{ then } \sim p \quad (\sim q \implies \sim p)$$
* *Crucial Note:* A conditional statement ($p \implies q$) is mathematically equivalent to its **Contrapositive** ($\sim q \implies \sim p$).

---

#### 5. Methods of Mathematical Proof
To validate a statement, mathematicians employ standard structural proof methods:
* **Direct Proof:** Assuming $p$ is true and logically deriving that $q$ must be true.
* **Proof by Contrapositive:** Proving that if $\sim q$ is true, then $\sim p$ must logically follow.
* **Proof by Contradiction:** A powerful indirect proof strategy.
  1. Assume the statement you want to prove is false (i.e., assume $\sim p$ is true).
  2. Carry out logical algebraic or geometric deductions based on this assumption.
  3. Arrive at a conclusion that breaks an established mathematical rule or directly contradicts your opening premise.
  4. Conclude that your original assumption ($\sim p$) must be false, which proves that $p$ is inherently true.

---

### Step-by-Step Examples

**Example 1:** Examine whether the following sentences are mathematically acceptable statements. Give reasons.
1. "The sum of angles in a triangle is $180^\circ$."
2. "Close the window immediately."
3. "Every square is a rectangle."

**Solution:**
1. This is a declarative sentence that is objectively and universally **True**. Therefore, it **is a mathematical statement**.
2. This is an imperative command or order. It cannot be assigned a true or false value. Therefore, it **is not a mathematical statement**.
3. This is a declarative geometric property that is objectively and universally **True**. Therefore, it **is a mathematical statement**.

**Example 2:** Write down the Converse and the Contrapositive of the following conditional implication:  
*"If a natural number is divisible by 10, then it is divisible by 5."* **Solution:**
1. Break the sentence down into its component parts:
   * $p$: A natural number is divisible by 10.
   * $q$: A natural number is divisible by 5.
2. Formulate the **Converse** ($q \implies p$):
   * *"If a natural number is divisible by 5, then it is divisible by 10."* (Note: The converse here happens to be false, as 15 is divisible by 5 but not 10).
3. Formulate the **Contrapositive** ($\sim q \implies \sim p$):
   * *"If a natural number is not divisible by 5, then it is not divisible by 10."* (This statement is universally true).

**Example 3:** Prove that $\sqrt{2}$ is an irrational number using the Method of Contradiction.  
**Solution:**
1. State the contradictory assumption: Assume that $\sqrt{2}$ is **not** irrational, meaning it is a **Rational Number**.
2. By definition, a rational number can be written as a fraction of coprime integers (integers sharing no common factors greater than 1):
$$\sqrt{2} = \frac{a}{b} \quad (\text{where } b \neq 0 \text{ and } \gcd(a,b) = 1)$$
3. Square both sides of the equation to eliminate the radical:
$$2 = \frac{a^2}{b^2} \implies a^2 = 2b^2 \quad \text{--- (Equation 1)}$$
4. Analyze divisibility: Equation 1 shows that $a^2$ is an even number, which logically means that the integer $a$ itself must also be an **even number**.
5. Express $a$ as an even integer substitution: Let $a = 2k$ for some integer $k$. Substitute this back into Equation 1:
$$(2k)^2 = 2b^2 \implies 4k^2 = 2b^2 \implies b^2 = 2k^2$$
6. Analyze divisibility again: This shows that $b^2$ is an even number, which means that the integer $b$ must also be an **even number**.
7. Evaluate the contradiction: We have deduced that both $a$ and $b$ are even numbers, meaning they both share a common factor of **2**. This directly contradicts our opening core definition that $a$ and $b$ are coprime ($\gcd(a,b)=1$).
8. Conclusion: Because our assumption leads to an impossible contradiction, the assumption must be false. Therefore, $\sqrt{2}$ is successfully proven to be an **irrational number**.

---

### Terminal Exercises & Self-Check Questions

1. **Negation Phrasing Workout:** Write out the negation of the statement: $p$: *"All prime numbers are odd integers."*
   * *Answer Hint:* Do not simply write "All prime numbers are not odd." The negation of "All" is "There exists at least one." The correct negation is: $\sim p$: *"There exists a prime number which is not an odd integer."* (This negation is true because the number 2 is a prime number that is even).

2. **Connective Truth Verification:** Let $p$: $3 + 4 = 7$ and $q$: $5 \times 4 = 25$. Evaluate the truth values of the compound expressions (a) "$p$ and $q$" and (b) "$p$ or $q$".
   * *Step-by-Step Solution:* 1. Determine individual truth states: $p$ is True ($\text{T}$) and $q$ is False ($\text{F}$).
     2. For (a) "$p \wedge q$": An "And" statement requires all parts to be true. Since $q$ is false, the compound statement is **False ($\text{F}$)**.
     3. For (b) "$p \vee q$": An "Or" statement requires at least one part to be true. Since $p$ is true, the compound statement is **True ($\text{T}$)**.

3. **Biconditional Phrase Interpretation:** What is the structural meaning of the logical connective phrase **"If and only if"** (abbreviated as "iff", denoted by $\iff$)?
   * *Answer Hint:* A biconditional statement $p \iff q$ means that both directional conditional implications are simultaneously true: "If $p$ occurs, then $q$ follows" ($p \implies q$) AND "If $q$ occurs, then $p$ follows" ($q \implies p$).