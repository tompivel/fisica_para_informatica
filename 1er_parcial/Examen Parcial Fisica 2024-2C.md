# CB024 Física para Informática - Primer Parcial

**2do Cuatrimestre 2024**

## Problema 1: Mecánica

Dos masas puntuales, $m_1$ y $m_2$ ($m_2 = 2m_1$), comprimen un resorte ideal de constante elástica $k$ y longitud natural $l_0$, manteniéndolo en una longitud $l_0/2$. El valor de la constante elástica es:

$$k = \frac{6m_1g}{l_0}$$

Donde $g$ es la aceleración de la gravedad.

![Pasted image 20260525104647](../assets/Pasted%20image%2020260525104647.png)

El conjunto se halla apoyado en una superficie sin rozamiento e inicialmente en reposo. A una distancia $2l_0$ de la masa $m_1$ se encuentra apoyada en la superficie otra masa puntual $m_3$ ($m_3 = 4m_1$), también en reposo y sin rozamiento con la superficie.

En un dado instante, el resorte se libera y comienza a expandirse, empujando a las masas. El resorte no está adherido a ellas, de modo que cuando alcanza su longitud natural se cae y deja de actuar sobre las masas. Finalmente, la masa $m_1$ impacta sobre la masa $m_3$, quedando adheridas ambas.

Considere como sistema a las 3 masas y al resorte.

- **a.** Analice la conservación del momento lineal y la energía mecánica del sistema en cada etapa del movimiento: entre el instante inicial y el momento en que se cae el resorte, entre este y el impacto de las masas $m_1$ y $m_3$, y luego de este impacto. Justifique.
    
- **b.** Calcule las velocidades de las masas $m_1$ y $m_2$ luego de que el resorte deja de actuar sobre ellas.
- **c.** Calcule la posición del Centro de Masa del sistema en función del tiempo.
- **d.** Calcule la energía mecánica del sistema como función del tiempo.
    

### Resolución

#### Punto A
Antes de considerar la conservación de momento lineal y energía mecánica por cada estado del sistema, definamos limpiamente estados:
- **Estado A:** El sistema se encuentra inicialmente en reposo. Resorte a punto de expandirse.
- **Estado B:** El resorte acaba de expandirse totalmente y se cae. Masa $m_{1}$ y $m_{2}$ poseen velocidades $v_{1b}$ y $v_{2b}$
- **Estado C:** Masas $m_{1}$ y $m_{3}$ a punto de colisionar.
- **Estado D:** Masas $m_{1}$ y $m_{3}$ adheridas inmediatamente después de la colisión con velocidad final $v_{13d}$  y masa $m_{2}$ con velocidad $v_{2d}$.
Entonces, definiendo eje x paralelo al suelo con dirección positiva hacia la izquierda y eje y perpendicular al suelo con dirección positiva hacia arriba, con un origen en el punto inicial de la masa $m_{2}$:
- **Entre A y B:** Momento lineal del sistema se conserva en el eje x paralelo al suelo, dado que no existen fuerzas externas actuando sobre el sistema. La energía mecánica también se conserva dado que no existen fuerzas no conservativas haciendo trabajo sobre el sistema.
- **Entre B y C:** Momento lineal del sistema se conserva en el eje x paralelo al suelo, dado que no existen fuerzas externas actuando sobre el sistema. La energía mecánica también se conserva dado que no existen fuerzas no conservativas haciendo trabajo sobre el sistema.
- **Entre C y D:**  Momento lineal del sistema se conserva en el eje x paralelo al suelo, dado que no existen fuerzas externas actuando sobre el sistema. El energía mecánica del sistema no se conserva, dado que las masas $m_{1}$ y $m_{3}$ quedan adheridas (colisión completamente inelástica), de modo que la energía cinética del sistema se ve reducida sin un incremento en la energía gravitatoria potencial del sistema. 

#### Punto B

Usando la conservación del momento lineal entre el estado A y B:

$$
\begin{align}
\vec{p_{A}} &  = 0 \implies \vec{p_{B}} =0 \\
\vec{p_{B}} & = (m_{1}v_{1_{B}} + m_{2} v_{2_{B}}) \hat{i} =0 \\
\vec{v_{1B}}  & = - \frac{m_{2}}{m_{1}} v_{2B} \hat{i} \\
\vec{v_{1B}}  & = - \frac{2m_{1}}{m_{1}} v_{2B} \hat{i} \\
\vec{v_{1B}}  & = - 2v_{2B} \hat{i}
\end{align}
$$

