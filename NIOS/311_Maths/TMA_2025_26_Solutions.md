# NIOS Senior Secondary Mathematics (311)
## Tutor Marked Assignment (TMA) — Session 2025-26
**Max. Marks: 20**

---

## Question 1 (2 Marks)
**Answer any one of the following questions.**

### Option (A)
According to a survey of 100 students, the number of students studying the various languages were found to be as follows:
* English only = 18
* English but not Hindi = 23
* English and Punjabi = 08
* English = 26
* Punjabi = 48
* Punjabi and Hindi = 08
* No Language = 24

**Find:**
1. How many students were studying Hindi?
2. How many students were studying English and Hindi?

#### Step-by-Step Solution:
Let $E$, $H$, and $P$ denote the sets of students studying English, Hindi, and Punjabi respectively.

1. **Find $n(E \cap H)$ (English and Hindi):**
   * We are given that the total number of English students is $n(E) = 26$.
   * We are also given "English but not Hindi" = 23. Mathematically, this is $n(E - H) = n(E) - n(E \cap H) = 23$.
   * Substituting $n(E) = 26$:
     $$26 - n(E \cap H) = 23 \implies n(E \cap H) = 26 - 23 = 3$$
   * **Answer (ii):** The number of students studying English and Hindi is **3**.

2. **Analyze the sub-regions to find Hindi students:**
   * $n(E \text{ only}) = 18$
   * $n(E \cap P) = 8$
   * Total $n(E) = 26$. The elements of $E$ are composed of:
     $$n(E) = n(E \text{ only}) + n(E \cap H \text{ only}) + n(E \cap P \text{ only}) + n(E \cap H \cap P)$$
   * We know $n(E \cap H) = n(E \cap H \text{ only}) + n(E \cap H \cap P) = 3$.
   * Therefore:
     $$n(E) = n(E \text{ only}) + n(E \cap P \text{ only}) + n(E \cap H) = 26$$
     $$18 + n(E \cap P \text{ only}) + 3 = 26 \implies 21 + n(E \cap P \text{ only}) = 26 \implies n(E \cap P \text{ only}) = 5$$
   * Since $n(E \cap P) = n(E \cap P \text{ only}) + n(E \cap H \cap P) = 8$:
     $$5 + n(E \cap H \cap P) = 8 \implies n(E \cap H \cap P) = 3$$
   * Since $n(E \cap H) = 3$ and $n(E \cap H \cap P) = 3$, it means $n(E \cap H \text{ only}) = 0$.

3. **Use the universal set total to find $n(H)$:**
   * Total surveyed = 100. Those studying at least one language:
     $$n(E \cup H \cup P) = 100 - n(\text{No Language}) = 100 - 24 = 76$$
   * We know:
     $$n(E \cup H \cup P) = n(E \text{ only}) + n(P \text{ only}) + n(H \text{ only}) + n(E \cap P \text{ only}) + n(E \cap H \text{ only}) + n(P \cap H \text{ only}) + n(E \cap H \cap P)$$
   * Given $n(P) = 48$. We know:
     $$n(P) = n(P \text{ only}) + n(E \cap P \text{ only}) + n(P \cap H \text{ only}) + n(E \cap H \cap P) = 48$$
     $$n(P \text{ only}) + 5 + n(P \cap H \text{ only}) + 3 = 48 \implies n(P \text{ only}) + n(P \cap H \text{ only}) = 40$$
   * Let's regroup the formula for $n(E \cup H \cup P)$:
     $$n(E \cup H \cup P) = n(E \text{ only}) + n(E \cap H \text{ only}) + n(E \cap P \text{ only}) + n(H \text{ only}) + n(P \text{ only}) + n(P \cap H \text{ only}) + n(E \cap H \cap P)$$
     $$76 = 18 + 0 + 5 + n(H \text{ only}) + [n(P \text{ only}) + n(P \cap H \text{ only})] + 3$$
     $$76 = 18 + 0 + 5 + n(H \text{ only}) + 40 + 3$$
     $$76 = 66 + n(H \text{ only}) \implies n(H \text{ only}) = 76 - 66 = 10$$

