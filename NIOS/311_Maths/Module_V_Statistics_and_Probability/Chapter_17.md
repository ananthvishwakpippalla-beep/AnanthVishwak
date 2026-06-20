# NIOS Senior Secondary Mathematics (311)

## Module V: Statistics and Probability
### Chapter 17: Measures of Dispersion

### Introduction & Key Objectives
In earlier descriptive statistics classes, we focused heavily on measures of central tendency (Mean, Median, and Mode). While central tendency locates the center point of data, it tells us nothing about how spread out or squeezed the data points are around that center. Two completely different datasets can share the exact same average mean, but possess wildly varying risk, variation, or stability profiles. This chapter introduces mathematical methods to quantify this variability, known as **dispersion**.

After studying this chapter, you will be able to:
* Understand the concept of dispersion and distinguish between absolute and relative measures.
* Compute the **Range** for ungrouped and grouped data frequencies.
* Calculate the **Mean Deviation (MD)** about the mean and about the median for ungrouped and grouped datasets.
* Calculate the **Variance** and **Standard Deviation (SD)** for ungrouped and grouped frequency distributions.
* Compute and interpret the **Coefficient of Variation (CV)** to compare the stability/consistency of two distributions.

---

### Core Concepts & Formulas

#### 1. Range
The simplest absolute measure of dispersion. It tracks the absolute distance between the two extreme boundary observations.
> $$\text{Range} = X_{\text{max}} - X_{\text{min}}$$
* **Coefficient of Range (Relative Measure):** $$\text{Coefficient of Range} = \frac{X_{\text{max}} - X_{\text{min}}}{X_{\text{max}} + X_{\text{min}}}$$

#### 2. Mean Deviation (MD)
Mean deviation measures the arithmetic average of the absolute differences (deviations) of data points from a central value (Mean or Median). We use absolute value bars $|x|$ to treat all deviations as positive.

> **MD about Mean for Ungrouped Data:**
> $$\text{MD}(\bar{x}) = \frac{\sum |x_i - \bar{x}|}{n}$$
> *(where $\bar{x}$ is the mean of $n$ observations)*

> **MD about Median for Grouped Data:**
> $$\text{MD}(M) = \frac{\sum f_i |x_i - M|}{N}$$
> *(where $M$ is the median, $f_i$ is the frequency, $x_i$ is the class midpoint, and $N = \sum f_i$)*

---

#### 3. Variance and Standard Deviation (SD)
To eliminate negative signs without using absolute value bars, we square the deviations. This leads to Variance, and its positive square root is Standard Deviation ($\sigma$), which shares the original unit of the dataset.



> **For Ungrouped Data:**
> * **Variance ($\sigma^2$):** $$\sigma^2 = \frac{\sum (x_i - \bar{x})^2}{n} = \frac{\sum x_i^2}{n} - (\bar{x})^2$$
> * **Standard Deviation ($\sigma$):** $$\sigma = \sqrt{\frac{\sum (x_i - \bar{x})^2}{n}}$$

> **For Grouped Data (Frequency Distribution):**
> * **Variance ($\sigma^2$):** $$\sigma^2 = \frac{\sum f_i(x_i - \bar{x})^2}{N} = \frac{\sum f_i x_i^2}{N} - \left(\frac{\sum f_i x_i}{N}\right)^2$$
> * **Standard Deviation ($\sigma$):** $$\sigma = \sqrt{\frac{\sum f_i(x_i - \bar{x})^2}{N}}$$

* **Short-cut (Step-Deviation) Method Form:** If classes have a uniform width $h$, we can substitute $u_i = \frac{x_i - A}{h}$ around an assumed mean $A$:
$$\sigma = h \times \sqrt{\frac{\sum f_i u_i^2}{N} - \left(\frac{\sum f_i u_i}{N}\right)^2}$$

---

#### 4. Coefficient of Variation (CV)
When comparing two groups with different units or vastly different mean sizes (e.g., comparing the variance of elephant weights versus mouse weights), we use a relative, unitless percentage measure.
> $$\text{CV} = \frac{\sigma}{\bar{x}} \times 100 \quad (\bar{x} \neq 0)$$
* **Interpretation Rule:** The series or group with a **higher CV** is more variable, less stable, and less consistent. The series with a **lower CV** is more stable and consistent.

---

### Step-by-Step Examples