Usando también que la energía mecánica se conserva, tenemos:

$$
\begin{align}
K_{A} + U_{A}  & = K_{B} + U_{B} \\
0 + U_{el} & = K_{1B} + K_{2B} + 0 \\
\frac{1}{2}\left( l_{0}-\frac{1}{2}l_{0} \right)^2k  & = \frac{1}{2}m_{1}v_{1B}^2 + \frac{1}{2}m_{2}v_{2B}^2 \\
\frac{l_{0}^2}{8}k  & = \frac{1}{2}m_{1}v_{1B}^2 + \frac{1}{2}m_{2}v_{2B}^2 \\
v_{2B}^2  & = \frac{{\frac{l_{0}^2}{4}k - m_{1}v_{1B}^2}}{m_{2}} \\
\end{align}
$$

Usando que $k = \frac{6m_{1}g}{l_{0}}$ y $m_{2} = 2m_{1}$, reemplazamos:

$$
\begin{align}
v_{2B}^2  & = \frac{{\frac{l_{0}^2}{4}\left( \frac{6m_{1}g}{l_{0}} \right) - m_{1}v_{1B}^2}}{2m_{1}} \\
v_{2B}^2  & = \frac{{\frac{3}{2}l_{0}g  -v_{1B}^2}}{2} \\
\end{align}
$$

Despejamos entonces $v_{1B}$ de nuestra primera ecuación:

$$
\begin{align}
v_{1B}  & = - 2 v_{2B} \\
v_{1B}^2  & = 4v_{2B}^2 \\
v_{1B}^2  & = 2\left( {\frac{3}{2}l_{0}g  -v_{1B}^2} \right) \\
v_{1B}^2  & = l_{0}g  \\
|v_{1B}|  & = \sqrt{l_{0}g} \\
\end{align}
$$

Por tanto, dado que la masa $m_{1}$ termina moviéndose a la izquierda y la masa $m_{2}$ hacia la derecha, asignamos signos corresponientes congruentes con nuestro sistema de referencia:

$$
\begin{align}
\vec{v_{1B}}  & = \sqrt{l_{0}g} \hat{i} \\
\vec{v_{2B}}  & = -\frac{1}{2} \sqrt{l_{0}g} \: \hat{i} \\
\end{align}
$$

#### Punto C

Dado que $\sum F_{\text{ext}_{x}} = 0$ desde el estado A hasta el estado D, la velocidad del centro de masa $V_{CM}$ es constante, y considerando que el sistema parte del reposo:

$$
\begin{align}
\vec{p_{A}} &  = 0 \implies v_{CM_{A}} = 0 \\
\end{align}
$$

Por tanto, $\vec{v_{CM}}(t) = 0 \hat{i} + 0 \hat{j}$ para todo t. Esto significa que la posición $\vec{r_{CM}}$ del centro de masa es constante. Asumiendo todas las partículas pertenecientes del sistema en una altura 0, nos dedicamos a calcular el $x_{CM}$ inicial:

$$
\begin{align}
x_{CM_{A}} & = \frac{{m_{1}x_{1A} + m_{2}x_{2A} + m_3x_{3A}}}{m_{1} + m_{2} + m_{3}} \\
& = \frac{{m_{1}\left( \frac{l_{0}}{2} \right) + (2m_{1})(0) + (4m_{1})\left( \frac{l_{0}}{2} + 2l_{0} \right)}}{m_{1} + 2m_{1} + 4m_{1} } \\
& = \frac{{m_{1}\left( \frac{l_{0}}{2} \right)  + (4m_{1})\left( \frac{l_{0}}{2} + 2l_{0} \right)}}{7m_{1}} = \frac{{\frac{21}{2}l_{0}m_{1}}}{7 m_{1}} \\
 & = \frac{3}{2} l_{0} 
\end{align}
$$

Por tanto:

$$
\begin{align}
r_{CM}(t)  & = \frac{3}{2}l_{0} \hat{i} + 0 \hat{j} \quad\forall t
\end{align}
$$

