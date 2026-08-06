---
id: 20260331210901
aliases: []
tags:
  - "#physics_eng"
created: 2026-03-31 21:09
status: draft
---
# Sears Chapter 7 Problems

## 7.41
At a construction site, a 65.0-kg bucket of concrete hangs from a light (but strong) cable that passes over a light, friction-free pulley and is connected to an 80.0-kg box on a horizontal roof (Fig. P7.41). The cable pulls horizontally on the box, and a 50.0-kg bag of gravel rests on top of the box. The coefficients of friction between the box and roof are shown. (a) Find the friction
force on the bag of gravel and on the box. (b) Suddenly a worker picks up the bag of gravel. Use energy conservation to find  the speed of the bucket after it has descended 2.00 m from rest. (You can check your answer by solving this problem using  Newton’s laws.)
Coefficients of friction between roof and box:
- $\mu_{s}$ =0.700
- $\mu_{k}$ = 0.400
### Resolution
Let's start with (a). To find the friction force between the bag of gravel and the box, we need to analyze both objects as isolated systems.

But two important questions arises:
- is the box being accelerated when the bag of gravel is placed on top of it? To know this, we will analyze both bodies as a unified system to check the answer to this question.
- we would have to analyze if the sum of the friction forces acting on the box are "enough" to contrarrest the pull of the bucket of concrete. But we don't have the static coefficient for the friction force between the bag and the box.
- Also, what happens when there are two friction forces acting on a body (the box), are both still proportionally equal to the normal force? Both are still proportional to the normal force, but **every contact surface has its own independent normal force.**.

Let's consider the unified system box + bag unified:
$$
\begin{align}
\sum F_{y}  & = n_{u}-w_{u} = 0 \rightarrow n_{u} = (m_{\text{box}} + m_{\text{bag}})g=1274N
\end{align}
$$
The maximum static friction force that the roof can exert on the unified system is:
$$
\begin{align}
f_{s_{max}} = \mu_{s}*n_{u} = 0,7*1274N=891.8N
\end{align}
$$
Now, we ask ourselves, is this force greater or at least equal to the weight of the concrete bucket? The weight of the concrete bucket is $m_{B}g = 65kg\left( 9.8 \frac{m}{s^2} \right)=637N$. As we can see, $f_{s_{max}} > w_{\text{bucket}}$  and thus the unified system is in equilibrium.

So, if the unified system is in equilibrium, the box is not moving and if the box is not moving, the bag isn't either. Morever, there are no forces pulling on the bag. This means there are no frictional forces acting on the bag. 

The frictional force acting on the box can be deduced by analyzing the forces exerted on the box using Newton's first law, we have:
$$
\begin{align}
\sum F_{x} = T -f_{s_{\text{roof}}} = 0
\end{align}
$$
The forces acting on the bucket are:
$$
\begin{align}
\sum F_{y_\text{bucket}} = T-w_{B} = 0 \rightarrow T = 637N
\end{align}
$$
So, the frictional force acting on the box is 637N

(b)
When the bag of gravel is removed from the system, the maximum static frictional force on the box becomes $\mu_{s}m_{\text{box}}g = (0.7)784N = 548.8$. This is less than the tension pulling the box, so it inmediately starts to move. 

Let's use energy conservation to find out the velocity $v_{2}$ after 2 meters the bucket has descended from rest.

Since the bucket is connected to the box, we must treat both as a system before applying the energy conservation law. Considering $m_{\text{block}} + m_{\text{bucket}} = m_{U}$. For the potential gravitational energy, only the bucket height changes, so we'll only consider its mass for the calculation. However, it is useful to remember that in this system:
$$
\begin{align}
U_{1}grav = mgy_{1\text{bucket}} + mgy_\text{box} \\
U_{2}grav = mgy_{2\text{bucket}} + mgy_\text{box}
\end{align}
$$

The energy conservation law on this system dictates:
$$
\begin{align}
K_{1} + U_1{\text{grav}}  + W_{\text{other}}& = K_{2} +U_{2\text{grav}} \\
m_{\text{bucket}}gy_{1}  + (-\mu_{k}n_{\text{block}})\Delta x& = K_{2} + m_{\text{bucket}}gy_{2} \\
K_{2}  & = \frac{1}{2}m_{u}v_{2}^2 =  m_{u}g(y_{1}-y_{2}) - \mu_{k}n_{\text{block}}(\Delta x)\\
v  & = \pm \sqrt{ \frac{2(m_{\text{bucket}}g(y_{1}-y_{2}) - \mu_{k}n_\text{block}\Delta x)}{m_{u}} } \\
v  & = 2.99 \frac{m}{s}
\end{align}
$$

