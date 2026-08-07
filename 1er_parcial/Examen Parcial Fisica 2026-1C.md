# Examen Parcial Fisica 2026-1C

**TEMA 1** **Fecha:** $09/05/26$ - $9$ hs.

**CB024 Física para Informáticos** **Apellido y Nombre:** 

**Curso:** **DNI:**

**Justificar cada una de las respuestas.** $\epsilon_{0}=8,85 \cdot 10^{-12} \mathrm{C}^{2} / \mathrm{Nm}^{2} \quad g=10 \mathrm{~m} / \mathrm{s}^{2}$

---

### 1)

Se tiene un cascarón esférico conductor ideal de radio interno $a$ y radio externo $b$. Este cascarón está cargado con una carga $Q$. El interior del cascarón ($r < r_a$) es vacío. Para esta configuración:

- **a)** Determinar cómo se distribuye la carga eléctrica en el conductor, indicando claramente su posición y densidad.
- **b)** Hallar el campo eléctrico $\vec{E}$ para todo el espacio. Teniendo en cuenta la configuración, ¿puede saberse de antemano si $\vec{E}$ es nulo en alguna zona?
- **c)** Hallar el potencial en todo el espacio.
- **d)** Si ahora el conductor se conecta a tierra, indicar cómo se modifican los resultados de los puntos anteriores.

#### Resolución
##### Punto a
Para el punto a, hay que considerar que en cualquier conductor en equilibrio electroestático, la carga se distribuye uniformemente en la superficie. Sin embargo, este cascarón tiene dos superficies, la cara externa ($r=r_{b}$) y la superficie interna ($r=r_{a}$), ¿cambia esto en algo la distribución de la carga?

No. La carga se distribuye uniformemente exclusivamente sobre la  cara externa. Esto sucede porque si las cargas quieren estar lo más alejadas posible unas de otras, irse a la cara interna (de radio menor) las obligaría a estar más juntas que si se van todas a la cara externa (de radio mayor). La cara externa $r_b$ es el límite absoluto de la pieza para alejarse.

Entonces, nos queda que la carga y la densidad es igual a:

$$
\begin{align}
A_{b} &  = 4\pi r_{b}^2 \\
Q_{\text{total}}  & = Q_{a} + Q_{b} = 0 + Q_{b}  \\
\sigma  & =\frac{Q_{total}}{A_{\text{b}}} = \frac{Q}{4 \pi r_{b}^2} \\
\end{align}
$$

Al usar una superficie gaussiana esférica de radio $r$ concéntrica al cascarón, tendremos que:
- Cuando $r < r_{a}$, nos encontramos sobre el vacío, donde la carga encerrada es nula, y por tanto, el campo eléctrico en $r<r_{a}$ será nulo y el potencial será constante.
- Cuando $r_{a} < r < r_{b}$, la carga encerrada también es nula,  y por tanto, el campo eléctrico en $r_{a}<r<r_{b}$ será nulo y el potencial será constante.
- Cuando $r > r_{b}$, la carga encerrada es $Q_{\text{total}}$, y $Q_{tot} = \sigma*A_{total}$.donde $Q_{\text{total}} = \sigma*A_{\text{total}}$, y por ley de gauss, $Q = \Phi_{E}*\epsilon_{0} = \epsilon_{0}\int \vec{E} *d \vec{A_{\text{total}}}=\epsilon_{0} EA_{1} = \epsilon_{0} E 4\pi (r_{b}^2)$

##### Por que la carga en un conductor reside unicamente sobre la superficie externa

Los electrones libres (o las cargas libres, si asumimos $Q$ positiva) experimentan una fuerza de repulsión eléctrica entre ellos. Se van a empujar y mover hasta que estén lo más separados posible, momento en el cual la fuerza neta sobre cada uno de ellos se vuelve cero. Si la fuerza es cero, significa que el campo eléctrico dentro del material también es cero ($E=0$). A ese estado le llamamos equilibrio electrostático.

> Si coloco a una carga puntual en el centro del material conductor entre $r_a$ y $r_b$, ¿no experimentaria fuerzas de repulsion por parte de las cargas en la superficie del conductor? Por que entonces dices que la fuerza neta en cada una de las cargas seria 0.

La respuesta corta y al pie es: **Sí, esa carga puntual experimentaría fuerzas de repulsión por parte de TODAS las cargas en la superficie.**

El secreto, que a veces vuela un poco la cabeza, no es que las fuerzas individuales no existan, sino que **la suma vectorial de todas esas infinitas fuerzas da exactamente cero.** A esto se lo conoce (tanto en gravedad como en electromagnetismo) como el **Teorema de los Cascarones** (o _Shell Theorem_).

Pensalo con esta imagen mental:

Imaginá que colocás tu carga de prueba cerca del borde interno (cerca de $r_a$).

1. Por un lado, tenés un "pedacito" de la superficie cargada que está **muy cerca**. Como está cerca, la fuerza de repulsión que ejerce es **muy fuerte** (empujando hacia el centro).
    
2. Por otro lado, del lado opuesto del cascarón, tenés cargas que están **muy lejos**. Como están lejos, su fuerza de repulsión individual es más débil. **Pero**, como mirás hacia un área mucho más grande del cascarón lejano, hay **mucha más cantidad de carga** empujando en sentido contrario.
    

La magia geométrica de nuestro universo (y de la Ley de Coulomb) es que la fuerza disminuye con el cuadrado de la distancia ($1/r^2$), mientras que el área de la superficie esférica aumenta exactamente con el cuadrado de la distancia ($r^2$). ¡Se cancelan perfectamente! La enorme cantidad de cargas lejanas y débiles empujan con exactamente la misma fuerza neta que las poquitas cargas cercanas y fuertes. El resultado es que la carga de prueba se queda quieta: fuerza neta cero, campo eléctrico nulo.

##### Punto b

El campo eléctrico en esta configuración en cualquier punto $r>r_{b}$ no tiene una preferencia horizontal, contando unicamente con una dirección radial desde el centro del cascarón. 