#### Punto D

La energía mecánica se conserva desde A hasta C, por tanto para este intervalo:

$$
\begin{align}
E_{A-C} &  = \frac{l_{0}^2}{8}k  = \frac{l_{0}^2}{8} \times\left( \frac{6m_{1}g}{l_{0}} \right)  \\
E_{A-C} &  = \frac{3}{4} m_{1}l_{0}g
\end{align}
$$

Desde el estado C hasta el D, la energía mecánica no se conserva, donde:

$$
\begin{align}
E_{D}  & = K_{D} + U_{D} \\
E_{D}  & = K_{13_{D}} + K_{2D}  + 0 \\
E_{D}  & = \frac{1}{2}(5m_{1})v_{13_{D}}^2 + \frac{1}{2}m_{2} v_{2D}^2 \\
\end{align}
$$

Sabemos que $v_{2D} = v_{2B}$ dado a la ausencia de fuerzas de rozamiento una vez que la masa $m_{2}$ se ve expulsada, es nuestro trabajo entonces encontrar $v_{13_{D}}$ después de la colisión. Para ello, usamos la conservación del momento lineal del sistema entre el estado C y D:

$$
\begin{align}
\vec{p_{C}}  & = 0  = \vec{p_{D}} \\
m_{1} v_{1C} + m_{2} v_{2C}  & = (m_{1} + m_{3})v_{13_{D}} + m_{2} v_{2C} \\
v_{13D}  & = \frac{m_{1}}{5m_{1}} vecv_{1C} \\
v_{13D}  & = \frac{1}{5} v_{1C} = \frac{1}{5} v_{1B}\\ \\
\vec{v_{13D} } & = \frac{1}{5} \vec{v_{1B}} = \frac{1}{5} \sqrt{l_{0}g} \hat{i}\\
\end{align}
$$

Reemplazamos en la fórmula y calculamos la energía cinética para el estado D:

$$
\begin{align}
E_{D} & =\frac{1}{2}(5m_{1})v_{13_{D}}^2 + \frac{1}{2}m_{2} v_{2D}^2  \\
E_{D} & =\frac{1}{2}(5m_{1})\left(  \frac{1}{5} \sqrt{l_{0}g} \right)^2 + m_{1}\left(  -\frac{1}{2} \sqrt{l_{0}g} \right)^2  \\
E_{D} & =\frac{1}{10}m_{1}l_{0}g + \frac{1}{4}m_{1} l_{0}g  \\
E_{D} & =\frac{7}{20} m_{1}l_{0}g
\end{align}
$$

Por tanto:

$$
\begin{align}
E_{t}  & = \begin{cases}
\frac{3}{4}m_{1}l_{0}g & \text{si} \quad t_{A}<t <t_{C} \\
\frac{7}{20}m_{1}l_{0}g & \text{si} \quad t\geq t_{C}
\end{cases}
\end{align}
$$

## Problema 2: Electrostática - Cargas Puntuales

Cuatro cargas puntuales están ubicadas en los vértices de un rectángulo alineado con los ejes coordenados de la siguiente manera:

- $q_1$ en el segundo cuadrante: $(-b, a)$
- $q_2$ en el primer cuadrante: $(b, a)$
- $q_3$ en el tercer cuadrante: $(-b, -a)$
- $q_4$ en el cuarto cuadrante: $(b, -a)$

![Pasted image 20260526090708](../assets/Pasted%20image%2020260526090708.png)

Se conocen los valores de las cargas $q_1 = 10$ nC, $q_3 = -7$ nC y $q_4 = 20$ nC. Se ajustará el valor de la carga $q_2$ para que el campo eléctrico en el origen $O(0,0)$ esté contenido únicamente en el eje $x$.

**Datos:** $a = 3$ cm, $b = 4$ cm.

- **a.** Encuentre el valor de la carga $q_2$ para que cumpla con lo pedido.
    
- **b.** ¿Cuánto vale el campo eléctrico en el lugar donde está ubicada $q_2$?
    
- **c.** Se desea llevar una carga puntual $q_0 = 1$ nC desde el punto $A$ (ubicado sobre el eje $x$ en $(b,0)$) hasta el origen de coordenadas. ¿Qué trabajo debe realizarse para hacer esto? La carga $q_0$, ¿gana o pierde energía potencial con el desplazamiento?
    
