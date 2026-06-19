# NIOS Senior Secondary Mathematics (311)

## Chapter 2: Relations and Functions-I

### Introduction & Key Objectives
In everyday life, we encounter relationships between pairs of objects or individuals, such as "is the father of," "is less than," or "is parallel to." In mathematics, these ideas are formalized using the concepts of relations and functions. This chapter serves as a building block for Calculus and advanced mathematical analysis.

After studying this chapter, you will be able to:
* Define the **Cartesian product** of two finite sets.
* Understand and define a **Relation**, its **Domain**, and its **Range**.
* Identify a **Function** as a special type of relation.
* Determine the domain, co-domain, and range of a function.
* Classify fundamental functions like identity, constant, polynomial, rational, and modulus functions.

---

### Core Concepts & Formulas

#### 1. Ordered Pairs
An **ordered pair** consists of two objects or elements in a fixed, specified order. It is written as $(a, b)$, where $a$ is the first element and $b$ is the second element.
> **Equality Rule for Ordered Pairs:**
> $$(a, b) = (c, d) \iff a = c \text{ and } b = d$$

#### 2. Cartesian Product of Two Sets
> **Cartesian Product ($A \times B$):** Let $A$ and $B$ be two non-empty sets. The Cartesian product $A \times B$ is the set of all ordered pairs $(a,b)$ such that $a \in A$ and $b \in B$.
> $$A \times B = \{(a, b) : a \in A \text{ and } b \in B\}$$

* If $n(A) = p$ and $n(B) = q$, then the total number of elements in the Cartesian product is given by:
> $$n(A \times B) = p \times q$$

#### 3. Relations
> **Relation ($R$):** A relation $R$ from a non-empty set $A$ to a non-empty set $B$ is a subset of the Cartesian product $A \times B$.
> $$R \subseteq A \times B$$

* **Domain of $R$:** The set of all first elements of the ordered pairs belonging to $R$.
$$\text{Domain} = \{a \in A : (a, b) \in R\}$$
* **Range of $R$:** The set of all second elements of the ordered pairs belonging to $R$.
$$\text{Range} = \{b \in B : (a, b) \in R\}$$
* **Co-domain:** The entire set $B$ is called the co-domain of the relation $R$. Note that $\text{Range} \subseteq \text{Co-domain}$.
* **Total Number of Relations:** If $n(A) = p$ and $n(B) = q$, then $n(A \times B) = pq$. The total number of subsets of $A \times B$ is $2^{pq}$. Therefore:
> $$\text{Total number of possible relations from } A \text{ to } B = 2^{pq}$$

#### 4. Functions
> **Function ($f$):** A function $f$ from a set $A$ to a set $B$ is a special relation in which **every element** of set $A$ has **one and only one** image in set $B$.



We write it as $f : A \rightarrow B$. If $(a, b) \in f$, we say that $b$ is the **image** of $a$ under $f$, and $a$ is the **pre-image** of $b$.
* **Domain:** The set $A$.
* **Co-domain:** The set $B$.
* **Range:** The set of all images of elements of $A$. 
$$\text{Range} = \{f(x) : x \in A\}$$

#### 5. Some Standard Real Functions
* **Identity Function:** Defined by $f(x) = x$ for all $x \in \mathbb{R}$. Both Domain and Range are $\mathbb{R}$.
* **Constant Function:** Defined by $f(x) = c$ (where $c$ is a constant) for all $x \in \mathbb{R}$. Domain is $\mathbb{R}$, Range is $\{c\}$.
* **Modulus Function:** Defined by:
$$f(x) = |x| = \begin{cases} x, & \text{if } x \ge 0 \\ -x, & \text{if } x < 0 \end{cases}$$
Domain is $\mathbb{R}$, Range is $[0, \infty)$.

---

### Step-by-Step Examples

**Example 1:** Find $x$ and $y$ if $(2x + 3, y - 2) = (7, 4)$.  
**Solution:**
1. Equate the corresponding components of the ordered pairs:
$$2x + 3 = 7 \quad \text{and} \quad y - 2 = 4$$
2. Solve the first equation for $x$:
$$2x = 7 - 3 \implies 2x = 4 \implies x = 2$$
3. Solve the second equation for $y$:
$$y = 4 + 2 \implies y = 6$$
4. Conclusion: $x = 2, y = 6$.

**Example 2:** Let $A = \{1, 2, 3\}$ and $B = \{4, 5\}$. Find $A \times B$ and the total number of relations from $A$ to $B$.  
**Solution:**
1. List all elements of $A \times B$ by pairing every element of $A$ with every element of $B$:
$$A \times B = \{(1, 4), (1, 5), (2, 4), (2, 5), (3, 4), (3, 5)\}$$
2. Count the number of elements: $n(A) = 3$, $n(B) = 2$, so $n(A \times B) = 3 \times 2 = 6$.
3. Use the formula for the total number of relations:
$$\text{Total Relations} = 2^{n(A \times B)} = 2^6 = 64$$

**Example 3:** Examine whether the relation $R = \{(1, 2), (2, 3), (2, 4), (3, 5)\}$ is a function or not. Find its domain and range.  
**Solution:**
1. Check the first elements of the ordered pairs: the element `2` appears twice as a first entry, mapping to two different values: $(2, 3)$ and $(2, 4)$.
2. By definition, a function cannot map a single element of the domain to multiple images. Therefore, $R$ is **not a function**.
3. **Domain:** Extract all unique first elements: $\{1, 2, 3\}$.
4. **Range:** Extract all unique second elements: $\{2, 3, 4, 5\}$.

---

### Terminal Exercises & Self-Check Questions

1. **Cartesian Analysis:** If $P = \{a, b, c\}$ and $Q = \{d\}$, form the sets $P \times Q$ and $Q \times P$. Are they equal?
   * *Answer Hint:* $P \times Q = \{(a,d), (b,d), (c,d)\}$ and $Q \times P = \{(d,a), (d,b), (d,c)\}$. They are not equal because their ordered pairs are not identical.

2. **Domain Determination:** Find the domain of the real-valued function $f(x) = \frac{1}{\sqrt{x - 3}}$.
   * *Step-by-Step Solution:* 1. For the function to yield a real output, the expression under the square root must be positive, and since it is in the denominator, it cannot be zero.
     2. Set up the inequality: $x - 3 > 0$.
     3. Solve for $x$: $x > 3$.
     4. Domain = $(3, \infty)$.

3. **Function Mapping Verification:** Let $A = \{1, 2, 3, 4\}$ and $B = \{1, 4, 9, 16, 25\}$. A rule is defined as $f(x) = x^2$ for $x \in A$. Write $f$ as a set of ordered pairs, and find its range.
   * *Answer Hint:* $f = \{(1, 1), (2, 4), (3, 9), (4, 16)\}$. The range is the set of images: $\{1, 4, 9, 16\}$.