4. **Calculate total $n(H)$:**
   * We know $n(P \cap H) = 8 \implies n(P \cap H \text{ only}) + n(E \cap H \cap P) = 8 \implies n(P \cap H \text{ only}) + 3 = 8 \implies n(P \cap H \text{ only}) = 5$.
   * Total students studying Hindi:
     $$n(H) = n(H \text{ only}) + n(E \cap H \text{ only}) + n(P \cap H \text{ only}) + n(E \cap H \cap P)$$
     $$n(H) = 10 + 0 + 5 + 3 = 18$$
   * **Answer (i):** The number of students studying Hindi is **18**.

---

### Option (B)
Check whether the function is even? Find its domain.
$$f(x)=\frac{x}{\sqrt{x^{2}-5x+4}}$$

#### Step-by-Step Solution:

1. **Parity Check (Even / Odd / Neither):**
   * Replace $x$ with $-x$:
     $$f(-x) = \frac{-x}{\sqrt{(-x)^{2}-5(-x)+4}} = \frac{-x}{\sqrt{x^{2}+5x+4}}$$
   * For a function to be even, $f(-x) = f(x)$. Here, $\frac{-x}{\sqrt{x^2+5x+4}} \neq \frac{x}{\sqrt{x^2-5x+4}}$.
   * For a function to be odd, $f(-x) = -f(x)$. Here, $\frac{-x}{\sqrt{x^2+5x+4}} \neq -\frac{x}{\sqrt{x^2-5x+4}}$.
   * **Conclusion:** The function is **neither even nor odd**.

2. **Domain Evaluation:**
   * For the expression to be real and defined, the term inside the square root in the denominator must be strictly greater than zero:
     $$x^{2} - 5x + 4 > 0$$
   * Factorize the quadratic inequality:
     $$(x - 4)(x - 1) > 0$$
   * By the sign-chart (wavy-curve) method, the product is positive when $x$ lies outside the roots 1 and 4:
     $$x \in (-\infty, 1) \cup (4, \infty)$$
   * **Domain:** **$(-\infty, 1) \cup (4, \infty)$**

---

## Question 2 (2 Marks)
**Answer any one of the following questions.**

### Option (A)
Ramesh tossed a coin three times. Find the probability of getting head and tail alternatively.
1. If the first toss is a Head.
2. If the first toss is a Tail.

#### Step-by-Step Solution:
The complete sample space for tossing a coin 3 times is:
$$S = \{HHH, HHT, HTH, HTT, THH, THT, TTH, TTT\} \quad \implies n(S) = 8$$

1. **Case (i): First toss is a Head.**
   * The reduced sample space where the first toss is Head ($H$) is:
     $$S_{H} = \{HHH, HHT, HTH, HTT\} \quad \implies n(S_{H}) = 4$$
   * Favorable outcomes for alternative faces starting with $H$: $\{HTH\}$. (Count = 1).
   * Probability $= \frac{1}{4}$ or **0.25**.

2. **Case (ii): First toss is a Tail.**
   * The reduced sample space where the first toss is Tail ($T$) is:
     $$S_{T} = \{THH, THT, TTH, TTT\} \quad \implies n(S_{T}) = 4$$
   * Favorable outcomes for alternative faces starting with $T$: $\{THT\}$. (Count = 1).
   * Probability $= \frac{1}{4}$ or **0.25**.

---

### Option (B)
Two numbers are chosen, one from each of the sets $\{1, 2, 3, 4, 5, 6, 7, 8, 9\}$ and $\{1, 2, 3, 4, 5, 6, 7, 8, 9\}$. Ram calculates the probability that their sum is 10, and Shyam calculates the probability that their sum is 8. What is the product of the probabilities calculated by Ram and Shyam?

#### Step-by-Step Solution:
Let the two sets be $A$ and $B$. Total possible pairs chosen $= 9 \times 9 = 81 \implies n(S) = 81$.

1. **Ram's Probability (Sum = 10):**
   * Favorable pairs $(a, b)$ such that $a + b = 10$:
     $$\{(1,9), (2,8), (3,7), (4,6), (5,5), (6,4), (7,3), (8,2), (9,1)\}$$
   * Number of favorable outcomes $= 9$.
   * $P(\text{Ram}) = \frac{9}{81} = \frac{1}{9}$.

