---
id: 20260329014846
aliases: []
tags:
  - uncataloged
created: 2026-03-29 01:48
status: draft
---
# Sears chapter 5 problems

## Problem 5.74
 A window washer pushes his scrub brush up a vertical window at constant speed by applying a force $\vec{F}$ as shown in Fig. P5.74. The brush weighs $15.0 N$ and the coefficient of kinetic friction is $\mu_{k} =0.150$. Calculate (a) the magnitude of the force  and (b) the normal force exerted by the window on the brush.
 ![Pasted image 20260329015942](assets/Pasted%20image%2020260329015942.png)
### Solution
The brush is pushed up with constant speed, that means that no acceleration is present and thus we will have to use Newton's First Law equations. Our target variables are: (a) magnitude of force $\vec{F}$ and normal force $\vec{n}$. We'll need two equations for these.

Let's first make our Free Body Diagram.

Let's use define the component net forces:
$$
\begin{align}
\sum F_{x} &= -(F\cos(53.1)) + n = 0  \tag{1} \\
\sum F_{y} &= -(w)- (f_{k})+ F\sin{53.1} = 0  \tag{2}
\end{align}
$$
We also now that:
$$
\begin{align}
f_{k}  & = \mu_{k}n = 0.150n \tag{3}
\end{align}
$$
We have three equations and three unknown variables, it should be enough. Let's start executing the math now.
 From (1) and (3), we get:
 $$
 \begin{align}
 f_{k}  & = 0.150F\cos(53.1) \tag{4}
 \end{align}
 $$
 We replace $f_{k}$ in (2) with this expression and solve for F:
 $$
 \begin{align}
\sum F_{y} &= -(w)-(0.150F\cos{53.1}) + F\sin{53.1} = 0  \\
F  & = \frac{w}{(-0.150\cos{53.1} + \sin{53.1})}  \\
F  & = 21.14N \tag{5}
 \end{align}
 $$
 With (5), we solve for $n$ on (1):
 $$
 \begin{align}
n &= F\cos(53.1) \\
n &= 12.69N \\
 \end{align}
 $$
We then have that the magnitude of the force $\vec{F}$ is 21.14N and the magnitude of the normal force $\vec{n}$ is 12.69N.

## Problem 5.84
If the coefficient of static friction between a table and a uniform massive rope is $\mu_{s}$ what fraction of the rope can hang over the edge of the table without the rope sliding?
### Solution
This problems happens when the rope is static, so we'll use Newton's First Law. But, we'll need to differentiate bettween the hanging section of the rope and the fraction that is over the table. We'll need to solve for the fraction of the rope (fraction of the weight) and thus find a relationship between $m_{1}$ and $m_{2}$.

Let's start drawing the free body diagrams for both sections.

We can see that the first section is affected by the static frictional force $f_{s}$. We'll need to work with the maximum value of this force in order to find the fraction of the rope that can hang without the frictional force switching to its kinetic coefficient. So, we'll work with:
$$
\begin{align}
f_{s_{max}} = \mu_{s}n \tag{1}
\end{align}
$$
Now, defining the newton's first law component equations for the first section of the rope, we get:
$$
\begin{align}
\sum F_{x}  & = -f_{s_{max}} + T = 0 \tag{2} \\
\sum F_{y}  & = n - w_{1} = 0 \tag{3}
\end{align}
$$
From (3), we get that $n = m_{1}g$  and thus pairing it with (1), we also have $f_{s_{max}} = \mu_{s}m_{1}g$. Finally, we can replace this expression of $f_{s_{max}}$ into (2), obtaining $T = \mu_{s}m_{1}g$.
Now, let's define the same newton's equations for the hanging section:
$$
\begin{align}
\sum F_{x}  & = 0 \\
\sum F_{y}  & = T - w_{2} =  0 \tag{4}
\end{align}
$$
This is just what we needed to correlate $m_{1}$ and $m_{2}$. We can replace the expression we deduced for $T$ into (4):
$$
\begin{align}
T  & = m_{2}g  \\
\mu_{s}m_{1}g  & = m_{2}g \\
m_{1}  & = \frac{m_{2}}{\mu_{s}} \tag{5}
\end{align}
$$
We then have that $m_{1}$ (the fraction of the rope that should be over the table) should be larger than $m_{2}$ (the fraction hanging) to avoid sliding. This makes sense. Specifically, $m_{2}$ shorter than $m_{1}$ by a factor of $\mu_{s}$.

Let's expand this. The net mass of the rope is $m = m_{1} + m_{2}$. The fraction that hangs is then $\frac{m_{2}}{m}$. Then:
$$
\begin{align}
\frac{m_{2}}{m}  & = \frac{\mu_{s}m_{1}}{m} = \frac{\mu_{s}m_{1}}{m_{1} + \mu_{s}m_{1}} = \frac{\mu_{s}}{1 + \mu_{s}}
\end{align}
$$
Then the fraction of the rope hanging in terms of frictional coefficient is $\frac{\mu_{s}}{1 + \mu_{s}}$. As $\mu_{s}$ goes to 0, the fraction of the rope that can hang before sliding is 0. Conversely, as $\mu_{s} \rightarrow \infty$, the fraction of the rope that can hang approaches the unity.
### Differentiating between massless and massive rope
You have hit on a fantastic and very insightful question! Your intuition is completely correct: because the rope has mass, the tension is **not** uniform throughout its entire length.