## 7.51 
Bungee Jump.
A bungee cord is 30.0 m long and, when stretched a distance x, it exerts a restoring force of magnitude kx. Your father-in-law (mass 95.0 kg) stands on a platform 45.0 m above the ground, and one end of the cord is tied securely to his ankle and the other end to the platform. You have promised him that when he steps off the platform he will fall a maximum distance of only 41.0 m before the cord stops him. You had several bungee cords to select from, and you tested them by stretching them out, tying one end to a tree, and pulling on the other end with a force of 380.0 N. When you do this, what distance will the bungee cord that you should select have stretched?
### Resolution
An elastic force and a the force exerted by gravity are acting on the man. The total mechanic energy is conserved through the movement, I can use this to solve for the k constant of the elastic force and then solve for how much the cord should have stretched when pulling on it with a force of 380N.

Let's determine point a and point b of the motion of the man:
- Point 1: The man jumps from a platform 45m high, the force of gravity starts inmediately doing positive work upon him. At this instant, kinetic energy is 0, elastic energy is 0 and potential gravitational energy is at its maximum.
- Point 2: The man stops falling at 41m because the cord has performed enough negative work on the man to deaccelerate its motion. The kinetic energy is again 0, elastic potential energy is its maximum and there is still some potential gravitational energy left.
Using the law of energy's conservation:
$$
\begin{align}
K_{1} + U_{el_{1}} + U_{\text{grav}_{1}} &= K_{2} + U_{el_{2}} + U_{\text{grav}_{2}}  \\ \\
0 + 0 + mgy_{1} &= 0 + \frac{1}{2}kx^2 + gy_{2}  \\
mgy_{1} &= \frac{1}{2}kx^2 + mgy_{2}  \\
k  & = \frac{2{mg(y_{1}-y_{2})}}{x^2} = \frac{2\times {95kg\times 9.8 \frac{m}{s^2}(45m - 4m)}}{(11m)^2}  \\
k  &=  630.92 \frac{kg}{s^2} = 630.9 \frac{N}{m}
\end{align}
$$
 Now that we have the k constant, we can apply to the second case: the cord tied to a tree. How long will it stretched being pulled by a 380N force? At the point in which the force cannot pull longer, the forces are in equilibrum, and thus we can apply newton's first law: $$ \begin{align} \sum F_{x} &= F_{p} -  F_{el}  = 0 \\  \\
 x  & = \frac{380N}{k}   = \frac{380N}{\frac{630.9N}{m}} = 0.6m
\end{align}
$$


## 7.54 
You are designing a delivery ramp for crates containing exercise equipment. The 1470-N crates will move at 1.8 m/s at the top of a ramp that slopes downward at $22^\circ$. The ramp exerts a 550-N kinetic friction force on each crate, and the maximum static friction force also has this value. Each crate will compress a spring at the bottom of the ramp and will come to rest after traveling a total distance of 8.0 m along the ramp. Once stopped, a crate must not rebound back up the ramp. Calculate the force constant of the spring that will be needed in order to meet the design criteria.
### Resolution
I'm wondering if the problem starts with an acceleration as the problem detail doesn't explicitely states this. However, it may not be needed to be calculated if we were to use the energy conservation theorem. 

Our target variable is the force constant $k$ of the spring.

We'll use the energy conservation theorem to get the an expression of the k constant in terms of the $\Delta x$ of the spring's compression. We know that the height $h$ is equal to $x\sin{\theta}$. We also use $m = \frac{w}{g} =\frac{1470}{9.8} = 150kg$.