2. **Shyam's Probability (Sum = 8):**
   * Favorable pairs $(a, b)$ such that $a + b = 8$:
     $$\{(1,7), (2,6), (3,5), (4,4), (5,3), (6,2), (7,1)\}$$
   * Number of favorable outcomes $= 7$.
   * $P(\text{Shyam}) = \frac{7}{81}$.

3. **Product of Probabilities:**
   * $$\text{Product} = P(\text{Ram}) \times P(\text{Shyam}) = \frac{1}{9} \times \frac{7}{81} = \frac{7}{729}$$

---

## Question 3 (2 Marks)
**Answer any one of the following questions.**

### Option (A)
A factory manufactures mobile handsets. It produces 680 units in the 4th year and 780 units in the 8th year. Assuming production uniformly increases by a fixed number every year, find:
1. Production in first year.
2. Production in 11th year.
3. The total production in 11 years.

#### Step-by-Step Solution:
Since the production increases uniformly by a fixed number, it forms an Arithmetic Progression (AP). Let $a$ be the production in the first year and $d$ be the uniform annual increase.

1. **Set up equations using $a_n = a + (n-1)d$:**
   * For the 4th year ($a_4 = 680$):
     $$a + 3d = 680 \quad \text{--- (Eq 1)}$$
   * For the 8th year ($a_8 = 780$):
     $$a + 7d = 780 \quad \text{--- (Eq 2)}$$

2. **Solve for $a$ and $d$:**
   * Subtract Eq 1 from Eq 2:
     $$(a + 7d) - (a + 3d) = 780 - 680 \implies 4d = 100 \implies d = 25$$
   * Substitute $d = 25$ back into Eq 1:
     $$a + 3(25) = 680 \implies a + 75 = 680 \implies a = 605$$
   * **Answer (i):** Production in the first year ($a$) is **605 units**.

3. **Find Production in the 11th year ($a_{11}$):**
   * $$a_{11} = a + 10d = 605 + 10(25) = 605 + 250 = 855$$
   * **Answer (ii):** Production in the 11th year is **855 units**.

4. **Find Total Production in 11 years ($S_{11}$):**
   * Using the sum formula $S_n = \frac{n}{2}[2a + (n-1)d]$:
     $$S_{11} = \frac{11}{2}[2(605) + 10(25)] = \frac{11}{2}[1210 + 250] = \frac{11}{2}[1460] = 11 \times 730 = 8030$$
   * **Answer (iii):** Total production over 11 years is **8030 units**.

---

### Option (B)
Find the sum of the following series up to the given number:
$$\frac{1^{3}+2^{3}+3^{3}+...................+15^{3}}{1^{2}+2^{2}+3^{2}+..........+15^{2}}$$

#### Step-by-Step Solution:
Using the given standard identities for $n = 15$:

1. **Numerator (Sum of cubes $\Sigma n^3$):**
   * $$\Sigma_{n=1}^{15} n^3 = \left[ \frac{15(15 + 1)}{2} \right]^2 = \left[ \frac{15 \times 16}{2} \right]^2 = [15 \times 8]^2 = (120)^2 = 14400$$

2. **Denominator (Sum of squares $\Sigma n^2$):**
   * $$\Sigma_{n=1}^{15} n^2 = \frac{15(15 + 1)(2(15) + 1)}{6} = \frac{15 \times 16 \times 31}{6} = \frac{7440}{6} = 1240$$

3. **Evaluate the ratio:**
   * $$\text{Value} = \frac{14400}{1240} = \frac{1440}{124} = \frac{360}{31} \approx 11.61$$

---

## Question 4 (4 Marks)
**Answer any one of the following questions.**

### Option (A)
1. Prove that: $\tan(60^{\circ}+A)\tan(60^{\circ}-A)=\frac{2 \cos 2A+1}{2 \cos 2A-1}$
2. Find the general value of $\theta$ satisfying $\tan \theta+\tan 2\theta+\tan 3\theta=0$

