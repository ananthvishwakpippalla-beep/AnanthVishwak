# NIOS Senior Secondary Mathematics (311)

## Module V: Statistics and Probability
### Chapter 19: Probability

### Introduction & Key Objectives
Building directly upon the foundational axioms of sample spaces and events explored in Chapter 18, this chapter transitions from qualifying events to **quantifying** their actual likelihood. Probability theory allows us to map uncertainty onto a strict numerical scale between 0 and 1. This chapter establishes the classical and axiomatic definitions of probability, compound conditional boundaries, and independent testing frameworks highly emphasized in public examinations.

After studying this chapter, you will be able to:
* Define and calculate the **Classical (Axiomatic) Probability** of an event.
* Apply the **Addition Theorem of Probability** for mutually exclusive and non-exclusive events.
* Understand and compute **Conditional Probability**.
* State and apply the **Multiplication Theorem of Probability**.
* Identify **Independent Events** using algebraic product checks.
* Construct a discrete **Probability Distribution** for a random variable, computing its **Mean** ($\mu$) and **Variance** ($\sigma^2$).

---

### Core Concepts & Formulas

#### 1. Classical Definition of Probability
If a sample space $S$ contains a finite number of equally likely outcomes, the probability of an event $E$ occurring is the ratio of favorable outcomes to total possible outcomes:
> $$P(E) = \frac{n(E)}{n(S)} = \frac{\text{Number of outcomes favorable to } E}{\text{Total number of possible outcomes}}$$

* **Probability Axiom Bounds:** For any event $E$:
  $$0 \le P(E) \le 1$$
* **Complementary Probability Rule:** The probability of an event happening plus it *not* happening always equals 1:
  $$P(E) + P(E') = 1 \implies P(E') = 1 - P(E)$$

#### 2. The Addition Theorem of Probability
> **General Rule (For any two events $A$ and $B$):**
> $$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$

* **For Mutually Exclusive Events:** Since they cannot happen concurrently, $A \cap B = \phi \implies P(A \cap B) = 0$:
> $$P(A \cup B) = P(A) + P(B)$$

#### 3. Conditional Probability
Conditional probability tracks the modified likelihood of an event $A$ occurring given the absolute certainty that another event $B$ has already occurred.
> **Conditional Formula:**
> $$P(A | B) = \frac{P(A \cap B)}{P(B)} \quad (\text{where } P(B) > 0)$$



#### 4. The Multiplication Theorem & Independent Events
Rearranging the conditional probability formula isolates the intersection probability:
> $$P(A \cap B) = P(B) \cdot P(A | B) = P(A) \cdot P(B | A)$$

> **Independent Events Condition:**
> Two events $A$ and $B$ are structurally independent if the occurrence of one does not alter the likelihood of the other ($P(A|B) = P(A)$). Mathematically, they are independent if and only if:
> $$P(A \cap B) = P(A) \cdot P(B)$$

---

#### 5. Probability Distributions of a Random Variable
A **Random Variable** $X$ is a real-valued function whose domain is the sample space of a random experiment. A probability distribution maps each value $x_i$ to its corresponding probability $p_i$.

* **Validity Constraint:** A distribution is mathematically valid if and only if all individual $p_i \ge 0$ and their total sum equals 1:
$$\sum p_i = 1$$

> **Mean (Expected Value $\mu$ or $E(X)$):**
> $$\mu = \sum x_i p_i$$

> **Variance ($\sigma^2$):**
> $$\sigma^2 = \sum x_i^2 p_i - (\mu)^2$$

---

### Step-by-Step Examples

**Example 1:** A single card is drawn from a well-shuffled standard pack of 52 playing cards. Find the probability that the card drawn is either a King or a Heart.  
**Solution:**
1. Determine the baseline sample space size: $n(S) = 52$.
2. Define individual events and count their elements:
   * Let $A$ be drawing a King $\implies n(A) = 4 \implies P(A) = \frac{4}{52}$
   * Let $B$ be drawing a Heart $\implies n(B) = 13 \implies P(B) = \frac{13}{52}$
3. Identify overlapping intersections: One card is simultaneously a King and a Heart (the King of Hearts):
   * $A \cap B = 1 \implies P(A \cap B) = \frac{1}{52}$
