## Problem 1: Kinematics and Dynamics of a Curling Stone
**Tags:** #Kinematics #Dynamics #Friction #Mechanics #IBPhysics #Paper2 #Flashcards/IBPhysics/SA1 


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

## Problem 2: Mechanics of a Golf Club Impact
**Tags:** #EnergyTransformation #Momentum #Impulse #ProjectileMotion #IBPhysics #Paper2 #Flashcards/IBPhysics/SA1 

![[Pasted image 20260307132349.png]]![[Pasted image 20260307132359.png]]![[Pasted image 20260307132404.png]]
?
### Error Analysis
- **Impulse Calculation (Part c-i):** Your calculation for force was nearly correct but contained a subtraction error in the momentum change. You used $\Delta p = p_1 - p_2$ instead of final momentum minus initial momentum ($\Delta p = p_f - p_i$) for the ball. The ball starts from rest ($u=0$), so $\Delta p = m_{ball} \times v_{ball}$.  
- **Vector Direction (Part c-ii):** You correctly identified that the magnitude of the force is equal due to Newton's Third Law, but missed the negative sign to indicate the opposite direction.
- **Energy Conservation in Collisions (Part c-iii):** You attempted to use kinetic energy ($E_k = \frac{p^2}{2m}$) to find the final speed of the club head. While valid, the teacher's note "Conservation equation" suggests using the Law of Conservation of Momentum ($m_1u_1 + m_2u_2 = m_1v_1 + m_2v_2$) is the more direct path.
- **Graphing Kinematics (Part d):** In the speed-time graph, you correctly identified that horizontal velocity ($v_x$) is constant (horizontal line). However, for vertical motion ($v_y$), you drew an increasing speed. Since the ball is traveling **upwards** to its maximum height, its vertical speed should **decrease** to zero at $t_1$.
---
### Correct Solution
**(c-i) Calculate the average force acting on the ball**
1. **Change in momentum ($\Delta p$):**
    The ball starts at rest ($u = 0$) and reaches $v = 63 \text{ m/s}$.
    $$\Delta p = m \times \Delta v = 0.045 \times (63 - 0) = 2.835 \text{ kg m s}^{-1} \text{}$$
2. **Calculate Force ($F$):**
    Using $F = \frac{\Delta p}{\Delta t}$ with $\Delta t = 220 \mu s = 220 \times 10^{-6} \text{ s}$.
    $$F = \frac{2.835}{220 \times 10^{-6}} \approx 12,886 \text{ N} \approx 1.29 \times 10^4 \text{ N} \text{}$$
**(c-ii) State the average force acting on the club head**
By Newton’s Third Law, the force is equal in magnitude and opposite in direction.
$$F = -1.29 \times 10^4 \text{ N} \text{}$$
**(c-iii) Calculate the speed of the club head at the instant of separation**
Using Conservation of Momentum:
$$m_{club}u_{club} + m_{ball}u_{ball} = m_{club}v_{club} + m_{ball}v_{ball}$$
$$(0.17 \times 38) + (0.045 \times 0) = (0.17 \times v_{club}) + (0.045 \times 63) \text{}$$
$$6.46 = 0.17v_{club} + 2.835$$
$$3.625 = 0.17v_{club} \implies v_{club} \approx 21.3 \text{ m s}^{-1} \text{}$$
**(d) Draw the speed-time graph ($t=0$ to $t=t_1$)**
- **$v_x$ (Horizontal):** A horizontal line at a constant value, as there is no horizontal acceleration (ignoring air resistance).
- **$v_y$ (Vertical):** A straight line starting from a maximum value at $t=0$ and sloping **downwards** to reach $0$ at $t_1$, representing constant deceleration due to gravity.
---