However, your solution is still **100% mathematically correct**. Here is why you can use a single $T$ in your equations, even though the rope is massive.

### The Secret of the Boundary Point

When you divided the rope into mass $m_1$ (on the table) and mass $m_2$ (hanging), you implicitly cut the system into two pieces right at the corner of the table.

The $T$ in your equations does not represent the tension of the _whole_ rope. It represents the tension at **one exact, infinitesimal point**: the boundary where $m_1$ meets $m_2$.

Because you are looking at a single point connecting the two sections, Newton's Third Law (action-reaction) applies. The hanging section pulls the table section toward the edge with a force of $T$, and the table section pulls the hanging section up with that exact same force $T$.

### How Tension Actually Varies in the Rope

If you were to look inside the rope, here is what is actually happening to the tension at different points:

**1. The Hanging Section ($m_2$)**

- At the very **bottom end** of the hanging rope, there is no mass below it to support. Therefore, the tension is $0$.
    
- As you move up the rope, the tension increases because it has to support the weight of the rope beneath it.
    
- Right at the **top** of the hanging section (at the edge of the table), the tension has to support the entire weight of $m_2$. This is why, exactly at the corner, $T = m_2g$.
    

**2. The Section on the Table ($m_1$)**

- At the very **far left end** of the rope on the table, there is nothing pulling it, so the tension is $0$.
    
- As you move right, towards the edge of the table, the tension increases to counteract the cumulative static friction of the rope behind it.
    
- Right at the **edge** of the table, the tension reaches its maximum value to pull the entire mass $m_1$ against maximum static friction. This is why, exactly at the corner, $T = \mu_s m_1g$.
    

### Summary

By splitting the rope into $m_1$ and $m_2$, you effectively treated the problem like two solid blocks connected by a microscopic, massless string right at the corner of the table. Because you only needed to analyze the forces at that specific boundary to link the two systems, setting the two $T$'s equal to each other was the perfect way to solve it.

## Problem 5.95
Two objects with masses 5.00 kg and 2.00 kg hang 0.600 m above the floor from the ends of a cord 6.00 m long passing over a frictionless pulley. Both objects start from rest. Find the maximum height reached by the 2.00-kg object.
### Solution
Here we're given a system in which acceleration immediately starts occurring. There will be vertical acceleration and hence we'll use newton's second law equations. Our target variables are the acceleration of the system and the maximum height reached by the 2kg object.

Let's start denoting the 5kg mass as $m_A$ and the 2kg mass as $m_{B}$. Let's draw their free body diagrams.

We have third states in this system:
- First:  $m_{A}$ is moving downwards and hasn't reached the floor. Thus, $m_{B}$ is moving upwards and has positive acceleration.
- Second: $m_{A}$ has just reached the floor, $m_{B}$ has accumulated velocity but starts having negative acceleration ($-g$) because of its weight, slowing down its velocity.
- Third: $m_{B}$ reaches velocity 0 and starts free falling and thus declining in height. This is where $m_{B}$ has reached its maximum height.

A good questions to ask ourselves is: are the accelerations of $m_{A}$ and $m_{B}$ the same? Their weights (thus their masses, too) are different, but the change in their speed and displacement is being "equalized" by the pulley, and thus their accelerations must be the same. Let's define the equations using Newton's Second Law.
$$
\begin{align}
\sum F_{y_{A}}  & = w_{A} -T = m_{A}a_{A} \tag{1}\\
\sum F_{y_{B}}  & = T- w_{B} = m_{B}a_{B} \tag{2} \\ 
a_{A} &= a_{B} = a \tag{3}
\end{align}
$$
We then have two unknown variables: $T$ and $a$, and two equations. Let's solve for a first, combining (2) and (3) :
$$
\begin{align}
T &= w_{B} + m_{B}a \\ 
w_{A} - m_{A}a &= w_{B} + m_{B}a \\ 
a  & = \frac{g(m_{A}-m_{B})}{m_{A} + m_{B}} = 4.2 \frac{m}{s^2} \tag {4}
\end{align}
$$
With this, we calculate the velocity $m_B$ has reached at the end of the $0.6m$ displacement with the next equation:
$$
\begin{align}
v_{B}^2 &= v_{B_{0}}^2 + 2a(y-y_{B}) \\
v_{B}^2 &= 2a(0.6)\\ \\
v_{B} &=\pm  \sqrt{2\left( 4.2 \frac{m}{s^2} \right)(0.6 m)}\frac{m}{s}\\ \\
v_{B} &= \pm 2.24 \frac{m}{s} \tag{5}
\end{align}
$$
We know use (5) and another constant acceleration formula to get the additional time it takes for $m_{B}$ to reach $v_{y} = 0$ after being subjected to the acceleration of gravity.
$$
\begin{align}
v_{f} &= v_{0} -gt  \\
t &= \frac{v_{0} - v_{f}}{g} = \frac{2.24 \frac{m}{s} - 0}{g} = 0.23s
\end{align}
$$
With this time, we calculate the additional displacement after $m_{B}$ reaches the free-fall state.
$$
\begin{align}
y &= y_{0} + \frac{v_{0} + v_{f}}{2}t \\
y  & =0.6m + \frac{2.24 \frac{m}{s} + 0}{2}(0.23s) = 0.8576m
\end{align}
$$
Thus the maximum displacement $m_{B}$ reaches is 0.8576m. This is summed to the initial 0.6m positioning above the floor, yielding a maximum height of 1.45m above the floor.
## problem 5.101
 Banked Curve I. A curve with a 120-m radius on a level road is banked at the correct angle for a speed of $20 \frac{m}{s}$ .If an automobile rounds this curve at $30 \frac{m}{s}$ what is the minimum coefficient of static friction needed between tires and road to prevent skidding?