### Resolución
#### Punto A
Para que el valor de la carga esté unicamente contenido en el eje x, igualamos la superposicion de campos eléctricos (del eje y) en el punto origen a 0 y despejamos $q_{2}$.
Primero, calculamos una expresión para el campo total:

$$
\begin{align}
\vec{E_{O}}  & = \vec{E_{1O}} +  \vec{E_{2O}} +  \vec{E_{3O}} +  \vec{E_{4O}}
\end{align}
$$

Para asignarle una dirección a cada campo individual, planteamos primero el vector posición del origen respecto a cada carga. Dado que cada uno apunta hacia el origen:

$$
\begin{align}
\vec{r}_{q_{i}\to f} & = \vec{r_{f}} - \vec{r_{q_{i}}} \\
\vec{r}_{q_{i}\to f} & = (x_{f}-x_{i})\hat{i} + (y_{f}- y_{i})\hat{j} \\
\vec{r}_{q_{i}\to O} & = (0 - x_{i})\hat{i} + (0 - y_{i})\hat{j} = -x_{i} \hat{i} - y_{i} \hat{j}   \\
\end{align}
$$

Calculamos el vector unitario que nos permitirá darle dirección al campo sin afectar su magnitud:

$$
\begin{align}
\hat{u_{E_{i}}} & = \frac{{-x_{i}\hat{i} - y_{i}\hat{j}}}{r} = \frac{-x_{i}}{r} \hat{i} + \frac{-y_{i}}{r}\hat{j} \\ 
\vec{E_{i}} & = E \hat{u_{E_{i}}} = E\frac{-x_{i}}{r} \hat{i} + E\frac{-y_{i}}{r}\hat{j}
\end{align}
$$

Entonces $E_{iy} = E \times-\frac{y_{i}}{r} \hat{j}$.  Siendo que $y_{1} = y_{2} = a$  y $y_{3}=y_{4}=-a$, y considerando $k= \frac{1}{4 \pi \epsilon_{0}}$a, planteamos la superposicion de campos:

$$
\begin{align}
E_{y}  & = E_{1y} + E_{2y} + E_{3y} + E_{4y} = 0 \\ 
 & = -\frac{E_{1}a}{r}  -\frac{E_{2}a}{r} +\frac{E_{3}a}{r} +\frac{E_{4}a}{r}\\ 
  & = \frac{k}{r^3}\left( -q_{1}  - q_{2} + q_{3} + q_{4} \right)\\
 0  & = -q_{1}  - q_{2} + q_{3} + q_{4}\\
q_{2}  & = -q_{1} + q_{3} + q_{4} = -10nC -7nC + 20nC = 3nC  \\
q_{2}  & =  3nC
\end{align}
$$

#### Punto B
Planteamos un enfoque similar al punto A. Nuestro punto objetivo $O$ será la posición de la carga $q_{2}$, situada en $(b,a)$. Por tanto, calculamos el vector posición del punto respecto de cada carga:

$$
\begin{align}
\vec{r_{O-i}} &  = \vec{r_{O}} - \vec{r_{i}} \\
 & =  (b-x_{i})\hat{i} + (a-y_{i})\hat{j} \\
\end{align}
$$

Por tanto, el vector unitario que aporta la dirección del campo generado por cada cargo será:

$$
\begin{align}
\hat{u_{E_{i}}}  & = \frac{{(b-x_{i})\hat{i} + (a-y_{i})\hat{j}}}{r_{i}}  \\
\hat{u_{E_{i}}}  & = \frac{{(b-x_{i})\hat{i}}}{r_{i}} + \frac{{(a-y_{i})\hat{j}}}{r_{i}} \\
\vec{E_{i}}  & = E_{i} \hat{u_{E_{i}}} =E_{i}\frac{{(b-x_{i})\hat{i}}}{r_{i}} + E\frac{{(a-y_{i})\hat{j}}}{r_{i}} 
\end{align}
$$