$$
\begin{align}
K_{1} + U_{el_{1}} + U_{\text{grav}_{1}} + W_{\text{other}} &= K_{2} + U_{el_{2}} \\
\frac{1}{2}mv_{1}^2 +\frac{1}{2}kx_{1}^2 + mgh_{1} - f_{k}\Delta x & = \frac{1}{2}mv_{2}^2 + \frac{1}{2}kx_{2}^2 \\
\frac{1}{2}mv_{1}^2 + mgh_{1} - f_{k}\Delta x  & = \frac{1}{2}kx_{2}^2\\
k  & = \frac{2{\left( \frac{1}{2}mv_{1}^2 + mgh_{1} - f_{k}\Delta x \right) }}{x_2^2} \\
k  & = \frac{{2\left( \frac{1}{2}mv_{1}^2 + mgy_{1}\sin \theta - f_{k}\Delta x \right)}}{x_2^2} \\
k  & =\frac{496}{x_{2}^2} \frac{N}{m}
\end{align}
$$

Given that the crate must not rebound after stopping, we should consider the exact instant in which the crate stops moving with Newton's first law:
$$
\begin{align}
\sum F_{x}  &  = f_{s} + w\sin{\theta} - f_{el} = 0  \\
\sum F_{y}  & = n - w\cos{\theta} = 0  
\end{align}
$$
We then have that $n = w\cos \theta$ and $f_{s} + w\sin \theta = f_{el}$. 

So, in order to stop the elastic force from producing acceleration upwards, $f_{s} + w\sin \theta$ must be at least equal or greater than $f_{el}$. 
$$
\begin{align}
f_{s_{max}} + w\sin \theta  & \ge f_{el} \\
550N + 1470N\sin {22} & \ge kx \\
550N + 1470N\sin {22} & \ge \left( \frac{496}{x^2} \right)x \\
x & \ge \frac{496}{550N + 1470N\sin {22}} = 0.45m
\end{align}
$$
Having this limit for the compression, we can calculate the constant:
$$
\begin{align}
k = \frac{496 \frac{N}{m}}{0.45m^2} = 2449 \frac{N}{m}
\end{align}
$$
## 7.58
A wooden rod of negligible mass and length 80.0 cm (0.4m radius) is pivoted about a horizontal axis through its center. A white rat A with mass 0.500 kg clings to one end of the stick, and a mouse B with mass 0.200 kg clings to the other end. The system is released from rest with the rod horizontal. If the animals can manage to hold on, what are their speeds as the rod swings through a vertical position?
### Resolution
The rod moves the same distance both for rat 1 and 2, since they are equidistant from the center. So, that means they have the same speed. But what about their energy? A normal force is acting upon the rats as they cling to the rod, this keeps them from free-fall. 

Let's consider the two rats and the rod a unified system. Since only gravity is acting upon the system, and it is a conservative force, we can use:
$$
\begin{align}
K_{1} + U_{1\text{grav}} = K_{2} + U_{2\text{grav}}
\end{align}
$$
Given that the rod is considered of neglible mass, its kinetic and gravitational potential energy can be dismissed. Thus, the terms can be formulated like:
$$
\begin{align}
K_{1}  & = \frac{1}{2}m_{A}v^2_{\text{1A}} + \frac{1}{2}m_{B}v^2_{\text{1B}}  \\
K_{2}  & = \frac{1}{2}m_{A}v^2_{\text{2A}} + \frac{1}{2}m_{B}v^2_{\text{2B}}  \\
U_{1\text{grav}}  & = m_{A}gy_{1A} + m_{B}gy_{1B} \\
U_{2\text{grav}}  & = m_{A}gy_{2A} + m_{B}gy_{2B}
\end{align}
$$
Considering that $v_{A} = v_{B}$, that $y_{1} =0$ for both A and B, and that $y_{2A} = - y_{2B}$ , we can simplify the terms:
$$
\begin{align}
K_{1}  & = \frac{1}{2}m_{A}v^2_{\text{1A}} + \frac{1}{2}m_{B}v^2_{\text{1B}} = \frac{1}{2}(m_{A} + m_{B})v_{1A}^2 = 0 \\
K_{2}  & = \frac{1}{2}m_{A}v^2_{\text{2A}} + \frac{1}{2}m_{B}v^2_{\text{2B}} =  \frac{1}{2}(m_{A} + m_{B})v_{2A}^2 \\
U_{1\text{grav}}  & = m_{A}gy_{1A} + m_{B}gy_{1B} = 0 \\
U_{2\text{grav}}  & = m_{A}gy_{2A} + m_{B}gy_{2B} = (m_{A}-m_{B})gy_{2A}
\end{align}
$$
Then, plugging this into the conservation of energy law:
$$
\begin{align}
K_{1} + U_{1\text{grav}}  & = K_{2} + U_{2\text{grav}} \\
0 + 0  & = \frac{1}{2}(m_{A} + m_{B})v_{2A}^2 + (m_{A}-m_{B})gy_{2A} \\
v_{2A}  & = \pm \sqrt{\frac{{2(m_{B}-m_{A})gy_{2A}}}{(m_{A} + m_{B})}} 
\end{align}
$$
Finally we know that $y_{2}A = -0.4m$, we substitute on the formula:
$$
\begin{align}
v_{2A}  & = \pm \sqrt{\frac{{(m_{B}-m_{A})gy_{2A}}}{(m_{A} + m_{B})}}  \\
v_{2A} & = 1.833 \frac{m}{s}
\end{align}
$$
Then both the rat A and the mouse B have a speed of $1.83 \frac{m}{s}$ at the end of the motion.
#### Should I consider their energy as an isolated system for each of the rats? or should I consider them as a unified system?
If you isolate just the rat, the rod is pulling/pushing on it. Because the rat is moving along an arc, calculating the exact work done by that changing contact force is an absolute nightmare.

