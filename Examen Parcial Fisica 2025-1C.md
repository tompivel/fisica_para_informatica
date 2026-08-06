---
id: 20260521123630
aliases: []
tags:
  - uncataloged
created: 2026-05-21 12:36
status: draft
---
# Examen Parcial Fisica 2025-1C
CB024 Física para Informática - Primer parcial
1er Cuatrimestre 2025
## Ejercicio 1
Una partícula puntual de masa $m$ se halla apoyada en una plataforma móvil de masa $M=3m$, comprimiendo un resorte no adherido a la partícula. Hay rozamiento entre la partícula y la plataforma, pero no entre la plataforma y el piso. Inicialmente, todo el conjunto se halla en reposo. En un dado instante, el resorte se suelta y, en el instante que la masa se libera de dicho resorte, la velocidad de la partícula respecto de la plataforma es $\vec{v}_0^{\,\prime}$.
![Pasted image 20260521125059](assets/Pasted%20image%2020260521125059.png)
- **a.** ¿Qué magnitudes se conservan?
- **b.** En el instante en que la partícula se libera y tiene velocidad $\vec{v}_0^{\,\prime}$ respecto de la plataforma, ¿cuál es la velocidad de la plataforma respecto del piso?
- **c.** Como hay rozamiento entre la partícula y la plataforma, la partícula recorre una distancia $d$ a lo largo de la plataforma y se frena, respecto de ésta. En ese instante, ¿cuánto se desplazó la plataforma, respecto de donde se encontraba en el instante en que se liberó la partícula del resorte? ¿Qué velocidad tiene la plataforma respecto del piso?
### Punto a
Considerando el sistema como la masa $m$, la plataforma con masa $M=3m$ y el resorte, entonces:
- La energía mecánica no se conserva, debido a la fuerza no conservativa de rozamiento haciendo trabajo sobre la trayectoria de las masas $m$ y $M$. 
- En cambio, el momento lineal  $\vec{p}$ del sistema se conserva, al no ser afectado por fuerzas externas. En el eje y, podemos observar:
$$
\begin{align}
\sum F_{\text{ext}} = & - w_{m+M} + N = 0
\end{align}
$$
	Y en el eje x, la sumatoria de fuerza externas es directamente 0 debido a que las fuerzas de rozamiento y elásticas son internas al sistema.
### Punto b
Usando como sistema de referencia un eje x paralelo al piso con coordenadas positivas a la izquierda, y un eje y perpendicular al piso con coordenadas positivas hacia arriba, con un origen en la posición inicial de la partícula en t=0.  relacionamos las velocidades relativas:
$$
\begin{align}
\vec{v_{\frac{m}{\text{piso}}}}  & = \vec{v_{\frac{m}{M}}} + \vec{v_{\frac{M}{\text{piso}}}}
\end{align}
$$
Siendo que todos estos vectores tienen componente $y=0$, trabajamos directamente con la componente en x.
$$
\begin{align}
v_{\frac{m}{\text{piso}}}  & = v'_{0} + v_{\frac{M}{\text{piso}}} \\
v_{\frac{M}{\text{piso}}}  & = v_{\frac{m}{\text{piso}}}-  v'_{0}
\end{align}
$$
Dado que el momento lineal del sistema se conserva, podemos expresar esta conservación entre ambos estados a (la particula m se libera del resorte) y b (la partícula y la plataforma retornan al reposo).
$$
\begin{align}
\vec{p_{a}}  & =  \vec{p_{b}} = 0 \\
\vec{p_{a}}  & =  m \vec{v_{\frac{m}{\text{piso}}}} + M \vec{v_{\frac{M}{\text{piso}}}} =0 \\
\vec{v_{\frac{m}{\text{piso}}}}  & = - \frac{M \cdot{\vec{v_{\frac{M}{\text{piso}}}}}}{m} \\
\vec{v_{\frac{m}{\text{piso}}}}  & = - 3 \cdot{\vec{v_{\frac{M}{\text{piso}}}}}
\end{align}
$$
Entonces, reemplazando en nuestra ecuación anterior, tenemos:

$$
\begin{align}
v_{\frac{M}{\text{piso}}}  & = v_{\frac{m}{\text{piso}}}-  v'_{0} \\
v_{\frac{M}{\text{piso}}}  & =  - 3 \cdot{\vec{v_{\frac{M}{\text{piso}}}}} -  v'_{0} \\
4v_{\frac{M}{\text{piso}}}  & =  -  v'_{0} \\

v_{\frac{M}{\text{piso}}}  & = -\frac{{v'_{0}}}{4}
\end{align}
$$
El signo negativo indica que la plataforma se mueve en sentido contrario al eje $x$ positivo definido, es decir, hacia la derecha.
### Punto c
Usando como sistema de referencia un eje x paralelo al piso con coordenadas positivas a la izquierda, y un eje y perpendicular al piso con coordenadas positivas hacia arriba, con un origen en la posición inicial de la partícula en t=0. 

Nos dicen que la velocidad relativa de la masa con respecto a la plataforma es 0. Entonces:
$$
\begin{align}
\vec{v_{\frac{m}{\text{piso}}}}  & = \vec{v_{\frac{m}{M}}} + \vec{v_{\frac{M}{\text{piso}}}} \\
\vec{v_{\frac{m}{\text{piso}}}}  & = 0 + \vec{v_{\frac{M}{\text{piso}}}} \\
\vec{v_{\frac{m}{\text{piso}}}}  & = \vec{v_{\frac{M}{\text{piso}}}}
\end{align}
$$
Ambos cuerpos se mueven a la misma velocidad con respecto del piso, llamemosle $v_{f}$. Considerando los siguientes estados:
- Estado a: El sistema inicial en reposo. 
- Estado b: Ambas masas se mueven con velocidad $v_{f}$ respecto al piso. 
Dado que el momento lineal se conserva durante todo el transcurso entre ambos eventos, podemos aplicar:
$$
\begin{align}
p_{a} & = p_{b} \\
0 & = v_{f}(4m) \\
v_{f} & = 0
\end{align}
$$
Por tanto, $v_{f}$ es 0.

Ahora, dado que la sumatoria de fuerzas externas en el eje x es nula, no existe aceleración durante todo el movimiento. Por tanto, la velocidad del centro de masa del sistema $v_{CM}$ es constante. Siendo que el estado inicial del sistema es el reposo con $V_{cm}=0$. Entonces esta velocidad se mantiene en 0 por el resto del evento. Esto implica a su vez que el desplazamiento del centro de masa $\Delta x_{CM}=0$. 
El desplazamiento del centro de masa se define mediante los desplazamientos absolutos respecto al piso de cada componente del sistema:
$$
\begin{align}
\Delta x_{CM} &  = \frac{m \Delta x_m + M \Delta x_M}{m + M} \\
0 &  = \frac{m \Delta x_m + M \Delta x_M}{m + M} \\
\Delta x_{M}  & = - \frac{m}{M} \Delta x_m  \\
\Delta x_{M}  & = - \frac{1}{3} \Delta x_m 
\end{align}
$$
A su vez, el enunciado ofrece el desplazamiento relativo $d$ de la masa $m$ con respecto a la plataforma.
$$
\begin{align}
\Delta x_m  & = \Delta x_{m/M} +  \Delta x_M  \\
\Delta x_{m/M} &  = \Delta x_m - \Delta x_M \\
d  & = \Delta x_m - \Delta x_M \\
\Delta x_m & = d + \Delta x_{M}
\end{align}
$$
Reemplazando en la anterior ecuación, obtenemos $x_{M}$:
$$
\begin{align}
3\Delta x_{M}  & = -( d + \Delta x_{M}) \\
\Delta x_{M}  & =  -\frac{d}{4}
\end{align}
$$
El signo negativo indica que la plataforma se desplazó en sentido contrario al eje x positivo definido (es decir, hacia la derecha).
## Ejercicio 2

Tres planos cuadrados de área $A$ se hallan colocados paralelamente unos con otros, separados una distancia $d$ cada uno, como indica la figura. El plano 2 tiene una carga $Q$, uniformemente distribuida, mientras que los otros planos se hallan inicialmente descargados. Se conecta una pila de valor $V_{0}$ entre los dos planos extremos. Despreciando efectos de borde, se pide:

- **a.** Las densidades de carga de los planos 1 y 3.
- **b.** El campo eléctrico en todo el espacio.
- **c.** La diferencia de potencial entre los puntos $P_{1}$ y $P_{2}$.
- **d.** Suponga ahora que la carga $Q=0$ y que entre los planos 1 y 2 hay un material dieléctrico de permitividad relativa $\epsilon_{r}=2$. ¿Cómo cambian los resultados de los puntos a y c?

### Punto A
Modelamos los tres planos de carga como planos infinitos de carga, aprovechamos que podemos desestimar los efectos de bode.
La densidad de carga del plano 2, ya es conocida $\sigma_{2} = \frac{Q}{A}$. Buscamos entonces las densidades de carga $\sigma_{1}$ y $\sigma_{3}$. 
$$
\begin{align}
\sigma_{1}  & = \frac{Q_{1}}{A} \\
\sigma_{3}  & = \frac{Q_{3}}{A}
\end{align}
$$
Sabemos que ambos planos tienen área A, entonces debemos enfocarnos en obtener la carga encerrada en ambos planos. Dos ecuaciones, cuatro incógnitas. Antes de proponer dos ecuaciones más para resolver el problema, consideremos:

La pila impone y mantiene constantemente que la diferencia de potencial eléctrico entre la placa 1 y la placa 3 sea exactamente $V_0$. Observando el símbolo de la pila en el diagrama, podemos asumir que la placa 1 está a mayor potencial, por lo que $V_1 - V_3 = V_0$.
Recordemos además que una pila **mueve carga, no la crea:** una pila ideal actúa como una "bomba" de electrones. Si ambas placas estaban inicialmente descargadas $Q_{i}=0$, y la pila solo movió electrones entre una placa y la otra, la suma de la carga total entre ambas placas debe ser  $Q_{1} + Q_{3} = 0  \implies \sigma_{1} = - \sigma_{3}$ . Esta es nuestra 3ra ecuación.

Ahora, pensemos en el campo eléctrico que existe entre ambas placas. Es decir:
- Campo eléctrico $E_{12}$ que existe entre placa 1 y 2.
- Campo eléctrico $E_{23}$ que existe enetre las placas 2 y 3.
Teniendo en cuenta que una placa infinita produce un campo eléctrico uniforme $E = \frac{\sigma}{2 \epsilon_{0}}$. Entonces superponemos campos para hallar el campo total en cada sección, asumiendo un sistema de referencia con y positivo hacia arriba.

Para $E_{12}$, tenemos:
$$
\begin{align}
\vec{E_{12}}  & = \vec{E_{1}} + \vec{E_{2}} + \vec{E_{3}} \\
E_{12}  & = -\frac{\sigma_{1}}{2\epsilon_{0}} + \frac{Q}{2A \epsilon_{0}} + \frac{\sigma_{3}}{2 \epsilon_{0}}
\end{align}
$$
Para $E_{23}$, tenemos:
$$
\begin{align}
\vec{E_{23}}  & = \vec{E_{1}} + \vec{E_{2}} + \vec{E_{3}} \\
E_{23}  & = -\frac{\sigma_{1}}{2\epsilon_{0}} - \frac{Q}{2A \epsilon_{0}} + \frac{\sigma_{3}}{2 \epsilon_{0}}
\end{align}
$$
Ahora, introducimos la relación del entre la diferencia potencial entre ambas placas y el campo eléctrico:
$$
\begin{align}
V_{1} - V_{3} &  = (V_{1} - V_{2}) + (V_{2}-V_{3}) \\
V_{1} - V_{3} &  = \int_{1}^2\vec{E_{12}} d \vec{l} + \int_{2}^3 \vec{E_{23}} d \vec{l}
\end{align}
$$
Siendo que el campo es uniforme durante toda la linea de campo en ambas regiones $1-2$ y $2-3$. Teniendo en cuenta que definimos un sistema de referencia con el eje y positivo hacia arriba y un origen en el placa 2 , el cálculo se simplifica:
$$
\begin{align}
V_{1} - V_{3} &  = \int_{y_{1}}^{y_{2}}E_{12}\hat{j} \cdot dy \hat{j} + \int_{y_{2}}^{y_{3}} E_{23} \hat{j} \cdot dy \hat{j}  \\
V_{1} - V_{3} &  = \int_{y_{1}}^{y_{2}}E_{12} dy  + \int_{y_{2}}^{y_{3}} E_{23}dy  \\
V_{1} - V_{3} &  = E_{12}\int_{y_{1}}^{y_{2}} dy  + E_{23}\int_{y_{2}}^{y_{3}}dy   \\
V_{1} - V_{3} &  = E_{12} (y_{2} - y_{1})  + E_{23}(y_{3} - y_{2})   \\
V_{1} - V_{3} &  = E_{12} (0 - d)  + E_{23}(-d-0)   \\
V_{1} - V_{3} &  = -E_{12}d  - E_{23}d   \\
\end{align}
$$
Ahora reemplazamos nuestras expresiones para el campo $E_{23}$ y $E_{12}$.
$$
\begin{align}
V_{1} - V_{3}  & = -d\left( -\frac{\sigma_{1}}{2\epsilon_{0}} + \frac{Q}{2A \epsilon_{0}} + \frac{\sigma_{3}}{2 \epsilon_{0}} -\frac{\sigma_{1}}{2\epsilon_{0}} - \frac{Q}{2A \epsilon_{0}} + \frac{\sigma_{3}}{2 \epsilon_{0}} \right) \\
V_{1} - V_{3}  & = -d\left( -\frac{2\sigma_{1}}{2\epsilon_{0}} + \frac{2\sigma_{3}}{2 \epsilon_{0}} \right) \\
V_{1} - V_{3}  & = -d\left( \frac{2\sigma_{3}}{2\epsilon_{0}} + \frac{2\sigma_{3}}{2 \epsilon_{0}} \right) \\
V_{1} - V_{3}  & = -d\frac{2\sigma_{3}}{\epsilon_{0}} \\
\sigma_{3}  & =- \frac{V_{0}\epsilon_{0}}{2d} \\
\sigma_{1}  & =\frac{V_{0}\epsilon_{0}}{2d}
\end{align}
$$
Esto hace sentido físico porque las líneas de campo eléctrico siempre apuntan desde las regiones de mayor potencial hacia las de menor potencial por $E = - \nabla V$ (es decir, el campo neto debe apuntar hacia abajo). Para que el campo neto apunte hacia abajo y se mantenga esa diferencia de potencial, la placa superior (1) debe tener carga neta positiva, y la placa inferior (3) carga neta negativa.
### Punto b
Ya calculamos el campo eléctrico para las regiones $E_{12}$ y $E_{23}$ en el punto anterior. Únicamente expandimos sus expresiones con los valores encontrados de $\sigma_{1}$ y $\sigma_{2}$. Para $E_{12}$, tenemos:
$$
\begin{align}
E_{12}  & = -\frac{\frac{V_{0}\epsilon_{0}}{2d}}{2\epsilon_{0}} + \frac{Q}{2A \epsilon_{0}} + \frac{-\frac{V_{0}\epsilon_{0}}{2d}}{2 \epsilon_{0}} \\
E_{12}  & = -\frac{V_{0}}{2d} + \frac{Q}{2A \epsilon_{0}}
\end{align}
$$
Para $E_{23}$, tenemos:
$$
\begin{align}
E_{23}  & = -\frac{\frac{V_{0}\epsilon_{0}}{2d}}{2\epsilon_{0}} - \frac{Q}{2A \epsilon_{0}} + \frac{-\frac{V_{0}\epsilon_{0}}{2d}}{2 \epsilon_{0}} \\
E_{23}  & = -\frac{V_{0}}{2d} - \frac{Q}{2A \epsilon_{0}}
\end{align}
$$

Para este punto, calculamos $E_{01}$ y $E_{34}$, siendo 0 la región encima de la placa 1 y 4 la región inferior a la placa 3.
Por tanto, tenemos: 
$$
\begin{align}
\vec{E_{01}} &  = \vec{E_{1}} + \vec{E_{2}} + \vec{E_{3}} \\
E_{01} &  = \frac{\sigma_{1}}{2\epsilon_{0}} +  \frac{\sigma_{2}}{2\epsilon_{0}} +  \frac{\sigma_{3}}{2\epsilon_{0}} \\
E_{01} &  = \frac{\frac{V_{0}\epsilon_{0}}{2d}}{2\epsilon_{0}} +  \frac{Q}{2A\epsilon_{0}} +  \frac{- \frac{V_{0}\epsilon_{0}}{2d}}{2\epsilon_{0}} \\
E_{01} &  =  \frac{Q}{2A\epsilon_{0}} 
\end{align}
$$

Para el campo $E_{34}$, tenemos:
$$
\begin{align}
\vec{E_{34}} &  = \vec{E_{1}} + \vec{E_{2}} + \vec{E_{3}} \\
E_{34} &  = -\frac{\sigma_{1}}{2\epsilon_{0}} -\frac{\sigma_{2}}{2\epsilon_{0}} -  \frac{\sigma_{3}}{2\epsilon_{0}} \\
E_{34} &  = -\frac{\frac{V_{0}\epsilon_{0}}{2d}}{2\epsilon_{0}} -  \frac{Q}{2A\epsilon_{0}} -  \frac{- \frac{V_{0}\epsilon_{0}}{2d}}{2\epsilon_{0}} \\
E_{34} &  =  -\frac{Q}{2A\epsilon_{0}} 
\end{align}
$$
La cancelación matemática de $\sigma_{1}$ y $\sigma_{3}$ refleja la realidad física: al tener cargas opuestas de igual magnitud, se comportan hacia el exterior como un capacitor ideal cuyo campo neto es nulo, dejando únicamente el aporte de la placa central. Por tanto, el campo eléctrico viene dado por:
$$
\vec{E}(y) = \begin{cases} 
 \frac{Q}{2A\epsilon_{0}} \hat{j}  & \text{si } y > d \\
(-\frac{V_{0}}{2d} + \frac{Q}{2A \epsilon_{0}}) \hat{j} & \text{si } 0 \leq y \leq d  \\
 (-\frac{V_{0}}{2d} - \frac{Q}{2A \epsilon_{0}}) \hat{j} & \text{si } -d \leq y \leq 0 \\
 -\frac{Q}{2A\epsilon_{0}} \hat{j}  & \text{si } y < -d \\
\end{cases}
$$
### Punto C
- El punto $P_{1}$ se encuentra una distancia d arriba de la placa 1, denominemos este punto entonces como $y_{0} = 2d$. 
- El punto $P_{2}$ se encuentra una distancia d debajo de la placa 3, denominemos este punto como $y_{4} = -2d$.
El diferencial de potencial entre ambos puntos viene dado por:

$$
\begin{align}
V_{P_{1}}-V_{P_{2}} &  = \int_{0}^{4} \vec{E} d \vec{l} \\
V_{P_{1}}-V_{P_{2}} &  = \int_{0}^{1} \vec{E_{01}} \cdot d \vec{l} + \int_{1}^{3} \vec{E_{13}} \cdot d \vec{l} + \int_{3}^{4} \vec{E_{34}} \cdot d \vec{l} \\
\end{align}
$$
Sabemos por el punto a, que la segunda integral equivale a $V_{0}$. Teniendo en cuenta que $d \vec{l} = dy \hat{j}$ y que $E_{01}$ y $E_{34}$ son uniformes en sus respectivas regiones, trabajamos la expresión:
$$
\begin{align}
V_{P_{1}}-V_{P_{2}} &  = \int_{0}^{1} \vec{E_{01}} \cdot d \vec{l} + V_{0} + \int_{3}^{4} \vec{E_{34}} \cdot d \vec{l} \\
V_{P_{1}}-V_{P_{2}} &  = \int_{y_{0}}^{y_{1}} E_{01}\hat{j} \cdot dy \hat{j}+ V_{0} + \int_{y_{3}}^{y_{4}} E_{34} \hat{j} \cdot dy \hat{j}  \\
V_{P_{1}}-V_{P_{2}}  &  = E_{01}\int_{y_{0}}^{y_{1}}  dy + V_{0} + E_{34}\int_{y_{3}}^{y_{4}}  dy   \\
V_{P_{1}}-V_{P_{2}}  &  = E_{01}(y_{1} - y_{0})  + V_{0} + E_{34}(y_{4}-y_{3})   \\
V_{P_{1}}-V_{P_{2}}  &  = E_{01}(d-2d)  + V_{0} + E_{34}(-2d-(-d))   \\
V_{P_{1}}-V_{P_{2}} &  = -(\frac{Q}{2A\epsilon_{0}})d  + V_{0} -(-\frac{Q}{2A\epsilon_{0}} )d \\
V_{P_{1}}-V_{P_{2}} &  = V_{0}
\end{align}
$$
Por tanto, el diferencial de potencial entre el punto $P_{1}$ y el punto $P_{2}$ es $V_{0}$. Como la distribución de carga externa de la placa 2 genera un campo uniforme que apunta hacia afuera simétricamente en ambos extremos, los campos en las regiones 0 y 4 tienen igual magnitud pero sentidos opuestos ($E_{01} = -E_{34}$). En consecuencia, la variación de potencial que sufres al alejarte una distancia $d$ "hacia arriba" desde la placa 1 se cancela de manera exacta y perfecta con la variación de potencial que ocurre al alejarte una distancia $d$ "hacia abajo" desde la placa 3.
### Punto d
Si existe un material dieléctrico entre las placas 1 y 2 con permitividad relativa $\epsilon_{r}=2$, entonces tenemos que trabajar con $\epsilon = \epsilon_{r}\epsilon_{0}$ en nuestras expresiones del campo eléctrico $E_{12}$. Si además removemos la carga de la placa 2, tenemos que para el punto a, las densidades de carga se convierten en:
$$
\begin{align}

\end{align}
$$
$$
\begin{align} \\
E_{12}  & = -\frac{\sigma_{1}}{4\epsilon_{0}} + \frac{\sigma_{3}}{4 \epsilon_{0}} \\
V_{1} - V_{3}  & = -d\left( -\frac{\sigma_{1}}{4\epsilon_{0}}  + \frac{\sigma_{3}}{4 \epsilon_{0}} -\frac{\sigma_{1}}{2\epsilon_{0}} + \frac{\sigma_{3}}{2 \epsilon_{0}} \right) \\ 
V_{1} - V_{3}  & = -d\left( -\frac{3\sigma_{1}}{4\epsilon_{0}}  + \frac{3\sigma_{3}}{ 4\epsilon_{0}} \right) \\ 
V_{1} - V_{3}  & = -d\left(\frac{3\sigma_{3}}{4\epsilon_{0}}  + \frac{3\sigma_{3}}{4 \epsilon_{0}} \right) \\ 
V_{1} - V_{3}  & = -d\left(\frac{3\sigma_{3}}{2\epsilon_{0}}\right) \\
\sigma_{3}  & = -2\frac{V_{0}\epsilon_{0}}{3d} \\
\sigma_{1}  & =\frac{2V_{0}\epsilon_{0}}{3d}
\end{align}
$$
Y para el punto c, se sigue manteniendo que $V_{0}$ representa la diferencia de potencial entre $P_{1}$ y $P_{2}$ dado que todas las expresiones que incluyen a Q en el cálculo se cancelan entre sí.
### Ejercicio 3

En el circuito de la figura, todas las resistencias son iguales a $R$, mientras que la batería tiene un valor $V_{0}$. Calcular:

- **a.** El valor de la resistencia equivalente vista desde la fuente.
- **b.** La corriente que entrega la fuente.
- **c.** La potencia disipada sobre la resistencia $R_{3}$.