Al usar una superficie gaussiana esférica de radio $r$ concéntrica al cascarón y teniendo en cuenta lo discutido en el punto a, podemos aprovechar la simetría y definir al campo eléctrico $\vec{E}$ como una función a tramos que depende exclusivamente de r. De tal forma que:
- Cuando $r < r_{a}$, nos encontramos sobre el vacío, donde la carga encerrada es nula, y por tanto, el campo eléctrico en $r<r_{a}$ será nulo y el potencial será constante.
- Cuando $r_{a} < r < r_{b}$, la carga encerrada también es nula, y por tanto, el campo eléctrico en $r_{a}<r<r_{b}$ será nulo y el potencial será constante.
- Cuando $r > r_{b}$, la carga encerrada es $Q_{\text{total}}$, y $Q_{tot} = \sigma*A_{total}$.donde $Q_{\text{total}} = \sigma*A_{\text{total}}$, y por ley de gauss podemos obtener el campo eléctrico:

$$
\begin{align}
\Phi_{E} =  & \oint \vec{E} d \vec{A} = \oint EdA = E 4 \pi r^2 \\
E 4\pi r_{b}^2  & = \frac{Q_{\text{total}}}{\epsilon_{0}} \\
E  & = \frac{Q_{\text{total}}}{\epsilon_{0} 4\pi r^2} 
\end{align}
$$

Entonces, nos queda que:

$$
\vec{E}(r) = \begin{cases} 
0 & \text{si } r < r_{a} \\
0 & \text{si } r_{a} < r < r_{b} \\
\frac{Q_{\text{total}}}{4\pi\epsilon_{0}r^2} \hat{r} & \text{si } r > r_{b}
\end{cases}
$$

##### Punto c
Para hallar el potencial en todo punto del espacio, utilizamos la relación:

$$
\begin{align}
V_{a}-V_{b} = \int_{a}^b \vec{E} \cdot d \vec{l}
\end{align}
$$

Tomando como referencia $V=0$ en el infinito, entonces tenemos que para cualquier punto a:

$$
\begin{align}
V(r) &  = V_{r}-0 = \int_{r}^{\infty} \vec{E} d \vec{l} = \int_{r}^{\infty} Edr \\
V(r)  & = - \int_{\infty}^{r} Edr 
\end{align}
$$

Diferenciando por casos, tenemos que:
- Cuando $r>r_{b}$, entonces $E  = \frac{Q_{\text{total}}}{\epsilon_{0} 4\pi r^2}$:

$$
\begin{align}
V(r) & = - \frac{Q_{\text{total}}}{\epsilon_{0} 4\pi}  \int_{\infty}^r \frac{1}{r^2} dr  \\
 & = - \frac{Q_{\text{total}}}{\epsilon_{0} 4\pi} \left. \frac{-1}{r} \right|_{\infty}^r \\
  V(r) & =  \frac{Q_{\text{total}}}{\epsilon_{0} 4\pi r}
\end{align}
$$

- Cuando $r_{a}<r<r_{b}$ , entonces $E= 0$ y el potencial puede calcularse fragmentando el recorrido de la integral:

$$
  \begin{align}
  V(r)  & = - \int_{\infty}^{r} Edr  \\
   & = - (\int_{\infty}^{r_{b}} Edr + \int_{r_{b}}^{r} Edr)
  \end{align}
$$

Usando los resultados obtenidos en el anterior punto, tenemos que el valor de la primera integral es: $\frac{Q_{\text{total}}}{\epsilon_{0} 4\pi r_{b}}$. Para la segunda integral, sabemos que el valor del campo eléctrico es nulo y por tanto el resultado se reduce a 0. Tenemos entonces que en esta región el potencial es constante, con valor: $V(r) =   \frac{Q_{\text{total}}}{\epsilon_{0} 4\pi r_{b}}$.
- Cuando $r<r_{a}$ , entonces $E= 0$ y el potencial puede calcularse fragmentando el recorrido de la integral:
$$
  \begin{align}
  V(r)  & = - \int_{\infty}^{r} Edr  \\
   & = - (\int_{\infty}^{r_{b}} Edr + \int_{r_{b}}^{r_{a}} Edr +  \int_{r_{a}}^{r} Edr)
  \end{align}
  $$

Usando los resultados obtenidos en el anterior punto, tenemos que el valor resultado de las primeras dos integrales se reduce a $\frac{Q_{\text{total}}}{\epsilon_{0} 4\pi r_{b}}$. Para la tercera integral, sabemos que el valor del campo eléctrico es nulo y por tanto el resultado se reduce a 0. Tenemos entonces que en esta región el potencial es constante, con valor: $V(r) =   \frac{Q_{\text{total}}}{\epsilon_{0} 4\pi r_{b}}$.

Entonces, nos queda que:

$$
V(r) = \begin{cases} 
\frac{Q_{\text{total}}}{\epsilon_{0} 4\pi r_{b}} & \text{si } r < r_{a} \\
\frac{Q_{\text{total}}}{\epsilon_{0} 4\pi r_{b}} & \text{si } r_{a} < r < r_{b} \\
\frac{Q_{\text{total}}}{\epsilon_{0} 4\pi r} & \text{si } r > r_{b}
\end{cases}
$$

##### Punto d

Exploremos qué significa conectar un conductor a tierra y lo que implica para el potencial: ¿qué condición impone obligatoriamente al potencial $V$ del cascarón el hecho de conectarlo a "tierra"?
Intutitivamente, pienso que conectar un conductor a tierra permite que los electrones libres de la superficie en el cascarón escapen, de forma que se neutraliza la carga en el conductor. Es decir, la carga libre en el conductor pasaría a ser 0. Al conectar el conductor a "tierra", lo estás uniendo a un reservorio gigantesco (prácticamente infinito) de cargas. Los electrones van a fluir libremente desde o hacia la Tierra hasta que el sistema alcance un nuevo estado de equilibrio electrostático.

La **condición matemática obligatoria** que representa este fenómeno es que ambos cuerpos (el cascarón y la Tierra) deben quedar al mismo potencial eléctrico. Pero, ¿por qué?