However, if you draw your system boundary around the _entire_ stick and both animals, those contact forces between the animals and the stick become **internal forces**. Internal forces cannot change the total mechanical energy of your system.

By unifying the system, the only external force doing work is gravity, which is a conservative force.
#### How does being equidistant from the center means you have the same speed?

Because the stick is straight, if the right side moves 10 degrees, the left side _must_ also move 10 degrees. This means they have the exact same **angular speed** (ω).

The relationship between linear speed (v) and angular speed (ω) is: v=ωr

Since both animals share the same angular speed (ω) and are at the exact same distance from the pivot (r=0.400 m), their linear speeds (v) must be mathematically identical at every single instant of the swing.

## 7.66 
A truck with mass $m$ has a brake failure while going down an icy mountain road of constant downward slope angle $\alpha$. (Fig. P7.66). Initially the truck is moving downhill at speed $v_{o}$. After careening downhill a distance $L$ with negligible friction, the truck driver steers the runaway vehicle onto a runaway truck ramp of constant upward slope angle $\beta$.The truck ramp has a soft sand surface for which the coefficient of rolling friction is $\mu_{T}$. What is the distance that the truck moves up the ramp before coming to a halt? Solve using energy methods.
### Resolution
Let's divide this problem into two parts:
- Part 1: The truck is moving down the road with the downward slope angle $\alpha$. There is neglible friction and no air friction. There are only conservative forces acting on the truck. The target variable is to get the velocity in which the truck reaches the truck ramp.
- Part 2: The truck is moving up the truck ramp with slope angle $\beta$. There is friction, and the coefficient of rolling friction is $\mu_{T}$. The target variable is the distance $L_{f}$ that the truck moves up the ramp before coming to half.

#### Part 1: Getting the final speed
We'll use the law of conservation of energy. Since there are no non-conservative external forces acting on the truck, we get that:
$$
\begin{align}
K_{1} + U_{1\text{grav}} = K_{2} + U_{2\text{grav}} \\
\frac{1}{2}mv^2_{0} + mgy_{0} = \frac{1}{2}mv^2_{1} + mgy_{1}
\end{align}
$$
We know that $y_{0} =  L\sin{\alpha}$ and that $y_{1} = 0$. So $v_{1}$ can be described as:
$$
\begin{align}
\frac{1}{2}mv^2_{0} + mgy_{0}  & = \frac{1}{2}mv^2_{1} + mgy_{1} \\
\frac{1}{2}mv^2_{0} + mgL\sin{\alpha}  & = \frac{1}{2}mv^2_{1} \\
v_{1}  & = \sqrt{ {(v^2_{0} + 2gL\sin{\alpha})} }
\end{align}
$$
Now that we have an expression for $v_{1}$, we can try to get the target variable $L_{f}$.

#### Part 2: Truck ramp
Here, there is friction, so there is a non-conservative external force acting on the truck, we must be sure to include it. Our energy conservation formula becomes:
$$
\begin{align}
K_{1} + U_{1\text{grav}} + W_{\text{other}} = K_{2} + U_{2\text{grav}} \\
\frac{1}{2}mv^2_{1} + \mu_{T}nL_{f} = \frac{1}{2}mv^2_{2} + mgy_{2}
\end{align}
$$