#### Step-by-Step Solution:

**Part 1: Proof**
* Apply the tangent addition and subtraction formulas $\tan(60^\circ \pm A) = \frac{\tan 60^\circ \pm \tan A}{1 \mp \tan 60^\circ \tan A}$:
  $$\text{LHS} = \left(\frac{\sqrt{3} + \tan A}{1 - \sqrt{3}\tan A}\right) \times \left(\frac{\sqrt{3} - \tan A}{1 + \sqrt{3}\tan A}\right) = \frac{3 - \tan^2 A}{1 - 3\tan^2 A}$$
* Convert $\tan^2 A$ into sine and cosine expressions ($\tan^2 A = \frac{\sin^2 A}{\cos^2 A}$):
  $$\text{LHS} = \frac{3 - \frac{\sin^2 A}{\cos^2 A}}{1 - 3\frac{\sin^2 A}{\cos^2 A}} = \frac{3\cos^2 A - \sin^2 A}{\cos^2 A - 3\sin^2 A}$$
* Substitute the identities $\sin^2 A = \frac{1 - \cos 2A}{2}$ and $\cos^2 A = \frac{1 + \cos 2A}{2}$:
  $$\text{Numerator} = 3\left(\frac{1 + \cos 2A}{2}\right) - \left(\frac{1 - \cos 2A}{2}\right) = \frac{3 + 3\cos 2A - 1 + \cos 2A}{2} = \frac{2 + 4\cos 2A}{2} = 1 + 2\cos 2A$$
  $$\text{Denominator} = \left(\frac{1 + \cos 2A}{2}\right) - 3\left(\frac{1 - \cos 2A}{2}\right) = \frac{1 + \cos 2A - 3 + 3\cos 2A}{2} = \frac{4\cos 2A - 2}{2} = 2\cos 2A - 1$$
* Combining them gives:
  $$\text{LHS} = \frac{2\cos 2A + 1}{2\cos 2A - 1} = \text{RHS} \quad (\text{Hence Proved})$$

**Part 2: General Solution**
* Group the terms using $\tan 3\theta = \tan(\theta + 2\theta) = \frac{\tan \theta + \tan 2\theta}{1 - \tan \theta \tan 2\theta} \implies \tan \theta + \tan 2\theta = \tan 3\theta(1 - \tan \theta \tan 2\theta)$.
* Substitute this into the equation:
  $$\tan 3\theta(1 - \tan \theta \tan 2\theta) + \tan 3\theta = 0$$
  $$\tan 3\theta (1 - \tan \theta \tan 2\theta + 1) = 0 \implies \tan 3\theta (2 - \tan \theta \tan 2\theta) = 0$$
* **Case 1:** $\tan 3\theta = 0 \implies 3\theta = n\pi \implies \theta = \frac{n\pi}{3}, \quad n \in \mathbb{Z}$
* **Case 2:** $2 - \tan \theta \tan 2\theta = 0 \implies \tan \theta \cdot \left(\frac{2\tan \theta}{1 - \tan^2 \theta}\right) = 2 \implies \frac{2\tan^2 \theta}{1 - \tan^2 \theta} = 2 \implies 2\tan^2 \theta = 2 - 2\tan^2 \theta \implies 4\tan^2 \theta = 2 \implies \tan^2 \theta = \frac{1}{2}$
  $$\tan \theta = \pm \frac{1}{\sqrt{2}} \implies \theta = m\pi \pm \tan^{-1}\left(\frac{1}{\sqrt{2}}\right), \quad m \in \mathbb{Z}$$

---

### Option (B)
Kiran is designing a triangular park. She wants the angles of the triangle to be in Arithmetic Progression. She also places two fences along two sides of the triangle. The lengths of these two sides are in the ratio $\sqrt{3} : \sqrt{2}$. These sides lie opposite to the smallest angle and the larger angle. Find:
1. The measures of all three angles.
2. Which side is opposite the largest angle?

#### Step-by-Step Solution:

1. **Find the angle measures:**
   * Let the three interior angles of the triangle be $A$, $B$, and $C$ in increasing order ($A < B < C$). Since they form an AP, we can represent them as:
     $$A = x - d, \quad B = x, \quad C = x + d$$
   * By the Angle Sum Property of triangles:
     $$(x - d) + x + (x + d) = 180^{\circ} \implies 3x = 180^{\circ} \implies x = 60^{\circ}$$
   * Thus, the middle angle $B$ is exactly **$60^\circ$**.
   * We are given that the two sides with ratio $\sqrt{3} : \sqrt{2}$ lie opposite the smallest angle ($A$) and the larger angle ($B$). Therefore, $\frac{a}{b} = \frac{\sqrt{3}}{\sqrt{2}}$.
   * By the Law of Sines ($\frac{a}{\sin A} = \frac{b}{\sin B}$):
     $$\frac{\sin A}{\sin B} = \frac{a}{b} \implies \frac{\sin A}{\sin 60^{\circ}} = \frac{\sqrt{3}}{\sqrt{2}}$$
     $$\sin A = \frac{\sqrt{3}}{\sqrt{2}} \times \sin 60^{\circ} = \frac{\sqrt{3}}{\sqrt{2}} \times \frac{\sqrt{3}}{2} = \frac{3}{2\sqrt{2}}$$
   * Wait, $\frac{3}{2\sqrt{2}} \approx 1.06$, which is greater than 1, making $\sin A$ impossible. Let's re-read the configuration: "opposite to the smallest angle and the larger angle". The larger angle of these two is $B = 60^{\circ}$, so side $b$ must be larger than side $a$. Thus, the inverse ratio applies: $\frac{a}{b} = \frac{\sqrt{2}}{\sqrt{3}}$.
     $$\sin A = \frac{\sqrt{2}}{\sqrt{3}} \times \sin 60^{\circ} = \frac{\sqrt{2}}{\sqrt{3}} \times \frac{\sqrt{3}}{2} = \frac{\sqrt{2}}{2} = \frac{1}{\sqrt{2}}$$
   * Since $\sin A = \frac{1}{\sqrt{2}}$, the smallest angle is $A = 45^{\circ}$.
   * Calculate the remaining largest angle $C$:
     $$C = 180^{\circ} - (A + B) = 180^{\circ} - (45^{\circ} + 60^{\circ}) = 75^{\circ}$$
   * **Answer (i):** The three angles are **$45^\circ$, $60^\circ$, and $75^\circ$**.

2. **Identify the side opposite the largest angle:**
   * The largest angle is $C = 75^{\circ}$.
   * **Answer (ii):** **Side $c$** is opposite the largest angle.

---

## Question 5 (4 Marks)
**Answer any one of the following questions.**

### Option (A)
Based on the given frequency distribution of monthly internet data usage (in GB) of 800 users, determine the following:
1. Upper limit of the fifth class.
2. Lower limit of the eighth class.
3. Size of the class interval.
4. Frequency of the fourth class.
5. Cumulative frequency of the sixth class.
6. Percentage of users who used 100 GB or more.
7. The median of the data.

#### Step-by-Step Solution:
First, let's establish continuous class boundaries since the given classes are discontinuous (discrete):
* 40-49 $\rightarrow$ 39.5-49.5 ($f = 28, cf = 28$)
* 50-59 $\rightarrow$ 49.5-59.5 ($f = 92, cf = 120$)
* 60-69 $\rightarrow$ 59.5-69.5 ($f = 116, cf = 236$)
* 70-79 $\rightarrow$ 69.5-79.5 ($f = 152, cf = 388$)
* 80-89 $\rightarrow$ 79.5-89.5 ($f = 136, cf = 524$)
* 90-99 $\rightarrow$ 89.5-99.5 ($f = 124, cf = 648$)
* 100-109 $\rightarrow$ 99.5-109.5 ($f = 96, cf = 744$)
* 110-119 $\rightarrow$ 109.5-119.5 ($f = 44, cf = 788$)
* 120-129 $\rightarrow$ 119.5-129.5 ($f = 12, cf = 800$)

