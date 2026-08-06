---
id: 20260529112300
aliases: []
tags:
  - uncataloged
created: 2026-05-29 11:23
status: draft
---
# Sears 23-Electric Potential
## 23.51
## Problem Statement

A point charge $q_1 = 4.00\text{ nC}$ is placed at the origin, and a second point charge $q_2 = -3.00\text{ nC}$ is placed on the $x$-axis at $x = +20.0\text{ cm}$. A third point charge $q_3 = 2.00\text{ nC}$ is to be placed on the $x$-axis between $q_1$ and $q_2$. (Take as zero the potential energy of the three charges when they are infinitely far apart.)

- **(a)** What is the potential energy of the system of the three charges if $q_3$ is placed at $x = +10.0\text{ cm}$?
- **(b)** Where should $q_3$ be placed to make the potential energy of the system equal to zero?
### Resolution
> La energía potencial total de un sistema de cargas puntuales no depende de una carga de prueba externa, sino que es la suma algebraica de las energías potenciales de todas las parejas posibles que se pueden formar con las cargas del sistema. Representa el trabajo total necesario para ensamblar el sistema trayendo las cargas una por una desde el infinito.

We first calculate the position vectors and distances $r$ from each charge to each charge:
- Charge $q_{1}$: $\vec{r}_{1} = (0,0) \implies \vec{r_{q_{1} \to q_{2}}}= 0.2m \hat{i} \land \vec{r_{q_{1}\to q_{3}}}=0.1m \hat{i}$
- Charge $q_{2}$: $\vec{r}_{2} = (0.2m,0) \implies \vec{r}_{q_{2} \to q_{1}} = -0.2m\hat{i} \land \vec{r}_{q_{2} \to q_{3}} = -0.1m \hat{i}$
#### a
- Charge $q_{3}$: $\vec{r}_{3} = (0.1m,0) \implies \vec{r}_{q_{3} \to q_{1}} = (-0.1m)\hat{i} \land \vec{r}_{q_{3} \to q_{2}}=0.1m \hat{i}$
We get the total potential energy of the system by calculating the potential energy between each possible pair of charges

$$
\begin{align}
U_{\text{sys}} & =U_{12} + U_{23} + U_{13} \\
U_{\text{sys}} & = \frac{q_{1}q_{2}}{4\pi\epsilon_{0}r_{12}} + \frac{q_{2}q_{3}}{4\pi\epsilon_{0}r_{23}} + \frac{q_{1}q_{3}}{4\pi\epsilon_{0}r_{13}} \\
U_{sys} &  = k \cdot 10^{-18} \left( \frac{4(-3)}{0.20} + \frac{4(2)}{0.10} + \frac{(-3)(2)}{0.10} \right) \\
U_{sys} = &  k \cdot 10^{-18} \left( -60 + 80 - 60 \right) = k \cdot 10^{-18} (-40) \\
U_{sys} &  = (8.99 \times 10^9) \cdot (-40 \times 10^{-18}) \approx -3.60 \times 10^{-7}\text{ J}
\end{align}
$$
#### b
$$
\begin{align}
U_{\text{sys}} = \frac{1}{4\pi\epsilon_{0}}\left( \frac{q_{1}q_{2}}{r_{12}} + \frac{q_{2}q_{3}}{x_{2}-x_{3}} + \frac{q_{1}q_{3}}{x_{3}-x_{1}}  \right) & = 0 \\
\frac{q_{1}q_{2}}{r_{12}} + \frac{q_{2}q_{3}}{x_{2}-x_{3}} + \frac{q_{1}q_{3}}{x_{3}-x_{1}}  & = 0 \\
\frac{(x_{3}-x_{1})(x_{2}-x_{3})q_{1}q_{2}}{r_{12}} + \frac{(x_{3}-x_{1})(x_{2}-x_{3})q_{2}q_{3}}{x_{2}-x_{3}} + \frac{(x_{3}-x_{1})(x_{2}-x_{3})q_{1}q_{3}}{x_{3}-x_{1}}  & = 0 \\
\frac{(x_{3}-x_{1})(x_{2}-x_{3})q_{1}q_{2}}{r_{12}} +(x_{3}-x_{1})q_{2}q_{3} + (x_{2}-x_{3})q_{1}q_{3} & = 0 \\ \\
\frac{(-x_{3}^2 +x_{3}x_{2} +x_{3}x_{1} - x_{1}x_{2})q_{1}q_{2}}{r_{12}} +x_{3}(q_{2}q_{3} - q_{1}q_{3})-x_{1}(q_{2}q_{3}) + x_{2}(q_{1}q_{3}) & = 0 \\
-x_{3}^2 \frac{q_{1}q_{2}}{r_{12}} + x_{3}\left(\frac{q_{1}q_{2}}{r_{12}}(x_{2} + x_{1}) +q_{2}q_{3} - q_{1}q_{3}\right) -x_{1}(q_{2}q_{3}) +x_{2}(q_{1}q_{3}) -\frac{x_{1}x_{2}q_{1}q_{2}}{r_{12}}  & =0
\end{align}
$$

Al resolver las constantes, la ecuación queda:
$$
\begin{align}
30x^2 - 13x + 0.8 = 0 \\
x = \frac{13 \pm \sqrt{(-13)^2 - 4(30)(0.8)}}{2(30)} \\
x = \frac{13 \pm \sqrt{169 - 96}}{60} = \frac{13 \pm \sqrt{73}}{60}
\end{align}
$$
Esto nos arroja dos raíces matemáticas posibles:
- $x_1 \approx \frac{13 + 8.544}{60} \approx 0.359\text{ m}$
- $x_2 \approx \frac{13 - 8.544}{60} \approx 0.0743\text{ m}$

Como el enunciado restringe la posición de $q_3$ al segmento entre $q_1$ y $q_2$ ($0 < x < 0.20\text{ m}$), debemos descartar $x_1$. La única respuesta con validez física para este sistema es $x = 0.0743\text{ m}$ (es decir, a $7.43\text{ cm}$ del origen).
