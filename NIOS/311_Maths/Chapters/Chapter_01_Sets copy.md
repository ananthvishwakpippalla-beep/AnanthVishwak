# NIOS Senior Secondary Mathematics (311)

## Chapter 1: Sets

### Introduction & Key Objectives
The concept of a set was introduced by the German mathematician George Cantor (1845–1918), who is known as the father of set theory. In modern mathematics, set theory forms the foundational base for defining concepts such as relations, functions, and probability. 

After studying this chapter, you will be able to:
* Define a set and represent it in different formal mathematical methods.
* Classify different types of sets (finite, infinite, empty, singleton, equal, equivalent, and disjoint sets).
* Define and apply concepts of **subsets**, **power sets**, and **universal sets**.
* Perform standard set operations including **union**, **intersection**, **difference**, and **complementation**.
* Use **Venn Diagrams** to solve problems and represent operational combinations visually.

---

### Core Concepts & Formulas

#### 1. Fundamental Definition
> **Set:** A set is a collection of well-defined objects. For a collection to be a set, the property defining the inclusion of its objects must be certain and universally objective (independent of changing individual perceptions). 

* **Elements:** The individual objects belonging to a set are called its elements. Sets are typically denoted by capital letters ($A, B, C$) and elements by small letters ($a, b, c$).
* **Belongs to ($\in$):** If $x$ is an element of set $A$, we write $x \in A$. If it is not an element, we write $x \notin A$.

#### 2. Standard Number System Notations
The following standard notations are strictly preserved throughout the curriculum:
* $\mathbb{N}$: The set of all natural numbers
* $\mathbb{W}$: The set of all whole numbers
* $\mathbb{Z}$: The set of all integers
* $\mathbb{Z}^+$ / $\mathbb{Z}^-$: The set of positive / negative integers
* $\mathbb{Q}$: The set of all rational numbers
* $\mathbb{I}$: The set of all irrational numbers
* $\mathbb{R}$: The set of all real numbers

#### 3. Methods of Representation
* **Roster Method (Tabular Form):** All elements are explicitly listed in a comma-separated format enclosed inside curly brackets $\{\}$. Elements cannot be duplicated or repeated.
* **Set-Builder Form:** Elements are not explicitly listed; instead, they are expressed via a common defining variable property. The symbol `:` is read as *"such that"*.

#### 4. Classification of Sets
* **Finite Set:** A set where the total number of elements can be comprehensively counted up to a final element.
* **Infinite Set:** A set where counting up to the last element is impossible.
* **Empty (Null / Void) Set ($\phi$ or $\{\}$):** A set containing zero elements. Note: $\{\phi\}$ is **not** an empty set; it is a singleton set containing the element $\phi$.
* **Singleton Set:** A set containing exactly one element.
* **Equal Sets ($A = B$):** Two sets containing exactly the same elements.
* **Equivalent Sets ($A \approx B$):** Two sets containing the same **number** of elements, irrespective of the identity of the elements.
* **Disjoint Sets:** Two sets that share zero common elements.

#### 5. Subsets and Power Sets
> **Subset ($\subseteq$):** Set $A$ is a subset of set $B$ if every element of $A$ is also an element of $B$.
> $$A \subseteq B \iff (x \in A \implies x \in B)$$

* **Null Set Rule:** The empty set $\phi$ is a subset of every set.
* **Proper Subset ($\subset$):** If $A \subseteq B$ and $A \neq B$, then $A$ is a proper subset of $B$, and $B$ is the super set ($B \supset A$).
* **Counting Subsets Rule:**
> If a finite set has $p$ elements ($n(A) = p$), then:
> * Total number of subsets $= 2^p$
> * Total number of proper subsets $= 2^p - 1$

* **Power Set ($P(A)$):** The set containing all the subsets of a given set $A$.

#### 6. Intervals as Subsets of Real Numbers
For real numbers $a, b \in \mathbb{R}$ where $a < b$:
* **Open Interval:** $(a,b) = \{x \in \mathbb{R} : a < x < b\}$
* **Closed Interval:** $[a,b] = \{x \in \mathbb{R} : a \le x \le b\}$
* **Semi-Open / Semi-Closed:** $(a,b] = \{x \in \mathbb{R} : a < x \le b\}$ and $[a,b) = \{x \in \mathbb{R} : a \le x < b\}$.

