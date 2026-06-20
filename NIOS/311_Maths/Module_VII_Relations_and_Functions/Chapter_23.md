# NIOS Senior Secondary Mathematics (311)

## Module VII: Relations and Functions
### Chapter 23: Relations and Functions-II

### Introduction & Key Objectives
In Module I (Chapter 2), we established the foundational language of coordinate ordered pairs, standard mappings, and the fundamental differences between basic relations and single-valued functions. In this chapter, we elevate these concepts to a more rigorous, algebraic level. We will explore how properties like symmetry, transitivity, and bijectivity allow us to classify complex abstract systems and pave the way for defining invertible functions—concepts that are highly tested in public examinations.

After studying this chapter, you will be able to:
* Classify relations into **Reflexive**, **Symmetric**, and **Transitive** types.
* Define and verify an **Equivalence Relation**.
* Test functions for structural behaviors: **One-to-One (Injective)** and **Onto (Surjective)** mappings.
* Define a **Bijective Function** and determine the mathematical criteria for a function to be **Invertible**.
* Compute the **Composition of Functions** ($g \circ f$) and find the **Inverse of a Function** ($f^{-1}$).

---

### Core Concepts & Formulas

#### 1. Advanced Types of Relations
Let $R$ be a relation defined on a non-empty set $A$ (meaning $R \subseteq A \times A$).

> **Reflexive Relation:** Every individual element must map to itself.
> $$(a, a) \in R \quad \text{for all } a \in A$$

> **Symmetric Relation:** If an element maps to another, the reverse mapping must also exist.
> $$(a, b) \in R \implies (b, a) \in R \quad \text{for all } a, b \in A$$

> **Transitive Relation:** If $a$ relates to $b$ and $b$ relates to $c$, then $a$ must relate directly to $c$.
> $$(a, b) \in R \text{ and } (b, c) \in R \implies (a, c) \in R \quad \text{for all } a, b, c \in A$$

#### 2. Equivalence Relation
> **Equivalence Relation:** A relation $R$ defined on a set $A$ is called an equivalence relation if and only if it is simultaneously **Reflexive**, **Symmetric**, and **Transitive**.

---

#### 3. Advanced Structural Classification of Functions
Let $f : A \rightarrow B$ be a function mapping from domain $A$ to co-domain $B$.

> **One-to-One Function (Injective Mapping):**
> Distinct elements in the domain must map to completely distinct images in the co-domain. No two inputs can share an output.
> $$\text{Algebraic Check:} \quad f(x_1) = f(x_2) \implies x_1 = x_2$$

> **Onto Function (Surjective Mapping):**
> Every element in the co-domain $B$ must have at least one pre-image in the domain $A$.
> $$\text{Condition Check:} \quad \text{Range of } f = \text{Co-domain } B$$



> **Bijective Function:**
> A function that is **both One-to-One (Injective) and Onto (Surjective)**.

---

#### 4. Composition of Functions
Let $f : A \rightarrow B$ and $g : B \rightarrow C$ be two conforming functions. The composition of $f$ and $g$, denoted by $g \circ f$, is a direct function mapping from set $A$ to set $C$:
> $$(g \circ f)(x) = g(f(x)) \quad \text{for all } x \in A$$

#### 5. Inverse of a Function ($f^{-1}$)
> **Invertibility Criterion:** A function $f : A \rightarrow B$ is invertible if and only if it is a **Bijective Function** (both 1-1 and onto).

If $f$ is bijective, its unique inverse function $f^{-1} : B \rightarrow A$ satisfies the condition:
$$f(x) = y \iff f^{-1}(y) = x$$

---

### Step-by-Step Examples

**Example 1:** Let $T$ be the set of all triangles in a plane. A relation $R$ is defined on $T$ as: $R = \{(T_1, T_2) : T_1 \text{ is congruent to } T_2\}$. Prove that $R$ is an equivalence relation.  
**Solution:**
1. **Reflexivity:** Every triangle $T_1$ is inherently congruent to itself ($T_1 \cong T_1$). Thus, $(T_1, T_1) \in R$ for all $T_1 \in T$. The relation is **reflexive**.
2. **Symmetry:** If $(T_1, T_2) \in R$, then triangle $T_1$ is congruent to $T_2$. This logically means triangle $T_2$ is congruent to $T_1$ ($T_2 \cong T_1$), so $(T_2, T_1) \in R$. The relation is **symmetric**.
3. **Transitivity:** If $(T_1, T_2) \in R$ and $(T_2, T_3) \in R$, then $T_1 \cong T_2$ and $T_2 \cong T_3$. By geometric extension, $T_1 \cong T_3$, which means $(T_1, T_3) \in R$. The relation is **transitive**.
4. **Conclusion:** Since $R$ satisfies all three criteria, it is successfully proven to be an **equivalence relation**.