**Example 1:** Calculate the Mean Deviation about the mean for the following ungrouped data: $6, 7, 10, 12, 13, 4, 8, 12$.  
**Solution:**
1. Count the number of observations: $n = 8$.
2. Calculate the arithmetic mean ($\bar{x}$):
$$\bar{x} = \frac{6 + 7 + 10 + 12 + 13 + 4 + 8 + 12}{8} = \frac{64}{8} = 8$$
3. Create a tracking checklist of absolute deviations $|x_i - \bar{x}|$ from 8:
   * $|6 - 8| = 2$
   * $|7 - 8| = 1$
   * $|10 - 8| = 2$
   * $|12 - 8| = 4$
   * $|13 - 8| = 5$
   * $|4 - 8| = 4$
   * $|8 - 8| = 0$
   * $|12 - 8| = 4$
4. Sum up the absolute deviations: $\sum |x_i - \bar{x}| = 2 + 1 + 2 + 4 + 5 + 4 + 0 + 4 = 22$.
5. Compute the final Mean Deviation:
$$\text{MD}(\bar{x}) = \frac{22}{8} = 2.75$$

**Example 2:** Find the variance and standard deviation for the discrete observations: $3, 5, 6, 7, 9$.  
**Solution:**
1. Number of data elements: $n = 5$.
2. Compute the mean ($\bar{x}$):
$$\bar{x} = \frac{3 + 5 + 6 + 7 + 9}{5} = \frac{30}{5} = 6$$
3. Find the squared values of the data points ($x_i^2$):
   * $3^2 = 9$, $5^2 = 25$, $6^2 = 36$, $7^2 = 49$, $9^2 = 81$
   * Sum of squares: $\sum x_i^2 = 9 + 25 + 36 + 49 + 81 = 200$
4. Apply the variance shortcut equation $\sigma^2 = \frac{\sum x_i^2}{n} - (\bar{x})^2$:
$$\sigma^2 = \frac{200}{5} - (6)^2 = 40 - 36 = 4$$
5. Extract the Standard Deviation ($\sigma$):
$$\sigma = \sqrt{4} = 2 \text{ units}$$

**Example 3:** Two factories show the following performance metrics for daily wage payouts:
* Factory A: Mean wage = $500 \text{ INR}$, Standard Deviation = $25 \text{ INR}$
* Factory B: Mean wage = $600 \text{ INR}$, Standard Deviation = $24 \text{ INR}$
Which factory has a more consistent wage distribution?  
**Solution:**
1. Compute the Coefficient of Variation ($\text{CV}$) for Factory A:
$$\text{CV}_A = \frac{\sigma_A}{\bar{x}_A} \times 100 = \frac{25}{500} \times 100 = 5\%$$
2. Compute the Coefficient of Variation ($\text{CV}$) for Factory B:
$$\text{CV}_B = \frac{\sigma_B}{\bar{x}_B} \times 100 = \frac{24}{600} \times 100 = 4\%$$
3. Compare the percentages: Since $\text{CV}_B < \text{CV}_A$ ($4\% < 5\%$), Factory B has lower relative variation.
4. Conclusion: **Factory B** is more consistent and stable in its wage distribution.

---

### Terminal Exercises & Self-Check Questions

1. **Range Metric Workout:** Find the range and coefficient of range for the data collection: $12, 25, 48, 5, 19, 36, 42, 11$.
   * *Answer Hint:* Identify limits: $X_{\text{max}} = 48$, $X_{\text{min}} = 5$. Range $= 48 - 5 = 43$. Coefficient of Range $= \frac{48 - 5}{48 + 5} = \frac{43}{53} \approx 0.811$.

2. **Standard Deviation Calculation:** Calculate the standard deviation for the first 5 consecutive natural numbers ($1, 2, 3, 4, 5$).
   * *Step-by-Step Solution:* 1. Mean $\bar{x} = \frac{1+2+3+4+5}{5} = \frac{15}{5} = 3$.
     2. Deviations from mean: $(1-3)=-2$, $(2-3)=-1$, $(3-3)=0$, $(4-3)=1$, $(5-3)=2$.
     3. Square the deviations: $4, 1, 0, 1, 4$. Sum of squares $= 4 + 1 + 0 + 1 + 4 = 10$.
     4. Variance $\sigma^2 = \frac{10}{5} = 2$.
     5. Standard Deviation $\sigma = \sqrt{2} \approx 1.414$.

3. **Relative Stability Workout:** The standard deviation of a dataset is $6$ and its mean is $20$. Find its Coefficient of Variation.
   * *Answer Hint:* Apply the CV definition: $\text{CV} = \frac{6}{20} \times 100 = 0.3 \times 100 = 30\%$.