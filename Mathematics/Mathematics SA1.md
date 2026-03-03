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

![[5.jpg]]
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
- **Vertical Asymptote:** $x = 0$ (since $\cos(0) = 1$, the denominator becomes $0$.
- **$x$-intercept:** None.
- **Endpoint:** When $x = \pi$, $y = \sqrt{\frac{1-1}{1+1}} = 0$. So the graph touches the axis at $(\pi, 0)$.
---

## Problem 8: Cumulative Frequency and Data Analysis

**Tags:** #Statistics #CumulativeFrequency #BoxPlot #Quartiles #Paper2

![[9.jpg]]
![[9 (2).jpg]]
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
### GDC Strategy
Python
```
# Use the List (Stat) editor to check your box plot parameters.
# If you have the raw data, use 1-Variable Statistics to confirm:
# Q1, Med, Q3, MinX, and MaxX.
```
---

## Problem 10: Financial Mathematics (Loans and Sequences)

**Tags:** #Finance #GeometricSequences #Loans #Amortization #GDC #Paper2

![[10.jpg]]
?
### Error Analysis
- **Sequence Misidentification:** In financial problems where interest is added _before_ the payment, the balance follows a specific recurrence relation. Many students mistake this for a simple interest problem or fail to set the final balance to zero.
- **Rounding in Intermediate Steps:** Because the exponent is $1200$, even a small rounding error in the value of $r$ or $k$ leads to a massive discrepancy in the final dollar amount. Always keep the full precision in your GDC.
- **Time Calculation (Part b):** "7 years and 4 months" must be converted correctly to total months ($7 \times 12 + 4 = 88$ payments) to find the remaining balance.
---
### Correct Solution
#### (a) Scenario 1: $p = \$5000$
** (i) Number of payments:**
$10 \text{ years} \times 12 \text{ months/year} = \mathbf{120 \text{ payments}}$.
** (ii) Show that $96k^{120} = \frac{k^{120}-1}{k-1}$:**
The balance $B_n$ after $n$ months is:
$B_n = Ak^n - p(\frac{k^n - 1}{k-1})$.
For the loan to be repaid, $B_{120} = 0$:
$480000k^{120} = 5000(\frac{k^{120}-1}{k-1})$.
Divide both sides by $5000$:
**$96k^{120} = \frac{k^{120}-1}{k-1}$** (as required).
** (iii) Find $r$:**
Using a GDC (Numerical Solver) for the equation above:
$k \approx 1.00388...$.
$1 + \frac{r}{1200} = 1.00388... \implies r \approx 4.66$.
**$r = 4.66\% \text{ (3sf)}$**.
#### (b) Scenario 2: Final Payment after 88 months
** (i) Payments before final:** The scenario says she makes payments of $p$ for 7 years and 4 months.
**$88 \text{ payments}$**.
** (ii) Final payment amount:**
First, find the balance remaining after 88 months ($B_{88}$):
$B_{88} = 480000k^{88} - 5000(\frac{k^{88}-1}{k-1})$.
Using $k$ from part (a): $B_{88} \approx \$157,640.48$.
The final payment includes this balance plus one last month of interest:
Final Payment $= B_{88} \times k \approx 157640.48 \times 1.00388...$.
**Final Payment $\approx \$158,300$ (to 4sf)**.
#### (c) Scenario 3: Increasing payments
Jane pays $p$ for 60 months, then $2p$ for 60 months.
The balance at month 60 ($B_{60}$) becomes the "initial" amount for the next 60 months:
1. $B_{60} = 480000k^{60} - p(\frac{k^{60}-1}{k-1})$.
2. $B_{120} = B_{60}k^{60} - 2p(\frac{k^{60}-1}{k-1}) = 0$.
    Substitute $B_{60}$ into the second equation:
    $480000k^{120} - p(\frac{k^{60}-1}{k-1})k^{60} - 2p(\frac{k^{60}-1}{k-1}) = 0$.
    Solve for $p$ using GDC:
    **$p \approx \$3,439$**.
### GDC Tip
Python
```
# For Financial Math, use the TVM Solver on GDC:
# N = 120
# I% = 4.66
# PV = 480000
# Pmt = -5000
# FV = 0
# P/Y = 12, C/Y = 12
# Always set PV and Pmt with opposite signs (Cash In vs Cash Out).
```
---

## Problem 11: Trigonometric Modeling (Tides)
Tags: #Trigonometry #SineFunctions #Modeling #Tides #Calculus #Paper2Problem Context:

![[11.jpg]]![[11(2).jpg]]
?
### Error Analysis
- **Period vs. $b$ Value:** A common error is setting $b = 12$. The parameter $b$ is related to the period by the formula $b = \frac{2\pi}{\text{Period}}$.
- **Phase Shift ($c$) Confusion:** The value of $c$ represents a horizontal shift. Since the first _high tide_ occurs at $t = 4.5$, and a sine graph reaches its maximum at one-quarter of its period, $c$ is not simply $4.5$. You must account for the nature of the sine wave starting at its principal axis.
- **Unit Consistency:** 04:30 must be converted to decimal hours ($4.5\text{ hours}$) before calculation.
---
### Correct Solution
#### (a) Show that $b = \frac{\pi}{6}$
The time between high tides is $12\text{ hours}$, so the Period $= 12$.
$$b = \frac{2\pi}{12} = \frac{\pi}{6}$$
#### (b) & (c) Find $a$ and $d$
- **Amplitude ($a$):** $\frac{\text{Max} - \text{Min}}{2} = \frac{6.8 - 2.2}{2} = 2.3\text{ m}$.
- **Vertical Shift ($d$):** $\frac{\text{Max} + \text{Min}}{2} = \frac{6.8 + 2.2}{2} = 4.5\text{ m}$.
#### (d) Find the smallest possible value of $c$
A sine wave reaches its maximum at $t = c + \frac{\text{Period}}{4}$.
$$4.5 = c + \frac{12}{4} \implies 4.5 = c + 3$$
$$c = 1.5$$
#### (f) Hours over 24-hour period where $H(t) > 5$
1. Solve $2.3 \sin(\frac{\pi}{6}(t - 1.5)) + 4.5 = 5$ using your GDC.
2. The intersections in the first 12 hours are $t_1 \approx 1.916$ and $t_2 \approx 7.084$.
3. Duration in one cycle $= 7.084 - 1.916 = 5.168\text{ hours}$.
4. Over 24 hours (2 cycles): $5.168 \times 2 \approx 10.3\text{ hours}$.
#### (h) Folkestone Harbour Equation
High tides occur 50 minutes ($50/60 = 5/6\text{ hours}$) earlier. This is a horizontal shift to the left. New $c = 1.5 - \frac{5}{6} \approx 0.667$.
$$H(t) = 2.3 \sin(\frac{\pi}{6}(t - 0.667)) + 4.5$$
#### (i) Show $H(t) = a \sin(bt)\cos(bc) - a \cos(bt)\sin(bc) + d$
Using the identity $\sin(A - B) = \sin A \cos B - \cos A \sin B$:$a \sin(b(t-c)) + d = a [\sin(bt)\cos(bc) - \cos(bt)\sin(bc)] + d$ 
Distributing $a$ yields the required form.
### GDC Strategy
Python
```
# Use the Graph mode to plot H(t).
# Use 'G-Solve' -> 'Intersection' with the line y = 5.
# Ensure your calculator is in RADIAN mode for all trig modeling.
```
---

## Problem 3: Quadratic Properties and Coefficients
**Tags:** #QuadraticFunctions #Symmetry #Intercepts #VertexForm #IBMathAA #Paper1 #Flashcards 

Consider $f(x) = x^2 + bx + c$, for $x \in \mathbb{R}$, where $b, c \in \mathbb{Z}$. The graph of $f$ has a local minimum when $x = 2.5$. The distance between the two $x$-intercepts of the graph of $f$ is $7$.
(a) Find the coordinates of the two $x$-intercepts.
(b) Find the value of $b$ and the value of $c$.
?
### Error Analysis
- **Symmetry Misinterpretation (Part a):** A common mistake is failing to realize that for a quadratic $ax^2 + bx + c$, the local minimum (the vertex) always lies exactly on the axis of symmetry. If the distance between intercepts is $7$, they must be spread equally ($3.5$ units each) from the line $x = 2.5$. Calculating the distance from the origin instead of the symmetry axis leads to incorrect coordinates.
- **Sign Errors in Expansion (Part b):** When using the factored form $f(x) = (x - p)(x - q)$, students often confuse the signs. For an intercept at $x = -1$, the factor is $(x + 1)$. Expanding $(x + 1)(x - 6)$ incorrectly (e.g., getting $+5x$ instead of $-5x$) results in the wrong value for $b$.
- **Coefficient Comparison:** Some may forget that the lead coefficient $a$ is given as $1$. If $a$ were different, the relationship between the roots and $c$ would involve a multiplier ($c = a \cdot x_1 \cdot x_2$).
- **Vieta’s Formulas Confusion:** Forgetting that the sum of roots $x_1 + x_2 = -b/a$. If a student simply adds the roots ($5$) and forgets the negative sign, they incorrectly conclude $b = 5$.
---
### Correct Solution
#### (a) Find the coordinates of the two $x$-intercepts
1. **Identify Symmetry:** The local minimum at $x = 2.5$ implies the axis of symmetry is $x = 2.5$.
2. **Apply Distance:** The distance between intercepts is $7$. Therefore, the intercepts are located $3.5$ units to the left and right of the axis of symmetry ($7 \div 2 = 3.5$).
3. **Calculate Coordinates:**
    - $x_1 = 2.5 - 3.5 = -1$
    - $x_2 = 2.5 + 3.5 = 6$
    - **The coordinates are $(-1, 0)$ and $(6, 0)$.**
#### (b) Find the value of $b$ and the value of $c$
**Method 1: Factored Form Expansion**
1. Using the intercepts found in part (a) and knowing the coefficient of $x^2$ is $1$:
    $$f(x) = (x - (-1))(x - 6)$$
    $$f(x) = (x + 1)(x - 6)$$
2. **Expand the expression:**    $$f(x) = x^2 - 6x + x - 6$$$$f(x) = x^2 - 5x - 6$$
3. **Identify coefficients:**
    - **$b = -5$**
    - **$c = -6$**
Method 2: Vertex/Symmetry Formula
4. The axis of symmetry is given by $x = -\frac{b}{2a}$. Given $x = 2.5$ and $a = 1$:
    $$2.5 = -\frac{b}{2(1)} \implies b = -5$$
5. Substitute one intercept, e.g., $(-1, 0)$, into the function $f(x) = x^2 - 5x + c$:
    $$0 = (-1)^2 - 5(-1) + c$$
    $$0 = 1 + 5 + c \implies c = -6$$
---

## Problem 4: Partial Fractions and Telescoping Series
**Tags:** #Algebra #PartialFractions #TelescopingSeries #Summation #IBMathAA #Paper1 #Flashcards 

(a) Write $\frac{1}{x^2 - x}$ using partial fractions.
(b) Hence evaluate $\frac{1}{1 \times 2} + \frac{1}{2 \times 3} + \frac{1}{3 \times 4} + \dots + \frac{1}{99 \times 100}$.
?
### Error Analysis
- **Conceptual Misunderstanding (Part a):** The student attempted to "complete the square" in the denominator rather than decomposing the expression into partial fractions. While completing the square is useful for integration or finding vertices, partial fraction decomposition requires factoring the denominator into linear terms like $x(x - 1)$.
- **Missing Decomposition Steps:** There was no attempt to set up the identity $\frac{1}{x(x-1)} = \frac{A}{x} + \frac{B}{x-1}$.
- **Inability to Connect Parts (Part b):** Because Part (a) was not solved correctly, the student could not apply the "Hence" instruction. Part (b) relies on using the result from (a) to create a **telescoping series**, where intermediate terms cancel out.
- **Pattern Recognition:** The student failed to recognize that each term in the sum is of the form $\frac{1}{n(n+1)}$, which is the numerical equivalent of the algebraic expression in Part (a) (with a slight sign/variable shift).
---
### Correct Solution
#### (a) Write $\frac{1}{x^2 - x}$ using partial fractions
1. **Factor the denominator:**    $$\frac{1}{x^2 - x} = \frac{1}{x(x - 1)}$$
2. **Set up the partial fraction form:**$$\frac{1}{x(x - 1)} = \frac{A}{x} + \frac{B}{x - 1}$$
3. **Solve for $A$ and $B$:**
    Multiply by $x(x - 1)$: $1 = A(x - 1) + Bx$
    - Let $x = 0 \implies 1 = A(-1) \implies A = -1$
    - Let $x = 1 \implies 1 = B(1) \implies B = 1$
4. **Final Expression:**$$\frac{1}{x^2 - x} = \frac{1}{x - 1} - \frac{1}{x}$$
#### (b) Evaluate $\frac{1}{1 \times 2} + \frac{1}{2 \times 3} + \dots + \frac{1}{99 \times 100}$
1. **Relate to Part (a):** Note that $\frac{1}{n(n+1)}$ can be decomposed using the same logic: $\frac{1}{n(n+1)} = \frac{1}{n} - \frac{1}{n+1}$.
2. **Expand the sum:**
    $$\left( \frac{1}{1} - \frac{1}{2} \right) + \left( \frac{1}{2} - \frac{1}{3} \right) + \left( \frac{1}{3} - \frac{1}{4} \right) + \dots + \left( \frac{1}{99} - \frac{1}{100} \right)$$
3. **Cancel terms (Telescoping):**
    Observe that $-\frac{1}{2} + \frac{1}{2} = 0$, $-\frac{1}{3} + \frac{1}{3} = 0$, and so on. Only the first and last terms remain.
    4. **Final Calculation:**
    $$1 - \frac{1}{100} = \frac{99}{100}$$
    **The sum evaluates to $0.99$.**
    
---

## Problem 6: Polynomial Roots and Arithmetic Sequences

**Tags:** #Polynomials #VietasFormulas #ArithmeticSequences #Algebra #IBMathAA #Paper1 #Flashcards 

Consider the equation $32x^3 - 144x^2 + 214x - 105 = 0$.
(a) Find the sum and product of the roots of this equation in their simplest forms.
(b) The roots of this equation are three consecutive terms of an arithmetic sequence. Taking the roots to be $a-d$, $a$, and $a+d$, solve the equation.
?
### Error Analysis
- **Vieta's Formula Application (Part a):** The student's work shows confusion regarding the coefficients $a_n$ used in Vieta's formulas. The student used $-105$ as the denominator. In Vieta's formulas for a cubic $Ax^3 + Bx^2 + Cx + D = 0$, the denominator must always be the leading coefficient $A$ (which is $32$ here), not the constant term $D$.
- **Sign Errors:** For a cubic equation, the product of the roots is $-\frac{D}{A}$. The student used an incorrect formula or sign convention, leading to a fraction that did not simplify correctly.
- **Algebraic Complexity (Part b):** Because the sum of the roots was calculated incorrectly in part (a), the value for the middle term $a$ (where $3a = \text{sum of roots}$) was incorrect. This led to extremely messy fractions and impossible radicals for $d$.
- **Logical Flow:** The student correctly identified that the sum of $(a-d) + a + (a+d) = 3a$, but used the wrong numerical target for $3a$.
---
## Correct Solution
#### (a) Find the sum and product of the roots
Given $32x^3 - 144x^2 + 214x - 105 = 0$:
1. **Sum of roots:** $\sum \alpha = -\frac{B}{A} = -\frac{-144}{32} = \frac{144}{32}$
    - Simplify: $\frac{144}{32} = \frac{18}{4} = \mathbf{4.5}$ (or $\frac{9}{2}$).
2. **Product of roots:** $\alpha\beta\gamma = -\frac{D}{A} = -\frac{-105}{32} = \mathbf{\frac{105}{32}}$.
#### (b) Solve the equation
1. **Find $a$:**
    The sum of roots is $(a-d) + a + (a+d) = 3a$.
    $$3a = \frac{9}{2} \implies a = \frac{3}{2} = \mathbf{1.5}$$
2. **Find $d$:**
    Using the product of roots: $(a-d)(a)(a+d) = \frac{105}{32}$
    $$a(a^2 - d^2) = \frac{105}{32}$$
    Substitute $a = \frac{3}{2}$:
    $$\frac{3}{2}\left(\frac{9}{4} - d^2\right) = \frac{105}{32}$$
    Multiply by $\frac{2}{3}$: $\frac{9}{4} - d^2 = \frac{105}{32} \cdot \frac{2}{3} = \frac{35}{16}$$$d^2 = \frac{9}{4} - \frac{35}{16} = \frac{36}{16} - \frac{35}{16} = \frac{1}{16}$$$$d = \pm \frac{1}{4}$$
3. **State the roots:**
    - $x_1 = a - d = \frac{3}{2} - \frac{1}{4} = \frac{5}{4}$
    - $x_2 = a = \frac{3}{2}$ (or $\frac{6}{4}$)
    - $x_3 = a + d = \frac{3}{2} + \frac{1}{4} = \frac{7}{4}$
        **The roots are $1.25, 1.5,$ and $1.75$.**
---

## Problem 7: Trigonometry and the Cosine Rule
**Tags:** #Trigonometry #CosineRule #SpecialAngles #Surds #IBMathAA #Paper1

(a) Expand and simplify $(1+\sqrt{3})^2$.
(b) By writing $75^\circ$ as $30^\circ + 45^\circ$, find the value of $\cos 75^\circ$.
(c) In triangle $ABC$, $BC = \sqrt{6}$, $CA = 2$, and $A\hat{C}B = 75^\circ$. Find $AB$ in the form $a + \sqrt{b}$ where $a, b \in \mathbb{Z}$.![[Excalidraw/Drawing 2026-03-03 17.43.25.excalidraw]]
?
### Error Analysis
- **Binomial Expansion (Part a):** The student incorrectly expanded $(1+\sqrt{3})^2$ as $1 + 2\sqrt{3} + 9$. The square of $\sqrt{3}$ is $3$, not $9$. This fundamental error in surd simplification affected the final answer in Part (c).
- **Exact Values (Part b):** While the student correctly used the compound angle identity $\cos(A+B) = \cos A \cos B - \sin A \sin B$, they encountered difficulties in the final simplification. However, the logic here was generally sound compared to the other sections.
- **Law of Cosines Application (Part c):** The student correctly identified the formula $c^2 = a^2 + b^2 - 2ab \cos C$. However, the substitution of the incorrect expansion from Part (a) led to an expression that could not be easily simplified into the required $a + \sqrt{b}$ format.
- **Simplifying Double Radicals:** The student reached a point involving $\sqrt{4 + 2\sqrt{3}}$ but struggled to realize that this is the square root of $(1+\sqrt{3})^2$, which would have reverted the answer to a simpler form.
---
### Correct Solution
#### (a) Expand and simplify $(1+\sqrt{3})^2$
1. Use the identity $(p+q)^2 = p^2 + 2pq + q^2$.
2. $(1)^2 + 2(1)(\sqrt{3}) + (\sqrt{3})^2 = 1 + 2\sqrt{3} + 3$.
3. **Result:** $4 + 2\sqrt{3}$.
#### (b) Find the value of $\cos 75^\circ$
1. $\cos(30^\circ + 45^\circ) = \cos 30^\circ \cos 45^\circ - \sin 30^\circ \sin 45^\circ$.
2. Substitute exact values: $\left(\frac{\sqrt{3}}{2}\right)\left(\frac{\sqrt{2}}{2}\right) - \left(\frac{1}{2}\right)\left(\frac{\sqrt{2}}{2}\right)$.
3. **Result:** $\frac{\sqrt{6} - \sqrt{2}}{4}$.
#### (c) Find $AB$ in the form $a + \sqrt{b}$
1. **Apply Cosine Rule:**
    $$AB^2 = 2^2 + (\sqrt{6})^2 - 2(2)(\sqrt{6}) \cos 75^\circ$$
2. **Substitute values:**
    $$AB^2 = 4 + 6 - 4\sqrt{6} \left(\frac{\sqrt{6} - \sqrt{2}}{4}\right)$$
3. **Simplify the expression:**$$AB^2 = 10 - \sqrt{6}(\sqrt{6} - \sqrt{2})$$$$AB^2 = 10 - (6 - \sqrt{12})$$$$AB^2 = 10 - 6 + 2\sqrt{3} = 4 + 2\sqrt{3}$$
4. **Find $AB$:**
    From part (a), we know $4 + 2\sqrt{3} = (1+\sqrt{3})^2$.$$AB = \sqrt{(1+\sqrt{3})^2}$$
    **$AB = 1 + \sqrt{3}$** (where $a=1, b=3$).
---

## Problem 8: Combinatorics (Arrangements)
**Tags:** #Combinatorics #Permutations #Arrangements #Probability #IBMathAA #Paper1

A coed soccer team consists of 2 boys and 3 girls. They are standing in a line posing for a team picture. Find the number of arrangements such that:
(a) All the boys stand next to each other and all the girls stand next to each other. 
(b) All the boys stand next to each other. 
(c) All the boys are apart and all the girls are apart. (d) Just the boys are apart.
?
### Error Analysis
- **Undercounting Group Permutations (Part a):** The student calculated $2! \times 3! = 12$, but forgot that the two "blocks" (the block of boys and the block of girls) can switch places. There are $2!$ ways to arrange the blocks themselves.
- **Treating Groups as the Whole (Part b):** The student wrote $2! = 2$, which only accounts for the internal arrangement of the boys. They failed to treat the 2 boys as one single "unit" and arrange that unit among the 3 remaining girls.
- **Missing Logic (Parts c & d):** These sections were left blank or incomplete. These require "slotting" or "complementary" logic, which is a common area of difficulty in IB combinatorics.
---
### Correct Solution
#### (a) Boys next to each other AND girls next to each other
1. Treat the boys as one unit $B$ and the girls as one unit $G$.
2. Arrange the units: $2! = 2$ ways ($BG$ or $GB$).
3. Arrange inside the units: Boys internal arrangement ($2!$) and girls internal arrangement ($3!$).
4. **Total:** $2! \times 2! \times 3! = 2 \times 2 \times 6 = \mathbf{24}$.
#### (b) All the boys stand next to each other
1. Treat the 2 boys as one unit. Now you have $1$ unit $+ 3$ individual girls $= 4$ items to arrange.
2. Arrange the 4 items: $4! = 24$ ways.
3. Arrange the boys internally: $2! = 2$ ways.
4. **Total:** $24 \times 2 = \mathbf{48}$.
#### (c) All boys apart AND all girls apart
1. For 2 boys and 3 girls to all be apart, they must alternate.
2. The only possible pattern is **G B G B G**.
3. Arrange the girls in their 3 slots: $3! = 6$ ways.
4. Arrange the boys in their 2 slots: $2! = 2$ ways.
5. **Total:** $6 \times 2 = \mathbf{12}$.
#### (d) Just the boys are apart
1. Use the "slot" method. First, arrange the 3 girls: $3! = 6$ ways.
    - $\text{\_ G \_ G \_ G \_}$
2. There are 4 available slots (indicated by underscores) for the 2 boys.
3. Choose 2 slots for the boys and arrange them: $^4P_2 = 4 \times 3 = 12$ ways.
4. **Total:** $6 \times 12 = \mathbf{72}$.
---

## Problem 9: Transformations and Trigonometric Identities
**Tags:** #Functions #Transformations #Trigonometry #InverseTrig #MathAAHL #Paper1 #Flashcards 

The following diagram shows the graph of $y = \arctan(2x - 3) + \frac{3\pi}{4}$ for $x \in \mathbb{R}$, with asymptotes at $y = \frac{\pi}{4}$ and $y = \frac{5\pi}{4}$.
**(a)** Describe a sequence of transformations that transforms the graph of $y = \arctan x$ to the graph of $y = \arctan(2x - 3) + \frac{3\pi}{4}$ for $x \in \mathbb{R}$.
**(b)** Show that $\arctan p - \arctan q \equiv \arctan\left(\frac{p - q}{1 + pq}\right)$.
?
### Error Analysis
- **Transformation Order (Part a):** You identified a "vertical sketch" (likely meaning stretch) of factor 2. However, the multiplier $2$ is _inside_ the function argument $(2x - 3)$, which indicates a **horizontal stretch/compression**, not vertical. Furthermore, the horizontal shift must be factored out as $2(x - 1.5)$ to see the correct translation of $1.5$ units.
- **Terminology (Part a):** The note "move $3$ units to the right" is incorrect because the horizontal compression affects the shift. The note "move $\frac{3\pi}{4}$ units to the upwards" is conceptually correct but was marked wrong likely due to the previous errors compounding.
- **Proof Logic (Part b):** Your attempt used $\arcsin$ and $\arccos$ expansions. While $\sin(A-B)$ and $\cos(A-B)$ formulas exist, the most direct way to prove an identity involving $\arctan$ is to use the tangent subtraction formula: $\tan(A - B) = \frac{\tan A - \tan B}{1 + \tan A \tan B}$.
---
### Correct Solution
#### (a) Describe a sequence of transformations
To identify the horizontal transformations correctly, we factor the inner expression:
$$y = \arctan(2(x - 1.5)) + \frac{3\pi}{4}$$
The transformations from $y = \arctan x$ are:
1. **Horizontal Stretch** (or compression) by a scale factor of $\frac{1}{2}$ parallel to the x-axis.
2. **Translation** by the vector $\begin{pmatrix} 1.5 \\ \frac{3\pi}{4} \end{pmatrix}$ (or "right by $1.5$ units and up by $\frac{3\pi}{4}$ units").
#### (b) Show that $\arctan p - \arctan q \equiv \arctan\left(\frac{p - q}{1 + pq}\right)$
Let $A = \arctan p$ and $B = \arctan q$. This implies:
$\tan A = p$ and $\tan B = q$.
Using the compound angle formula for tangent:
$$\tan(A - B) = \frac{\tan A - \tan B}{1 + \tan A \tan B}$$
Substitute $p$ and $q$ into the formula:
$$\tan(A - B) = \frac{p - q}{1 + pq}$$
Take the arctangent of both sides:
$$A - B = \arctan\left(\frac{p - q}{1 + pq}\right)$$
Substitute back the original definitions of $A$ and $B$:
$$\arctan p - \arctan q = \arctan\left(\frac{p - q}{1 + pq}\right)$$
---

## Problem 10: Set Theory and Venn Diagrams
**Tags:** #Sets #VennDiagrams #Probability #Logic #MathAAHL #Paper1

![[2f059bc9912a53005d2662d360151d81.jpg]]
?
### Error Analysis
- **Interpreting Region (iii) (Part a):** You wrote $c + e = 8$. However, the problem states "8 eighteen year olds either walk or take the train to school." Looking at the diagram, the 18-year-olds ($E$) who walk or take the train are represented by regions $c$ and $e$. While your equation $c + e = 8$ is correct based on that specific sentence, you likely missed that this is a system of equations where total set values must be balanced.
- **Algebraic Manipulation (Part b/c):** Your scribbles show $2e = 4 \Rightarrow e = 2$. While $e$ does eventually equal 2, the derivation path shown in the margins is a bit disorganized, making it easy to lose track of the "Total Students" constraint ($n(U) = 20$).
- **Probability Calculation (Part e):** You wrote $\frac{2}{20}$, which looks like the probability for a single student. The question asks for the probability that **two** students selected at random both use the same method. This requires considering multiple scenarios (both Walk, both Train, or both Cycle) and using combinations or sequential probability without replacement.
---
### Correct Solution
#### (a) Write down the value of:
- **(i) $b + c = 10$**: These are all students who walk ($W$).
- **(ii) $d + e = 5$**: These are all students who take the train ($T$).
- **(iii) $c + e = 8$**: These are 18-year-olds ($E$) who either walk or take the train.
#### (b) Find a further three equations:
1. **Total students:** $a + b + c + d + e + f = 20$.
2. **17-year-olds total:** $a + b + d = 8$.
3. **18-year-olds total:** $c + e + f = 12$.
#### (c) Show that $a = 1$ and $f = 4$:
Subtract the equation from (a)(iii) from the 18-year-old total:
$(c + e + f) - (c + e) = 12 - 8 \Rightarrow f = 4$.
Since $n(S) = 8$ and $n(E) = 12$, and $n(S \cup E) = 20$, there is no overlap between $S$ and $E$.
Using the total sum: $(a+b+d) + (c+e+f) = 8 + 12 = 20$.
Substitute $b+d = (b+c+d+e) - (c+e) = (10+5) - 8 = 7$.
$a + 7 = 8 \Rightarrow a = 1$.
#### (d) Find the values of $b, c, d, e$:
We are given: "18-year-olds who walk ($c$) is three times 18-year-olds who take the train ($e$)."
1. $c = 3e$
2. Substitute into (a)(iii): $3e + e = 8 \Rightarrow 4e = 8 \Rightarrow \mathbf{e = 2}$.
3. Then $\mathbf{c = 6}$.
4. From (a)(i): $b + 6 = 10 \Rightarrow \mathbf{b = 4}$.
5. From (a)(ii): $d + 2 = 5 \Rightarrow \mathbf{d = 3}$.
#### (e) Probability both use the same method:
First, find the number of students for each method:
- **Walk ($W$):** $b + c = 10$
- **Train ($T$):** $d + e = 5$
- **Cycle ($C$):** $a + f = 1 + 4 = 5$ (those who don't walk or take train)
$P(\text{Same}) = P(WW) + P(TT) + P(CC)$
$$P = \left(\frac{10}{20} \times \frac{9}{19}\right) + \left(\frac{5}{20} \times \frac{4}{19}\right) + \left(\frac{5}{20} \times \frac{4}{19}\right)$$
$$P = \frac{90}{380} + \frac{20}{380} + \frac{20}{380} = \frac{130}{380} = \frac{13}{38}$$
---

## Problem 11: Rational Functions and Asymptotes
**Tags:** #Functions #RationalFunctions #Asymptotes #Calculus #IBMathAAHL #Paper1 #Flashcards 

![[4535c794cd7c1349a9e73ab87422c6d3.jpg]]
?
### Error Analysis
- **Long Division Calculation (Part b-ii):** Your long division shows $(x^2 - 4x + 4) \div (x - 1) = x - 3$ with a remainder of $1$. While the division steps were mostly correct, you missed that the constant term in the numerator is $4$. $x(x-1) = x^2 - x$, leaving $-3x + 4$. Then $-3(x-1) = -3x + 3$. The remainder is $4 - 3 = 1$. The oblique asymptote is the quotient part of this division.
- **Finding the "Gap" in Range (Part c):** You attempted to solve for $k$ where $y=k$ does not intercept the graph. This requires setting the function equal to $k$ and finding the values of $k$ for which the resulting quadratic has no real roots (discriminant $\Delta < 0$).
- **Graph Sketching (Part e):** Without the correct oblique asymptote and the values of $a$ and $b$ (the local maximum and minimum $y$-values), the sketch would lack the necessary boundaries to show where the function exists and where the "gap" is located.
---
### Correct Solution
#### (a) Solve $f(x) = 0$
The function is zero when the numerator is zero:
$x^2 - 4x + 4 = 0 \Rightarrow (x - 2)^2 = 0$.
**Solution:** $x = 2$.
#### (b) Determine the equations of the asymptotes
- **(i) Vertical Asymptote:** Occurs where the denominator is zero.
    **Equation:** $x = 1$.
- **(ii) Oblique Asymptote:** Perform long division:
    $f(x) = (x - 3) + \frac{1}{x - 1}$
    As $x \to \infty$, $\frac{1}{x-1} \to 0$.
    **Equation:** $y = x - 3$.
#### (c) Determine the values of $a$ and $b$
Set $f(x) = k$ and solve for $x$:
$\frac{x^2 - 4x + 4}{x - 1} = k \Rightarrow x^2 - 4x + 4 = kx - k$
$x^2 - (4 + k)x + (4 + k) = 0$.
For no intersection, the discriminant $\Delta < 0$:
$\Delta = (4 + k)^2 - 4(1)(4 + k) < 0$
$(4 + k)(4 + k - 4) < 0 \Rightarrow k(k + 4) < 0$.
This inequality holds for $-4 < k < 0$.
**Values:** $a = -4, b = 0$.
#### (d) Solve the equations
- **(i) $f(x) = -4$**: $x^2 - (4 - 4)x + (4 - 4) = 0 \Rightarrow x^2 = 0 \Rightarrow x = 0$.
- **(ii) $f(x) = 0$**: Already solved in part (a), $x = 2$.
    These represent the $x$-coordinates of the local maximum and minimum points.
#### (e) Sketch the graph
- The graph has two branches.
- One branch stays below $y = -4$ (turning point at $(0, -4)$).
- One branch stays above $y = 0$ (turning point at $(2, 0)$).
- The region $-4 < y < 0$ is empty.
---

## Problem 12: Trigonometric Identities and Cubic Equations
**Tags:** #Trigonometry #CubicFunctions #VietaFormulas #RootsOfEquations #MathAAHL #Paper1 #Flashcards 

![[01eb88622da3c0f7b697556414555d2c.jpg]]
?
### Error Analysis
- **Triple Angle Identity (Part a):** You correctly identified the final form $\cos(3\theta) = 4\cos^3\theta - 3\cos\theta$ in your notes, but a formal proof requires using the compound angle formulas: $\cos(2\theta + \theta) = \cos(2\theta)\cos\theta - \sin(2\theta)\sin\theta$.
- **Root Verification (Part b):** The "Hence" implies using the identity from (a). If $x = \cos k$, then $f(\cos k) = 4\cos^3 k - 3\cos k - \cos(3k)$. By the identity, $4\cos^3 k - 3\cos k = \cos(3k)$, so the expression becomes $\cos(3k) - \cos(3k) = 0$, proving it is a root.
- **Relationship Between Roots (Part c/d):** For a cubic equation $ax^3 + bx^2 + cx + d = 0$, Vieta's formulas state that the sum of roots is $-b/a$. In $f(x) = 4x^3 - 3x - \cos(3k)$, the $x^2$ term is missing ($b=0$), meaning the sum of all three roots ($\alpha + \beta + \cos k$) must be $0$. Your notes didn't explicitly show this connection to solve for $\beta$ in terms of $\alpha$ and $\cos k$.
- **Discriminant and Number of Roots (Part f):** The condition for a cubic to have exactly 2 distinct roots (one single and one repeated) is that its local maximum or minimum must lie exactly on the x-axis. This occurs when the "constant" part of the function aligns with the extremal values of the oscillating part $4x^3 - 3x$.
---
### Correct Solution
#### (a) Show that $\cos(3\theta) = 4\cos^3\theta - 3\cos\theta$
$$\cos(3\theta) = \cos(2\theta + \theta) = \cos(2\theta)\cos\theta - \sin(2\theta)\sin\theta$$
Substitute $\cos(2\theta) = 2\cos^2\theta - 1$ and $\sin(2\theta) = 2\sin\theta\cos\theta$:
$$= (2\cos^2\theta - 1)\cos\theta - (2\sin\theta\cos\theta)\sin\theta$$
$$= 2\cos^3\theta - \cos\theta - 2\sin^2\theta\cos\theta$$
Substitute $\sin^2\theta = 1 - \cos^2\theta$:
$$= 2\cos^3\theta - \cos\theta - 2(1 - \cos^2\theta)\cos\theta$$
$$= 2\cos^3\theta - \cos\theta - 2\cos\theta + 2\cos^3\theta = 4\cos^3\theta - 3\cos\theta$$
#### (b) Verify that $\cos k$ is a root of $f(x)$
$$f(\cos k) = 4\cos^3 k - 3\cos k - \cos(3k)$$
From part (a), $4\cos^3 k - 3\cos k = \cos(3k)$.
Therefore, $f(\cos k) = \cos(3k) - \cos(3k) = 0$.
#### (c) Find $\alpha\beta$ and show $\beta = -\alpha - \cos k$
Using Vieta's formulas for $4x^3 + 0x^2 - 3x - \cos(3k) = 0$:
1. **Sum of roots:** $\alpha + \beta + \cos k = -\frac{0}{4} = 0 \Rightarrow \beta = -\alpha - \cos k$.
2. **Product of roots:** $\alpha \cdot \beta \cdot \cos k = \frac{\cos(3k)}{4} \Rightarrow \alpha\beta = \frac{\cos(3k)}{4\cos k}$.
#### (f) Find values of $k$ for 2 distinct roots
For $f(x)$ to have a repeated root, the local extrema of $y = 4x^3 - 3x$ must be shifted by $\cos(3k)$ to touch the x-axis.
Find stationary points of $g(x) = 4x^3 - 3x$:
$g'(x) = 12x^2 - 3 = 0 \Rightarrow x^2 = \frac{1}{4} \Rightarrow x = \pm \frac{1}{2}$.
The $y$-values at these points are $g(\frac{1}{2}) = 4(\frac{1}{8}) - \frac{3}{2} = -1$ and $g(-\frac{1}{2}) = 1$.
So, we need $\cos(3k) = 1$ or $\cos(3k) = -1$.
- $3k = n\pi \Rightarrow k = \frac{n\pi}{3}$ for $n \in \{0, 1, 2, 3, 4, 5, 6\}$.
    **Values:** $k = 0, \frac{\pi}{3}, \frac{2\pi}{3}, \pi, \frac{4\pi}{3}, \frac{5\pi}{3}, 2\pi$.
---
