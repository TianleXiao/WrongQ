## Problem 1: Functions and Trigonometry
**Tags:** #Functions #Trigonometry #GDC_Skills #Accuracy #SignifantFigures
#Paper2 
### 1. Problem Description
Consider the function $f(x) = x^2 \arcsin(x)$, for $-1 \leq x \leq 1$.
(a) Sketch the graph.
(b) Write down the range.
(c) Solve the inequality $|x^2 \arcsin(x)| > 0.5$.

### 2. Error Analysis
* **Graphing Accuracy:** Failed to label the endpoints $(-1, -1.57)$ and $(1, 1.57)$. In IB, "Sketch" requires key features like endpoints and intercepts to be clear.
* **Precision (SF):** Used 2 significant figures (0.76) instead of the required **3 significant figures** (0.762).
* **Inequality Logic:** Missed the negative region of the absolute value. $|f(x)| > 0.5$ implies $f(x) > 0.5$ OR $f(x) < -0.5$.

### 3. Correct Solution
* **(a) Sketch:** Ensure the curve is flatter at the origin and ends precisely at $x = \pm 1$.
* **(b) Range:** $[-\frac{\pi}{2}, \frac{\pi}{2}]$ or $[-1.57, 1.57]$.
* **(c) Solving:** Use GDC to find intersections with $y = 0.5$ and $y = -0.5$.
    * $x \in [-1, -0.762) \cup (0.762, 1]$

---

## Problem 2: Probability Laws
**Tags:** #Probability #LogicError #Independence_Fallacy #VennDiagram
#Paper2 
### 1. Problem Description
Two events $A$ and $B$ such that $P(A) = 3k$, $P(B) = k$, $P(A \cap B) = \frac{k^2}{2}$, and $P(A \cup B) = 0.78$.
(a) Find the value of $k$.
(b) Find $P(A' \cap B)$.

### 2. Error Analysis
* **The Independence Fallacy:** Incorrectly assumed $P(A \cap B) = P(A)P(B)$. Never assume independence unless the question explicitly states "Events A and B are independent."
* **Mutual Exclusivity Error:** Incorrectly assumed $P(A \cup B) = P(A) + P(B)$. This only works if the events do not overlap.

### 3. Correct Solution
Use the **Inclusion-Exclusion Principle**:
$$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$
Substitute the given terms:
$$0.78 = 3k + k - \frac{k^2}{2}$$
$$0.78 = 4k - 0.5k^2 \implies 0.5k^2 - 4k + 0.78 = 0$$
Solving the quadratic (via GDC):
* $k = 0.2$ (Valid)
* $k = 7.8$ (Reject, as $P(A) = 3k$ would be $> 1$)

For part (b), $P(A' \cap B) = P(B) - P(A \cap B)$.
$$0.2 - \frac{0.2^2}{2} = 0.2 - 0.02 = 0.18$$
---
