## Problem 1: Functions and Trigonometry
**Tags:** #Functions #Trigonometry #GDC_Skills #Accuracy #SignifantFigures #Paper2 #Flashcards #SectionA

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
**Tags:** #Probability #LogicError #Independence_Fallacy #VennDiagram #Paper2 #Flashcards #SectionA

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
#Paper2 #Flashcards #SectionA

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

**Tags:** #Trigonometry #Bearings #CosineRule #SineRule #Paper2 #Geometry #Flashcards #SectionA

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
$$\frac{\sin \alpha}{40} = \frac{\sin 125^\circ}{98.5}$$$$\sin \alpha = \frac{40 \times \sin 125^\circ}{98.5} \approx 0.332...$$
$$\alpha \approx 19.4^\circ$$
The bearing from A to C is the original bearing to B minus this internal angle:
$$\text{Bearing} = 130^\circ - 19.4^\circ = 110.6^\circ$$
#### (c) Find the area of $\triangle ABC$
Use the **Area Formula**: $\text{Area} = \frac{1}{2}ab\sin C$
$$\text{Area} = \frac{1}{2}(70)(40)\sin(125^\circ)$$
$$\text{Area} = 1400 \times 0.819... \approx 1147\text{ km}^2$$
---
## Problem 5: Exponential Functions and Graphing

**Tags:** #Functions #Exponential #Graphing #Intercepts #GDC #Paper2
#SectionA
Let $f(x) = 0.2e^{x+2} - 4$, for $-3 \le x \le 2$.
(a) Sketch the graph of $y = f(x)$ on the grid.
![[Excalidraw/Drawing 2026-02-09 14.08.39.excalidraw]]
(b) Find the coordinates of:
+ (i) The $x$-intercept.
+ (ii) The $y$-intercept.
?
### Error Analysis
- **Domain Misinterpretation:** The sketch failed to respect the restricted domain $-3 \le x \le 2$. An IB "sketch" requires clear endpoints if a domain is specified.
- **Asymptote Neglect:** The horizontal asymptote $y = -4$ was not clearly indicated or approached correctly in the drawing.
- **Calculation/Accuracy Error:** * The $x$-intercept was rounded prematurely to $(1, 0)$. In IB Math, answers should be given to **3 significant figures** (3sf) unless exact.
    - The $y$-intercept was identified as $(0, -3.8)$, but $0.2e^2 - 4 \approx -2.52$. It appears the value $-3.8$ was a visual estimate or a calculator entry error.
---
### Correct Solution
#### (a) Sketching the Graph
To get full marks, your sketch must show:
1. **Correct Shape:** An increasing exponential curve.
2. **Endpoints:** Left: $(-3, f(-3)) \approx (-3, -3.93)$
    - Right: $(2, f(2)) \approx (2, 10.8)$ (Note: This point is off the provided grid, so the curve should exit the top of the grid accurately).
3. **Horizontal Asymptote:** The curve should flatten as it moves left, approaching $y = -4$.
#### (b) Finding the Intercepts
**(i) $x$-intercept:**
Set $f(x) = 0$:
$$0 = 0.2e^{x+2} - 4$$
$$4 = 0.2e^{x+2}$$
$$20 = e^{x+2}$$
$$\ln(20) = x + 2$$
$$x = \ln(20) - 2 \approx 0.996$$
**Coordinates: $(0.996, 0)$**
**(ii) $y$-intercept:**
Set $x = 0$:
$$f(0) = 0.2e^{0+2} - 4$$
$$f(0) = 0.2e^2 - 4$$
$$f(0) \approx 0.2(7.389) - 4$$
$$f(0) \approx 1.478 - 4 = -2.522$$
**Coordinates: $(0, -2.52)$**
---
### GDC Tips for this Problem
- **Table Mode:** Use the table function to find exact values for $x = -3, -2, -1, 0, 1, 2$ before sketching.
- **Zero/Intercept Tools:** Use `Analyze Graph` -> `Zero` to find the $x$-intercept precisely.
---
## Problem 6: Function Properties and Inequalities

**Tags:** #Functions #OddFunctions #Inequalities #RationalFunctions #GDC #Paper2 #SectionA

