---
id: 20260328182544
aliases: []
tags:
  - uncataloged
created: 2026-03-28 18:25
status: draft
---
# Sears chapter 3 problems
## Problem 3.56
As a ship is approaching the dock at $45 \frac{cm}{s}$ an important piece of landing equipment needs to be thrown to it before it can dock. This equipment is thrown at $15 \frac{m}{s}$ at 60.0° above the horizontal from the top of a tower at the edge of the water, 8.75 m above the ship’s deck (Fig. P3.56). For this equipment to land at the front of the ship, at what distance D from the dock should the ship be when the equipment is thrown? Air resistance can be neglected.
## Solution
This problem is basically asking for the distance $D$ the ship should be away from the dock to meet with the projectile thrown. The distance D is the horizontal range plus the distance the boat moves until the projectile reaches the water. Let's define our known and unknown variables.
$$
\begin{align}
\theta_{0}  &  = \text{angle at which the projectile is thrown} = 60 \\
h_{0}  &  = \text{height at which the projectile is thrown} = 8.75m \\
|\vec{v}_{0}|  & = \text{speed at which the projectile is thrown} = 15 \frac{m}{s}
\end{align}
$$
Let's start defining the initial components
$$
\begin{align}
v_{0_{x}} &  = \vec{v}_{0}\cos{\theta} = 15 \frac{m}{s}\times\cos{60} = \frac{15}{2} \frac{m}{s} \\
v_{0_{y}}  & = \vec{v}_{0}\sin{\theta} = 15 \frac{m}{s} \times \sin{60} = 12.99 \frac{m}{s} \\
\end{align}
$$
Now we calculate the time when the projectile reaches 0 (the height of the ship's deck).
$$
\begin{align}
y  & = y_{0} + v_{0_{y}}t - \frac{1}{2}gt^2  \\
0  & = 8.75m + 12.99 \frac{m}{s}t - \frac{1}{2}\left( 9.8 \frac{m}{s^2} \right)t^2 \\
 0  & = \frac{1}{2}\left( 9.8 \frac{m}{s^2} \right)t^2  - 12.99 \frac{m}{s}t - 8.75m
\end{align}
$$
We calculate the roots of this equation:
$$
\begin{align} 
t_{1,2} &  = \frac{{12.99 \frac{m}{s} \pm \sqrt{ \left( 12.99 \frac{m}{s} \right)^2 - 4\left( \frac{1}{2}\left( 9.8 \frac{m}{s^2} \right) \right)(-8.75m)}}}{9.8 \frac{m}{s^2}} \\
t_{1}  & = 3.2s \\
t_{2}  & = -0.56s
\end{align}
$$
Then the time at which the projectile reaches the ship's deck is $0.17s$. Let's calculate the distance in the x-coordinate:
$$
\begin{align}
x_{f} = v_{0_{x}}t = \frac{15}{2} \frac{m}{s} (3.2s) = 24.1m
\end{align}
$$
Then the distance $D$ that the ship should be from the dock is $24m$. But we also have to calculate how far from this point $D$ the ship should be to meet with the projectile just in time. Let's then calculate how much did the ship would have moved in $t_1$.
$$
\begin{align}
x_{b} = \left( \frac{45cm}{s} \right) \times\left( \frac{1m}{100cm} \right) \times(3.2s) = 1.44m
\end{align}
$$
Then the boat should be $24.1m + 1.44m = 25.44m$ away from the dock to meet with the projectile at point $D$.

## Problem 3.77
In an action-adventure film, the hero is supposed to throw a grenade from his car, which is going $90 \frac{km}{h}$ to his enemy’s car, which is going $110 \frac{km}{h}$The enemy’s car is 15.8 m in front of the hero’s when he lets go of the grenade. If the hero throws the grenade so its initial velocity relative to him is at an angle of $45$ above the horizontal, what should the magnitude of the initial velocity be? The cars are both traveling in the same direction on a level road. You can ignore air resistance. Find the magnitude of the velocity both relative to the hero and relative to the earth.

### Solution
This problem mixes projectile motion and relative velocity. First it is asking us for the magnitude of the initial velocity at which the grenade is thrown relative to the hero (a). Then it ask us to find the magnitude of the velocity relative to the earth (b).

Let's define our known variables. 
$$
\begin{align}
v_{\frac{E}{Earth}} & = 110 \frac{km}{h} = \text{velocity of enemy relative to earth} \\
v_{\frac{H}{Earth}} & = 90 \frac{km}{h} = \text{velocity of hero relative to earth} \\
\Delta x  & = \text{distance between hero and enemy} = 15.8m = 15.8 m\times \frac{1km}{1000m} = -0.0158 km \\
v_{\frac{P}{H}}  & = \text{unknown} \\ \\
\theta  & = 45 = \text{angle at which the projectile is thrown} \\
g  & = 9.8 \frac{m}{s^2} = 127008 \frac{km}{h^2}


\end{align}
$$
We have to find the magnitude such that a projectile thrown with $\theta$ inclination, meets with the enemy's car. In order to find this, we're analyze the scenario within the hero's reference frame. We'll use the relative velocity equation to transform the velocity of the enemy's car.
$$
\begin{align}
v_{\frac{E}{Earth}}  &  = v_{\frac{E}{H}} + v_{\frac{H}{Earth}}  \\
v_{\frac{E}{H}}  & = v_{\frac{E}{Earth}} - v_{\frac{H}{Earth}} = 110 \frac{km}{h} - 90 \frac{km}{h}  \\ 
v_{\frac{E}{H}} & = 20 \frac{km}{h} = \text{velocity of enemy relative to earth} \\
\end{align}
$$
With this, we can set up the equations for the projectile motion (all within the reference frame of the hero):
$$
\begin{align}
v_{P_{0_{x}}} &  = v_{P_{0}}\times \cos{45} \\
v_{P_{0_{y}}} &  = v_{P_{0}}\times \sin{45} \\
x_{P}  & = v_{P_{o_{x}}}t = v_{P_{0}}\cos_{45}t  \\
y_{P}  & = v_{P_{0_{y}}}t - \frac{1}{2}gt^{ 2 } = v_{P_{0}} \sin{45}t - \frac{1}{2}gt^2
\end{align}
$$

We can describe the enemy's car movement at a given time through:
$$
\begin{align}
x_{\frac{E}{H}} = 0.0158km + \left( 20 \frac{km}{h} \right)t
\end{align}
$$

We want $X_{E}$ and $X_{P}$ to be equal, and the solve for the time at which that happens:
$$
\begin{align}
x_{P} = x_{E}  \\
 v_{P_{0}}\cos_{45}t & =  0.0158km + 20 \frac{km}{h}t
\end{align}
$$
We also want $y_{P}$ to be equal to 0 at the time at which $x_{P}$ and $x_{E}$ meet, so:
$$
\begin{align}
0  & = v_{P_{0_{y}}}t - \frac{1}{2}gt^{ 2 } = v_{P_{0}} \sin{45}t - \frac{1}{2}gt^2 \\
v_{P_{0}}  & = \frac{{\frac{1}{2}gt^2}}{\sin_{45}t}
\end{align}
$$
We use this expression of $v_{P_{0}}$ into the previous equation and solve for t:
$$
\begin{align}
 \frac{{\frac{1}{2}gt^2}}{\sin{45}t}\cos_{45}t & =  0.0158km + 20 \frac{km}{h}t  \\
 0  & = \frac{\tan{45}}{2}gt^2  - 20 \frac{km}{h}t - 0.0158km\\
\end{align}
$$
Solving for the roots of the quadratic equations, we get:
$$
\begin{align}
t_{1} = 6.805 \times 10^{-4}h \\
t_{2} = 3.65 \times 10^{-4}h
\end{align}
$$
With this, we can get $v_{P_{0}}$
$$
\begin{align}
v_{P_{0}} = \frac{\frac{1}{2}gt}{\sin{45}} = 61.1 \frac{km}{h}
\end{align}
$$
Now, to find the magnitude relative to the earth, we calculate the relative to the earth components of the projectile's velocity and then the magnitude:
$$
\begin{align}
v_{\frac{P_{0_{x}}}{Earth}}  & = v_{\frac{P_{o_{x}}}{H}} + v_{\frac{H_{x}}{Earth}} = 61.1(\cos{45}) + 90 = 133.2 \frac{km}{h}  \\
v_{\frac{P_{0_{y}}}{Earth}}  & = v_{\frac{P_{o_{y}}}{H}} + v_{\frac{H_{y}}{Earth}} = 61.1(\sin{45}) + 0 = 43.2 \frac{km}{h}  \\
|\vec{v}_{\frac{P_{0}}{Earth}}| & =\sqrt{ \left( 133.2 \frac{km}{h} \right)^2 + \left( \frac{43.2 km}{h} \right)^2 }  =  140 \frac{km}{h}
\end{align}
$$