Si conectás tu cascarón conductor a la Tierra mediante un cable metálico, estás uniendo dos conductores. Si hubiera una diferencia de potencial entre ellos ($\Delta V \neq 0$), eso implicaría obligatoriamente que existe un campo eléctrico $\vec{E}$ a lo largo de ese cable. Ese campo eléctrico funcionaría como una "bomba de agua", empujando a los electrones libres de la superficie de tu cascarón para que viajen por el cable.

Las cargas se van a mover (se escapan del cascarón o suben desde la Tierra) hasta que el campo eléctrico en el cable desaparezca. Y para que desaparezca, la diferencia de potencial debe ser nula ($\Delta V = 0$). Es decir, el sistema alcanza un nuevo equilibrio electrostático **solo cuando ambos cuerpos tienen exactamente el mismo potencial**.

**¿Y por qué el potencial de la Tierra es cero?** En física, asumimos que la Tierra es un conductor infinitamente grande, capaz de absorber o entregar cualquier cantidad de carga sin que su propio potencial se modifique. Por convención universal, fijamos ese nivel inalterable de la Tierra en $0\text{ V}$.

Por tanto, cuando conectamos el conductor a tierra, tenemos que:
$V(r)=0$ y $E(r) = 0$ en todos los puntos del espacio, dado que no hay más carga encerrada.

---

### 2)

Tres cargas puntuales se encuentran fijas en un plano, como indica la figura. Las cargas $q_{1}$ y $q_{2}$ valen $1 \mu \mathrm{C}$ cada una. La carga $q_{3}$ es desconocida. Dato: $a=1 \mathrm{~cm}$.
Disposición de cargas en un plano xy:

$$
\begin{align}
q_{1} = (0,a) \\
q_{2} = (a, 0) \\
q_{3} = (0,0) \\
A = (a,a)
\end{align}
$$

![Pasted image 20260513124604](../assets/Pasted%20image%2020260513124604.png)


- **a)** ¿Qué valor debe tomar $q_{3}$ para que el campo eléctrico en el punto $A$ sea nulo?
- **b)** Con el valor de carga $q_{3}$ calculado en **a)**, ¿cuál es el trabajo que debe realizarse externamente (contra el campo) para traer otra carga igual a $q_{3}$ desde el infinito hasta el punto $A$?
- **c)** Se reemplaza la carga $q_{3}$ del punto $O$ por un hilo muy largo, uniformemente cargado con densidad lineal $\lambda$, ubicado en la dirección perpendicular al plano de la figura. ¿Cuánto debe valer $\lambda$ para que, como en el punto **a)**, el campo eléctrico en el punto $A$ sea nulo?

#### Resolución
##### Punto a
![Pasted image 20260519093949](../assets/Pasted%20image%2020260519093949.png)
Para resolver este punto, usaremos la ley de coulomb para el caso de varias cargas puntuales y el principio de superposición de campos eléctricos. Tenemos entonces que en el punto A, donde la distancia r entre A y $q_1$ y $q_2$ es $a$, y la distancia entre A y $q_3$ es $\sqrt{ a^2 + a^2 } = \sqrt{ 2 }a$ el campo eléctrico total percibido es:

$$
\begin{align}
\vec{E}  & = \vec{E_{1}} + \vec{E_{2}} + \vec{E_{3}} = E_{x} \hat{i} + E_{y} \hat{j} = 0\\
\end{align}
$$

Calculando la ecuación por componentes, tenemos:

$$
\begin{align}
E_{x}  & = E_{1x} + E_{2x} + E_{3x} \\
E_{y}  & = E_{1y} + E_{2y} + E_{3y} \\
E_{x}  & = \frac{q_{1}}{4 \pi \epsilon_{0}a^2}  + \frac{q_{3}}{4 \pi \epsilon_{0}(\sqrt{ 2 }a)^2}\cos(45^\circ) \\
E_{y}  & = \frac{q_{2}}{4 \pi \epsilon_{0}a^2} + \frac{q_{3}}{4 \pi \epsilon_{0}(\sqrt{ 2 }a)^2}\sin(45^\circ) \\
\end{align}
$$

Teniendo en cuenta que buscamos que $\vec{E} =0$ , entonces despejamos $q_{3}$ de una de las dos ecuaciones:

$$
\begin{align}
E_{x}  =  & \frac{q_{1}}{4 \pi \epsilon_{0}a^2}  + \frac{q_{3}}{4 \pi \epsilon_{0}(\sqrt{ 2 }a)^2}\cos(45^\circ) = 0 \\
q_{3} =  & -\frac{q_{1}(8\pi \epsilon_{0}a^2)}{4\pi \epsilon_{0}a^2 \cos{45^\circ}}  \\
q_{3} =  & -\frac{2}{\cos{45}}q_{1} = -\frac{4}{\sqrt{2}}q_{1} = -2\sqrt{ 2 }q_{1}
\end{align}
$$

Reemplazando los valores $a = 0.01m$ y $q_{1} = 1 \mu C = 1 \cdot 10^{-6}C$, entonces obtenemos $q_{3}$:

$$
\begin{align}
q_{3} =  &  -2\sqrt{ 2 }q_{1} \\

q_{3} =  & - -2\sqrt{ 2 } (1 \cdot 10^{-6}C) \\
q_{3} = & - -2\sqrt{ 2 } \mu C
\end{align}
$$

##### Punto b

"""
- When a particle moves from point a to b point the work done on it by the electric field is $W_{a\to b} = -\Delta U = U_{a}-U_{b}$.Thus the potential-energy difference $U_{a}-U_{b}$ equals the work that is done by the electric force when the particle moves from a to b. Equivanlently, the potential-energy difference $U_{a} - U_{b}$ is then defined as the work $W_{\text{ext}}$ that must be done by an external force to move the particle slowly from $b$ to $a$ against the electric force, that is $\Delta U$. 
- the potential of a with respect b to equals the work done by the electric force when a UNIT charge moves from a to b. Equivalently, the potential of a with respect to b equals the work that must be done to move a UNIT charge slowly from to against the electric force.
"""

Para resolver este punto, utilizamos la relación que existe entre el trabajo realizado por una fuerza externa para mover una carga desde  un punto b hasta a un punto a contra el campo eléctrico y el diferencial de energía potencial eléctrica:

$$
\begin{align}
W_{ext} = \Delta U_{b \to a}= U_{a}-U_{b}
\end{align}
$$

