## Problem 1: Functions and Trigonometry
**Tags:** #Functions #Trigonometry #GDC_Skills #Accuracy #SignifantFigures #Paper2 #Flashcards

Consider the function $f(x) = x^2 \arcsin(x)$, for $-1 \leq x \leq 1$.
(a) Sketch the graph.
(b) Write down the range.
(c) Solve the inequality $|x^2 \arcsin(x)| > 0.5$.
?
### Error Analysis
* **Graphing Accuracy:** Failed to label the endpoints $(-1, -1.57)$ and $(1, 1.57)$. In IB, "Sketch" requires key features like endpoints and intercepts to be clear.
* **Precision (SF):** Used 2 significant figures (0.76) instead of the required **3 significant figures** (0.762).
* **Inequality Logic:** Missed the negative region of the absolute value. $|f(x)| > 0.5$ implies $f(x) > 0.5$ OR $f(x) < -0.5$.
---
### Correct Solution
* **(a) Sketch:** Ensure the curve is flatter at the origin and ends precisely at $x = \pm 1$.
  ![[Excalidraw/Drawing 2026-02-04 21.11.05.excalidraw]]**Reference:**![[Pasted image 20260204212525.png]]
* **(b) Range:** $[-\frac{\pi}{2}, \frac{\pi}{2}]$ or $[-1.57, 1.57]$.
* **(c) Solving:** Use GDC to find intersections with $y = 0.5$ and $y = -0.5$.
    * $x \in [-1, -0.762) \cup (0.762, 1]$
---


## Problem 2: Probability Laws
**Tags:** #Probability #LogicError #Independence_Fallacy #VennDiagram #Paper2 #Flashcards

