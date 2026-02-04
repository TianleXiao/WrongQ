## Problem 1: Functions and Trigonometry 
**Tags:** #Functions #Trigonometry #GDC_Skills #Accuracy #SignifantFigures #Paper2 #Flashcards
### 1. Problem Description
Consider the function $f(x) = x^2 \arcsin(x)$, for $-1 \leq x \leq 1$.
(a) Sketch the graph.
(b) Write down the range.
(c) Solve the inequality $|x^2 \arcsin(x)| > 0.5$.
?
### 2. Error Analysis
* **Graphing Accuracy:** Failed to label the endpoints $(-1, -1.57)$ and $(1, 1.57)$. In IB, "Sketch" requires key features like endpoints and intercepts to be clear.
* **Precision (SF):** Used 2 significant figures (0.76) instead of the required **3 significant figures** (0.762).
* **Inequality Logic:** Missed the negative region of the absolute value. $|f(x)| > 0.5$ implies $f(x) > 0.5$ OR $f(x) < -0.5$.
---
### 3. Correct Solution
* **(a) Sketch:** Ensure the curve is flatter at the origin and ends precisely at $x = \pm 1$.
* **(b) Range:** $[-\frac{\pi}{2}, \frac{\pi}{2}]$ or $[-1.57, 1.57]$.
* **(c) Solving:** Use GDC to find intersections with $y = 0.5$ and $y = -0.5$.
    * $x \in [-1, -0.762) \cup (0.762, 1]$
---

## Problem 2: Probability Laws
**Tags:** #Probability #LogicError #Independence_Fallacy #VennDiagram #Paper2 #Flashcards
### 1. Problem Description
Two events $A$ and $B$ such that $P(A) = 3k$, $P(B) = k$, $P(A \cap B) = \frac{k^2}{2}$, and $P(A \cup B) = 0.78$.
(a) Find the value of $k$.
(b) Find $P(A' \cap B)$.
?
### 2. Error Analysis
* **The Independence Fallacy:** Incorrectly assumed $P(A \cap B) = P(A)P(B)$. Never assume independence unless the question explicitly states "Events A and B are independent."
* **Mutual Exclusivity Error:** Incorrectly assumed $P(A \cup B) = P(A) + P(B)$. This only works if the events do not overlap.
---
### 3. Correct Solution
Use the **Inclusion-Exclusion Principle**:
$$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$
Substitute the given terms:
$$0.78 = 3k + k - \frac{k^2}{2}$$
$$0.78 = 4k - 0.5k^2 \implies 0.5k^2 - 4k + 0.78 = 0$$
Solving the quadratic (via GDC):
* $k = 0.2$ (Valid)
* $k = 7.8$ (Reject, as $P(A) = 3k$ would be $> 1$)
<!--SR:!2026-02-05,1,230-->

For part (b), $P(A' \cap B) = P(B) - P(A \cap B)$.
$$0.2 - \frac{0.2^2}{2} = 0.2 - 0.02 = 0.18$$
---

## Problem 3: Exponential Functions and Modeling
**Tags:** #Functions #Exponential_Models #GDC_Skills #IB_Presentation
#Paper2 
## 1. Problem Description
The mass $m(t)$ (in nanograms) of radioactive carbon in a plant fossil after $t$ years is modeled by the function:
$$m(t) = 120e^{-0.000121t}$$

(a) Write down the initial mass of the radioactive carbon.  
(b) Find the mass of the radioactive carbon after 20,000 years.  
(c) Calculate the smallest number of complete years it takes for more than half the sample to decay.

## 2. Error Analysis
* **Missing Visual Evidence:** I failed to provide a sketch of the graph when using the GDC to solve part (c). In IB Math Paper 2, showing the GDC screen logic is often required for method marks. 
    * *Examiner Note:* "I don't see any graph."
* **Calculation Incompleteness:** In part (b), I correctly substituted the values but failed to write down the final numerical result. 
* **Precision/Rounding:** I did not reach the final 3 Significant Figures (SF) requirement for the numerical parts of the question.

## 3. Correct Solution

### (a) Initial Mass
When $t = 0$:
$$m(0) = 120e^0 = 120 \text{ ng}$$

### (b) Mass after 20,000 years
$$m(20000) = 120e^{-0.000121 \times 20000}$$
Using GDC: 
**$m \approx 10.7$ ng** (to 3 significant figures).

### (c) Solving for Decay Time
To find when more than half has decayed, the remaining mass must be less than 60 ($120 \div 2$):
$$120e^{-0.000121t} < 60$$

**GDC Method:**
1. Plot $y_1 = 120e^{-0.000121x}$ and $y_2 = 60$.
2. Find the intersection point using the `Intersect` tool.
3. $t \approx 5728.48...$

**Final Answer:**
Since we need the "smallest number of **complete years**" for the decay to exceed 50%, we round up to the next integer:
**$t = 5729$ years.**
## 4. Preventive Actions (Checklist)
* [ ] **GDC Sketch:** Always draw a small, labeled sketch of the GDC screen (showing the intersection) to justify the answer in Paper 2.
* [ ] **Completion Check:** Ensure every calculation leads to a final numerical value—never leave an expression as the final answer.
* [ ] **Round Wisely:** Pay attention to keywords like "complete years" which usually imply an integer answer, otherwise default to 3 SF.
---