Esto es equivalente a calcular el trabajo realizado por la fuerza del campo eléctrico al mover una carga desde punto a hasta el punto b.

$$
\begin{align}
W_{a\to b} = - \Delta U_{a \to b} = U_{a}-U_{b} \\
\end{align}
$$

Si usamos $q_{3}$ como carga de prueba, podemos afirmar que $U = V q_{3}$.  Por tanto: 

$$
\begin{align}
W_{\text{ext}} = - \Delta U = q_{3}V_{a}-q_{3}V_{b} \\
\end{align}
$$

En este punto en particular, nuestro punto de partida $b= \infty$ y $a=A$. Si definimos el potencial en el infinito como cero $V_{\infty}=0$, entonces nuestra expresión del trabajo se convierte en:

$$
\begin{align}
W_{\text{ext}} =  q_{3}V_{a} \\
\end{align}
$$

Por último, podemos calcular el potencial en el punto A usando la sumatoria de potenciales debidos a una colección de cargas puntuales:

$$
\begin{align}
V_{a} & = \frac{1}{4 \pi \epsilon_{0}}\sum_{i} \frac{q_{i}}{r_{i}} \\
V_{a} & = \frac{1}{4 \pi \epsilon_{0}} \left( \frac{q_{1}}{a}  + \frac{q_{2}}{a}  + \frac{q_{3}}{\sqrt{2}a}\right)
\end{align}
$$

Usando esta expresión de $V_{a}$ en nuestra expresión del trabajo, tenemos: 

$$
\begin{align}
W_{\text{ext}} =  q_{3}V_{a} = q_{3}  \frac{1}{4 \pi \epsilon_{0}} \left( \frac{q_{1}}{a}  + \frac{q_{2}}{a}  + \frac{q_{3}}{\sqrt{2}a}\right)\\
\end{align}
$$

Reemplazamos valores y calculamos:

$$
\begin{align}
W_{\text{ext}}  &  = -2\sqrt{2 } \cdot 10^{-6}C  \frac{1}{4 \pi \epsilon_{0}} \left( \frac{2\cdot 10^{-6}C}{0.01m}  + \frac{-2 \sqrt{ 2 }\cdot 10^{-6}C}{\sqrt{2} \cdot 0.01m}\right)\\
W_{\text{ext}} & = 0
\end{align}
$$

Significa que durante el trayecto de la carga desde el infinito hasta $A$, en algunas partes del camino tu mano tuvo que empujar _contra_ la repulsión de $q_3$ (hiciste trabajo positivo), pero en otras partes del camino la atracción de $q_1$ y $q_2$ hizo el trabajo por vos "chupando" a la carga (trabajo negativo). Al llegar al punto $A$, la suma de todo lo que empujaste y todo lo que te dejaste arrastrar dio exactamente cero. El campo eléctrico no se "quedó" con nada de tu energía.

##### Punto c

Para resolver este punto, seguimos usando el principio de superposición de campos eléctricos. Entonces tenemos que para el punto A, el campon eléctrico total es:

$$
\begin{align}
\vec{E}  & = \vec{E_{1}} + \vec{E_{2}} + \vec{E_{\lambda}} = E_{x} \hat{i} + E_{y} \hat{j} = 0\\
\end{align}
$$

Sabemos que para un hilo muy largo uniformemente cargado, el campo eléctrico es radial, sin preferencia horizontal debido a la simetría. Entonces, si usamos un cilindro concéntrico al hilo como superficie gaussiana de largo l, tenemos que el flujo eléctrico viene dado por:

$$
\begin{align}
\Phi_{E} & = \oint \vec{E}d \vec{A} = E\oint dA= EA=E 2 \pi rl \\
\Phi_{E} & = E 2 \pi rl = \frac{Q_{\text{encl}}}{\epsilon_{0}} \\
E & = \frac{Q_{\text{encl}}}{\epsilon_{0}2\pi rl}
\end{align}
$$

Finalmente, reemplazando con $Q_{\text{encl}}=\lambda l$, tenemos:

$$
\begin{align}
E & = \frac{Q_{\text{encl}}}{\epsilon_{0}2\pi rl} = \frac{\lambda}{\epsilon_{0}2\pi r} \\
\vec{E} &  = \frac{\lambda}{\epsilon_{0}2\pi r} \vec{r}
\end{align}
$$

Usando este valor dentro de nuestra ecuación superponiendo los campos eléctricos, tenemos:

$$
\begin{align}
E_{x}  & = E_{1x} + E_{2x} + E_{\lambda x} \\
E_{x}  & = \frac{1}{4\pi\epsilon_{0}}\left( \frac{q_{1}}{a^2}+ 0 \right) +\frac{\lambda}{\epsilon_{0}2\pi \sqrt{2 }a}\cos{45^\circ} \\
\end{align}
$$

Y para $E_{y}$, obtenemos una expresión muy similar:

$$
\begin{align}
E_{y}  & = E_{1y} + E_{2y} + E_{\lambda y} \\
E_{y}  & = \frac{1}{4\pi\epsilon_{0}}\left( 0+ \frac{q_{2}}{a^2} \right)  +\frac{\lambda}{\epsilon_{0}2\pi \sqrt{2 }a}\sin{45^\circ}\\
\end{align}
$$

Podemos despejar el valor de $\lambda$ de cualquiera de las dos ecuaciones. En este caso, usaremos la ecuación de $E_{y}$. Despejando $\lambda$, tenemos:

$$
\begin{align}
E_{y}  & = \frac{1}{4\pi\epsilon_{0}}\left(\frac{q_{2}}{a^2} \right) +\frac{\lambda}{\epsilon_{0}2\pi \sqrt{2 }a}\sin{45^\circ} =0  \\
\lambda & = -\frac{\epsilon_{0}2\pi \sqrt{2 }a}{4\pi\epsilon_{0} \sin{45^\circ}}\left(\frac{q_{2}}{a^2} \right) \\
\lambda & = -\frac{ \sqrt{2 }}{2\sin{45^\circ}a} q_{2} = -\frac{q_{2}}{a}\\
\lambda & =  \frac{-1 \cdot10^{-6}}{1 \cdot 10^{-2}} \frac{C}{m} = -1 \cdot 10^{-4} \frac{C}{m}
\end{align}
$$