Consider $f(x) = 2^x - \frac{1}{2^x}$ for $x \in \mathbb{R}$.
(a) Show that $f$ is an odd function.
(b) Solve $f(x) \ge g(x)$ where $g(x) = \frac{x-1}{x^2 - 2x - 3}$.
?
### Error Analysis
- **Notation and Logic (Part a):** You correctly identified the symmetry, but the concluding statement "$f(x) = f(-x)$" describes an **even** function. For an **odd** function, you must show $f(-x) = -f(x)$.
- **Inequality Boundary Errors (Part b):**
    - **Asymptote Neglect:** When solving $f(x) \ge g(x)$, you must consider the vertical asymptotes of $g(x)$. The function $g(x)$ is undefined at $x = -1$ and $x = 3$.
    - **Region Selection:** You missed the interval where the curve $f(x)$ is above $g(x)$ between the vertical asymptotes.    
    - **Rounding:** The intersection point was written as $0.18$, but the exactness of the intervals is crucial in IB Paper 2.
---
### Correct Solution
#### (a) Show that $f$ is an odd function
To show a function is odd, we must prove $f(-x) = -f(x)$.
1. Find $f(-x)$:    $$f(-x) = 2^{-x} - \frac{1}{2^{-x}} = \frac{1}{2^x} - 2^x$$
2. Factor out a negative sign:
    $$f(-x) = -(2^x - \frac{1}{2^x})$$
3. Therefore:$$f(-x) = -f(x)$$
    Hence, $f$ is an **odd function**.
#### (b) Solve $f(x) \ge g(x)$
1. **Identify Critical Values:**
    - **Intersections (from GDC):** $x \approx -1.27, x \approx 0.183, x \approx 3.06$.
    - **Vertical Asymptotes (of $g(x)$):** Solve $x^2 - 2x - 3 = 0 \implies (x-3)(x+1)=0$. So, $x = -1$ and $x = 3$.
2. **Test Intervals:** Look at the graph to see where the line for $f(x)$ is "higher" than the curve for $g(x)$.
3. **Solution Set:**    $$-1.27 \le x < -1 \quad \text{or} \quad 0.183 \le x < 3 \quad \text{or} \quad x \ge 3.06$$
    _(Note: Use $<$ for asymptotes because the function is undefined there, and $\le$ for intersection points.)
---
## Problem 7: Composite and Inverse Functions

**Tags:** #Functions #InverseFunctions #RangeAndDomain #Trigonometry #GDC #Paper2 #SectionA

A function $g$ is defined by $g(x) = \arccos\left(\frac{x^2 - 1}{x^2 + 1}\right), x \in \mathbb{R}, x \ge 0$.
(a) Find the range of $g$.
(b) Find an expression for $g^{-1}(x)$.
(c) State the domain of $g^{-1}(x)$.
(d) Sketch the graph of $y = g^{-1}(x)$, indicating asymptotes and intercepts.
?
### Error Analysis
- **Range Misunderstanding (Part a):** The range of $y = \arccos(u)$ is $[0, \pi]$. You indicated $y \ge \pi$, which is outside the possible output of the arccosine function.
- **Inverse Algebra (Part b):** Your attempt swapped the function name but didn't solve for $x$. To find an inverse, you must swap $x$ and $y$ and then isolate $y$.
- **Domain Relationship (Part c):** While you correctly stated that "the domain of $g^{-1}$ is the range of $g$," the numerical value was incorrect because the range in part (a) was wrong.
- **Graphing Error (Part d):** The sketch showed a bell-shaped curve. Since $g(x)$ is strictly increasing for $x \ge 0$, its inverse $g^{-1}(x)$ must also be strictly increasing.
---
### Correct Solution
#### (a) Find the range of $g$
Consider the inner function $f(x) = \frac{x^2 - 1}{x^2 + 1}$.
- When $x = 0$, $f(0) = -1$.
- As $x \to \infty$, $f(x) \to 1$.
- Therefore, the input to $\arccos$ ranges from $[-1, 1)$.
- $\arccos(-1) = \pi$ and $\arccos(1) = 0$.
    **Range:** $0 < y \le \pi$.