**Example 2:** Check whether the real-valued function $f : \mathbb{R} \rightarrow \mathbb{R}$ defined by $f(x) = 3x + 4$ is a bijective function. If so, find its inverse formula.  
**Solution:**
1. **Test for Injective (One-to-One):** Set $f(x_1) = f(x_2)$:
$$3x_1 + 4 = 3x_2 + 4$$
$$3x_1 = 3x_2 \implies x_1 = x_2$$
Since $f(x_1) = f(x_2)$ strictly isolates $x_1 = x_2$, the function is **One-to-One**.
2. **Test for Surjective (Onto):** Let an arbitrary element in the co-domain be $y$. Set $y = f(x)$ and solve explicitly for $x$:
$$y = 3x + 4 \implies 3x = y - 4 \implies x = \frac{y - 4}{3}$$
For every real number $y \in \mathbb{R}$ (co-domain), there exists a corresponding real pre-image $x = \frac{y-4}{3} \in \mathbb{R}$ (domain). Thus, the range equals the co-domain, and the function is **Onto**.
3. **Conclusion on Bijectivity:** Since $f$ is both 1-1 and onto, it is **bijective** and therefore **invertible**.
4. **Find the Inverse Function ($f^{-1}$):** Replace $x$ with $f^{-1}(y)$ in our pre-image equation:
$$f^{-1}(y) = \frac{y - 4}{3} \implies f^{-1}(x) = \frac{x - 4}{3}$$

**Example 3:** If $f(x) = x^2$ and $g(x) = 2x + 1$ are two real-valued functions, find the composition functions (i) $(g \circ f)(x)$ and (ii) $(f \circ g)(x)$.  
**Solution:**
* **(i) Calculate $(g \circ f)(x)$:**
$$(g \circ f)(x) = g(f(x)) = g(x^2)$$
Substitute $x^2$ into the variable position of $g(x)$:
$$g(x^2) = 2(x^2) + 1 = 2x^2 + 1$$
* **(ii) Calculate $(f \circ g)(x)$:**
$$(f \circ g)(x) = f(g(x)) = f(2x + 1)$$
Substitute $(2x + 1)$ into the variable position of $f(x)$:
$$f(2x + 1) = (2x + 1)^2 = 4x^2 + 4x + 1$$
*(Note how this confirms that function composition is non-commutative: $g \circ f \neq f \circ g$).*

---

### Terminal Exercises & Self-Check Questions

1. **Relation Property Analysis:** Let $A = \{1, 2, 3\}$. A relation is defined as $R = \{(1,1), (2,2), (3,3), (1,2), (2,1)\}$. Is this an equivalence relation?
   * *Answer Hint:* Yes. It contains all diagonal pairs, so it is reflexive. For the pair $(1,2)$, its flip $(2,1)$ is present, making it symmetric. Testing transitivity: $(1,2)$ and $(2,1) \implies (1,1)$, which is in the set. Thus, it is an equivalence relation.

2. **Structural Mapping Workout:** Show that the function $f : \mathbb{R} \rightarrow \mathbb{R}$ defined by $f(x) = x^2$ is neither injective nor surjective.
   * *Step-by-Step Solution:* 1. Test Injective: Notice that $f(-2) = (-2)^2 = 4$ and $f(2) = (2)^2 = 4$. Two distinct inputs yield the same output image, so it is **not one-to-one**.
     2. Test Surjective: The square of any real number is always non-negative ($x^2 \ge 0$). This means negative real numbers in the co-domain (e.g., $-5$) have no real pre-images. Range $\neq$ Co-domain, so it is **not onto**.

3. **Composite Identity Problem:** If $f(x) = \sin x$ and $g(x) = x^2$, write down the explicit expression for $(f \circ g)(x)$.
   * *Answer Hint:* Apply definitions: $(f \circ g)(x) = f(g(x)) = f(x^2) = \sin(x^2)$.