---

### 3)

Se tiene un plano inclinado de ángulo $\alpha$ ($\alpha=30^{\circ}$). En la base hay un resorte ideal de constante elástica $k$ y longitud natural $l_{0}$, cuyo extremo está fijo a una pared ($k=50 \mathrm{~N} / \mathrm{m}, l_{0}=9 \mathrm{~cm}$). Una masa $m_{1}$ ($m_{1}=600 \mathrm{~g}$) se encuentra en el otro extremo del resorte, en equilibrio, como indica la figura. Suponga despreciable el rozamiento de las masas con el plano.

- **a)** Encontrar en un sistema de referencia adecuado, la posición de la masa $m_{1}$ en equilibrio.
- **b)** Una masa $m_{2}$ ($m_{2}=200 \mathrm{~g}$) se encuentra inicialmente en reposo en la parte superior del plano. En un dado instante, se libera y cae hacia la masa $m_{1}$. Calcular la energía mecánica y el impulso lineal de la masa $m_{2}$ justo antes de chocar con la masa $m_{1}$. ($H=48 \mathrm{~cm}$).
- **c)** Suponiendo que las masas quedan adheridas después del impacto, calcular cuánto es la máxima compresión del resorte.

#### Resolución

Primero recopilemos los datos que conocemos:

$$
\begin{align}
m_{1} &   = 0.6kg \\
m_{2} &   = 0.2kg \\
H  & = 0.48m \\
\alpha  & = 30^\circ \\
k  & = 50 \frac{N}{m} \\
l_{o}  & = 0.09m
\end{align}
$$

##### Punto a

Proponemos un plano donde el eje x es paralelo a la rampa (con dirección positiva a la izquierda) y el eje y es perpendicular (dirección positiva hacia arriba), con un origen situado en en el fondo de la rampa. 
![Pasted image 20260521100759](../assets/Pasted%20image%2020260521100759.png)
Por tanto, utilizando primera ley de newton, tenemos:

$$
\begin{align}
\sum F_{x} & =0 \\ \\
F_{e} - w_{\text{1}}\sin{\alpha} & =0 \\
k(l_{0}- x_{1}) - m_{1}g\sin{\alpha} & =0 \\
x_{1} &  = \frac{{kl_{0} - m_{1}g\sin{\alpha}}}{k} \\
x_{1} &  = \frac{50 \frac{N}{m} \cdot 0.09m - 0.6kg \cdot 10 \frac{m}{s^2} \sin{\alpha}}{50 \frac{N}{m}} \\
x_{1} &  = 0.03m
\end{align}
$$

##### Punto b
Definiendo a como el estado inicial del sistema y b como el estado del sistema en el que se encuentra la masa $m_{2}$ apunto de colisionar como $m_{1}$. En el recorrido de $m_{2}$ desde a hasta b, la única fuerza no conservativa actuando sobre la masa es $\vec{N_{2}}$, pero siendo que esta fuerza no ejerce trabajo sobre la particular al ser penperdicular a la trayectoria durante todo el recorrido, tenemos que se conserva la energía mecánica de la partícula. Definamos entonces la energía mecánica en ambos estados.
Para definir la energía potencial gravitatoria, definimos un punto de referencia. El punto de referencia será el suelo con $h=0$. Entonces $h_{a} = H$ y $h_{b} = x_{1}\cdot \sin{\alpha}$. Definamos la energía para el estado a:

$$
\begin{align}
E_{2a} & = K_{2a} + U_{2a} \\
E_{2a} & = m_{2}gH \\
E_{2a} & = E_{2b} = 0.2kg \cdot \frac{10m}{s^2}\cdot 0.48m \\
E_{2a} & = E_{2b} =0.96J
\end{align}
$$

Para calcular el impulso lineal, usamos la relación:

$$
\begin{align}
\vec{J} = \Delta p = p_{2b}-p_{2a} \\
\end{align}
$$

Siendo que $m_{2}$ parte del reposo, tenemos que:

$$
\begin{align}
\vec{J} = m_{2}\vec{v_{2b}}
\end{align}
$$

Obtenemos $v_{2b}$ de la expresión de $E_{2b}$:

$$
\begin{align}
E_{2b} &  = E_{a} = 0.96J \\
E_{2b} &  = \frac{1}{2}m_{2b}v_{2b}^2  + m_{2}gh_{b} = 0.96J \\
E_{2b} &  = \frac{1}{2}0.2kg \cdot v_{2b}^2  + 0.2kg \cdot 10 \frac{m}{s^2} \cdot 0.03m \cdot \sin{\alpha} = 0.96J \\ \\
|v_{2b}|  & = \sqrt{\frac{{ 0.96J - 0.2kg \cdot 10 \frac{m}{s^2} \cdot 0.03m \cdot \sin{\alpha}}}{0.1kg}} \\
|v_{2b}|  & = 3.05 \frac{m}{s}
\end{align}
$$

Dado nuestro sistema de referencia, definimos $\vec{v_{2b}} = -3.05 \frac{m}{s} \hat{i}$. Usamos esta expresión para calcular el impulso:

$$
\begin{align}
\vec{J} &  = m_{2}\vec{v_{2b}} = 0.2kg \cdot -3.05 \frac{m}{s} \hat{i} \\
\vec{J}  & = -0.61 \frac{kg \cdot m}{s} \hat{i}
\end{align}
$$

##### Punto c
Para resolver este punto, añadimos dos nuevos estados al sistema:
- Estado c: instante inmediatamente después que las masas colisionan. Ambas masas quedan adheridas. La velocidad resultante de las masas fusionadas es $V_{Tc}$ y la masa total es $m_{T}=m_{1} + m_{2}$.
- Estado d: Instante en el que se alcanza máxima compresión del resorte, con $x_{max}$ denotando este valor.
Entre el estado b y c, es decir, durante la colisión, el momento lineal se conserva. Entre el estado c y d, la energía mecánica se conserva. Utilizaremos estas nociones.
Empezemos obteniendo la velocidad $V_{Tc}$ a través de la conservación del momento lineal:

$$
\begin{align}
\vec{p_{b}} &  = \vec{p_{c}} \\
m_{2} \vec{v_{2c}}  & = m_{T} \vec{v_{Tc}} \\
\vec{v_{Tc}} & = \frac{m_{2} \vec{v_{2c}}}{m_{1} + m_{2}} \\
\vec{v_{Tc}} & = \frac{0.2kg  \cdot -3.05 \frac{m}{s} \hat{ i}}{0.8kg} \\
\vec{v_{Tc}}  & = -0.76 \hat{i}
\end{align}
$$

Ahora expresamos la conservación de energías mecánicas entre c y d:

$$
\begin{align}
E_{c} &  = E_{d} \\
\frac{1}{2}m_{T}v_{Tc}^2 + m_{T}gh_{c} + \frac{1}{2}k(l_{0}- x_{c})^2  & = m_{T}gh_{d} + \frac{1}{2}k(l_{0}- x_{max})^2 \\
\frac{1}{2}m_{T}v_{Tc}^2 + m_{T}gh_{c} + \frac{1}{2}k(l_{0}- x_{c})^2  & = m_{T}gx_{max}\sin{\alpha} + \frac{1}{2}k(l_{0}^2 -2l_{0}x_{max}+x_{max}^2)
\end{align}
$$

Agrupando la ecuación por términos:

$$
\begin{align}
x_{max}^2\left( \frac{1}{2}k \right) +x_{max}(m_{T}g\sin{\alpha}-kl_{0}) & + \frac{kl_{0}^2}{2} - (\frac{1}{2}m_{T}v_{Tc}^2 + m_{T}gh_{c} + \frac{1}{2}k(l_{0}- x_{c})^2) = 0
\end{align}
$$

Reemplazando por los valores pertinentes ($h_{c}=x_{c}\sin{\alpha}$ y $x_{c}=x_{b}=0.03m$), tenemos:

$$
\begin{align}
\frac{25N}{m} x_{max}^2 - 0.5 N x_{max} - 0.24J &  = 0
\end{align}
$$

Las soluciones a la ecuación son:

$$
\begin{align}
x_{1}  & = 0.11m \\
x_{2} & = -0.09m
\end{align}
$$

La primera solución no hace sentido físico, mientras que la segunda sugiere que las masas terminan impactando con la base de la rampa. Por tanto, para este problema se propone $x_{max}=0m$ y por ende la compresión máxima termina siendo la longitud natural del resorte $l_{0} = 9cm$.
![Pasted image 20260511181345](../assets/Pasted%20image%2020260511181345.png)

## Intento
### Ejercicio 1
#### Punto A
Al tratarse de un conductor ideal sin una carga dentro de la cavidad interna, la carga $Q$ se distribuye uniformemente sobre la superficie externa (de radio $r_{b}$). Por tanto, la densidad de carga resultante es:

$$
\begin{align}
\sigma  & = \frac{Q}{A_{B}} = \frac{Q}{4 \pi r_{B}^2}
\end{align}
$$

#### Punto B
Dividamos nuestro analisis por secciones:
- $0<r<r_{A}$: considerando la cavidad interna ($r<r_{A}$), usando una superficie gaussiana $0<r< r_{a}$, la carga encerrada es nula, y la ley de Gauss dicta entonces que el campo eléctrico debe ser nulo.
- $r_{A} < r < r_{B}$: Sabemos que en el volumen interno del conductor, el campo eléctrico $\vec{E} =0$. Dado que si no fuera así, las cargas se moverían. Por tanto, para $r_{A}< r < r_{B}$, $\vec{E}=0$. 
- $r>r_{B}$: Acá aprovechamos la simetría que ofrece una superficie esférica gaussiana con radio r concéntrica a la esfera original, en donde el campo eléctrico mantendrá una dirección perpendicular a esta misma en todos los puntos. Por tanto la ley de Gauss dicta que $EA = \frac{Q}{\epsilon_{0}} \implies E = \frac{\sigma4\pi r_{B}^2}{\epsilon_{0}4\pi r^2} = \frac{\sigma r_{B}^2}{\epsilon_{0}r^2}a= \frac{Q}{4\pi \epsilon_{0}r^2}$.
Finalmente, entonces tenemos que:

$$
\vec{E}(r) = \begin{cases}
0 &\text{si} & 0<r<r_{B} \\
\frac{\sigma r_{B}^2}{\epsilon_{0}r^2}  = \frac{Q}{4\pi\epsilon_{0}r^2} &\text{si} & r\geq r_{B}
\end{cases}
$$

#### Punto C
Para hallar el potencial, dividimos por secciones:
Cuando $r>r_{B}$, el campo eléctrico resultante es idéntico al de una carga puntual ubicada en el centro, usamos esto para calcular el potencial resultante directamente: 

$$
\begin{align} \\
V(r) = \frac{Q}{4\pi\epsilon_{0}r} 
\end{align}
$$

Cuando $r<r_{B}$, el campo eléctrico es 0, esto significa que el potencial es contante y por tanto $V = \frac{Q}{4 \pi \epsilon_{0} r_{B}}$. 
Entonces la expresión final es:

$$
V(r) = \begin{cases}
\frac{Q}{4\pi \epsilon_{0} r_{B}} & \text{si} & r < r_{B} \\
\frac{Q}{4\pi \epsilon_{0} r} & \text{si} & r\geq r_{B} 
\end{cases}
$$

#### Punto D
Conectar el conductor a tierra implica darle via libre a la carga acumulada en la superficie del conductor para que "escapen". Naturalmente, esto induce a que el conductor se descargue, y termine con una carga neta Q = 0. Tanto el campo eléctrico como el diferencial de potencial terminan con $\vec{E} = 0$ y $V=0$ para todos los casos.

### Ejercicio 2

#### Punto A
Tenemos las siguientes posiciones en el plano cartesiano:

$$
\begin{align}
\vec{r_{1}} = (0,a)  \\ 
\vec{r_{2}} = (a,0) \\
\vec{r_{3}} = (0,0) \\
\vec{r_{A}} = (a, a)
\end{align}
$$

