# Module III — Algebra I

# NIOS Senior Secondary Mathematics (311)

## Chapter 11: Permutations and Combinations

### Introduction & Key Objectives
In everyday life, we regularly encounter problems that involve counting the total number of ways a task can be performed, items can be arranged, or groups can be selected. For instance, finding the total number of possible pin codes, phone numbers, or picking a committee out of a group of candidates. Rather than counting manually, Permutations and Combinations provide algebraic tools to compute huge arrangements and selection groups systematically.

After studying this chapter, you will be able to:
* Apply the **Fundamental Principle of Counting** (Multiplication and Addition rules).
* Understand the notation, definition, and expansion of **Factorials ($n!$)**.
* Define and compute **Permutations ($^nP_r$)** as arrangements where order matters.
* Define and compute **Combinations ($^nC_r$)** as selections where order does not matter.
* Understand and apply the core mathematical identities relating $^nP_r$ and $^nC_r$.

---

### Core Concepts & Formulas

#### 1. Fundamental Principle of Counting (FPC)
* **Multiplication Principle:** If an event can occur in $m$ different ways, and following this, a second event can occur in $n$ different ways, then the total number of ways both events can occur in succession is:
> $$\text{Total Ways} = m \times n$$
* **Addition Principle:** If an event can occur in $m$ ways and a second independent event can occur in $n$ ways, and both cannot happen simultaneously, then the number of ways either event can occur is:
> $$\text{Total Ways} = m + n$$

#### 2. Factorial Notation ($n!$)
The product of the first $n$ consecutive natural numbers is called $n$ factorial:
> $$n! = n \times (n - 1) \times (n - 2) \times \dots \times 3 \times 2 \times 1$$

* *Important Defined Values:* * $0! = 1$
  * $1! = 1$
* *Recursive Property:* $n! = n \times (n - 1)!$

#### 3. Permutations ($^nP_r$)
> **Permutation:** An arrangement of a selection of objects in a **definite, specific order**. Order is critically important.

The number of unique permutations of $n$ distinct objects taken $r$ at a time ($0 \le r \le n$) is denoted by $^nP_r$:
> $$^nP_r = \frac{n!}{(n - r)!}$$

* **Permutations with Repetition:** The number of permutations of $n$ objects, where $p$ objects are of one identical kind, $q$ are of another identical kind, and $r$ are of a third kind, is given by:
> $$\text{Total Arrangements} = \frac{n!}{p! \cdot q! \cdot r!}$$

#### 4. Combinations ($^nC_r$)
> **Combination:** A selection or collection of objects where the **order of arrangement does not matter**. 

The number of unique combinations of $n$ distinct objects taken $r$ at a time ($0 \le r \le n$) is denoted by $^nC_r$:
> $$^nC_r = \frac{n!}{r!(n - r)!}$$

#### 5. Core Algebraic Operational Laws & Identities
> * **Relation between Permutation and Combination:**
>   $$^nP_r = r! \times ^nC_r$$
> * **Complementary Selection Identity:**
>   $$^nC_r = ^nC_{n-r}$$
> * **Pascal's Formula / Identity:**
>   $$^nC_r + ^nC_{r-1} = ^{n+1}C_r$$

---

### Step-by-Step Examples

**Example 1:** How many 3-digit numbers can be formed from the digits 1, 2, 3, 4, and 5 assuming that (i) repetition of digits is allowed, and (ii) repetition of digits is not allowed?  
**Solution:**
* **(i) Repetition allowed:**
  1. There are 3 positions to fill: Hundreds, Tens, and Units.
  2. The hundreds place can be filled by any of the 5 digits (5 ways).
  3. Since repetition is allowed, the tens place can also be filled in 5 ways, and the units place in 5 ways.
  4. By Multiplication Principle: $\text{Total} = 5 \times 5 \times 5 = 125$ numbers.
* **(ii) Repetition NOT allowed:**
  1. The hundreds place can be filled in 5 ways.
  2. The tens place can then be filled by any of the remaining 4 digits (4 ways).
  3. The units place can be filled by any of the remaining 3 digits (3 ways).
  4. By Multiplication Principle: $\text{Total} = 5 \times 4 \times 3 = 60$ numbers. (Alternatively, $^5P_3 = \frac{5!}{(5-3)!} = \frac{120}{2} = 60$).

**Example 2:** Find the total number of unique arrangements that can be made using all the letters of the word **MATHEMATICS**.  
**Solution:**
1. Count the total number of letters in the word: $n = 11$.
2. Identify repeating identical elements:
   * **M** appears 2 times.
   * **A** appears 2 times.
   * **T** appears 2 times.
   * Other letters (H, E, I, C, S) appear exactly 1 time.
3. Apply the Permutations with Repetition formula:
$$\text{Total Arrangements} = \frac{11!}{2! \cdot 2! \cdot 2!} = \frac{39,916,800}{2 \times 2 \times 2} = \frac{39,916,800}{8} = 4,989,600$$

**Example 3:** A committee of 3 members is to be selected from a group of 5 men and 4 women. In how many ways can this committee be formed if it must contain exactly 2 men and 1 woman?  
**Solution:**
1. Break down the task into independent selection stages: Selecting men and selecting women.
2. Select 2 men out of 5 available distinct men:
$$\text{Ways} = ^5C_2 = \frac{5!}{2!(5-2)!} = \frac{5 \times 4}{2 \times 1} = 10$$
3. Select 1 woman out of 4 available distinct women:
$$\text{Ways} = ^4C_1 = 4$$
4. Since both tasks must be completed to build the final committee, apply the Multiplication Principle:
$$\text{Total Ways} = ^5C_2 \times ^4C_1 = 10 \times 4 = 40 \text{ ways}$$

---

### Terminal Exercises & Self-Check Questions

1. **Evaluation Workout:** If $^{12}P_r = 1320$, find the value of $r$.
   * *Answer Hint:* Expand the permutation definition: $\frac{12!}{(12-r)!} = 1320$. Note that $12 \times 11 \times 10 = 1320$. This means 3 consecutive decreasing factors are expanded, implying $r = 3$.

2. **Combination Equation Workout:** If $^nC_8 = ^nC_2$, find the value of $^nC_2$.
   * *Step-by-Step Solution:* 1. Apply the complementary identity $^nC_x = ^nC_y \implies x = y \text{ or } x + y = n$.
     2. Here, $8 \neq 2$, so we use $n = 8 + 2 = 10$.
     3. Now calculate $^{10}C_2$:
        $$^{10}C_2 = \frac{10!}{2!(10-2)!} = \frac{10 \times 9}{2 \times 1} = 45$$

3. **Condition Optimization Problem:** In how many ways can 5 persons be seated around a circular table?
   * *Answer Hint:* This is a circular permutation problem. For circular tracking arrangements, one position is held fixed to avoid rotational copies. The formula is $(n - 1)!$.
     $$\text{Total circular paths} = (5 - 1)! = 4! = 4 \times 3 \times 2 \times 1 = 24 \text{ ways}$$