### Solution
The solution for this problem is divided into two parts. First, getting the angle in which the road is banked, supposing it allows a maximal speed of $20 \frac{m}{s}$. Second, after getting the angle, calculating the minimum coefficient of static friction $\mu_{s}$ needed to avoid skidding between tires and a road banked at the angle found in step 1 with a velocity of $30 \frac{m}{s}$.

Let's start with step 1. For a banked curve to have the correct angle means that it has zero frictional forces. Let's draw our free body diagram.

With this, we use Newton's First and Second Law to describe the system:
$$
\begin{align}
\sum F_{x} &=  n\sin{\theta} = ma_{rad} \tag{1} \\
\sum F_{y}  & = n\cos(\theta) - w = 0 \tag{2}
\end{align}
$$

From the definition of $f_{s_{max}}$ and $a_{rad}$, we also have that:
$$
\begin{align}
f_{s_{max}} &= \mu_{s}n \tag{3} \\
a_{rad}  & = \frac{v^2}{R} \tag{4}
\end{align}
$$
We use (4) and (2) into 1 to derive the angle:
$$
\begin{align}
n &= \frac{mg}{\cos{\theta}} \\
\left( \frac{mg}{\cos{\theta}} \right)\sin{\theta} &= m\left( \frac{v^2}{R} \right) \\
\tan{\theta} &= \frac{v^2}{gR} \\
\theta  & =\arctan{\frac{v^2}{gR}}  \tag{5}
\end{align}
$$
We solve (5) to get the angle $\theta = 18.78$.
Now, having the angle, we can step into the second part of the problem.

As the velocity increases, a static frictional force starts supporting the normal force to maintain the centripetal acceleration needed to keep the curve. The maximal static frictional force represents contains the minimal static coefficient to avoid skidding. Let's set the Newton's equations with this new system:
$$
\begin{align}
\sum F_{x} &= f_{s_{max}}\cos{\theta +} n\sin{\theta} = ma_{rad} \tag{6} \\
\sum F_{y}  & = n\cos(\theta) - w - f_{s_{max}}sen{\theta} = 0 \tag{7}
\end{align}
$$
Our target variable is $\mu_{s}$. 
From (2), get an expression for $n$:
$$
\begin{align}
\sum F_{y}  & = n\cos(\theta) - w - \mu_{s}n\sin{\theta} = 0 \tag{7} \\
n &= \frac{mg}{\cos{\theta}-\mu_{s}\sin{\theta}} \tag{8}
\end{align}
$$
Substituting (8), (3) and (4) in (6), we get:
$$
\begin{align}
\mu_{s}\left( \frac{mg}{\cos{\theta}-\mu_{s}\sin{\theta}} \right)\cos(\theta) +\frac{mg}{\cos{\theta}-\mu_{s}\sin{\theta}}\sin{\theta} &= m\left( \frac{v^2}{R} \right) \tag{1} \\
\frac{g(\mu_{s}\cos{\theta} + \sin{\theta})}{\cos{\theta} - \mu_{s}\sin{\theta}} &= \frac{v^2}{R}  \\
\frac{v^2}{R}\cos{\theta} - \frac{v^2}{R}\mu_{s}\sin{\theta}  & = g(\mu_{s}\cos{\theta} + \sin{\theta}) \\
g\mu_{s}\cos{\theta} + g\sin{\theta} + \frac{v^2}{R}\mu_{s}\sin{\theta}  & =\frac{v^2}{R}\cos{\theta}  \\
\mu_{s}\left( g\cos{\theta} + \frac{v^2}{R}\sin{\theta} \right) &= \frac{v^2}{R}\cos{\theta} - g\sin{\theta}  \\
\mu_{s} &= \frac{{\frac{v^2}{R}\cos{\theta} - g\sin{\theta}}}{\left( g\cos{\theta} + \frac{v^2}{R}\sin{\theta} \right)} \tag{9} \\
\end{align}
$$

Solving (9), we get that the minimum coefficient needed is $\mu_{s} = 0.34$
## Problem 5.110
![Pasted image 20260329021738](assets/Pasted%20image%2020260329021738.png)
## Problem 5.125
![Pasted image 20260329020652](assets/Pasted%20image%2020260329020652.png)
