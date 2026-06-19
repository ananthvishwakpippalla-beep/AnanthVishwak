# NIOS Senior Secondary Mathematics (311)

## Chapter 5: Relation between Sides and Angles of a Triangle

### Introduction & Key Objectives
In engineering, architecture, surveying, and navigation, measuring distances and heights often requires solving triangles where some angles or sides are unknown. While basic trigonometry deals with right-angled triangles, this chapter provides powerful tools—the Sine Rule, Cosine Rule, and Projection Formula—to analyze the exact mathematical relationships between sides and angles in **any** oblique (non-right) triangle.

After studying this chapter, you will be able to:
* State and prove the **Sine Rule** for any triangle.
* State and apply the **Cosine Rule** to calculate sides or interior angles.
* State and apply the **Projection Formula**.
* Solve practical triangles given various combinations of sides and angles (e.g., SSS, SAS, ASA).

---

### Core Concepts & Formulas

#### Standard Notations
In any triangle $ABC$:
* The angles at the vertices $A$, $B$, and $C$ are denoted simply by capital letters $A$, $B$, and $C$.
* The lengths of the sides opposite to these angles are denoted by lowercase letters $a$, $b$, and $c$ respectively (where side $a = BC$, side $b = AC$, and side $c = AB$).



#### 1. The Sine Rule
> **The Sine Rule:** The sides of any triangle are proportional to the sines of their opposite angles.
> $$\frac{a}{\sin A} = \frac{b}{\sin B} = \frac{c}{\sin C} = k$$
*(where $k$ is a constant of proportionality, often equal to $2R$, the diameter of the triangle's circumcircle).*

*Useful Constant Form Variations:*
* $a = k\sin A$, $b = k\sin B$, $c = k\sin C$
* $\frac{\sin A}{a} = \frac{\sin B}{b} = \frac{\sin C}{c}$

#### 2. The Cosine Rule
> **The Cosine Rule:** In any triangle, the square of any side is equal to the sum of the squares of the other two sides minus twice their product multiplied by the cosine of their included angle.
> * $$a^2 = b^2 + c^2 - 2bc\cos A$$
> * $$b^2 = a^2 + c^2 - 2ac\cos B$$
> * $$c^2 = a^2 + b^2 - 2ab\cos C$$

*Formula Variations for Calculating Angles:*
* $$\cos A = \frac{b^2 + c^2 - a^2}{2bc}$$
* $$\cos B = \frac{a^2 + c^2 - b^2}{2ac}$$
* $$\cos C = \frac{a^2 + b^2 - c^2}{2ab}$$

#### 3. The Projection Formula
> **The Projection Formula:** In any triangle $ABC$, any side can be expressed as the sum of the projections of the other two sides onto it.
> * $$a = b\cos C + c\cos B$$
> * $$b = c\cos A + a\cos C$$
> * $$c = a\cos B + b\cos A$$

---

### Step-by-Step Examples

**Example 1:** In a triangle $ABC$, if $A = 30^\circ$, $B = 45^\circ$, and side $a = 2 \text{ cm}$, find the exact length of side $b$.  
**Solution:**
1. Identify the given elements: $A = 30^\circ$, $B = 45^\circ$, and $a = 2$. We need to find $b$.
2. Choose the appropriate rule. Since we have two angles and an opposite side, apply the **Sine Rule**:
$$\frac{a}{\sin A} = \frac{b}{\sin B}$$
3. Rearrange the formula to solve for $b$:
$$b = \frac{a \cdot \sin B}{\sin A}$$
4. Substitute the values:
$$b = \frac{2 \cdot \sin 45^\circ}{\sin 30^\circ} = \frac{2 \cdot \left(\frac{1}{\sqrt{2}}\right)}{\frac{1}{2}}$$
5. Simplify the expression:
$$b = 2 \cdot \left(\frac{1}{\sqrt{2}}\right) \cdot 2 = \frac{4}{\sqrt{2}} = 2\sqrt{2} \text{ cm}$$

**Example 2:** The sides of a triangle $ABC$ are $a = 3 \text{ cm}$, $b = 5 \text{ cm}$, and $c = 7 \text{ cm}$. Find the value of $\cos C$ and determine if angle $C$ is obtuse.  
**Solution:**
1. Since all three sides are known (SSS condition), use the **Cosine Rule** to find angle $C$:
$$\cos C = \frac{a^2 + b^2 - c^2}{2ab}$$
2. Substitute the given side lengths:
$$\cos C = \frac{3^2 + 5^2 - 7^2}{2(3)(5)}$$
$$\cos C = \frac{9 + 25 - 49}{30} = \frac{34 - 49}{30} = -\frac{15}{30} = -\frac{1}{2}$$
3. Analyze the result: Since $\cos C = -\frac{1}{2}$, the value is negative. In a triangle, cosine is negative only in Quadrant II ($90^\circ < C < 180^\circ$).
4. Therefore, angle $C = 120^\circ$, which confirms that it is an **obtuse angle**.

**Example 3:** Using the projection formula, prove that $(b + c)\cos A + (c + a)\cos B + (a + b)\cos C = a + b + c$.  
**Solution:**
1. Expand the left-hand side ($\text{LHS}$) of the equation:
$$\text{LHS} = b\cos A + c\cos A + c\cos B + a\cos B + a\cos C + b\cos C$$
2. Group the terms intentionally to form the standard projection formulas:
$$\text{LHS} = (b\cos C + c\cos B) + (c\cos A + a\cos C) + (a\cos B + b\cos A)$$
3. Substitute the standard projection identities ($a = b\cos C + c\cos B$, etc.):
$$\text{LHS} = a + b + c = \text{RHS}$$
4. Hence proved.

---

### Terminal Exercises & Self-Check Questions

1. **Ratio Calculation:** In any triangle $ABC$, if the angles are in the ratio $1 : 2 : 3$, find the ratio of their corresponding opposite sides.
   * *Step-by-Step Solution:* 1. Let the angles be $x, 2x, 3x$. Sum of angles: $x + 2x + 3x = 180^\circ \implies 6x = 180^\circ \implies x = 30^\circ$.
     2. The angles are $A = 30^\circ$, $B = 60^\circ$, and $C = 90^\circ$.
     3. By the Sine Rule, side ratios match the sine of the angles: $a : b : c = \sin 30^\circ : \sin 60^\circ : \sin 90^\circ$.
     4. $a : b : c = \frac{1}{2} : \frac{\sqrt{3}}{2} : 1 = 1 : \sqrt{3} : 2$.

2. **Side Determination:** In triangle $ABC$, if $b = 3 \text{ cm}$, $c = 5 \text{ cm}$, and the included angle $A = 60^\circ$, calculate the length of side $a$.
   * *Answer Hint:* Use $a^2 = b^2 + c^2 - 2bc\cos A$.
     $$a^2 = 3^2 + 5^2 - 2(3)(5)\cos 60^\circ = 9 + 25 - 30(0.5) = 34 - 15 = 19 \implies a = \sqrt{19} \text{ cm}$$

3. **Identity Verification:** Prove that in any triangle $ABC$, $\frac{\sin(B - C)}{\sin(B + C)} = \frac{b^2 - c^2}{a^2}$.
   * *Answer Hint:* Expand the numerator using compound angle formulas, then substitute $b = k\sin B$, $c = k\sin C$, and notice that $\sin(B+C) = \sin(\pi - A) = \sin A$.