#### 7. Operations on Sets
* **Union ($A \cup B$):** The set of elements belonging to either $A$, $B$, or both.
* **Intersection ($A \cap B$):** The set of elements belonging simultaneously to both $A$ and $B$.
* **Difference ($A - B$):** The set of elements belonging to $A$ but strictly **not** belonging to $B$.
* **Complement ($A'$ or $A^c$):** Relative to a universal set $U$, the complement of $A$ contains all elements of $U$ that are not in $A$.
$$A' = U - A = \{x : x \in U \text{ and } x \notin A\}$$

#### 8. Core Algebraic Operational Laws
> **De Morgan's Laws:**
> 1. $(A \cup B)' = A' \cap B'$
> 2. $(A \cap B)' = A' \cup B'$

> **Cardinal Number Rules:**
> * $n(A \cup B) = n(A) + n(B) - n(A \cap B)$
> * If $A$ and $B$ are disjoint ($A \cap B = \phi$): $n(A \cup B) = n(A) + n(B)$

---

### Step-by-Step Examples

**Example 1:** Convert the set $B = \{3, 6, 9, 12\}$ from Roster form into Set-builder form.  
**Solution:**
1. Observe the algebraic pattern of the listed elements: $3 = 3(1)$, $6 = 3(2)$, $9 = 3(3)$, $12 = 3(4)$.
2. The elements are multiples of 3 up to the 4th multiple.
3. Formulate the conditional statement: 
$$B = \{x : x = 3n \text{ and } n \in \mathbb{N}, n \le 4\}$$

**Example 2:** Find the solution set of the quadratic equation $x^2 - 5x + 6 = 0$ and write it in Roster form.  
**Solution:**
1. Factorize the given quadratic expression:
$$x^2 - 3x - 2x + 6 = 0$$
$$x(x - 3) - 2(x - 3) = 0$$
$$(x - 3)(x - 2) = 0$$
2. Solving for $x$ yields $x = 3$ or $x = 2$.
3. List the distinct elements inside curly brackets:
$$D = \{2, 3\}$$

**Example 3:** If $A = \{1, 2, 3, 4, 5\}$ and $B = \{2, 4, 6\}$, calculate (i) $A - B$ and (ii) $B - A$.  
**Solution:**
* **(i) $A - B$:** Identify elements that are strictly in $A$ but not in $B$.
$$A - B = \{1, 2, 3, 4, 5\} - \{2, 4, 6\} = \{1, 3, 5\}$$
* **(ii) $B - A$:** Identify elements that are strictly in $B$ but not in $A$.
$$B - A = \{2, 4, 6\} - \{1, 2, 3, 4, 5\} = \{6\}$$

---

### Terminal Exercises & Self-Check Questions

1. **Classification Analysis:** Which of the following collections are mathematically valid sets?
   * (a) The collection of fat students in a high school.
   * (b) The collection of prime factors exact divisors of 60.
   * *Answer Hint:* (a) is not a set as 'fatness' is not well-defined; (b) is a valid finite set: $\{2, 3, 5\}$.

2. **Subset Permutations Calculation:** If a set is given as $M = \{a, e, i, o, u\}$, determine the total possible number of subsets and proper subsets that can be derived from it.
   * *Answer Hint:* Here $n(M) = 5$ elements. Number of subsets $= 2^5 = 32$. Number of proper subsets $= 32 - 1 = 31$.

3. **Verification Problem:** Given a universal set $U = \{1, 2, 3, 4, 5, 6, 7, 8, 9, 10\}$ with subsets $A = \{2, 4, 6, 8\}$ and $B = \{1, 3, 5, 7\}$. Verify De Morgan's Law: $(A \cup B)' = A' \cap B'$.
   * *Step-by-Step Verification:*
     1. $A \cup B = \{1, 2, 3, 4, 5, 6, 7, 8\}$.
     2. $\text{LHS} = (A \cup B)' = U - (A \cup B) = \{9, 10\}$.
     3. Find individual complements: $A' = \{1, 3, 5, 7, 9, 10\}$ and $B' = \{2, 4, 6, 8, 9, 10\}$.
     4. $\text{RHS} = A' \cap B' = \{9, 10\}$.
     5. $\text{LHS} = \text{RHS}$. Hence verified.