4. Apply the General Addition Theorem:
$$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$
$$P(A \cup B) = \frac{4}{52} + \frac{13}{52} - \frac{1}{52} = \frac{16}{52} = \frac{4}{13}$$

**Example 2:** A box contains 5 red and 4 black marbles. Two marbles are drawn one after another without replacement. Find the probability that both marbles drawn are red.  
**Solution:**
1. Let $R_1$ be the event that the first marble drawn is red, and $R_2$ be the event that the second marble is red.
2. Find $P(R_1)$ from the baseline counts (5 red out of 9 total):
$$P(R_1) = \frac{5}{9}$$
3. Since the marble is **not replaced**, the box now contains 4 red marbles and 4 black marbles (8 total). Find the conditional probability $P(R_2 | R_1)$:
$$P(R_2 | R_1) = \frac{4}{8} = \frac{1}{2}$$
4. Apply the Multiplication Theorem to find the intersection probability:
$$P(R_1 \cap R_2) = P(R_1) \cdot P(R_2 | R_1) = \frac{5}{9} \times \frac{1}{2} = \frac{5}{18}$$

**Example 3:** Two unbiased coins are tossed simultaneously. Let the random variable $X$ denote the number of Heads obtained. Find the complete probability distribution, its mean, and its variance.  
**Solution:**
1. Set up the sample space: $S = \{HH, HT, TH, TT\} \implies n(S) = 4$.
2. Identify the possible values of the random variable $X$: 0, 1, or 2 heads.
3. Calculate the individual probabilities for each value of $X$:
   * $P(X = 0) = P(\{TT\}) = \frac{1}{4}$
   * $P(X = 1) = P(\{HT, TH\}) = \frac{2}{4} = \frac{1}{2}$
   * $P(X = 2) = P(\{HH\}) = \frac{1}{4}$
4. Arrange the probability distribution table and compute the Mean ($\mu = \sum x_i p_i$):
$$\mu = (0 \times \frac{1}{4}) + (1 \times \frac{2}{4}) + (2 \times \frac{1}{4}) = 0 + \frac{2}{4} + \frac{2}{4} = \frac{4}{4} = 1$$
5. Compute $\sum x_i^2 p_i$ to find the variance:
$$\sum x_i^2 p_i = (0^2 \times \frac{1}{4}) + (1^2 \times \frac{2}{4}) + (2^2 \times \frac{1}{4}) = 0 + \frac{2}{4} + \frac{4}{4} = \frac{6}{4} = 1.5$$
6. Calculate Variance using $\sigma^2 = \sum x_i^2 p_i - (\mu)^2$:
$$\sigma^2 = 1.5 - (1)^2 = 1.5 - 1 = 0.5 \quad (\text{or } \frac{1}{2})$$

---

### Terminal Exercises & Self-Check Questions

1. **Independence Verification Workout:** If $P(A) = 0.3$ and $P(B) = 0.6$, and $A$ and $B$ are explicitly given as independent events, calculate $P(A \cap B)$ and $P(A \cup B)$.
   * *Answer Hint:* For independent events, $P(A \cap B) = P(A) \cdot P(B) = 0.3 \times 0.6 = 0.18$. 
     Then use addition: $P(A \cup B) = 0.3 + 0.6 - 0.18 = 0.9 - 0.18 = 0.72$.

2. **Conditional Probability Problem:** Given that $P(X) = 0.4$, $P(Y) = 0.8$, and $P(Y | X) = 0.6$, calculate the exact value of $P(X | Y)$.
   * *Step-by-Step Solution:* 1. Rearrange the conditional formula to find the intersection value: $P(X \cap Y) = P(X) \cdot P(Y | X) = 0.4 \times 0.6 = 0.24$.
     2. Apply the formula to find the missing conditional direction:
        $$P(X | Y) = \frac{P(X \cap Y)}{P(Y)} = \frac{0.24}{0.8} = 0.3$$

3. **Distribution Validation Exercise:** Examine whether the following distribution mapping is mathematically valid: $X = \{0, 1, 2\}$ mapped to $P(X) = \{0.2, 0.5, 0.4\}$.
   * *Answer Hint:* Sum up the given probabilities: $\sum p_i = 0.2 + 0.5 + 0.4 = 1.1$. Since the total sum exceeds 1, it violates the fundamental axiom of probability. Therefore, it **is not valid**.