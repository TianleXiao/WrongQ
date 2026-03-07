## Problem 1: Kinematics and Dynamics of a Curling Stone
**Tags:** #Kinematics #Dynamics #Friction #Mechanics #IBPhysics #Paper2
![[Pasted image 20260307130850.png]]
?

### Error Analysis
- **Calculation Success (Part a):** Your calculation for the maximum speed was correct. You accurately used the area under the speed-time graph (the sum of two triangles) to set up the equation $29.8 = \frac{1}{2}(3.5)v + \frac{1}{2}(17.5 - 3.5)v$.
- **Missing Analysis (Part b):** The second part of the question was left blank. To solve for the coefficient of friction, you need to link the **deceleration** of the stone to the **frictional force** acting on it.
- **Conceptual Link:** You must recognize that during the "coasting" phase (from $3.5\text{ s}$ to $17.5\text{ s}$), the only horizontal force is friction ($F_f = \mu_k R$). By Newton's Second Law ($F = ma$), this allows you to solve for $\mu_k$.
---
### Correct Solution
**(a) Find the maximum speed $v$**
The total distance is the area under the $v-t$ graph:
$$s = \text{Area}_1 + \text{Area}_2$$
$$29.8 = \frac{1}{2}(3.5)(v) + \frac{1}{2}(17.5 - 3.5)(v)$$
$$29.8 = 1.75v + 7.0v = 8.75v$$
$$v = \frac{29.8}{8.75} \approx 3.41 \text{ m/s}$$
**(b) Find the coefficient of dynamic friction $\mu_k$**
1. **Calculate acceleration ($a$) during the final $14.0\text{ s}$:**
    The stone slows from $3.41\text{ m/s}$ to $0\text{ m/s}$ in $14.0\text{ s}$.
    $$a = \frac{\Delta v}{\Delta t} = \frac{0 - 3.41}{14.0} = -0.2436 \text{ m/s}^2$$
2. **Relate acceleration to friction:**
    The resultant force $F_{net} = ma$. On a horizontal surface, $F_{net} = -F_f$ and the normal reaction force $R = mg$.
    $$- \mu_k mg = ma$$
    $$\mu_k = \frac{-a}{g}$$
3. **Solve for $\mu_k$:**
    Using $g = 9.81 \text{ m/s}^2$:
    $$\mu_k = \frac{0.2436}{9.81} \approx 0.0248$$
---
