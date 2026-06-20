# NIOS Senior Secondary Mathematics (311)

## Module V: Statistics and Probability
### Chapter 18: Random Experiments and Events

### Introduction & Key Objectives
In everyday life, we frequently use terms like "probably," "chance," or "uncertainty" when discussing events such as weather forecasts, match outcomes, or stock market fluctuations. In mathematics, probability theory provides a formal framework to quantify this uncertainty. This chapter introduces the absolute bedrock of probability: the precise terminology of sample spaces, random testing parameters, and the algebraic classification of events.

After studying this chapter, you will be able to:
* Distinguish between deterministic experiments and **Random Experiments**.
* Establish and write down the **Sample Space ($S$)** for various multi-stage random trials.
* Define an **Event** as a subset of a sample space.
* Classify different types of events (Sure, Impossible, Simple, Compound, and Complementary events).
* Identify and calculate relationships between **Mutually Exclusive** and **Exhaustive Events**.

---

### Core Concepts & Formulas

#### 1. Random Experiments
An experiment is called a **Random Experiment** if it satisfies two essential conditions:
1. It has more than one possible outcome.
2. It is impossible to predict the exact outcome in advance, even if the experiment is repeated under identical conditions.
* *Example:* Tossing a fair coin or rolling an unbiased six-sided die.

#### 2. Sample Space ($S$)
> **Sample Space:** The set of all possible outcomes of a random experiment is called the sample space, denoted by the capital letter $S$. Each individual element or outcome in this set is called a **Sample Point**.

* *Example (Tossing two coins simultaneously):*
$$S = \{HH, HT, TH, TT\} \quad \implies n(S) = 4$$

#### 3. Events
> An **Event** ($E$) is a specific collection of outcomes. Mathematically, any event is a subset of the baseline sample space $S$.
> $$E \subseteq S$$

* We say an event $E$ has **occurred** if the final outcome of the experiment belongs to the set $E$.

#### 4. Classification of Events
* **Impossible Event ($\phi$):** An event containing zero outcomes. It can never occur. (e.g., rolling a number greater than 6 on a standard die).
* **Sure (Certain) Event ($S$):** An event that contains all sample points of the sample space. It is guaranteed to happen.
* **Simple (Elementary) Event:** An event that contains exactly **one single sample point**.
* **Compound Event:** An event that contains **more than one sample point**.
* **Complementary Event ($E'$ or $E^c$):** For any event $E$, its complement represents the event "not $E$," containing all sample points in $S$ that do not belong to $E$.
$$E' = S - E$$



---

#### 5. Relationships Between Multiple Events
Let $A$ and $B$ be two distinct events within a sample space $S$:

> **Mutually Exclusive (Disjoint) Events:**
> Two events are mutually exclusive if they cannot occur at the same time. Their sets share zero common elements.
> $$A \cap B = \phi$$

> **Exhaustive Events:**
> A set of events is exhaustive if their union completely reconstructs the entire sample space. At least one of the events must occur during a trial.
> $$A \cup B = S$$

---

### Step-by-Step Examples

**Example 1:** A coin is tossed. If it shows a Head, a standard six-sided die is rolled. If it shows a Tail, the coin is tossed one more time. Write down the complete sample space $S$ for this multi-stage experiment.  
**Solution:**
1. Analyze the branch conditions from the initial coin toss:
   * **Branch 1 (Head):** Followed by a die roll ($1, 2, 3, 4, 5, 6$). This creates the sample points: $H1, H2, H3, H4, H5, H6$.
   * **Branch 2 (Tail):** Followed by another coin toss ($H, T$). This creates the sample points: $TH, TT$.
2. Combine all branches into a single set:
$$S = \{H1, H2, H3, H4, H5, H6, TH, TT\}$$
3. Count the total sample points: $n(S) = 8$.

**Example 2:** Consider the experiment of rolling a single fair die. Let event $A$ be "rolling an even number" and event $B$ be "rolling an odd number." Examine whether $A$ and $B$ are (i) Mutually Exclusive and (ii) Exhaustive.  
**Solution:**
1. Write down the baseline Sample Space: $S = \{1, 2, 3, 4, 5, 6\}$.
2. List the sample points for both events:
   * $A = \{2, 4, 6\}$
   * $B = \{1, 3, 5\}$
3. Test condition (i) Intersections:
$$A \cap B = \{2, 4, 6\} \cap \{1, 3, 5\} = \phi$$
Since their intersection is an empty set, they are **Mutually Exclusive**.
4. Test condition (ii) Unions:
$$A \cup B = \{2, 4, 6\} \cup \{1, 3, 5\} = \{1, 2, 3, 4, 5, 6\} = S$$
Since their union equals the complete sample space, they are **Exhaustive**.

---

### Terminal Exercises & Self-Check Questions

1. **Sample Space Formulation Workout:** Two dice (one red and one blue) are rolled simultaneously. Determine the total number of sample points in the sample space $S$.
   * *Answer Hint:* Each die has 6 possible outcomes. By the Fundamental Multiplication Principle of counting, $n(S) = 6 \times 6 = 36$ sample points.

2. **Event Extraction Workout:** Three coins are tossed simultaneously. Write out the explicit subset elements for the following events:
   * (a) Event $A$: Obtaining exactly two heads.
   * (b) Event $B$: Obtaining at least two heads.
   * *Step-by-Step Solution:* 1. The full sample space is $S = \{HHH, HHT, HTH, THH, HTT, THT, TTH, TTT\}$.
     2. For $A$ (exactly 2 heads), pick elements with two H entries: $A = \{HHT, HTH, THH\}$.
     3. For $B$ (at least 2 heads, meaning 2 or 3 heads), pick elements with two or three H entries: $B = \{HHH, HHT, HTH, THH\}$.

3. **Exclusivity Verification Problem:** A card is drawn from a standard deck of 52 cards. Let event $X$ be "drawing a red card" and event $Y$ be "drawing a spade card." Are $X$ and $Y$ mutually exclusive?
   * *Answer Hint:* No. All spades are black cards. Since no card can be simultaneously red and a spade, $X \cap Y = \phi$. Therefore, they **are mutually exclusive**. (Note: If $Y$ had been "drawing a king," they would not be exclusive, as the King of Hearts/Diamonds is both red and a king).