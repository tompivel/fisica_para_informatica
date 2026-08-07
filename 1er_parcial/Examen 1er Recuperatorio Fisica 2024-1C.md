# Examen Modelo 2 Parcial Fisica 2024-1C
## Ejercicio 1

Una partícula puntual de masa $m$ parte del reposo desde el extremo superior de un plano inclinado de masa $M$ que es libre de moverse horizontalmente, como se indica en la figura. El plano también se halla en reposo en el instante inicial y existe rozamiento entre la masa y el plano, no así entre el plano y el suelo.

![Pasted image 20260524113415](../assets/Pasted%20image%2020260524113415.png)

- **a)** ¿Se conserva alguna componente del momento lineal del sistema? 
    
- **b)** ¿Se conserva la energía mecánica del sistema?

* **c)** Al llegar la partícula a la parte más baja del plano, ¿cuánto se desplazó el plano?
    
- **d)** ¿Cuánto vale la velocidad del Centro de Masa en el momento en que la partícula llega a la parte más baja del plano? (ayuda: no es nula) .

### Resolución

#### Punto A

Considerando al sistema como la masa $m$ y el plano inclinado, las fuerzas externas actuando sobre el sistema son el peso y la normal que el piso ejerce sobre el mismo. Ambas fuerzas externas actúan en la componente vertical. Por tanto, al no haber fuerza de rozamiento entre el piso y el plano, $\sum F_{\text{ext en X}} = 0 \implies \frac{dp_{x}}{dt}=0$ . Por tanto, el momento lineal se conserva en la componente paralela al suelo.

#### Punto B

No, no se conserva la energía mecánica del sistema debido a la fuerza de rozamiento entre la masa $m$ y el plano, generando energía interna que afecta la energía mecánica entre un estado y otro. 
#### Punto C
Sabemos que la masa realiza un recorrido relativo al plano $\Delta x_{m}=\frac{H}{\tan{\alpha}} = d$. 
Usando relaciones de velocidad relativa, tenemos que:

$$
\begin{align}
\Delta x_{\frac{m}{\text{piso}}} &  = \Delta x_{\frac{m}{M}} + \Delta x_{\frac{M}{\text{piso}}}  \\
\Delta x_{\frac{m}{\text{piso}}}  & = d + \Delta x_{\frac{M}{\text{piso}}}
\end{align}
$$

Por tanto, el recorrido absoluto de $\Delta x_{m} = d + \Delta x_{M}$. Siendo que para la componente en x (paralela al suelo), el momento lineal del sistema se conserva y el sistema parte del reposo, tenemos que entre el estado A (el sistema parte del reposo) y el estado B (la masa $m$ llega al final del plano):

$$
\begin{align}
p_{A_{x}} &  = p_{B_{x}} \\
p_{A_{x}} & = (m +M)v_{x_{CM}} = 0 \implies p_{B_{x}} =0
\end{align}
$$

Si $\Delta v_{x_{CM}}=0$ durante todo el trayecto debido a que no hay fuerzas externas actuando sobre el sistema en esta componente y el sistema parte del reposo, entonces $\Delta x_{CM}=0$. Por tanto, podemos establecer:

$$
\begin{align}
\Delta{x_{CM}} &  = \frac{{m \Delta x_{m}}  + M \Delta{x_{M}}}{m + M} \\
0  & = \frac{{m \Delta x_{m}}  + M \Delta{x_{M}}}{m + M}  \\
0  & ={m (d + \Delta x_{M})  + M \Delta{x_{M}}}  \\
0  & =md + (m + M )\Delta x_{M}    \\
\Delta  x_{M}  & =\frac{{-md}}{m + M} \\
\end{align}
$$

#### Punto D
En el anterior punto obtuvimos que la velocidad del centro de masa en la componente paralela al suelo era 0. Sin embargo, la velocidad si varía en la componente perpendicular debido a la fuerza externa de la gravedad actuando sobre el sistema.
Para el estado B del sistema, tenemos que:

$$
\begin{align}
v_{y_{CM}} =  & \frac{{mv_{y_{m}} + Mv_{y_{M}}}}{m + M} \\
v_{y_{CM}} =  & \frac{{mv_{y_{m}}}}{m + M}
\end{align}
$$

Para calcular $v_{y_{m}}$, 

## Ejercicio 2