La dificultad acá yace en que las distancias $r_{i}$ varían dependiendo de la carga, consideremos cada caso:
- $q_{1}$: $r_{1}=2b$
- $q_{3}$ $r_{3}=2 \sqrt{ a^2 +b^2} =2r$
- $q_{4}$: $r_{4} = 2a$
Planteemos la superposición de campos:

$$
\begin{align}
\vec{E_{O}}  & = \vec{E_{1O}} +  \vec{E_{2O}} +  \vec{E_{3O}} +  \vec{E_{4O}} \\
E_{x}  & = E_{1}\frac{{2b}}{2b} + E_{3}\frac{{2b}}{2r} + E_{4}\frac{{0}}{2a} = E_{1} + \frac{E_{3}b}{r} \\ 
E_{x}  & = k \frac{q_{1}}{4b^2}  + k \frac{q_{3}b}{4r^3} \\
E_{x}  & =  \frac{1}{4\pi \epsilon_{0}}\left(\frac{10 \cdot 10^{-9}C}{4(0.04m)^2} + \frac{-7 \cdot 10^{-9}C(0.04m)}{4\sqrt{ 0.03^2+ 0.04^2 }^3m^3}\right)\\
E_{x}  & = 
\end{align}
$$

Para la componente en y, tenemos:

$$
\begin{align}
E_{y}  & = E_{1}\frac{{0}}{2b} + E_{3}\frac{{2a}}{2r} + E_{4}\frac{{2a}}{2a} =  \frac{E_{3}a}{r} + E_{4} \\
E_{y}  & = \frac{kq_{3}a}{r^3} + \frac{kq_{4}}{4a^2} \\
E_{y}  & = \frac{1}{4\pi \epsilon_{0}}\left(\frac{-7 \cdot 10^{-9}C(0.03m)}{\sqrt{ 0.03^2+ 0.04^2 }^3m^3} + \frac{20 \cdot 10^{-9}C}{4\times (0.03m)^2}\right) \\
\end{align}
$$

#### Punto C
Se asume que se habla de una fuerza externa, entonces el trabajo que esta fuerza externa debe realizar para mover una carga puntual desde el punto $A=(b,0)$ hasta el origen $O=(0,0)$, viene dado por:

$$
\begin{align}
W_{ext} & = \Delta U = U_{O} - U_{A} \\
\end{align}
$$

Además, sabemos que:

$$
\begin{align}
U_{O}-U_{A} & =  kq_{0} \sum_{i} \frac{q_{i}}{r_{i}}
\end{align}
$$

Para $U_{0}$, tenemos:

$$
\begin{align}
U_{O} & = k q_{0}\left( \frac{q_{1}}{\sqrt{b^2 + a^2}} + \frac{q_{2}}{\sqrt{b^2 + a^2}} +  \frac{q_{3}}{\sqrt{b^2 + a^2}} +  \frac{q_{4}}{\sqrt{b^2 + a^2}}\right) \\
U_{O} & = kq_{0}\left( \frac{q_{1} +q_{2} + q_{3} + q_{4}}{\sqrt{b^2 + a^2}} \right) \\
U_{O} & = \frac{1nC}{4\pi \epsilon_{0}}\left(  \frac{26nC}{0.05m}\right) = 4.67 \micro J\\
\end{align}
$$

Para $U_{A}$, tenemos:

$$
\begin{align}
U_{A} & = k q_{0}\left( \frac{q_{1}}{\sqrt{ 4b^2 + a^2}} + \frac{q_{2}}{a} + \frac{q_{3}}{\sqrt{ 4b^2 + a^2}} + \frac{q_{4}}{a}\right) \\
U_{A} & = kq_{0}\left( \frac{q_{1}+q_{3}}{\sqrt{ 4b^2 + a^2}} + \frac{q_{2} + q_{4}}{a}\right) \\
U_{A} & = \frac{1nC}{4\pi \epsilon_{0}}\left( \frac{3nC}{0.085m} + \frac{23nC}{0.03m}\right) \\
U_{A}  & =7.21 \micro J
\end{align}
$$

Por tanto, $W_{ext} =  4.67 \micro J - 7.21 \micro J= -2.53 \mu J$. El trabajo de esta fuerza externa es negativo, lo cuál indica que la carga pierde energía potencial con el desplazamiento, ya que la carga es empujada por el campo eléctrico y en realidad la fuerza externa empuja hacia el lado contrario para evitar un incremento en la energía cinética.
## Problema 3: Electrostática - Conductores y Dieléctricos