1. **Upper limit of fifth class (80-89):** **89** (or continuous limit **89.5**)
2. **Lower limit of eighth class (110-119):** **110** (or continuous limit **109.5**)
3. **Size of class interval ($h$):** $49.5 - 39.5 =$ **10**
4. **Frequency of fourth class (70-79):** **152**
5. **Cumulative frequency of sixth class (90-99):** **648**
6. **Percentage of users using 100 GB or more:**
   * Users $\ge 100 \text{ GB} = 96 + 44 + 12 = 152$.
   * Percentage $= \frac{152}{800} \times 100 =$ **19%**
7. **Calculate the Median:**
   * $N = 800 \implies \frac{N}{2} = 400$.
   * The cumulative frequency just greater than 400 is 524, which belongs to the class **79.5 - 89.5**.
   * Lower limit ($L$) $= 79.5$, preceding $cf = 388$, frequency $f = 136$, width $h = 10$.
   * $$\text{Median} = L + \left( \frac{\frac{N}{2} - cf}{f} \right) \times h = 79.5 + \left( \frac{400 - 388}{136} \right) \times 10 = 79.5 + \frac{120}{136} \approx 79.5 + 0.88 = 80.38 \text{ GB}$$

---

### Option (B)
Choose the correct code option for the given statement and validate it with structural reasoning.
* **Assertion (A):** Set A has 6 observations: 5,15,25,35,45,55 (Mean = 30, Var = 291.67). Set B has 31 observations: 15,16,17,18,...45 (Mean = 30, Var = 80).
* **Reason (R):** (Provides the two structural dot diagrams highlighting data distribution around the mean value 30).

#### Step-by-Step Solution:
1. **Verify Assertion (A):**
   * Set A mean $= \frac{5+15+25+35+45+55}{6} = \frac{180}{6} = 30$. (True)
   * Set B consists of consecutive integers from 15 to 45. It is a symmetric arithmetic progression, so its mean is the middle value: $\frac{15+45}{2} = 30$. (True)
   * The spread of data points in Set A ($\pm 5, \pm 15, \pm 25$ from the mean) is visibly much wider and more dispersed than the compact consecutive block of Set B ($\pm 1$ up to $\pm 15$). This directly accounts for Set A's significantly higher variance ($291.67 > 80$). Thus, the assertion numbers are valid.

2. **Verify Reason (R):**
   * The dot plots accurately show the visual distribution of the data. Set A has widely spaced points, demonstrating high dispersion, while Set B has a dense, uniform distribution clustered closely around the mean, demonstrating lower dispersion. This visual representation serves as the exact qualitative explanation for why the variance of Set A is much larger than that of Set B.

* **Correct Option:** **(a) Both (A) and (R) are true and (R) is the correct explanation of (A)**.

---

## Question 6 (6 Marks - Long Project)
**Prepare any one project as given below.**

### Option (A)
#### Part I:
A carpenter wants to cut three lengths from a single piece of cardboard of length $101 \text{ cm}$. The second length is $11 \text{ cm}$ longer than the shortest and the third length is thrice the shortest. What are the possible lengths of the shortest piece, if the third piece is at least $8 \text{ cm}$ longer than the second?

##### Step-by-Step Solution:
Let the length of the shortest piece be $x \text{ cm}$.
* First (shortest) length $= x$
* Second length $= x + 11$
* Third length $= 3x$

1. **Set up the total length inequality:**
   * The sum of all three cut pieces cannot exceed the total cardboard limit of 101 cm:
     $$x + (x + 11) + 3x \le 101$$
     $$5x + 11 \le 101 \implies 5x \le 90 \implies x \le 18 \quad \text{--- (Inequality 1)}$$

2. **Set up the comparative piece constraint:**
   * The third piece is *at least* 8 cm longer than the second piece:
     $$3x \ge (x + 11) + 8$$
     $$3x \ge x + 19 \implies 2x \ge 19 \implies x \ge 9.5 \quad \text{--- (Inequality 2)}$$

3. **Combine constraints:**
   * Combining both conditions gives the range for the shortest piece:
     $$9.5 \le x \le 18$$
   * **Conclusion:** The possible length of the shortest piece ranges from **$9.5 \text{ cm}$ to $18 \text{ cm}$** (inclusive).

