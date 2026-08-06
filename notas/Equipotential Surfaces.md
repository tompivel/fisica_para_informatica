---
id: 20260527114854
aliases: []
tags:
  - uncataloged
created: 2026-05-27 11:48
status: draft
---
# Equipotential Surfaces
Surfaces that hold the same potential $V$ everywhere. Los conductores son volúmenes equipotenciales. 
![Pasted image 20260527114938](../assets/Pasted%20image%2020260527114938.png)
## Conductor with a cavity
In an electrostatic situation, if a conductor contains a cavity and if no charge is present inside the cavity, then there can be no net charge anywhere on the surface of the cavity.
![Pasted image 20260527115243](../assets/Pasted%20image%2020260527115243.png)
### Proof

The inner surface of the cavity is an equipotential surface precisely because it forms the physical boundary of the conductor's solid volume. Here is the logical progression that justifies this step in the proof:

1. **Zero Internal Field:** In electrostatics, the electric field is zero everywhere inside the solid meat of the conducting material ($\vec{E} = 0$). If not, the charges would move.
2. **Equipotential Volume:** The potential difference between any two points within the solid is defined by $\Delta V = -\int \vec{E} \cdot d\vec{l}$. Since $\vec{E} = 0$, $\Delta V = 0$. This makes the entire solid mass a single equipotential volume.
3. **Boundary Continuity:** The wall of the cavity (Surface $A$ in the diagram) is the inner boundary of this solid material. Because it is continuous with the bulk of the conductor, it must share that exact same potential.
    
This also dictates that the inner cavity surface, the bulk solid volume, and the outer exterior surface of the conductor are all at the exact same electric potential.

To see how this sets up the rest of the textbook's proof:

Now consider a Gaussian surface, shown in the figure, between the two equipotential surfaces.
Electric field lines must always point from a region of higher potential to a region of lower potential, because of $\Delta V = - \int_{i}^f \vec{E} \cdot d \vec{l}$.   Because of the relationship between $\vec{E}$ and the equipotentials, we know that the field at every point between the equipotentials is from $A$ toward $B$ or else at every point it is from B toward A, depending on which equipotential surface is at higher potential. In either case the flux through this Gaussian surface is certainly not zero. But then Gauss’s law says that the charge enclosed by the Gaussian surface cannot be zero. This contradicts our initial assumption that there is no charge in the cavity. So the potential at P cannot be different from that at the cavity wall. The entire region of the cavity must therefore be at the same potential. But for this to be true, the electric field inside the cavity must be zero everywhere. 

Finally, Gauss’s law shows that the electric field at any point on the surface of a conductor is proportional to the surface charge density $\sigma$ at that point. We conclude that the surface charge density $\sigma$ on the wall of the cavity is zero at every point. 

An alternative way to see this is: Since Surface $A$ is an equipotential surface, if an electric field existed in the empty space of the cavity, its field lines would have to start on Surface $A$ and end on a point of lower potential, or vice versa. However, field lines cannot loop back and terminate on the same equipotential surface they started from, and because the cavity contains no point charges to act as alternative start or end points, no field lines can exist at all. Therefore, $\vec{E} = 0$ everywhere inside the empty cavity space. By Gauss's Law, if $\vec{E} = 0$ just inside the cavity, the enclosed charge must be zero, meaning the inner wall holds zero net charge.