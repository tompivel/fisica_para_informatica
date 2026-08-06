---
id: 20260330191232
aliases: []
tags:
  - uncataloged
created: 2026-03-30 19:12
status: draft
---
## Problem 6.60
A balky cow is leaving the barn as you try harder and harder to push her back in. In coordinates with the origin at the barn door, the cow walks from $x=0$ to $x = 6.9m$ as you apply a force with x-component $F_{x} = -\left[20 N + \left( \frac{3.0N}{m} \right)x \right]$. 

How much work does the force you apply do on the cow during this displacement?
### Resolution
The cow goes through a displacement while there's a varying force being applied throughout the whole movement. Our target variable is the total work $W_{tot}$ done by this force during the direction of the displacement $\Delta x$. We expect the work to be negative as the force is being applied at a $180^{\circ}$ angle from the displacement vector. 

We'll use the next equation:
$$
\begin{align}
\int_{x_{1}}^{x_2} F_{x} \: dx \tag{1}
\end{align}
$$
Note that $\cos{\theta} = 180^{\circ}$ is a constant throughout the displacement so we can get it out of the integral, we then solve it:
$$
\begin{align}
\int_{x_{1}}^{x_2} F_{x} \: dx & = -\int_{x_{1}}^{x_2} \left[20 N + \left( \frac{3.0N}{m} \right)x \right] \: dx\\
 & = -\left( 20Nx  + 3.0 \frac{N}{m} \frac{x^2}{2} \right|_{x_{1}}^{x_{2}}) \tag{2}  \\
 
\end{align}
$$
We then evaluate both ends of the integration with $x_{1} = 0$ and $x_{2} = 6.9m$:
$$
\begin{align}
 & = -\left(20N(6.9m)  + 3.0 \frac{N}{m} \frac{(6.9m)^2}{2} \right)\tag{3} = -\left( 209 J \right)  \\
\end{align}
$$
We then get that the total work performed by the force applied is $-209 N{m} = -209 J$. This is in accordance both in unit measurements and the direction in which the force is applied (against the movement).

## Problem 6.65
A 20.0-kg crate sits at rest at the bottom of a 15.0-m-long ramp that is inclined at 34.0 above the horizontal. A constant horizontal force of 290 N is applied to the crate to push it up the ramp. While the crate is moving, the ramp exerts a constant frictional force on it that has magnitude 65.0 N. 

(a) What is the total work done on the crate during its motion from the bottom to the top of the ramp?
(b) How much time does it take the crate to travel to the top of the ramp?

### Resolution
To solve this problem, we will need to use the work-energy theorem, constant acceleration formulas and the newton's law, because we are told about a displacement without involvement of time (for the first part) and constant forces involving time for the second part. 


#### First part: total work done
The total work is the work of the net force or the sum of the work of each individual force acting on the particle. Here we'll use the first approach.

Our target variable is the total work done. We've taken a coordinate system with an x-coordinate aligned with that of the displacement.
$$
\begin{align}

\end{align}
$$
We know that
$$
\begin{align}
W_{tot} = \sum_{i=1}^{k}  W_{F_{i}}
\end{align}
$$
The net force in the $y$ coordinate is 0 because of newton's first law, so these no do work on the particle (one could also argue that these don't do on the particle because the direction is perpendicular to that of the displacement.) The net force in the x-coordinate is:
$$
\begin{align}
\sum F_{x} = - f_{k} - w\cos{\theta} + F\sin{\theta} =  -65N - (20kg)\left( 9.8 \frac{m}{s^2} \right)\sin{34^\circ} + 290N\cos{34} = 65.82N \tag{1}
\end{align}
$$
Then the total work is:
$$
\begin{align}
\sum F_{x}\Delta x = 65.82N(15m) = 987.3J
\end{align}
$$
### Second part: how much time it takes
We know that the object starts from rests so $v_{0} = 0$, and we can get the final velocity through the work-energy theorem. Plus, we can get the acceleration through newton's second law, knowing that all forces are applied constantly and thus we are able to use constant acceleration formulas to derive the time.

