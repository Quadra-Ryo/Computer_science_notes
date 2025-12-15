# Numerical Sets and Intervals on ℝ

## 1. Numerical Sets

The fundamental numerical sets are in an inclusion relation with each other:  
\[
ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ
\]

| Symbol | Name | Definition |
| :--- | :--- | :--- |
| **ℕ** | Natural Numbers | Set of non-negative integers: ℕ = {0, 1, 2, 3, 4, ...}. |
| **ℤ** | Integers | Set of positive and negative integers: ℤ = {..., -2, -1, 0, 1, 2, ...}. |
| **ℚ** | Rational Numbers | Set of numbers that can be expressed as fractions p/q, where p, q are elements of ℤ (integers) and q ≠ 0. They represent equivalence classes of fractions. |
| **ℝ** | Real Numbers | Set that includes all rational and irrational numbers (e.g., √2 or π). |

## 2. Relations Between Sets

The sets are included within one another:  
\[
ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ
\]

---

## 3. Intervals on ℝ

An **interval** I ⊂ ℝ is a subset of real numbers that contains no "gaps".  

**Definition:** A subset *I ⊂ ℝ* is called an interval if, given any two elements *x, y ∈ I* with *x < y*, every element z such that x < z < y also belongs to I.  

![Interval](media/interval/interval.png)

### Interval Notation

Given a, b ∈ ℝ with a < b, the following types of intervals are distinguished:

| Interval Type | Notation | Definition |
| :------------ | :------- | :--------- |
| **Closed** | [a, b] | {x ∈ ℝ : a ≤ x ≤ b} |
| **Open** | (a, b) or ]a, b[ | {x ∈ ℝ : a < x < b} |
| **Half-open** | [a, b) | {x ∈ ℝ : a ≤ x < b} |
| **Half-open** | (a, b] | {x ∈ ℝ : a < x ≤ b} |

### Half-lines (Unbounded Intervals)

| Type | Notation | Definition |
| :--- | :------- | :--------- |
| Closed half-line | [a, +∞) | {x ∈ ℝ : x ≥ a} |
| Open half-line | (a, +∞) | {x ∈ ℝ : x > a} |
| Entire real axis | (-∞, +∞) | ℝ |

### Examples of Intervals

A = {x ∈ ℝ : 2 < x < 3}   
![Interval](media/interval/interval_A.png)
**This is an open interval**

B = {x ∈ ℝ : 1 ≤ x < 2 or 6 < x < 7}   
![Interval](media/interval/interval_B.png)
**This is not an interval**  
  
Explanation: Consider **x** belonging to the interval [1, 2), for example 1.5, and **y** belonging to the interval (6, 7), for example 6.3.  
By taking a number **z** greater than 1.5 and less than 6.3, for example 5, we can see that this number does not belong to the set B proposed in the exercise, and therefore B is not an interval.