Two events $A$ and $B$ such that $P(A) = 3k$, $P(B) = k$, $P(A \cap B) = \frac{k^2}{2}$, and $P(A \cup B) = 0.78$.
(a) Find the value of $k$.
(b) Find $P(A' \cap B)$.
?
### Error Analysis
* **The Independence Fallacy:** Incorrectly assumed $P(A \cap B) = P(A)P(B)$. Never assume independence unless the question explicitly states "Events A and B are independent."
* **Mutual Exclusivity Error:** Incorrectly assumed $P(A \cup B) = P(A) + P(B)$. This only works if the events do not overlap.
---
### Correct Solution
Use the **Inclusion-Exclusion Principle**:
$$P(A \cup B) = P(A) + P(B) - P(A \cap B)$$
Substitute the given terms:
$$0.78 = 3k + k - \frac{k^2}{2}$$
$$0.78 = 4k - 0.5k^2 \implies 0.5k^2 - 4k + 0.78 = 0$$
Solving the quadratic (via GDC):
* $k = 0.2$ (Valid)
* $k = 7.8$ (Reject, as $P(A) = 3k$ would be $> 1$
---
For part (b), $P(A' \cap B) = P(B) - P(A \cap B)$.
$$0.2 - \frac{0.2^2}{2} = 0.2 - 0.02 = 0.18$$
---


## Problem 3: Exponential Functions and Modeling
**Tags:** #Functions #Exponential_Models #GDC_Skills #IB_Presentation
#Paper2 #Flashcards

The mass $m(t)$ (in nanograms) of radioactive carbon in a plant fossil after $t$ years is modeled by the function:
$$m(t) = 120e^{-0.000121t}$$
(a) Write down the initial mass of the radioactive carbon.
(b) Find the mass of the radioactive carbon after 20,000 years.
(c) Calculate the smallest number of complete years it takes for more than half the sample to decay.
?
### Error Analysis
* **Missing Visual Evidence:** I failed to provide a sketch of the graph when using the GDC to solve part (c). In IB Math Paper 2, showing the GDC screen logic is often required for method marks.
    * *Examiner Note:* "I don't see any graph."
* **Calculation Incompleteness:** In part (b), I correctly substituted the values but failed to write down the final numerical result.
* **Precision/Rounding:** I did not reach the final 3 Significant Figures (SF) requirement for the numerical parts of the question.
---
### Correct Solution
#### (a) Initial Mass
When $t = 0$:
$$m(0) = 120e^0 = 120 \text{ ng}$$
#### (b) Mass after 20,000 years
$$m(20000) = 120e^{-0.000121 \times 20000}$$
Using GDC:
**$m \approx 10.7$ ng** (to 3 significant figures).
#### (c) Solving for Decay Time
To find when more than half has decayed, the remaining mass must be less than 60 ($120 \div 2$):
$$120e^{-0.000121t} < 60$$
**GDC Method:**
1. Plot $y_1 = 120e^{-0.000121x}$ and $y_2 = 60$.
2. Find the intersection point using the `Intersect` tool.
3. $t \approx 5728.48...$
**Final Answer:**
Since we need the "smallest number of **complete years**" for the decay to exceed 50%, we round up to the next integer:
**$t = 5729$ years.**
---
#### 4. Preventive Actions (Checklist)
* [ ] **GDC Sketch:** Always draw a small, labeled sketch of the GDC screen (showing the intersection) to justify the answer in Paper 2.
* [ ] **Completion Check:** Ensure every calculation leads to a final numerical value—never leave an expression as the final answer.
* [ ] **Round Wisely:** Pay attention to keywords like "complete years" which usually imply an integer answer, otherwise default to 3 SF.
---

## Problem 4: Bearings and Triangle Trigonometry

**Tags:** #Trigonometry #Bearings #CosineRule #SineRule #Paper2 #Geometry #Flashcards

City B is $70\text{ km}$ from A on a bearing of $130^\circ$. City C is $40\text{ km}$ from B on a bearing of $75^\circ$.
![[Excalidraw/Drawing 2026-02-09 13.53.43.excalidraw]]
(a)  Find the distance from City A to C.
(b)) If you wanted to travel rom city A directly to City C, find the bearing you would need to travel.
(c)  Find the area enclosed by connecting the three cities in a triangle ABC.
?

### Error Analysis

- **Data Transcription Error:** In the original attempt, the distance $BC$ was taken as $10$ instead of $40\text{ km}$ (as circled in the question). This led to an incorrect value for $AC$.
    
- **Angle Miscalculation:** The angle used in the Cosine Rule was $130^\circ$. However, $\angle ABC$ must be calculated using the geometry of parallel lines (North lines). The interior angle is actually $125^\circ$.
    
- **Bearing Logic:** For part (b), the bearing is not just the internal angle of the triangle; it is the clockwise angle from the North line at A to the line AC.
---
### Correct Solution

#### (a) Find the distance $AC$

First, calculate the included angle $\angle ABC$:

- The bearing from A to B is $130^\circ$. By the property of parallel lines (alternate interior angles), the angle from B's South-to-North line back toward A is $180^\circ - 130^\circ = 50^\circ$.
    
- Adding the bearing from B to C ($75^\circ$): $\angle ABC = 50^\circ + 75^\circ = 125^\circ$.
    

Apply the **Cosine Rule**:

$$AC^2 = 70^2 + 40^2 - 2(70)(40)\cos(125^\circ)$$

$$AC^2 = 4900 + 1600 - 5600(-0.5735...)$$

$$AC = \sqrt{9711.6...} \approx 98.5\text{ km}$$

#### (b) Find the bearing from A to C

Use the **Sine Rule** to find the internal angle $\angle BAC$ (let's call it $\alpha$):

$$\frac{\sin \alpha}{40} = \frac{\sin 125^\circ}{98.5}$$

$$\sin \alpha = \frac{40 \times \sin 125^\circ}{98.5} \approx 0.332...$$

$$\alpha \approx 19.4^\circ$$

The bearing from A to C is the original bearing to B minus this internal angle:

$$\text{Bearing} = 130^\circ - 19.4^\circ = 110.6^\circ$$

#### (c) Find the area of $\triangle ABC$

Use the **Area Formula**: $\text{Area} = \frac{1}{2}ab\sin C$

$$\text{Area} = \frac{1}{2}(70)(40)\sin(125^\circ)$$

$$\text{Area} = 1400 \times 0.819... \approx 1147\text{ km}^2$$
---