#### (b) Find an expression for $g^{-1}(x)$
1. Set $x = \arccos\left(\frac{y^2 - 1}{y^2 + 1}\right)$.
2. Take the cosine of both sides: $\cos(x) = \frac{y^2 - 1}{y^2 + 1}$.
3. Multiply through: $y^2\cos(x) + \cos(x) = y^2 - 1$.
4. Rearrange to isolate $y^2$: $1 + \cos(x) = y^2(1 - \cos(x))$.
5. $y^2 = \frac{1 + \cos(x)}{1 - \cos(x)}$.
    **$g^{-1}(x) = \sqrt{\frac{1 + \cos(x)}{1 - \cos(x)}}$** (Note: only the positive root as $x \ge 0$).
#### (c) State the domain of $g^{-1}(x)$
The domain of the inverse is the range of the original function.
**Domain:** $0 < x \le \pi$.
#### (d) Sketch the graph of $y = g^{-1}(x)$
- **Vertical Asymptote:** $x = 0$ (since $\cos(0) = 1$, the denominator becomes $0$).
- **$x$-intercept:** None.
- **Endpoint:** When $x = \pi$, $y = \sqrt{\frac{1-1}{1+1}} = 0$. So the graph touches the axis at $(\pi, 0)$.
---
## Problem 8: Cumulative Frequency and Data Analysis

**Tags:** #Statistics #CumulativeFrequency #BoxPlot #Quartiles #Paper2
A study of 80 Uber drivers in San Francisco records the distance traveled in April. 
(a) Find the number of drivers who traveled between $3200$ and $5000$ km. 
(b) Find the median, lower quartile ($Q_1$), and upper quartile ($Q_3$). 
(c) Find the Interquartile Range (IQR). 
(d) Write down the percentage of drivers traveling more than $Q_3$. 
(e) Find the number of drivers who traveled $\le 2750$ km. 
(f) Find $m$ if 11 drivers traveled more than $m$ km. 
(g) Draw a box-and-whisker diagram.
?
### Error Analysis
- **Graph Reading Precision:** On cumulative frequency curves, small deviations in reading the $x$-axis lead to significant errors in the frequency ($y$-axis). For example, in part (e), $2750$ km must be mapped precisely to the curve.
- **Percentage vs. Count:** In part (d), the question asks for a **percentage**. Since $Q_3$ is the 75th percentile, $25\%$ of the data always lies above it, regardless of the total frequency.
- **Inverse Reading (Part f):** To find $m$ where 11 drivers traveled more than $m$, you must look for the value at $80 - 11 = 69$ on the cumulative frequency axis, then find the corresponding $x$.
- **Box Plot Scale:** Part (g) explicitly requires a scale of $2\text{ cm}$ to $1000\text{ km}$. Failure to use this specific scale on graph paper results in a loss of all marks for that section.
---
### Correct Solution

#### (a) Drivers between $3200$ and $5000$ km
1. At $x = 5000$, $y = 78$ (approx).
2. At $x = 3200$, $y = 50$ (approx).
3. **Number of drivers:** $78 - 50 = 28$.
#### (b) Quartiles
1. **Median ($M$):** $50\%$ of $80 = 40$. Read from $y=40 \implies x \approx 2800\text{ km}$.
2. **Lower Quartile ($Q_1$):** $25\%$ of $80 = 20$. Read from $y=20 \implies x \approx 2200\text{ km}$.
3. **Upper Quartile ($Q_3$):** $75\%$ of $80 = 60$. Read from $y=60 \implies x \approx 3600\text{ km}$.
#### (c) Interquartile Range (IQR)
$$IQR = Q_3 - Q_1 = 3600 - 2200 = 1400\text{ km}$$
#### (d) Percentage above $Q_3$
By definition, the upper quartile is the 75th percentile.
**Percentage:** $100\% - 75\% = 25\%$.
#### (e) Drivers $\le 2750$ km
Read from $x = 2750$ up to the curve and across to the $y$-axis.
**Number of drivers:** $\approx 38$.
#### (f) Find $m$ for 11 drivers $> m$
1. Cumulative frequency $= 80 - 11 = 69$.
2. Find $y = 69$ on the graph and read the corresponding $x$.
    **$m \approx 4100\text{ km}$**.
#### (g) Box-and-Whisker Diagram
- **Endpoints:** Whiskers should go from $500$ to $6000$ km.
- **Box:** Ends at $2200$ ($Q_1$) and $3600$ ($Q_3$).
- **Median:** Vertical line inside the box at $2800$.
---
