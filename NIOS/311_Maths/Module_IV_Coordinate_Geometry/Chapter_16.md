# NIOS Senior Secondary Mathematics (311)

## Module IV: Co-ordinate Geometry
### Chapter 16: Conic Sections

### Introduction & Key Objectives
Conic Sections (or conics) are curves obtained by intersecting a double-napped right circular cone with a flat plane. Depending on the angle of the cutting plane, we obtain three distinct types of open and closed curves: the Parabola, the Ellipse, and the Hyperbola. Historically studied by ancient Greek mathematicians like Apollonius, conic sections are vital in modern science for understanding planetary orbits, satellite dish designs, and the trajectories of projectiles.

After studying this chapter, you will be able to:
* Define a **Conic Section** using the focus-directrix property.
* Understand the role of **Eccentricity ($e$)** in classifying conics.
* Derive and apply the standard equations and geometric features of a **Parabola**.
* Derive and apply the standard equations and geometric features of an **Ellipse**.
* Derive and apply the standard equations and geometric features of a **Hyperbola**.

---

### Core Concepts & Formulas

#### 1. General Focus-Directrix Definition
> **Conic Section:** The locus of a point $P$ which moves in a plane such that its distance from a fixed point $S$ (called the **Focus**) bears a constant ratio to its perpendicular distance from a fixed straight line $L$ (called the **Directrix**).

This constant ratio is called the **Eccentricity**, denoted by $e$:
$$\frac{\text{Distance from Focus } (SP)}{\text{Distance from Directrix } (PM)} = e \implies SP = e \cdot PM$$

The value of $e$ completely determines the type of curve:
* If $e = 1$: The curve is a **Parabola**.
* If $0 < e < 1$: The curve is an **Ellipse**.
* If $e > 1$: The curve is a **Hyperbola**.

---

#### 2. The Parabola ($e = 1$)
A parabola is symmetric along its axis and has one vertex. There are four standard orientations, but the primary baseline is the rightward-opening parabola.

> **Standard Equation (Rightward Form):**
> $$y^2 = 4ax \quad (a > 0)$$



**Key Geometric Properties of $y^2 = 4ax$:**
* **Vertex:** $(0,0)$
* **Focus ($S$):** $(a,0)$
* **Equation of Directrix:** $x = -a \implies x + a = 0$
* **Axis of Symmetry:** y-axis ($y = 0$)
* **Length of Latus Rectum:** $4a$

*Alternative Orientations:*
* Leftward: $y^2 = -4ax \implies$ Focus at $(-a,0)$, Directrix $x = a$
* Upward: $x^2 = 4ay \implies$ Focus at $(0,a)$, Directrix $y = -a$
* Downward: $x^2 = -4ay \implies$ Focus at $(0,-a)$, Directrix $y = a$

---

#### 3. The Ellipse ($0 < e < 1$)
An ellipse is a closed oval curve with two foci and two directrices.

> **Standard Equation (Horizontal Major Axis):**
> $$\frac{x^2}{a^2} + \frac{y^2}{b^2} = 1 \quad (\text{where } a > b)$$