Se nos pide que el campo eléctrico $\vec{E_{A}}$ resultante en el punto A sea 0, por tanto planteamos superposición:

$$
\begin{align}
\vec{E_{A}} & = \vec{E_{1}} +\vec{E_{2}} + \vec{E_{3}} = 0
\end{align}
$$

Definimos las direcciones de cada vector:

$$
\begin{align}
\vec{\Delta r}  & = (x_{f}-x_{i})\hat{i} + (y_{f}-y_{i})\hat{j} = \Delta x \hat{i} + \Delta y \hat{j} \\
\vec{r_{i \to A}}  & = \vec{\Delta r_{Ai}}  \\
\vec{u}_{i\to A}  & = \frac{\Delta x}{|r|} \hat{i} + \frac{\Delta y}{|r|} \hat{j} \\
\vec{E_{i}}  & = \frac{q_{i}}{4 \epsilon_{0}\pi r^2}(\frac{\Delta x}{|r|} \hat{i} ) + \frac{q_{i}}{4 \epsilon_{0}\pi r^2}(\frac{\Delta y}{|r|} \hat{j} ) \\ 
\end{align}
$$

Teniendo en cuenta que $|r| = \sqrt{ \Delta x^2 + \Delta y^2}$, tenemos la expresión resultante:

$$
\vec{E_{i}} = \frac{q_{i} \Delta x}{4 \epsilon_{0}\pi ( \Delta x^2  + \Delta y ^2 )^{\frac{3}{2}} } \hat{i}+ \frac{q_{i} \Delta y}{4 \epsilon_{0}\pi( \Delta x^2  + \Delta y ^2 )^{\frac{3}{2}} } \hat{j} \\ 
$$

Calculamos los campos resultantes para cada carga, teniendo en cuenta $r$ para cada caso:
- $r_{1} = \sqrt{ a^2 } =a$
-  $r_{2} = \sqrt{ a^2 } =a$
-  $r_{3} = \sqrt{ 2a^2 } =\sqrt{2}a$

$$
\begin{align}
\vec{E_{1}}  & = \frac{q_{1}(a)}{4 \pi \epsilon_{0}(a^2)^{3/2}} \hat{i} = \frac{q_{1}}{4 \pi \epsilon_{0}a^2} \hat{i} \\
\vec{E_{2}} & = \frac{q_{2}(a)}{4 \pi \epsilon_{0}(a^2)^{3/2}} \hat{j} = \frac{q_{2}}{4 \pi \epsilon_{0}a^2} \hat{j} \\
\vec{E_{3}} & = \frac{q_{3}}{8 \pi \epsilon_{0}\sqrt{2} a^2} \hat{i} + \frac{q_{3}}{8 \pi \epsilon_{0}\sqrt{2} a^2} \hat{j}  \\
\end{align}
$$

Planteamos la ecuación con uno de los dos ejes y tenemos:

$$
\begin{align}
E_{1x} = 0  & =  \frac{q_{1}}{4 \pi \epsilon_{0}a^2} + \frac{q_{3}}{8 \pi \epsilon_{0}\sqrt{2} a^2} \\
q_{3}  & = -2 \sqrt{ 2 }q_{1}   = -2\sqrt{ 2 } \mu C \\
\end{align}
$$

#### Punto B

Planteando $U_{\infty} =0$, usamos la relación:

$$
\begin{align}
W_{\text{ext} q_{0}}  & = \Delta U = U_{A} - U_{\infty} = U_{A}\\
W_{\text{ext}}   & = \frac{q_{0}}{4\pi \epsilon_{0}} \sum_{i} \frac{q_{i}}{r_{i}} \\
W_{\text{ext}}   & = \frac{q_{0}}{4\pi \epsilon_{0}} \left( \frac{q_1}{a} + \frac{q_{2}}{a} + \frac{q_{3}}{\sqrt{ 2 }a}  \right) \\
W_{\text{ext}}  & = 0\\
\end{align}
$$

No hay que hacer trabajo neto alguno, dado que en partes del trayecto la fuerza externa empuja contra el campo eléctrico y en otras es ayudado por el campo, por lo que debe hacer trabajo negativo. Al final el trabajo neto termina siendo 0.

#### Punto C

Al posicionar un hilo O muy largo perpendicular al planos, nos encontramos que la superposición de campos buscada sigue siendo igual a 0, $\vec{E_{3}}$ es distinta:

$$
\begin{align}
\vec{E_{A}} & = \vec{E_{1}} +\vec{E_{2}} + \vec{E_{3}} = 0
\end{align}
$$

donde $\vec{E_{3}}$ resulta del campo generado por un hilo. Se sabe que el campo electrico generado por un hilo infinito es radial al hilo, sin preferencia horizontal. Usando una superficie gaussiana cilindrica de largo l concentrica al hilo, aprovechamos la simetria para simplificar el despeje del campo usando la ley de Gauss:

$$
\begin{align}
\int \vec{E} \cdot d \vec{A} &  = E \int dA = E 2\pi rl = \frac{Q}{\epsilon_{0}} \\
\end{align}
$$

Por tanto: $E_{3} = \frac{Q}{\epsilon_{0}2 \pi rl}$, donde $Q = \lambda l$, dando como resultado $E_{3}=\frac{\lambda}{\epsilon_{0}2 \pi r}$. Ahora planteamos la dirección del campo:

$$
\begin{align}
\vec{u_{3\to A}} = \frac{\Delta x}{r} \hat{i} + \frac{\Delta y}{r} \hat{j} \\
\vec{E_{3}} = \frac{\lambda}{\epsilon_{0}2 \pi r} \frac{\Delta x}{r} \hat{i} + \frac{\lambda}{\epsilon_{0}2 \pi r} \frac{\Delta y}{r} \hat{j}   \\
\vec{E_{3}} = \frac{\lambda}{\epsilon_{0}4 \pi a }(\hat{i} + \hat{j} )
\end{align} $$

Usamos este valor para la superposicion:

$$
\begin{align}
0  & = \frac{q_{1}}{4 \pi \epsilon_{0}a^2}( \hat{i} + \hat{j}) + \frac{\lambda}{\epsilon_{0}4 \pi a }(\hat{i} + \hat{j} ) \\
\lambda & = -\frac{q_{1}\epsilon_{0}4\pi a}{4\pi\epsilon_{0}a^2} = -\frac{q_{1}}{a} =  1 \times 10 ^{-4} \frac{C}{m}
\end{align}
$$

### Ejercicio 3

![Pasted image 20260528160437](../assets/Pasted%20image%2020260528160437.png)
#### Punto A
#### Punto B
#### Punto C

### Ejercicio 4: Cascarón Esférico con Carga Interna
#### Enunciado

Se tiene un cascarón esférico conductor ideal de radio interno $a$ y radio externo $b$, que posee una carga neta nula ($Q_{neta} = 0$). En el centro exacto de la cavidad vacía ($r = 0$), se encuentra fijada una carga puntual $+q$.

- **a)** Determina detalladamente cómo se distribuye la carga en las superficies interna ($r=a$) y externa ($r=b$) del cascarón conductor. Justifica físicamente.
- **b)** Halla el campo eléctrico $\vec{E}$ para todo el espacio.
- **c)** Halla el potencial eléctrico $V(r)$ en todo el espacio asumiendo que $V \to 0$ cuando $r \to \infty$.
### Resolucion

#### Punto a

Imaginemos una superficie gaussiana concentrica al conductor, de radio r, de tal forma que $r_{a}<r<r_{b}$. Para que el campo eléctrico en el conductor en el interior sea 0 (condicion obligatoria para un conductor en condiciones electroestaticas), obligatoriamente una carga $-q$ se debe posicionar en la superficie interna $r_{A}$ del conductor. Además, debido a la conservación de la carga dentro del conductor, la superficie externa $r_{b}$ debe compensar con acumulando una carga $+q$ ,de tal forma que la carga total del conductor siga siendo 0.

#### Punto B

Para el campo electrico, analizamos por secciones:
- Para $0<r <r_{a}$:
La carga encerrada es unicamente la carga puntual +q, por tanto es la unica capaz de ejercer flujo sobre la superficie. Por tanto:
$E= \frac{q}{4\pi\epsilon_{0}r^2}$
- Para $r_{a} <r <r_{b}$:
En esta sección, nos encontramos adentro del conductor, obligatoriamente se debe cumplir que $E=0$
- Para $r > r_{b}$:
La carga neta encerrada es +q.  Tenemos que el campo electrico generado por el conductor es identico al producido por una carga puntual situada en el centro del conductor. El campo electrico resulta totalmente radial, sin preferencia horizontal. Aprovechamos esta simetria usando una esfera gaussiana concentrica al conductor con radio r. Usando la ley de Gauss, entonces tendriamos: $EA = \frac{Q_{enc}}{\epsilon_{0}} \implies E= \frac{q}{4 \epsilon_{0} \pi r^2}$.

Entonces tenemos que:

$$
\vec{E}(r) = \begin{cases}
\frac{q}{4\pi\epsilon_{0}r^2} \hat{r} & \text{si}& 0 < r < r_{a} \\
0 & \text{si}& r_{a} < r < r_{b} \\
\frac{q}{4 \epsilon_{0} \pi r^2} \hat{r} & \text{si}& r \geq r_{b}
\end{cases}
$$

#### Punto c

Asumiendo $V(r)=0$ en el infinito, dividimos el calculo del potencial por secciones.
- Para $r > r_{b}$:

Dado el campo electrico obtenido para esta region del espacio, tenemos que el potencial eléctrico es igual al provocado por una carga puntual q en el centro del conductor:

$$
V = \frac{q}{4\pi\epsilon_{0}r}
$$

- Para $r_{a} <r \leq r_{b}$:
Dado que dentro del conductor, el campo electrico es 0 en todo punto, el potencial se mantiene constante: $V = \frac{q}{4\pi\epsilon_{0}r_{b}}$ para todo punto.

- Para $0<r \leq r_{a}$:
El potencial eléctrico es igual al provocado por una carga puntual $q$ más el potencial arrastrado de las superficies externas. Planteando el principio de superposicion, tenemos:

$$
\begin{align}
\Delta V_{\infty \to r} &  = \Delta V_{\infty\to r_{a}} + \Delta V_{r_{a} \to r} \\
\end{align}
$$

$$
\begin{align}
V & = V(r_{a}) - \int_{r_{a}}^r \vec{E} \cdot d \vec{l} \\
V & = V(r_{a}) - \frac{q}{4\pi\epsilon_{0}}\int_{r_{a}}^r \frac{1}{ r^2}dr  \\
V & = V(r_{a}) - \frac{q}{4\pi\epsilon_{0}} \left( \left. -\frac{1}{r}\right|_{r_{a}}^r \right) \\ \\
V & = V(r_{a}) - \frac{q}{4\pi\epsilon_{0}} \left( \frac{1}{r_{a}} -\frac{1}{r} \right) \\ \\
V & = V(r_{a}) + \frac{q}{4\pi\epsilon_{0}} \left(\frac{1}{r} - \frac{1}{r_{a}} \right) \\
V  & = \frac{q}{4\pi\epsilon_{0}r_{b}} + \frac{q}{4\pi\epsilon_{0}} \left(\frac{1}{r} - \frac{1}{r_{a}} \right) \\
V  & =\frac{q}{4\pi\epsilon_{0}} \left(\frac{1}{r_{b}} +\frac{1}{r} - \frac{1}{r_{a}} \right)
\end{align}
$$

Por tanto, tenemos que:

$$
V(r) = \begin{cases}
\frac{q}{4\pi\epsilon_{0}} \left(\frac{1}{r_{b}} +\frac{1}{r} - \frac{1}{r_{a}}\right) & \text{si} & 0<r<r_{a} \\
\frac{q}{4\pi\epsilon_{0}r_{b}} & \text{si} & r_{a}\leq r < r_{b} \\
\frac{q}{4\pi\epsilon_{0}r}& \text{si} & r > r_{b}
\end{cases}
$$

Ver [Principio de Superposicion para Calculo de Potencial](../notas/Principio%20de%20Superposicion%20para%20Calculo%20de%20Potencial.md) para approach alternativo de resolucion de este punto.