Dos conductores planos, con forma de chapa cuadrada de lados $L = 2$ cm y espesor $e = 1$ mm, están ubicados paralelamente entre sí, separados una distancia $d = 2$ mm. Inicialmente están conectados a una pila de valor $V_0 = 10$ V (**Figura a**).
![Pasted image 20260528092335](../assets/Pasted%20image%2020260528092335.png)

- **a.** Si los conductores están inicialmente descargados, y despreciando efectos de borde, encuentre las densidades de carga que gana cada uno de ellos y el campo eléctrico en todo el espacio.

- **b.** Después de equilibrarse, se desconectan de la pila y se introduce un material dieléctrico de permitividad relativa $\epsilon_r = 2$, ocupando un cuarto de la superficie de cada chapa, con un ancho de $L/4$ (**Figura b**). Calcule la redistribución de carga y los valores del campo eléctrico, también sin tener en cuenta efectos de borde.
    ![Pasted image 20260528095312](../assets/Pasted%20image%2020260528095312.png)
- **c.** Recalcular la diferencia de potencial entre los conductores, una vez equilibrada la configuración del punto **b**.

### Resolución

#### Punto A
Sabemos que en dos placas conductoras paralelas, se cumple que el campo eléctrico es uniforme y $E = \frac{\sigma}{\epsilon}$. Además, tenemos que el diferencial de potencial entre ambas placas resulta: $V = Ed$. También se sabe, por ley de Gauss usando superficies cilíndricas justo después y antes de cada placa, que el campo eléctrico arriba de la placa superior y debajo de la capa inferior es 0.

Debido a la redistribución de carga forzada por la pila, ambas placas terminan teniendo Q y -Q como carga. Teniendo en cuenta que el area de las placas $A$ es el mismo, y que la densidad de carga $\sigma = \frac{Q}{A}$, el modulo de la densidad de carga $\sigma$ sera el mismo para ambas placa:

$$
\begin{align}
V  & = \frac{\sigma}{\epsilon}d \\
\sigma & = \frac{V\epsilon}{d} \\
\sigma & = \frac{10V\left( 8.854 \times 10^{-12} \frac{C^2}{Nm^2} \right)}{0.002m} \\
\sigma  & = 4.427 \times 10^{-8} \frac{\text{C}}{\text{m}^2} = 44.27 \frac{\text{nC}}{\text{m}^2}
\end{align}
$$

Por tanto, si dividimos el espacio en secciones tenemos que:
- Entre las placas: El campo eléctrico es uniforme.
$$E = \frac{V}{d} = \frac{10\text{ V}}{0.002\text{ m}} = 5000 \frac{\text{V}}{\text{m}}$$
- **Por fuera del conjunto de placas (arriba y abajo):** El campo es nulo ($\vec{E} = 0$), asumiendo que despreciamos los efectos de borde como indica el problema.
- **En el interior del material de las chapas:** El campo eléctrico es nulo dado que la carga se distribuye únicamente sobre las superficies enfrentadas. 
#### Punto B
Duda conceptual surgida:  [Adding a Dielectric, keeps the same Electric field and potential?](../notas/Adding%20a%20Dielectric,%20keeps%20the%20same%20Electric%20field%20and%20potential?.md)
Los conductores son volúmenes equipotenciales. Cada conductor, al desconectarles la pila, deben mantener un potencial $V_{\text{sup}}$ y $V_{\text{inf}}$ a través de toda la superficie de los conductores, independientemente de sí hay un diélectrico en alguna parte entre ambos. Esto genera un nuevo diferencial de potencial $V' = V_{\text{sup}}-V_{\text{inf}}$, el cuál será menor al diferencial original $V$ (dado que $C'>C \implies V'<V$.  

Dado que ahora se introduce un material dieléctrico en una sección entre las placas, las cargas dentro de cada placa se deben redistribuir entre la sección dieléctrico y la sección con vacío para cumplir con este requerimiento de equipotencialidad, alternando la uniformidad de la densidad de carga. Dado que la carga total $Q$ almacenada en cada placa se debe conservar:

$$
\begin{align}
Q_{\text{total}} & = Q_{\text{vacio}} + Q_{\text{dielec}}
\end{align}
$$

Sabiendo que la carga total en la superficie de un conductor es $Q = \sigma A$, se puede reescribir la ecuación de conservación:

$$
\sigma_{total}A_{\text{total}} = \sigma_{vacio}A_{vacio} + \sigma_{dielec}A_{\text{dielec}}
$$

donde  $A_{\text{total}} = L^2$ y $A_{dielec} = \frac{L^2}{4}$ y $A_{\text{vacio}} = \frac{3L^2}{4}$.

$$
\begin{align}
\sigma_{inicial}L^2 &  = \sigma_{vacio} \frac{3L^2}{4} + \sigma_{dielec} \frac{L^2}{4} \\
\sigma_{inicial} & = \frac{3}{4}\sigma_{vacio}  + \frac{1}{4}\sigma_{dielec} \tag{1}
\end{align}
$$

Ahora, dado que el diferencial de potencial $V'$ debe ser el mismo en ambas secciones: $V_{\text{vacio}} = V_{\text{dielec}}$ y recordando que el campo eléctrico en esta configuración (placas paralelas conductoras) es $V' = E'd$. Dado que la distancia $d$ sigue siendo la misma, entonces, el campo eléctrico $E'$ también debe ser igual para ambas secciones.

$$
E_{\text{dielec}} = E_{\text{vacio}} = \frac{V'}{d} = E'
$$

Además, usando la relación $E = \frac{\sigma}{\epsilon}$, tenemos:

$$
\begin{align}
\frac{\sigma_{\text{vacio}}}{\epsilon_{0}} &  = \frac{\sigma_{\text{dielec}}}{e_{0}e_{r}} \\
\sigma_{\text{vacio}} & = \frac{\sigma_{\text{dielec}}}{\epsilon_{r}} \tag{2}
\end{align}
$$

Dos ecuaciones, dos incógnitas. Reemplazamos (2) en (1) y despejamos:

$$
\begin{align}
\sigma_{inicial} & = \frac{3}{4}\left( \frac{\sigma_{dielec}}{\epsilon_{r}} \right)  + \frac{1}{4}\sigma_{dielec} \\
\sigma_{inicial} & = \frac{\sigma_{\text{dielec}}}{4 \epsilon_{r}}\left( 3 + \epsilon_{r} \right)  \\
\sigma_{\text{dielec}} & =\frac{4\epsilon_{r}\sigma_{inicial}}{3 + \epsilon_{r}} \\
\sigma_{\text{dielec}} & =\frac{8\sigma_{inicial}}{5}
\end{align}
$$

Usando esta expresión resultante en (2), encontramos también $\sigma_{\text{vacio}}= \frac{4}{5}\sigma_{\text{inicial}}$. Por tanto:

$$
\begin{align}
\sigma_{vacio} = \frac{4}{5} (44.27) = 35.42 \text{ nC/m}^2 \\
\sigma_{dielec} = \frac{8}{5} (44.27) = 70.83 \text{ nC/m}^2
\end{align}
$$

Los valores del campo eléctrico afuera y en el interior de cada conductor se mantienen, lo único que cambia es el valor entre la superficie de ambos conductores:

$$
\begin{align}
E' &  = \frac{\sigma_{vacio}}{\epsilon_{0}}= \frac{4\sigma_{inicial}}{5\epsilon_{0}} \\
E' &  = 4000 \frac{V}{m}
\end{align}
$$

Esto hace sentido físico, dado que si el diferencial de potencial resultante $V'$ es menor al original, inevitablemente el campo eléctrico también lo será. 

#### Punto C

Usamos la relación $V' = E'd$. 

$$
\begin{align}
V'  & = \left( 4000 \frac{V}{m} \right)\times 0.002m \\
V'  & = 8V
\end{align}
$$

Este diferencial de potencial se mantiene entre ambas superficies, incluyendo la sección con dieléctrico. Llegar a la respuesta de $8\text{V}$ confirma matemáticamente todo el análisis físico previo: al introducir el dieléctrico en un sistema aislado, la capacitancia total aumenta, provocando que tanto el campo eléctrico como la diferencia de potencial disminuyan respecto a su estado inicial.