**Key Geometric Properties:**
* **Center:** $(0,0)$
* **Vertices:** $(\pm a, 0)$
* **Length of Major Axis:** $2a$ | **Length of Minor Axis:** $2b$
* **Foci ($S$ and $S'$):** $(\pm ae, 0)$
* **Equations of Directrices:** $x = \pm \frac{a}{e}$
* **Length of Latus Rectum:** $\frac{2b^2}{a}$
* **Eccentricity Formula Relation:**
> $$b^2 = a^2(1 - e^2) \implies e = \sqrt{1 - \frac{b^2}{a^2}}$$

*(Note: If $b > a$, the major axis lies vertically along the y-axis, and terms swap roles accordingly).*

---

#### 4. The Hyperbola ($e > 1$)
A hyperbola consists of two separate symmetric open branches stretching outwards indefinitely.

> **Standard Equation (Transverse Axis along x-axis):**
> $$\frac{x^2}{a^2} - \frac{y^2}{b^2} = 1$$



**Key Geometric Properties:**
* **Center:** $(0,0)$
* **Vertices:** $(\pm a, 0)$
* **Length of Transverse Axis:** $2a$ | **Length of Conjugate Axis:** $2b$
* **Foci ($S$ and $S'$):** $(\pm ae, 0)$
* **Equations of Directrices:** $x = \pm \frac{a}{e}$
* **Length of Latus Rectum:** $\frac{2b^2}{a}$
* **Eccentricity Formula Relation:**
> $$b^2 = a^2(e^2 - 1) \implies e = \sqrt{1 + \frac{b^2}{a^2}}$$

---

### Step-by-Step Examples

**Example 1:** Find the coordinates of the focus, the equation of the directrix, and the length of the latus rectum for the parabola $y^2 = 12x$.  
**Solution:**
1. Compare the given equation with the standard form $y^2 = 4ax$:
$$4a = 12 \implies a = 3$$
2. Since it is a standard rightward parabola ($a=3$):
   * **Focus ($S$):** $(a, 0) = (3, 0)$
   * **Directrix Equation:** $x = -a \implies x = -3 \implies x + 3 = 0$
   * **Length of Latus Rectum:** $4a = 12$

**Example 2:** Find the eccentricity, the coordinates of the foci, and the length of the latus rectum for the ellipse $\frac{x^2}{25} + \frac{y^2}{16} = 1$.  
**Solution:**
1. Identify the baseline values: $a^2 = 25 \implies a = 5$ and $b^2 = 16 \implies b = 4$. Since $a > b$, this is a horizontal ellipse.
2. Calculate the eccentricity ($e$) using the core relation formula:
$$e = \sqrt{1 - \frac{b^2}{a^2}} = \sqrt{1 - \frac{16}{25}} = \sqrt{\frac{9}{25}} = \frac{3}{5} = 0.6$$
3. Calculate focal points using $(\pm ae, 0)$:
$$ae = 5 \times \frac{3}{5} = 3 \implies \text{Foci} = (\pm 3, 0)$$
4. Compute the length of the latus rectum:
$$\text{Latus Rectum Length} = \frac{2b^2}{a} = \frac{2(16)}{5} = \frac{32}{5} = 6.4 \text{ units}$$

**Example 3:** Find the equation of the hyperbola whose foci are at $(\pm 5, 0)$ and whose transverse axis has a total length of $8$.  
**Solution:**
1. From the given focus properties, the foci are along the x-axis, so the equation matches the standard format $\frac{x^2}{a^2} - \frac{y^2}{b^2} = 1$.
2. Extract parameters:
   * Focal distance: $ae = 5$
   * Transverse axis length: $2a = 8 \implies a = 4$
3. Find $e$ from $ae$: $4e = 5 \implies e = \frac{5}{4}$.
4. Calculate $b^2$ using the hyperbola's key algebraic identity:
$$b^2 = a^2(e^2 - 1) = 4^2 \left[ \left(\frac{5}{4}\right)^2 - 1 \right] = 16 \left( \frac{25}{16} - 1 \right) = 16 \left(\frac{9}{16}\right) = 9$$
5. Substitute $a^2 = 16$ and $b^2 = 9$ into the standard form:
$$\frac{x^2}{16} - \frac{y^2}{9} = 1 \implies 9x^2 - 16y^2 = 144$$

---

### Terminal Exercises & Self-Check Questions

1. **Parabola Equation Extraction:** Find the equation of a parabola with its vertex at the origin, opening upwards, and passing through the coordinate point $(4, 2)$.
   * *Answer Hint:* An upward-facing parabola matches the profile $x^2 = 4ay$. Substitute the coordinates to solve for $a$: $4^2 = 4a(2) \implies 16 = 8a \implies a = 2$. The equation is $x^2 = 8y$.

2. **Conic Identification Workout:** Determine the type of conic section represented by the parameters: Focus at $(2,0)$, Directrix line $x = -2$, and passing through point $P(2,4)$. Verify its eccentricity.
   * *Step-by-Step Solution:* 1. Distance $SP$ from Focus to point: $\sqrt{(2-2)^2 + (4-0)^2} = \sqrt{0 + 16} = 4$.
     2. Perpendicular distance $PM$ from Directrix $x+2=0$ to point: $\frac{|2 + 2|}{\sqrt{1^2}} = 4$.
     3. Check eccentricity ratio: $e = \frac{SP}{PM} = \frac{4}{4} = 1$.
     4. Since $e = 1$, the conic section is a **Parabola**.

3. **Hyperbola Parameter Calculation:** Find the eccentricity of the hyperbola given by the equation $9x^2 - 16y^2 = 144$.
   * *Answer Hint:* Convert to standard form by dividing through by 144: $\frac{x^2}{16} - \frac{y^2}{9} = 1$. Here $a^2 = 16, b^2 = 9$.
     $$e = \sqrt{1 + \frac{b^2}{a^2}} = \sqrt{1 + \frac{9}{16}} = \sqrt{\frac{25}{16}} = \frac{5}{4}$$