Using newton's first law for the vertical plane of the truck (aligned perpendiculary to the slope), we get that:
$$
\begin{align}
\sum F_{y} = n - w\cos{\beta} = 0 \rightarrow n = w\cos{\beta}
\end{align}
$$
We also know that $v_{2} = 0$ and that $y_{2} = L_{f}\sin{\beta}$. So, replacing this and our previous derivation for $v_{1}$, we get:
$$
\begin{align}
\frac{1}{2}mv^2_{1} + \mu_{T}nL_{f}  & = \frac{1}{2}mv^2_{2} + mgy_{2} \\
\frac{1}{2}m(\sqrt{ {(v^2_{0} + 2gL\sin{\alpha})} })^2 + \mu_{T}(mg\cos{\beta})L_{f}  & =  mgL_{f}\sin{\beta}  \\
\frac{1}{2}m{(v^2_{0} + 2gL\sin{\alpha})} + \mu_{T}(mg\cos{\beta})L_{f}  & =  mgL_{f}\sin{\beta}  \\
\end{align}
$$
Then, solving for $L_{f}$, we get:
$$
\begin{align}
\frac{1}{2}m{(v^2_{0} + 2gL\sin{\alpha})} - \mu_{T}(mg\cos{\beta})L_{f}  & =  mgL_{f}\sin{\beta}  \\
L_{f}g(\sin{\beta} +\mu_{T}\cos{\beta})  & = \frac{1}{2}{(v^2_{0} + 2gL\sin{\alpha})} \\
L_{f}  & = \frac{{\frac{1}{2}{(v^2_{0} + 2gL\sin{\alpha})}}}{g(\sin{\beta} +\mu_{T}\cos{\beta})}
\end{align}
$$

Then, we have an expression for $L_{f}$ in terms of $v_{0}, L,\alpha,\beta$.

## 7.73
A 3.00-kg fish is attached to the lower end of a vertical spring that has negligible mass and force constant $900 \frac{N}{m}$. The spring initially is neither stretched nor compressed. The fish is released from rest. 
- (a) What is its speed after it has descended 0.0500 m from its initial position? 
- (b) What is the maximum speed of the fish as it descends?
### Resolution
Does this exercise needs calculus? Where? It seems is as simple as replacing values in the energy conservation formula...
Let's solve first the part a
#### Part A: speed after 0.05m
We use the energy conservation formula. There are no non-conservative external forces.
$$
\begin{align}
K_{1} + U_{1\text{grav}} + U_{1\text{el}} & = K_{2} + U_{2\text{grav}}  + U_{2\text{el}}\\
0 + 0 +0  & = \frac{1}{2}mv_{2}^2 + mgy_{2} + \frac{1}{2}ky_{2}^2 \\
v_{2} &  = \sqrt{\frac{-(2mgy_{2} +ky_{2}^2)}{m} } \\
v_{2} & = 0.48 \frac{m}{s}
\end{align}
$$
#### Part B: maximum speed of the fish as it decends
To find the maximum speed of the fish as it decends, we equal the derivate of our our expression for $v_{2}$  with respect to position to 0.
$$
\begin{align}
\frac{d}{dy} v_{2}  & = \frac{d}{dy}\left(-2gy_{2} - \frac{k}{m}y_{2}^2 \right)^{1/2} \\
 & =\frac{1}{2}\left( -2gy_{2} - \frac{k}{m}y_{2}^2 \right)^{-1/2} \times\left( -2g-\frac{2k}{m}y_{2} \right) \\
  & = \frac{{ -2g-\frac{2k}{m}y_{2}}}{\sqrt{ -2gy_{2} - \frac{k}{m}y_{2}^2 }} \\
 & =  0
\end{align}
$$
For a fraction to be zero, only the numerator needs to be zero, so:
$$
\begin{align}
-2g-\frac{2k}{m}y_{2}  & = 0 \\
y_{2}  & = \frac{-gm}{k}
\end{align}
$$

We then have that the maximum speed occurs at $y_{2}=-0.033m$, giving a maximum speed of 0.565m