Un cilindro muy largo de radio $R$ se encuentra cargado con una densidad superficial de carga $\sigma$, uniformemente distribuida.

- **a)** Calcular el campo eléctrico que genera en todo el espacio.
- **b)** Calcular el trabajo que debe realizarse para llevar una carga puntual $q_{0}$ desde un punto a una distancia $R$ de la superficie del cilindro hasta otro punto a una distancia $3R$ del mismo.

### Resolución
#### Punto A
Construimos una superficie gaussiana S cilíndrica de radio r y largo l concéntrica con el cilindro descrito en el enunciado. Aprovechamos la simetría para simplicar el cálculo del campo con la ley de Gauss dado que $\vec{E} \cdot \vec{n} = E$ en todo diferencial de área de la superficie descrita. Además consideremos que $\sigma = \frac{Q}{A} = \frac{Q_{encl}}{2 \pi r l}$.

$$
\begin{align}
\Phi_{E}  & = \iint_{S} \vec{E} \cdot d \vec{A}   = \iint_{S} E \hat{r} \cdot dA \hat{r}\\
  & = \iint_{S} E dA = E \iint_{S}dA \\
 & = E 2\pi rl = \frac{Q_{\text{encl}}}{\epsilon_{0}} \\
E & = \frac{Q_{\text{encl}}}{\epsilon_{0}2 \pi rl}= \frac{\sigma 2 \pi Rl}{\epsilon_{0}2 \pi rl} \\
E & = \frac{\sigma R}{\epsilon_{0}r} \\
\end{align}
$$

Por tanto, considerando que si $r<R$, entonces $Q_{\text{encl}}=0 \implies E = 0$:

$$
E(r) = \begin{cases}
 0  & \text{si} & r< R \\
 \frac{\sigma R}{\epsilon_{0}r} \hat{r} & \text{si} & r\geq R
\end{cases}
$$

#### Punto B
Acá se asume que sería con una fuerza externa en contra del campo. Entonces para llevar una carga puntual $q_{0}$ desde una distancia 2R (R del cilindro)  hasta una distancia 4R (3R del cilindro), usamos la relación de trabajo realizado por una fuerza externa y la energía potencial:

$$
\begin{align}
W_{\text{ext }} &  = \Delta U = U_f-U_{i} = q_{0} \Delta V  \\
 & = q_{0}V_{f} - q_{0}V_{i} = q_{0}(V_{f} - V_{i}) \\
\end{align}
$$

Teniendo en cuenta además que $\Delta V = V_{f}-V_{i} = -\int_{i}^f \vec{E} \cdot d \vec{l}$, calculamos:

$$
\begin{align}
V_{fi}  & = - \int_{i}^f \vec{E} \cdot d \vec{l} = - \int_{i}^f E \hat{r} \cdot dr \hat{r} \\
  & = - \int_{i}^f E  dr = - \int_{i}^f \frac{\sigma R}{\epsilon_{0}r} dr \\
& = - \frac{\sigma R}{\epsilon_{0}}  \int_{i}^f \frac{1}{r}dr \\
& = - \frac{\sigma R}{\epsilon_{0}}   \left. \ln r \right|_{i}^f \\
& = - \frac{\sigma R}{\epsilon_{0}}  (\ln 4R - \ln 2R) \\
& = - \frac{\sigma R}{\epsilon_{0}} \ln 2
\end{align}
$$

El diferencial de potencial es negativo, lo cual hace sentido dado que durante todo el trayecto, el campo eléctrico empuja a la carga. 
Por tanto, el trabajo necesario de una fuerza externa para mover una carga puntual $q_{0}$ desde 2R hasta 4R es:

$$
\begin{align}
W_{\text{ext}}  & = -q_{0} \frac{\sigma R}{\epsilon_{0}} \ln 2
\end{align}
$$

## Ejercicio 3

Los capacitores de la figura se encuentran inicialmente descargados. Una vez alcanzado el equilibrio la pila $V_{p}=10\text{ V}$ ha transferido $400\text{ nC}$ de carga.

- **a)** Calcular la capacidad $C_{0}$.
- **b)** Si el capacitor $C_{0}$ es de placas planas paralelas, cuadradas de lado $L=1\text{ m}$ y separación $d=1\text{ mm}$, calcular la permitividad relativa ($\epsilon_r$) del aislante empleado.

### Resolución
#### Punto A
#### Punto B