#### Part II:
Given $z_{1}=3-2i$, $z_{2}=3+2i$, and $z_{3}=1+i$. Find:
1. $\alpha = z_1 + z_2 + z_3$
2. $\beta = z_1 \times z_2 \times z_3$
3. $\gamma = \frac{2z_1z_2}{z_3}$
4. Represent $\alpha, \beta, \gamma$ on the complex plane.
5. Find the Argument and Modulus of $\alpha, \beta, \gamma$.

##### Step-by-Step Solution:

1. **Calculate and analyze $\alpha$:**
   $$\alpha = (3 - 2i) + (3 + 2i) + (1 + i) = 7 + i$$
   * Modulus $|\alpha| = \sqrt{7^2 + 1^2} = \sqrt{50} = 5\sqrt{2}$
   * Argument $\theta_\alpha = \tan^{-1}\left(\frac{1}{7}\right)$ (Quadrant I)

2. **Calculate and analyze $\beta$:**
   * Notice that $z_1 \times z_2$ is a product of conjugates: $(3-2i)(3+2i) = 3^2 - (2i)^2 = 9 + 4 = 13$.
   $$\beta = 13 \times (1 + i) = 13 + 13i$$
   * Modulus $|\beta| = \sqrt{13^2 + 13^2} = 13\sqrt{2}$
   * Argument $\theta_\beta = \tan^{-1}\left(\frac{13}{13}\right) = \tan^{-1}(1) = \frac{\pi}{4}$ or **$45^\circ$** (Quadrant I)

3. **Calculate and analyze $\gamma$:**
   $$\gamma = \frac{2 \times 13}{1 + i} = \frac{26}{1 + i}$$
   * Rationalize the denominator by multiplying by $(1 - i)$:
     $$\gamma = \frac{26(1 - i)}{(1 + i)(1 - i)} = \frac{26(1 - i)}{2} = 13 - 13i$$
   * Modulus $|\gamma| = \sqrt{13^2 + (-13)^2} = 13\sqrt{2}$
   * Argument: The real part is positive and the imaginary part is negative (Quadrant IV):
     $$\theta_\gamma = -\tan^{-1}\left(\frac{13}{13}\right) = -\frac{\pi}{4} \text{ or } \frac{7\pi}{4} \quad (-45^\circ)$$

4. **Complex Plane Mapping Coordinates:**
   * Plot $\alpha$ at $(7, 1)$
   * Plot $\beta$ at $(13, 13)$
   * Plot $\gamma$ at $(13, -13)$

---

### Option (B)
#### Part I: Invitation combinations
Rohan has 7 relatives (4 women, 3 men). Sunita has 7 relatives (3 women, 4 men). They want to invite a total of 3 women and 3 men, such that 3 guests are Rohan's relatives and 3 are Sunita's relatives. In how many ways can they invite them?

##### Step-by-Step Solution:
Let Rohan choose $k$ women from his 4 female relatives, meaning he must choose $(3-k)$ men from his 3 male relatives to make a total of 3 guests. Consequently, to reach a total of 3 women and 3 men, Sunita must choose $(3-k)$ women from her 3 female relatives and $k$ men from her 4 male relatives.

Let's look at the valid values for $k$:
* **Case 1 ($k=0$):** Rohan chooses 0 women, 3 men. Sunita chooses 3 women, 0 men.
  $$\text{Ways} = \left( \binom{4}{0} \times \binom{3}{3} \right) \times \left( \binom{3}{3} \times \binom{4}{0} \right) = (1 \times 1) \times (1 \times 1) = 1$$
* **Case 2 ($k=1$):** Rohan chooses 1 woman, 2 men. Sunita chooses 2 women, 1 man.
  $$\text{Ways} = \left( \binom{4}{1} \times \binom{3}{2} \right) \times \left( \binom{3}{2} \times \binom{4}{1} \right) = (4 \times 3) \times (3 \times 4) = 12 \times 12 = 144$$