Expanding (1) with Newton's Second Law, we get:
$$
\begin{align}
\sum F_{x} = - f_{k} - w\cos{\theta} + F = 65.82N = ma_{x} \tag{1}
\end{align}
$$
We then derive the acceleration through:
$$
\begin{align}
a_{x} = \frac{65.5N}{20kg} = 3.291 \frac{m}{s^2}
\end{align}
$$
We also get the final velocity using the work-energy theorem.
$$
\begin{align}
W_{tot}  & = \Delta K  \\
W_{tot}  & = \frac{1}{2}mv_{2}^2 - \frac{1}{2}mv_{1}^2 \\
987.3J & = \frac{1}{2}mv_{2}^2 - \frac{1}{2}m\left( 0 \frac{m}{s} \right)^2 \\
v_{2} &  = \sqrt{ \frac{2 \times987.3J}{20kg} } = 9.93 \frac{m}{s}
\end{align}
$$
Finally, we use the constant acceleration formula to derive the time $t$:
$$
\begin{align}
v_{2} &  = v_{1} + at \\
t  & = \frac{v_{2} -v_{1}}{a} = \frac{\frac{9.93 m}{s}}{3.293 \frac{m}{s^2}} =3.03s
\end{align}
$$
It then took 3.03s to move the particle 15m.
## Problem 6.82 
**Pushing a Cat.** Your cat “Ms.” (mass 7.00 kg) is trying to make it to the top of a frictionless ramp 2.00 m long and inclined upward at $30.0^{\circ}$ above the horizontal. Since the poor cat can’t get any traction on the ramp, you push her up the entire length of the ramp by exerting a constant 100-N force parallel to the ramp. 

If Ms. takes a running start so that she is moving at $\frac{2.40m}{s}$ at the bottom of the ramp, what is her speed when she reaches the top of the incline? Use the work–energy theorem.
### Resolution
Our target variable is the final velocity $v_{2}$ of the cat when it reaches the top of the incline. For this, we will be using the work-energy theorem to correlate the total work performed to the change in kinetic energy of the particle, and thus get its velocity. We start with an initial velocity, and because the cat can't get any traction on the ramp, there is no friction to be considered in this case.

Let's consider the axis x parallel to the ramp. Then the total work performed will be given by $\sum F_{x} \Delta x$. We already know the distance traveled is 2.0m, let's get now the x-component of the net force $\sum F_{x}$.
$$
\begin{align}
\sum F_{x} = F - w\sin{\theta} = 100N - (7kg)\left( 9.8 \frac{m}{s^2} \right)\sin{30^\circ} = 65.7N
\end{align}
$$
The y-component doesn't perform any work on the particle as it perpendicular to the displacement. We then get the net work $W_{tot}$ as $\sum F_{x}\Delta x = 65.7N\times 2.0m = 131.4J$.

We now use the work-energy theorem to get the final velocity of the cat:
$$
\begin{align}
W_{tot} &  = \Delta K = K_{2} - K_{1} = \frac{1}{2}mv_{2}^2 - \frac{1}{2}m v_{1}^2 \\
v  & = \sqrt{ \frac{2\left( W_{tot} + \frac{1}{2} mv_{1}^2\right)}{m}} \\
v  & = \sqrt{ \frac{2\left( 131.4J + \frac{1}{2} 7.0kg \left( 2.40 \frac{m}{s} \right)^2\right)}{7.0kg}} = 6.58 \frac{m}{s}
\end{align}
$$
Then the final velocity $v_{2}$ is $6.58 \frac{m}{s}$.
## Problem 6.84
A physics professor is pushed up a ramp inclined upward at $30^\circ$ above the horizontal as he sits in his desk chair that slides on frictionless rollers. The combined mass of the professor and chair is 85.0 kg. He is pushed 2.50 m along the incline by a group of students who together exert a constant horizontal force of 600 N. The professor’s speed at the bottom of the ramp is $2.00 \frac{m}{s}$. 

Use the work–energy theorem to find his speed at the top of the ramp.

### Resolution
This exercise is similar to the problem 6.82. Here will use a traditional coordinate system and calculate the individual work of each force, add it to get net work and then apply the work-energy theorem to get the final velocity $v_{2}$ (our target variable).

Let's then calculate the individual work of each force using $W_{F} = F\cos{\theta}\Delta x$:
$$
\begin{align}
W_{F} &= 600N\cos{30^\circ}(2.5m) = 1299J   \\
W_{n} &= n\cos{90}= 0  \\
W_{w}  & = mg\cos{90 + 30}(2.5m) = -1041.3J \\
W_{tot}  & = 1299J - 1041.3J = 257.7J
\end{align}
$$
Now we use the work-energy theorem to get $v^2$:
$$
\begin{align}
W_{tot}  & = \Delta K = \frac{1}{2}mv^2_{2} = \frac{1}{2}mv_{1}^2 \\
v_{2}  & = \sqrt{\frac{2(W_{tot} + K_{1})}{m} } = \sqrt{ \frac{2}{85kg}\left( 257.7J + \frac{1}{2} \left( 85kg\times \left( 2.00 \frac{m}{s} \right)^2 \right) \right) } = 3.17 \frac{m}{s}
\end{align}
$$