* **Case 3 ($k=2$):** Rohan chooses 2 women, 1 man. Sunita chooses 1 woman, 2 men.
  $$\text{Ways} = \left( \binom{4}{2} \times \binom{3}{1} \right) \times \left( \binom{3}{1} \times \binom{4}{2} \right) = (6 \times 3) \times (3 \times 6) = 18 \times 18 = 324$$
* **Case 4 ($k=3$):** Rohan chooses 3 women, 0 men. Sunita chooses 0 women, 3 men.
  $$\text{Ways} = \left( \binom{4}{3} \times \binom{3}{0} \right) \times \left( \binom{3}{0} \times \binom{4}{3} \right) = (4 \times 1) \times (1 \times 4) = 4 \times 4 = 16$$

Total possible invitation configurations:
$$\text{Total Ways} = 1 + 144 + 324 + 16 = 485$$

#### Part II: Binomial Progression Proof
Prove that if the 5th, 6th, and 7th terms in the expansion of $(1+y)^n$ form an AP, then one possible value of $n$ is double the other.

##### Step-by-Step Solution:
The general term is given by $T_{r+1} = \binom{n}{r} y^r$. The coefficients for the 5th, 6th, and 7th terms are $\binom{n}{4}$, $\binom{n}{5}$, and $\binom{n}{6}$ respectively. Since they form an Arithmetic Progression:
$$2 \cdot \binom{n}{5} = \binom{n}{4} + \binom{n}{6}$$
Divide the entire equation by $\binom{n}{5}$:
$$2 = \frac{\binom{n}{4}}{\binom{n}{5}} + \frac{\binom{n}{6}}{\binom{n}{5}}$$
Using the factorial reduction identity $\frac{\binom{n}{r}}{\binom{n}{r-1}} = \frac{n-r+1}{r}$:
* $\frac{\binom{n}{4}}{\binom{n}{5}} = \frac{5}{n-4}$
* $\frac{\binom{n}{6}}{\binom{n}{5}} = \frac{n-5}{6}$

Substitute these back into the equation:
$$2 = \frac{5}{n-4} + \frac{n-5}{6}$$
Multiply the entire equation by the common denominator $6(n-4)$:
$$12(n-4) = 30 + (n-5)(n-4)$$
$$12n - 48 = 30 + n^2 - 9n + 20$$
$$12n - 48 = n^2 - 9n + 50$$
Rearrange this into a standard quadratic form:
$$n^2 - 21n + 98 = 0$$
Factorize the quadratic equation:
$$(n - 14)(n - 7) = 0 \implies n = 14 \quad \text{or} \quad n = 7$$
Notice that $14 = 2 \times 7$. Thus, one value of $n$ is exactly double the other. **(Hence Proved)**.

#### Part III: Area Optimization
The length of a table is $(x+3)$ feet and the width is $(x+1)$ feet. The area must be less than 30 square feet. Write and solve an inequality for $x$.

##### Step-by-Step Solution:
1. **Set up the area inequality:**
   $$\text{Area} = \text{Length} \times \text{Width} < 30$$
   $$(x + 3)(x + 1) < 30$$
   $$x^2 + 4x + 3 < 30 \implies x^2 + 4x - 27 < 0$$

2. **Find the roots using the quadratic formula ($x = \frac{-b \pm \sqrt{b^2-4ac}}{2a}$):**
   $$x = \frac{-4 \pm \sqrt{16 - 4(1)(-27)}}{2} = \frac{-4 \pm \sqrt{16 + 108}}{2} = \frac{-4 \pm \sqrt{124}}{2} = \frac{-4 \pm 2\sqrt{31}}{2} = -2 \pm \sqrt{31}$$
   * Since $\sqrt{31} \approx 5.57$, the roots are approximately $-7.57$ and $3.57$.
   * For the polynomial to be less than zero, $x$ must lie between these two values: $-2 - \sqrt{31} < x < -2 + \sqrt{31}$.

3. **Apply physical boundaries:**
   * Length and width must be strictly positive quantities, meaning $x+1 > 0 \implies x > -1$.
   * Combining this with our upper bound gives the valid range for $x$:
     $$-1 < x < -2 + \sqrt{31} \quad (\text{or approximately } -1 < x < 3.57)$$