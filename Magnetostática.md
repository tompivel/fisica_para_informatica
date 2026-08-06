---
id: 20260609120516
aliases: []
tags:
  - uncataloged
created: 2026-06-09 12:05
status: draft
---
# Guía de Problemas: Magnetostática
**Física para Informática - Primer Cuatrimestre 2024**
**Facultad de Ingeniería - Universidad de Buenos Aires**

### Problema 1

**a)** Calcular el campo $\vec{B}$ en un punto genérico del espacio generado por un tramo de conductor rectilíneo de largo $L$ que transporta una corriente $I$ uniforme y constante.

**b)** Ídem a) para longitud infinita.

**c)** Resolver el ítem b) utilizando condiciones de simetría y la Ley de Ampere. Para hacerlo, primero determine por consideraciones geométricas cómo son las líneas de campo (dirección y dependencia con las coordenadas). Luego elija, justificando, un camino cerrado ("curva de Ampere") adecuado.

#### Resolución
#### Punto a
Para calcular el campo magnético generado por un segmento infinitesimal de un conductor rectilíneo de largo L en un punto $P$ a distancia $r$ del segmento, usamos la ley de Biot y Savart:
$$
\begin{align}
d\vec{B} = \frac{\mu_0 I}{4\pi} \frac{d\vec{l} \times \hat{r}}{r^2}
\end{align}
$$
Para obtener el campo mágnetico generado por todo el largo L del conductor, integramos estos segmentos infinitesimales. La expresión de la integral a través de toda la longitud se detalla paso a paso en (28.3 Sears), finalmente obtenemos la expresión:
$$B = \frac{\mu_0 I}{4\pi R} \frac{L}{\sqrt{R^2 + (L/2)^2}}$$
#### Punto b
Para calcular el campo magnético generado por un segmento de conducto rectilíneo de largo infinito, desestimamos el término $R$ en $\sqrt{ R^2+ \left( \frac{L}{2} \right)^2}$:
$$
\begin{align}
B =  \frac{\mu_0 I}{4\pi R} \frac{L}{\sqrt{ (L/2)^2}} = \frac{\mu_0 I}{2\pi R} 
\end{align}
$$

#### Punto c
1. **Inexistencia de componente radial:** Por la simetría de traslación del cable infinito, si el campo tuviera una componente radial hacia adentro o hacia afuera del cable, implicaría la existencia de monopolos magnéticos, violando la Ley de Gauss para el magnetismo ($\nabla \cdot \vec{B} = 0$).
    
2. **Inexistencia de componente longitudinal:** Al invertir la dirección de la corriente, Biot-Savart indica que el campo debe invertirse. Sin embargo, girar el cable $180^\circ$ en el espacio (lo cual físicamente es idéntico) mantendría una hipotética componente longitudinal inalterada. La única forma de que ambas cosas sean ciertas es que la componente paralela al cable sea cero.
    
3. **Conclusión geométrica:** Por tanto, $\vec{B}$ solo puede tener dirección tangencial (azimutal, envolviendo al cable). Dada la simetría rotacional y traslacional, su magnitud solo puede depender de la distancia radial $r$.

Usando coordenadas cilíndricas, colocando al conductor en el origen del sistema, nos damos cuenta que el campo magnético mantiene simetría cilíndrica respecto de este, dependiendo exclusivamente del radio r respecto al eje axial.
Por tanto, tomamos como camino de integración un circulo cerrado de radio r en un plano perpendicular al conductor. El campo $\vec{B}$ es constante (dado que r se m)
$$
\begin{align}
\oint \vec{B} \cdot d \vec{l} = \oint B \times dl \cos \theta
\end{align}
$$
Tomando un camino de integración en contra de las manecillas de un reloj, tenemos que el campo es siempre paralelo al camino, de forma que la integral se simplifica:
$$
\begin{align}
B \oint  dl  = B(2\pi r)= I \mu_{0}
\end{align}
$$
Por tanto, el campo mágnetico generado resultante es $B = I \frac{\mu_{0}}{2\pi_{r}}$. Esto coincide con el resultado obtenido en el punto b.


### Problema 2
Por la periferia de un cuadrado de lado $L = 20\text{ cm}$ circula una corriente estacionaria $I = 5\text{ mA}$.

**a)** Calcular el campo magnético en el eje perpendicular al plano del cuadrado y que pasa por la intersección de las diagonales.
**b)** Graficar la componente relevante del campo calculado en función de la distancia a la intersección de las diagonales mencionadas.

### Resolucion
#### Punto a
Usamos como sistema de coordenadas x,y y z. Colocamos el centro del cuadrado en el origen del plano xy. De manera que el eje z representa el la intersección entre las diagonales.

Calcularemos el campo generado por cada tramo y posteriormente, aplicamos Principio de Superposición para obtener el campo resultante dependiendo de z. Dado que usaremos ley de savart para un conductor de largo L, es fundamental saber la distancia R desde un punto en el eje perpendicular y el centro de cada tramo.  Aplicando teorema de pitágoras obtenemos $\begin{align}R = \sqrt{ \frac{L}{2}^2 + z^2 }\end{align}$.

- **campo generado por L1 (-x -> +x): tramo inferior horizontal:**
$$
\begin{align} \\
B_{1}  & = \frac{\mu_0 I}{4\pi R} \frac{L}{\sqrt{R^2 + (L/2)^2}}  \\
\end{align}
$$
Tenemos la magnitud, ahora calculamos la dirección usando la ley de Biot-Savart:
Según la ley de Biot-Savart, el campo generado por un tramo infinitesimal  de un conductor rectilineo en un punto P a distancia R del mismo, viene dado por:
$$
\begin{align}
d \vec{B} = \frac{\mu_{0} I d \vec{l} \times \vec{r}}{4\pi R^3}
\end{align}
$$
Por tanto, la dirección de este campo viene "encapsulada" en el término:
$$
\begin{align}
d \vec{l} \times \vec{r}
\end{align}
$$
Tenemos que $\vec{r}$ es $\vec{r}_{P} - \vec{r}_{tramo} =  (0 \hat{i} + 0 \hat{i} + z \hat{k}) - \left( x \hat{i} - \frac{L}{2} \hat{j} + 0 \hat{k} \right) = -x \hat{i} + \frac{L}{2} \hat{j} + z \hat{k}$. Sabiendo que $d \vec{l} = dx \hat{i}$, calculamos el producto vectorial:
$$
d \vec{l} \times \vec{r}  = 0 \hat{i} -dx z \hat{j} + dx \frac{L}{2} \hat{k}
$$
Ahora, buscamos el versor dirección diviendo este resultado por su magnitud:
$$
\begin{align} \\
\hat{u_{dB_{1}}} = \frac{{d \vec{l} \times \vec{r}}}{|d \vec{l} \times \vec{r}|} = \frac{-dx z \hat{j} + dx \frac{L}{2} \hat{k}}{dx\sqrt{ z^2 +\left( \frac{L}{2} \right)^2}} = \frac{-z \hat{j} + \frac{L}{2} \hat{k}}{R}
\end{align}
$$
Teniendo en cuenta que el vector dirección de $d B_{1}$ obtenido para un tramo infinitesimal dx ubicado en una posición $(x,-L/2, z)$, no depende de esta posición x, en que el diferencial del conductor es evaluado, se puede aplicar:
$$
\begin{align}
\vec{B_{1}} = \int d \vec{B_{1}} = \int |dB_{1}| \hat{u}_{dB_{1}} = \hat{u}_{dB_{1}}\int |dB_{1}| = |B_{1}| \hat{u}_{dB_{1}}
\end{align}
$$
Ahondando más en esta explicación, demostramos:
### La demostración rigurosa (Cero simbolismo)
El campo total generado por el tramo L1 es la integral de todos sus diferenciales:
$$\vec{B}_1 = \int d\vec{B}_1 = \int_{-L/2}^{L/2} \frac{\mu_0 I}{4\pi |\vec{R}|^3} (d\vec{l} \times \vec{R})$$
Reemplazando el producto vectorial calculado ($-z\,dx\,\hat{j} + \frac{L}{2}\,dx\,\hat{k}$) y la magnitud del vector distancia $|\vec{R}| = \sqrt{x^2 + (L/2)^2 + z^2}$, la integral queda:

$$\vec{B}_1 = \frac{\mu_0 I}{4\pi} \int_{-L/2}^{L/2} \frac{-z\,\hat{j} + \frac{L}{2}\,\hat{k}}{\left(x^2 + (L/2)^2 + z^2\right)^{3/2}} dx$$

Aquí está la clave de tu duda: **observa el numerador**. El vector direccional $\left(-z\,\hat{j} + \frac{L}{2}\,\hat{k}\right)$ **no contiene la variable $x$**. Físicamente, esto significa que sin importar en qué posición $x$ a lo largo del cable tomes el diferencial, el vector siempre apunta en esa exacta dirección. Matemáticamente, significa que es una constante respecto a la variable de integración $dx$.

Por la propiedad de linealidad, las constantes salen de la integral:

$$\vec{B}_1 = \left( -z\,\hat{j} + \frac{L}{2}\,\hat{k} \right) \left[ \frac{\mu_0 I}{4\pi} \int_{-L/2}^{L/2} \frac{1}{\left(x^2 + (L/2)^2 + z^2\right)^{3/2}} dx \right]$$

El término gigantesco entre corchetes es una integral puramente escalar. Si la resuelves, te dará exactamente $\frac{|B_1|}{R}$. Por lo tanto, la ecuación se reduce a:

$$\vec{B}_1 = \left( \frac{-z\,\hat{j} + \frac{L}{2}\,\hat{k}}{R} \right) |B_1| = \hat{u}_{dB_1} |B_1|$$

La matemática demuestra por sí sola que si la dirección de los infinitos diferenciales no depende de la variable de integración, el versor del diferencial aisaldo es obligatoriamente el versor del campo total. Esta lógica es idéntica para los demás tramos.

- **campo generado por L2 (-y -> +y):**
Para este conductor, tenemos que el versor resulta:
Tenemos que $\vec{r}$ es $\vec{r}_{P} - \vec{r}_{tramo} =  z \hat{k} - \left(-\frac{L}{2} \hat{i}  + y\hat{j} + 0 \hat{k} \right) = -\frac{L}{2} \hat{i} -y \hat{j} + z \hat{k}$. Sabiendo que $d \vec{l} = dy \hat{j}$, calculamos el producto vectorial:
$$
d \vec{l} \times \vec{r}  = -zdy \hat{i} + 0\hat{j} + dy \frac{L}{2} \hat{k}
$$

Ahora, buscamos el versor dirección diviendo este resultado por su magnitud:
$$
\begin{align} \\
\hat{u_{dB_{1}}} = \frac{{d \vec{l} \times \vec{r}}}{|d \vec{l} \times \vec{r}|} = \frac{-zdy \hat{i} + dy \frac{L}{2} \hat{k}}{dy\sqrt{ z^2 +\left( \frac{L}{2} \right)^2}} = \frac{-z \hat{i} + \frac{L}{2} \hat{k}}{R}
\end{align}
$$
- **campo generado por L3 (+x -> -x):**
Para este conductor, tenemos que el versor resulta:
Tenemos que $\vec{r}$ es $\vec{r}_{P} - \vec{r}_{tramo} =  z \hat{k} - \left(x \hat{i} - \frac{L}{2} \hat{j} + 0 \hat{k} \right) = -x \hat{i} + \frac{L}{2} \hat{j} + z \hat{k}$. 
Sabiendo que $d \vec{l} = -dx \hat{i}$, calculamos el producto vectorial:
![Pasted image 20260620141458](assets/Pasted%20image%2020260620141458.png)
$$
d \vec{l} \times \vec{r}  = 0 \hat{i} + dx z \hat{j} + dx \frac{L}{2} \hat{k}
$$

Ahora, buscamos el versor dirección diviendo este resultado por su magnitud:
$$
\begin{align} \\
\hat{u_{dB_{1}}} = \frac{{d \vec{l} \times \vec{r}}}{|d \vec{l} \times \vec{r}|} = \frac{-dx z \hat{j} + dx \frac{L}{2} \hat{k}}{dx\sqrt{ z^2 +\left( \frac{L}{2} \right)^2}} = \frac{+z \hat{j} + \frac{L}{2} \hat{k}}{R}
\end{align}
$$

- **campo generado por L4 (+y -> -y):**
Para este conductor, tenemos que el versor resulta:
Tenemos que $\vec{r}$ es $\vec{r}_{P} - \vec{r}_{tramo} =  z \hat{k} - \left(\frac{L}{2} \hat{i}  + y\hat{j} + 0 \hat{k} \right) = -\frac{L}{2} \hat{i} -y \hat{j} + z \hat{k}$. Sabiendo que $d \vec{l} = -dy \hat{j}$, calculamos el producto vectorial:
$$
d \vec{l} \times \vec{r}  = zdy \hat{i} + 0\hat{j} + dy \frac{L}{2} \hat{k}
$$

Ahora, buscamos el versor dirección diviendo este resultado por su magnitud:
$$
\begin{align} \\
\hat{u_{dB_{1}}} = \frac{{d \vec{l} \times \vec{r}}}{|d \vec{l} \times \vec{r}|} = \frac{zdy \hat{i} + dy \frac{L}{2} \hat{k}}{dy\sqrt{ z^2 +\left( \frac{L}{2} \right)^2}} = \frac{+z \hat{i} + \frac{L}{2} \hat{k}}{R}
\end{align}
$$

**Aplicando principio de superposición**:
Finalmente, sumamos los cuatro campos para obtener el campo total:
$$
\begin{align}
\vec{B_{total}} = \frac{\mu_0 I}{\pi R} \frac{L}{\sqrt{R^2 + (L/2)^2}} \frac{L}{2R} \hat{k} 
\end{align}
$$
### Problema 3

**a)** Calcular el campo $\vec{B}$ en el eje de un solenoide de radio $R$, longitud $L$ y $N$ espiras (suponer que las espiras están distribuidas uniformemente y muy próximas entre sí).
**b)** Extender el resultado para un solenoide de longitud infinita (solenoide ideal).
**c)** ¿Cuál es la relación entre diámetro y largo de un solenoide, para que la expresión obtenida en (a), y evaluada en el punto medio, difiera de la obtenida en (b) en menos del $5\%$?

### Resolucion
#### a
Pero en un solenoide **finito** (ítem a), las líneas de campo se curvan al llegar a los extremos y el campo se "escapa" hacia afuera. Al perderse la uniformidad, la Ley de Ampere deja de ser útil para despejar el campo, porque $B$ no es constante a lo largo de tu camino de integración. Por lo tanto, la herramienta a usar para el **ítem a** es el Principio de Superposición (Biot-Savart).

Debemos modelar el solenoide no como un tubo, sino como un apilamiento continuo de $N$ espiras circulares.

1. **Punto de partida:** Utiliza la fórmula ya conocida del campo en el eje $z$ de _una sola_ espira de radio $R$ ubicada en el origen:
    $$B_{espira} = \frac{\mu_0 I R^2}{2(R^2 + z^2)^{3/2}}$$
    
2. **Definir el diferencial:** Si el solenoide tiene longitud $L$ y $N$ espiras, la cantidad de espiras por unidad de longitud es $n = N/L$. Si tomas una pequeña rebanada del solenoide de grosor $dz'$ a una posición $z'$, esa rebanada contiene $dn = n\,dz'$ espiras.
    
3. **Plantear la integral:** 
	La fórmula original para una sola espira asume que el centro de la espira está anclado exactamente en el origen de coordenadas $(0,0,0)$. Bajo esa condición específica, la coordenada $z$ del punto de evaluación es idéntica a la **distancia física** entre la espira y el punto. La fórmula original realmente no pide una coordenada espacial, sino una distancia relativa.

	Al modelar el solenoide, colocamos el centro de todo el tubo en el origen $(0,0,0)$. Esto cambia el escenario:

	- Tu punto de evaluación sigue estando en una coordenada fija $z$.
	- La porción diferencial de espiras (la rebanada $dz'$ que genera el campo $dB$) no está en el origen, sino desplazada en una coordenada móvil que llamamos $z'$.

Para aplicar la fórmula original a esta rebanada desplazada, necesitas reemplazar el término original por la **verdadera distancia recta** entre la posición de la fuente de corriente y la posición de tu punto de evaluación.

Geométricamente, la distancia unidimensional entre dos puntos en un eje es la resta de sus coordenadas:

$$\text{Distancia} = \text{Posición final} - \text{Posición inicial} = z - z'$$

Por lo tanto, donde la ecuación base requería la distancia al cuadrado ($z^2$), la geometría del nuevo sistema te obliga a sustituirla por el cuadrado de la distancia relativa real: $(z - z')^2$. El pequeño campo $dB$ que genera esa rebanada en un punto genérico $z$ es:
    $$dB = \frac{\mu_0 (n\,dz') I R^2}{2(R^2 + (z - z')^2)^{3/2}}$$
    
4. **Integrar:** Colocando el origen $(0,0,0)$ en el centro exacto del solenoide, los extremos están en $-L/2$ y $+L/2$. Debes integrar la expresión anterior desde $z' = -L/2$ hasta $z' = L/2$.

    _(Ayuda matemática: puedes resolver esta integral por sustitución trigonométrica o haciendo el cambio de variable $u = z - z'$)._
    El resultado exacto al que debes llegar es:
    
    $$B(z) = \frac{\mu_0 n I}{2} \left[ \frac{z + L/2}{\sqrt{R^2 + (z + L/2)^2}} - \frac{z - L/2}{\sqrt{R^2 + (z - L/2)^2}} \right]$$
#### b)
El enunciado dice "Extender el resultado". Esto te pide matemáticamente que tomes la expresión obtenida en (a) y le calcules el límite cuando $L \to \infty$. Físicamente, si el solenoide es infinito, tu punto de evaluación $z$ siempre estará infinitamente lejos de los bordes.

Al hacer tender $L \to \infty$ en tu fórmula:

- El primer término dentro del corchete tiende a $+1$.
- El segundo término tiende a $-1$.
- El corchete total queda como $[1 - (-1)] = 2$.
$$
\begin{align}
\lim_{ L \to \infty } B(z)  & = \lim_{ L \to \infty } \frac{\mu_0 n I}{2} \left[ \frac{z + L/2}{\sqrt{R^2 + (z + L/2)^2}} - \frac{z - L/2}{\sqrt{R^2 + (z - L/2)^2}} \right]  = \frac{\mu_0 n I}{2} \left( \frac{L}{|L|} - \frac{-L}{|L|} \right) = \mu_{0}nI \\
 & = \mu_{o} \frac{N}{L}I
\end{align}
$$
    $$B_{ideal} = \frac{\mu_0 n I}{2} [2] = \mu_0 n I = \mu_0 \frac{N}{L} I$$
#### c)
Piden encontrar la relación Diámetro/Largo ($2R/L$) para que el error entre la fórmula real (fina) y la fórmula ideal sea menor al 5% en el centro exacto.

1. **Evaluar en el centro:** Toma tu fórmula del ítem (a) y evalúala en $z = 0$:
    $$B_{centro} = \frac{\mu_0 n I}{2} \left[ \frac{L/2}{\sqrt{R^2 + (L/2)^2}} - \frac{-L/2}{\sqrt{R^2 + (-L/2)^2}} \right]$$
    Simplificando:
    $$B_{centro} = (\mu_0 n I) \frac{L/2}{\sqrt{R^2 + L^2/4}}$$
    Nota que el término $(\mu_0 n I)$ es exactamente $B_{ideal}$. Por tanto:
    $$B_{centro} = B_{ideal} \frac{L/2}{\sqrt{R^2 + L^2/4}}$$
    
2. **Plantear la inecuación de tolerancia:** Quieres que el campo real difiera del ideal en menos del 5%. Como el campo real siempre es menor al ideal debido a las pérdidas por los bordes, esto significa que $B_{centro}$ debe conservar al menos el 95% de la fuerza de $B_{ideal}$:
    $$B_{centro} \ge 0.95 \, B_{ideal}$$
    
    Reemplazando tu ecuación:
    $$\frac{L/2}{\sqrt{R^2 + L^2/4}} \ge 0.95$$
    
3. **Despejar la geometría:** Ahora es puro álgebra. Eleva ambos lados al cuadrado, despeja los términos con $L$ hacia un lado y los términos con $R$ hacia el otro, y forma el cociente $\frac{4R^2}{L^2}$ (que es equivalente a $(2R/L)^2$). Al aplicarle raíz cuadrada, obtendrás el número final para la relación Diámetro/Largo que te garantiza ese nivel de precisión.
	$\frac{D}{L} = 0.23$
### Problema 4

Resolver el Problema 3b) utilizando condiciones de simetría y la Ley de Ampere. Para hacerlo, primero determine por consideraciones geométricas cómo son las líneas de campo (dirección y dependencia con las coordenadas). Luego elija, justificando, un camino cerrado ("curva de Ampere") adecuado.

### Resolucion
#### 1. Consideraciones Geométricas (Justificación del campo)

Se define un sistema de coordenadas cilíndricas $(r, \phi, z)$ con el eje $z$ coincidiendo con el eje longitudinal del solenoide.
  ![Pasted image 20260621140419](assets/Pasted%20image%2020260621140419.png)  
- **Inexistencia de componente radial ($B_r = 0$):** Por la longitud infinita, si existiera una componente radial, las líneas de campo divergirían desde el eje. El flujo magnético a través de un cilindro coaxial cerrado no sería nulo, violando la Ley de Gauss para el magnetismo ($\oint \vec{B} \cdot d\vec{A} = 0$, no existen monopolos magnéticos). Por tanto, el campo no entra ni sale radialmente del tubo.
- **Inexistencia de componente azimutal ($B_\phi = 0$):** Modelamos el solenoide ideal como un apilamiento continuo de espiras circulares perfectas, donde la corriente fluye estrictamente en la dirección azimutal ($\hat{\phi}$). La Ley de Biot-Savart dicta que un elemento de corriente genera un campo perpendicular a sí mismo; una corriente puramente azimutal no puede generar un campo magnético azimutal.
- **Dirección puramente axial:** Descartadas las componentes radial y azimutal, el campo magnético solo puede tener componente longitudinal $\vec{B} = B_z \hat{k}$.
- **Dependencia de las coordenadas:** Al ser un cilindro infinito, trasladarse a lo largo del eje $z$ no cambia la configuración del sistema (simetría de traslación), por lo que $\vec{B}$ no depende de $z$. Al girar alrededor del eje, todo se ve igual (simetría rotacional), por lo que $\vec{B}$ no depende de $\phi$. La magnitud del campo solo puede depender de la distancia al centro $r$.
- **Campo exterior nulo ($B_{ext} = 0$):** Las líneas de campo magnético deben formar bucles cerrados. Todo el flujo interno debe retornar por el exterior. Como el solenoide ideal es infinito, el espacio exterior de retorno posee un área tendiente a infinito. Un flujo magnético finito disperso en un área infinita resulta en una densidad de campo magnético igual a cero en el exterior.
### 2. Elección del Camino Cerrado ("Curva de Ampere")

Sabiendo que $\vec{B} = B(r) \hat{k}$ adentro y $\vec{B} = 0$ afuera, se elige una curva de integración rectangular (análoga al rectángulo $abcd$ del Sears) para explotar el comportamiento del campo:

- **Lados paralelos al eje $z$ (longitud $L$):** Trazamos uno por el interior a una distancia arbitraria $r < R$ (donde queremos hallar el campo), y otro por el exterior a una distancia $r > R$ (donde sabemos que el campo es nulo).
- **Lados perpendiculares al eje $z$:** Trazamos lados radiales para conectar los tramos paralelos y cerrar el bucle.

### 3. Ejecución de la Ley de Ampere

Se plantea la integral de línea subdividida en los cuatro tramos rectos: $a \to b$ (interior), $b \to c$ (perpendicular saliente), $c \to d$ (exterior), y $d \to a$ (perpendicular entrante).

$$\oint \vec{B} \cdot d\vec{l} = \int_a^b \vec{B} \cdot d\vec{l} + \int_b^c \vec{B} \cdot d\vec{l} + \int_c^d \vec{B} \cdot d\vec{l} + \int_d^a \vec{B} \cdot d\vec{l} = \mu_0 I_{\text{encl}}$$

Evaluamos rigurosamente cada término:

1. **Tramo interior ($a \to b$):** El camino ($d\vec{l} = dz\,\hat{k}$) es perfectamente paralelo al campo ($\vec{B} = B\,\hat{k}$). La magnitud $B$ es constante a lo largo de esa línea, por lo que sale de la integral. El producto es $B \int dz = BL$.
2. **Tramos perpendiculares ($b \to c$ y $d \to a$):** El campo es axial ($\hat{k}$) y el camino es radial ($\hat{r}$). Al ser vectores ortogonales ($\vec{B} \perp d\vec{l}$), su producto escalar es invariablemente cero en cada punto del trayecto.
3. **Tramo exterior ($c \to d$):** Como demostramos que el campo exterior es nulo por expansión infinita del área de retorno, la integral entera vale cero independientemente de la dirección del camino.

La integral cerrada colapsa al único término sobreviviente:

$$\oint \vec{B} \cdot d\vec{l} = BL$$

### 4. Corriente Encerrada y Conclusión

Si el solenoide tiene $n$ vueltas de alambre por unidad de longitud, el tramo de nuestro rectángulo de largo $L$ atraviesa exactamente $nL$ espiras. Por cada vuelta circula la misma corriente estacionaria $I$. La corriente total que cruza la superficie limitada por nuestro rectángulo es:

$$I_{\text{encl}} = nLI$$

Igualando los resultados en la ecuación general de Ampere:

$$BL = \mu_0 (nLI)$$

Las longitudes de la curva imaginaria $L$ se cancelan a ambos lados:

$$B = \mu_0 n I$$

Como este resultado final es completamente independiente de la variable $r$ (la distancia radial a la que colocaste inicialmente el tramo $a \to b$), **queda demostrado matemáticamente que el campo es perfectamente uniforme en cualquier punto interior del solenoide transversal**.

### Problema 5
![Pasted image 20260622105710](assets/Pasted%20image%2020260622105710.png)
**a)** Calcular la fuerza sobre cada tramo y la fuerza resultante sobre la espira rectangular de la figura, por la cual circula una corriente $I_2$, debida al campo generado por un alambre muy largo paralelo a la espira, que transporta una corriente $I_1$. Calcule para $I_1 = 10\text{ A}$ e $I_2 = 0.1\text{ A}$.

**b)** Calcular el momento que actúa sobre la espira, respecto de la línea de trazos que pasa por su centro. ¿Cambia el resultado si se cambia el "eje"?

_(Referencia a la figura 1: Un hilo conductor infinito con corriente $I_1$ paralelo a una espira rectangular con corriente $I_2$. La distancia entre el hilo y el lado más cercano de la espira es de $10\text{ cm}$. La espira tiene un ancho de $20\text{ cm}$ y un largo de $40\text{ cm}$. El eje de la espira se encuentra a la mitad de su ancho.)

### Resolucion
#### Conceptos Previos y Aclaración de Fuerzas

Para resolver este ejercicio, el primer paso es corregir una confusión común: **las fuerzas sobre la espira no son eléctricas, son exclusivamente magnéticas.** Los cables transportan corriente (cargas en movimiento), pero la materia de los conductores es eléctricamente neutra (tienen la misma cantidad de electrones que de protones estacionarios). Al no tener carga neta, no existe campo eléctrico neto interactuando entre los cables. Toda la fuerza se debe a la interacción entre el campo magnético del primer cable y las cargas en movimiento del segundo.

Los dos conceptos que necesitas combinar son:

1. **Ley de Ampere (o Biot-Savart para hilos largos):** Para calcular el campo magnético $\vec{B}$ que el alambre largo genera en el espacio.
    $$B = \frac{\mu_0 I_1}{2\pi r}$$
    
2. **Fuerza magnética sobre un conductor:** Para calcular cómo ese campo empuja a los tramos de la espira.
    $$\vec{F} = I_2 \int d\vec{l} \times \vec{B}$$
    

#### a) Fuerzas sobre cada tramo y Fuerza Neta

Ubicamos el hilo infinito sobre el eje $y$. Su corriente $I_1$ apunta hacia arriba ($+\hat{j}$). Por la regla de la mano derecha, el campo magnético que atraviesa el plano de la espira (ubicada a la derecha en el eje $x$) entra perpendicularmente en la página ($-\hat{k}$).

Asumiremos que la corriente $I_2$ en la espira circula en sentido horario (el tramo más cercano al hilo tiene la corriente paralela a $I_1$). _Si tu figura muestra el sentido opuesto, las magnitudes serán idénticas pero los signos de las fuerzas se invertirán._

**Datos numéricos:**

- $I_1 = 10\text{ A}$
- $I_2 = 0.1\text{ A}$
- $\mu_0 = 4\pi \times 10^{-7}\text{ T}\cdot\text{m/A}$
- Largo $L = 40\text{ cm} = 0.4\text{ m}$
- Ancho $w = 20\text{ cm} = 0.2\text{ m}$
- Distancia al tramo cercano $d_1 = 10\text{ cm} = 0.1\text{ m}$
- Distancia al tramo lejano $d_2 = 10 + 20 = 30\text{ cm} = 0.3\text{ m}$

**1. Tramo cercano (paralelo, a $0.1\text{ m}$):**
Definimos que el tramo cercano va desde $y = 0$ hasta $y = L$, manteniendo una posición constante $x = d_1$.

$$\begin{align} \vec{F}_{cercano} &= I_2 \int d\vec{l} \times \vec{B} \\ &= I_2 \int_{0}^{L} (dy\,\hat{j}) \times (-B\,\hat{k}) \end{align}$$

Aplicamos la propiedad distributiva del producto vectorial sobre los escalares:

$$\begin{align} \vec{F}_{cercano} &= I_2 \int_{0}^{L} -B\,dy\,(\hat{j} \times \hat{k}) \\ &= I_2 \int_{0}^{L} -B\,dy\,\hat{i} \end{align}$$

**Justificación para sacar los términos:** 1. El versor $\hat{i}$ es constante en el sistema cartesiano.

2. La magnitud del campo magnético es $B = \frac{\mu_0 I_1}{2\pi x}$. Como a lo largo de todo este tramo vertical la coordenada $x$ es una constante ($x = d_1$), el valor de $B$ no varía al movernos en $y$.

Por lo tanto, $-B$ e $\hat{i}$ salen de la integral:

$$\begin{align} \vec{F}_{cercano} &= -I_2 B\,\hat{i} \int_{0}^{L} dy \\ &= -I_2 B L\,\hat{i} \end{align}$$
Sustituyendo la expresión de $B$:

$$\vec{F}_{cercano} = -I_2 L \left( \frac{\mu_0 I_1}{2\pi d_1} \right) \hat{i}$$
    
$$F_{cercano} = (0.1) (0.4) \frac{(4\pi \times 10^{-7}) (10)}{2\pi (0.1)} = (0.04) \frac{2 \times 10^{-6}}{0.1} = 8 \times 10^{-7}\text{ N}$$

_(Dirección: hacia la izquierda, atraído por el hilo)._

**2. Tramo lejano (paralelo, a $0.3\text{ m}$):**

La corriente va en sentido opuesto (hacia abajo), por lo que la fuerza es repulsiva ($+\hat{i}$). El campo es más débil por la distancia.

$$F_{lejano} = I_2 L B(d_2) = I_2 L \left( \frac{\mu_0 I_1}{2\pi d_2} \right)$$

$$F_{lejano} = (0.1) (0.4) \frac{(4\pi \times 10^{-7}) (10)}{2\pi (0.3)} = (0.04) \frac{2 \times 10^{-6}}{0.3} \approx 2.67 \times 10^{-7}\text{ N}$$

_(Dirección: hacia la derecha, repelido por el hilo)._

**3. Tramos superior e inferior (perpendiculares al hilo):**

En estos tramos, la distancia $r$ varía a medida que nos alejamos del hilo (de $0.1\text{ m}$ a $0.3\text{ m}$). Habría que integrar: $F = \int I_2 \cdot dx \cdot B(x)$.

Sin embargo, por simetría geométrica, la fuerza sobre el tramo superior apunta estrictamente hacia arriba ($\hat{i} \times -\hat{k} =+\hat{j}$) y la fuerza sobre el tramo inferior (cuya corriente va en sentido contrario) apunta estrictamente hacia abajo ($-i \times \times -\hat{k} =-\hat{j}$). Al tener exactamente las mismas dimensiones y estar inmersos en el mismo gradiente de campo magnético, sus magnitudes son idénticas y **se cancelan matemáticamente entre sí.**

$$F_{superior} + F_{inferior} = 0$$
**4. Fuerza Resultante ($\vec{F}_{neta}$):**

Al anularse las componentes verticales, la fuerza neta es la suma de los tramos verticales. Como el tramo cercano experimenta un campo más intenso, la atracción gana la pulseada contra la repulsión.

$$F_{neta} = F_{cercano} - F_{lejano} = (8 \times 10^{-7}\text{ N}) - (2.67 \times 10^{-7}\text{ N})$$

$$F_{neta} = 5.33 \times 10^{-7}\text{ N}$$

_(Dirección: hacia el hilo largo, es decir, el sistema experimenta una fuerza neta de atracción)._

### b) Momento sobre la espira (Torque)

El momento de torsión ($\vec{\tau}$) respecto a un eje se define como la suma de todos los momentos generados por cada fuerza: $\vec{\tau} = \sum \vec{r} \times \vec{F}$.

**1. Momento respecto a la línea central:**

Si el eje de rotación pasa por el centro geométrico de la espira (a una distancia $x = 20\text{ cm}$ del hilo largo, paralelo a este):

- Todas las fuerzas magnéticas ($F_{cercano}$, $F_{lejano}$, $F_{superior}$, $F_{inferior}$) son **coplanares** (están acostadas exactamente en el mismo plano bidimensional que la espira).
    
- En física, una fuerza coplanar nunca puede provocar que un objeto tridimensional "salga" de su plano o rote sobre un eje que también está contenido en ese plano. La espira se estira, se comprime y se traslada hacia el hilo, pero no tiene ninguna tendencia a "voltearse" ni girar sobre su propio centro.
    
- **Resultado:** El momento sobre ese eje es exactamente **cero** ($\vec{\tau} = 0$).
    

_Forma alternativa de justificarlo:_ El momento de un dipolo magnético es $\vec{\tau} = \vec{\mu} \times \vec{B}$. El vector área $\vec{\mu}$ de la espira es perpendicular a la página. El campo $\vec{B}$ del hilo también es perpendicular a la página. Al ser vectores paralelos, el producto vectorial es cero.

**2. ¿Cambia el resultado si se cambia el eje?**

**Sí.** Este es un principio de la mecánica clásica: si la fuerza neta sobre un sistema _no_ es cero (como demostramos en el punto a, donde la espira es arrastrada hacia el hilo), el momento de torsión depende estrictamente del punto o eje de referencia que elijas.

Si trasladas el eje de rotación, por ejemplo, a la esquina superior izquierda de la espira, la fuerza neta ($\vec{F}_{neta}$ aplicada en el centro de masa) ahora tendrá un "brazo de palanca" respecto a esa esquina, generando un momento que tendería a hacer rotar la espira como un molinete dentro de su propio plano ($xy$). La única vez que el momento es independiente del eje es cuando la fuerza neta del sistema es exactamente cero.

#### ¿Por qué mi resolución conceptual coincidía con estas fórmulas?

Las expresiones $\vec{\tau} = \vec{\mu} \times \vec{B}$ y $\tau = IBA \sin\phi$ son atajos matemáticos válidos **única y exclusivamente si el campo magnético es constante en todo el espacio que ocupa la espira.** En tu problema, el campo generado por el hilo infinito ($B = \frac{\mu_0 I_1}{2\pi r}$) es **no uniforme**. Es más intenso en el lado izquierdo de la espira y más débil en el derecho. Por lo tanto, no puedes introducir un solo valor de $B$ en la fórmula del momento dipolar ($\vec{\mu} \times \vec{B}$) para obtener un resultado general de la torsión.

A pesar de que el campo varía en magnitud a lo ancho de la espira, su **dirección** ($-\hat{k}$, entrando en la página) se mantiene constante.

El momento magnético dipolar de la espira ($\vec{\mu} = I\vec{A}$) es un vector perpendicular al área de la espira. Al estar la espira apoyada en el plano $xy$, su vector $\vec{\mu}$ también apunta en el eje $z$ (entrando o saliendo de la página, dependiendo del sentido de la corriente).

Dado que $\vec{B}$ y $\vec{\mu}$ son paralelos o antiparalelos (el ángulo $\phi$ entre ellos es $0^\circ$ o $180^\circ$), el producto vectorial $\vec{\mu} \times \vec{B}$ (que contiene el término $\sin\phi$) dará estrictamente **cero**. Por esta coincidencia geométrica, el análisis del momento dipolar predice correctamente que no hay rotación, pero intentar usar la fórmula para calcular un valor numérico si la espira estuviera inclinada sería un error grave.

#### La Forma Rigurosa de Resolverlo (Demostración Analítica)

Para calcular el momento de una fuerza en un campo no uniforme, debes abandonar los atajos e ir a la definición fundamental, integrando el torque diferencial sobre cada tramo:

$$\vec{\tau} = \int \vec{r}' \times d\vec{F}$$

donde $\vec{r}'$ es el vector posición desde tu eje de rotación hasta el diferencial de cable $d\vec{l}$.

El problema pide evaluar el torque respecto a la "línea de trazos que pasa por su centro". Vamos a situar el origen de coordenadas $(0,0,0)$ exactamente en el centro geométrico de la espira.

- El ancho de la espira va desde $x = -w/2$ hasta $x = +w/2$.
    
- El largo va desde $y = -L/2$ hasta $y = +L/2$.
    
- El campo magnético tiene dirección constante $-\hat{k}$, pero su magnitud depende de $x$: $\vec{B}(x) = -B(x)\hat{k}$.
    

Asumiremos corriente $I_2$ en sentido horario.

**1. Torque sobre el tramo superior ($y = L/2$):**

La corriente fluye hacia la derecha ($d\vec{l} = dx\,\hat{i}$).

La fuerza diferencial es $d\vec{F} = I_2 (dx\,\hat{i}) \times (-B(x)\hat{k}) = I_2 B(x) dx\,\hat{j}$.

El vector posición desde el centro es $\vec{r}' = x\,\hat{i} + (L/2)\hat{j}$.

$$d\vec{\tau}_{sup} = \vec{r}' \times d\vec{F} = (x\,\hat{i} + (L/2)\hat{j}) \times (I_2 B(x) dx\,\hat{j}) = x I_2 B(x) dx\,(\hat{i} \times \hat{j}) = x I_2 B(x) dx\,\hat{k}$$

$$\vec{\tau}_{sup} = \left( \int_{-w/2}^{w/2} x I_2 B(x) dx \right) \hat{k}$$

**2. Torque sobre el tramo inferior ($y = -L/2$):**

La corriente fluye hacia la izquierda ($d\vec{l} = -dx\,\hat{i}$).

La fuerza diferencial es $d\vec{F} = I_2 (-dx\,\hat{i}) \times (-B(x)\hat{k}) = -I_2 B(x) dx\,\hat{j}$.

El vector posición es $\vec{r}' = x\,\hat{i} - (L/2)\hat{j}$.

$$d\vec{\tau}_{inf} = \vec{r}' \times d\vec{F} = (x\,\hat{i} - (L/2)\hat{j}) \times (-I_2 B(x) dx\,\hat{j}) = -x I_2 B(x) dx\,(\hat{i} \times \hat{j}) = -x I_2 B(x) dx\,\hat{k}$$

$$\vec{\tau}_{inf} = \left( \int_{-w/2}^{w/2} -x I_2 B(x) dx \right) \hat{k}$$

_Conclusión parcial:_ Observa las integrales. $\vec{\tau}_{sup} = -\vec{\tau}_{inf}$. Sin necesidad de resolver la integral logarítmica, **los torques de los tramos horizontales se cancelan exactamente entre sí.**

**3. Torque sobre el tramo izquierdo ($x = -w/2$):**

La corriente fluye hacia abajo ($d\vec{l} = -dy\,\hat{j}$).

Fuerza diferencial: $d\vec{F} = I_2 (-dy\,\hat{j}) \times (-B_1\hat{k}) = I_2 B_1 dy\,\hat{i}$. (Aquí $B_1$ es constante porque $x$ es constante).

Vector posición: $\vec{r}' = -(w/2)\hat{i} + y\,\hat{j}$.

$$d\vec{\tau}_{izq} = \vec{r}' \times d\vec{F} = (-(w/2)\hat{i} + y\,\hat{j}) \times (I_2 B_1 dy\,\hat{i}) = -y I_2 B_1 dy\,(\hat{j} \times \hat{i}) = y I_2 B_1 dy\,\hat{k}$$

Integramos a lo largo del tramo (de $-L/2$ a $L/2$):

$$\vec{\tau}_{izq} = I_2 B_1 \left( \int_{-L/2}^{L/2} y \, dy \right) \hat{k} = I_2 B_1 \left[ \frac{y^2}{2} \right]_{-L/2}^{L/2} \hat{k} = 0$$

**4. Torque sobre el tramo derecho ($x = w/2$):**

Corriente hacia arriba ($d\vec{l} = dy\,\hat{j}$).

Fuerza diferencial: $d\vec{F} = I_2 (dy\,\hat{j}) \times (-B_2\hat{k}) = -I_2 B_2 dy\,\hat{i}$.

Vector posición: $\vec{r}' = (w/2)\hat{i} + y\,\hat{j}$.

$$d\vec{\tau}_{der} = ((w/2)\hat{i} + y\,\hat{j}) \times (-I_2 B_2 dy\,\hat{i}) = y I_2 B_2 dy\,\hat{k}$$

Al igual que en el tramo izquierdo, la integral de $y\,dy$ en un intervalo simétrico es cero.

$$\vec{\tau}_{der} = 0$$

### Suma Total

$$\vec{\tau}_{neta} = \vec{\tau}_{sup} + \vec{\tau}_{inf} + \vec{\tau}_{izq} + \vec{\tau}_{der} = \vec{\tau}_{sup} - \vec{\tau}_{sup} + 0 + 0 = 0$$

Esta es la demostración rigurosa que no asume campo uniforme y prueba irrefutablemente que el momento respecto al eje central es nulo.

### Problema 6

Dos alambres conductores paralelos muy largos, separados $10\text{ cm}$, transportan corrientes iguales de $20\text{ A}$. Los alambres están situados en el aire. Calcular el valor de la fuerza por unidad de longitud entre los alambres si:

**a)** las corrientes tienen el mismo sentido de circulación.
**b)** las corrientes tienen sentidos de circulación opuestos.

Grafique la componente relevante del campo $\vec{B}$ sobre el eje que pasa perpendicular a ambos hilos.
#### Resolución
Según Sears, para dos conductores largos paralelos separados a una distancia r entre ambos:
$$
\frac{F}{L} =  \frac{II'}{2 \pi r}
$$
donde la dirección si las corrientes comparten sentido, se atraen. Si las corrientes difieren en sentido, se repelen.

Tomando un camino de deducción similar:

Situando a los dos conductores (A y B) a lo largo del eje y, tenemos que el campo generado se sitúa únicamente sobre el eje z (la dirección dependiendo de la dirección de la corriente). Consideremos la fuerza provocada por el conductor A sobre el conductor B. La dirección de la fuerza provocada en un segmento del conductor viene dada por la regla de la mano derecha  ($dF = Id \vec{l} \times \vec{B}$). Integrando esto por todo el conductor y teniendo en cuenta que B se mantiene constante tenemos que la fuerza ejercida en todo el conductor resulta:
$$
\begin{align}
\vec{F} = I_{B} \vec{L}\times \vec{B_{A}}
\end{align}
$$
Dado que $\vec{B_{A}}$ es perpendicular a $\vec{L}$: $F = I_{B}LB_{A}$. De manera que la fuerza por unidad de longitud es:
$$
\begin{align}
\frac{F}{L} &   = \frac{I_{B}LB_{A}}{L} \\
 & = \frac{I_{B} L \frac{\mu_0 I_{A}}{4\pi R} \frac{L}{\sqrt{R^2 + (L/2)^2}}}{L} \\
  & = I_{B} I_{A}  \frac{\mu_0}{4\pi R} \frac{L}{\sqrt{R^2 + (L/2)^2}}
\end{align}
$$
Tu intuición de que hay un problema en la simplificación es excelente, pero el error conceptual no está en la variación de la distancia $R$.

Si dos cables son perfectamente paralelos, la distancia perpendicular $R$ entre ellos es **estrictamente constante** a lo largo de toda su longitud. El verdadero error está en una contradicción entre la fórmula que elegiste y la premisa del problema.

**La solución rigurosa:**

Debes usar la expresión del campo para un cable de longitud infinita. Como demostraste en tu Problema 1b, si tomas tu fórmula finita y aplicas el límite cuando $L \to \infty$, el término con la raíz se simplifica y recuperas la Ley de Ampere:

$$B_A = \frac{\mu_0 I_A}{2\pi R}$$

Al ser un cable infinito, este campo $B_A$ es **perfectamente uniforme** en cualquier punto a lo largo del cable B. Por lo tanto, tu integral ahora sí es trivial:

$$\vec{F} = I_B \int_0^L d\vec{l} \times \vec{B}_A = I_B L B_A$$

Sustituyendo el campo correcto:

$$F = I_B L \left( \frac{\mu_0 I_A}{2\pi R} \right)$$

$$\frac{F}{L} = \frac{\mu_0 I_A I_B}{2\pi R}$$


#### 2. Resolución Numérica (Partes a y b)

Dado que las corrientes son iguales ($I_A = I_B = 20\text{ A}$) y la distancia es constante ($R = 10\text{ cm} = 0.1\text{ m}$), la magnitud de la fuerza por unidad de longitud es idéntica para ambos incisos:

$$\frac{F}{L} = \frac{(4\pi \times 10^{-7}\text{ T}\cdot\text{m/A}) (20\text{ A}) (20\text{ A})}{2\pi (0.1\text{ m})}$$

Simplificando $\pi$ y ordenando:

$$\frac{F}{L} = \frac{2 \times 10^{-7} \times 400}{0.1} = \frac{8 \times 10^{-5}}{0.1} = 8 \times 10^{-4}\text{ N/m}$$

- **a) Mismo sentido:** Los campos magnéticos interactúan de forma atractiva. La fuerza es de **$8 \times 10^{-4}\text{ N/m}$ (Atracción)**.
    
- **b) Sentidos opuestos:** Los campos interactúan de forma repulsiva. La fuerza es de **$8 \times 10^{-4}\text{ N/m}$ (Repulsión)**.
    

#### 3. Gráfica del Campo Magnético $\vec{B}$

El problema te pide graficar la componente relevante del campo sobre el eje perpendicular a ambos hilos. Llamemos a este eje $x$, ubicando el Hilo 1 en $x = 0$ y el Hilo 2 en $x = 0.1\text{ m}$. El campo neto en cualquier punto $x$ entre los hilos es la superposición de los campos de cada hilo: $\vec{B}_{neto} = \vec{B}_1 + \vec{B}_2$.

**a) Corrientes en el mismo sentido:**

Por regla de la mano derecha, a la derecha del Hilo 1 el campo entra a la página ($-\hat{k}$). A la izquierda del Hilo 2, el campo sale de la página ($+\hat{k}$). ¡Los campos apuntan en direcciones opuestas!

La componente z es: $B_z(x) = -\frac{\mu_0 I}{2\pi x} + \frac{\mu_0 I}{2\pi (0.1 - x)}$.

En el punto medio exacto ($x = 0.05\text{ m}$), los campos se anulan y $\vec{B} = 0$.

**b) Corrientes en sentidos opuestos:**

El Hilo 1 empuja el campo hacia adentro de la página ($-\hat{k}$). El Hilo 2, al tener la corriente invertida, ahora también empuja el campo hacia adentro de la página a su izquierda ($-\hat{k}$). ¡Los campos se suman!

La componente z es: $B_z(x) = -\frac{\mu_0 I}{2\pi x} - \frac{\mu_0 I}{2\pi (0.1 - x)}$.

En el punto medio, el campo nunca es cero; de hecho, alcanza un mínimo local (un "valle" magnético), pero sigue siendo intensamente negativo.
### Problema 7

Se tiene un cilindro de radio $a$ por el que circula una corriente $I_1$ uniformemente distribuida en la sección transversal. Concéntrico a él se coloca otro cilindro de radios interior y exterior $b$ y $c$ respectively, por el cual circula una corriente $I_2$ uniformemente distribuida en la sección transversal según se muestra en la figura.

**a)** Calcular $\vec{B}$ en todo el espacio en función de $I_1$ e $I_2$.

**b)** Si en un cierto instante un electrón se mueve paralelo al eje de los cilindros a una distancia $2c$ y con una velocidad $\vec{v}$, calcule la fuerza que aparece sobre él y determine la dependencia temporal de la energía cinética.

**c)** ¿Qué relación debe existir entre $I_1$ e $I_2$ para que $\vec{B}$ sea nulo en la zona entre ambos cilindros? ¿Cuál debería ser la relación para que $\vec{B}$ sea nulo en algún radio mayor que el del cilindro exterior?

### Resolución
#### a)
 Trabajaremos en **coordenadas cilíndricas** $(r, \phi, z)$.
 
Empezamos justificando la dirección del campo en el espacio. Notamos que la distribución de corriente tiene simetría cilíndrica, de manera que las lineas de campo magneticas deben ser circulos concentricos al eje del cilindro. Expandiendo la justificación:

- **Inexistencia de componente radial ($B_r = 0$):** Si el campo tuviera una componente radial que sale o entra del cilindro infinito, existiría un flujo magnético neto no nulo a través de una superficie cilíndrica coaxial, lo cual viola la Ley de Gauss para el magnetismo ($\nabla \cdot \vec{B} = 0$).
- **Inexistencia de componente longitudinal ($B_z = 0$):** Como la corriente es estrictamente longitudinal ($\hat{z}$), la Ley de Biot-Savart ($d\vec{l} \times \hat{r}$) dicta que el campo generado debe ser perpendicular a la corriente. Es imposible que una corriente genere un campo paralelo a sí misma.
- **Dependencia exclusiva de $r$:** Al ser un sistema infinito en el eje $z$, trasladarse longitudinalmente no altera el entorno físico (no depende de $z$). Al tener sección transversal circular uniforme, rotar alrededor del eje tampoco altera el entorno (no depende del ángulo $\phi$).

**Conclusión:** Por descarte, el campo solo puede tener componente tangencial $\vec{B} = B_\phi(r) \hat{\phi}$. 


Aplicamos la ley de Ampere $\oint \vec{B} \cdot d\vec{l} = \mu_0 I_{encl}$ definiendo 4 zonas espaciales distintas, calculando el $I_{encl}$ correcto para cada una:

1. Zona 1: interior maciza ($r \le a$)
2. Zona 2: vacía entre cilindros ($a < r < b$)
3. Zona 3: interior del tubo exteriI_{2}or ($b \le r \le c$)
4. Zona 4: exterior total ($r > c$)

Teniendo en cuenta que para la zona 1, $I_{encl}$ será $J_{1}\pi r^2$. Para la zona 2, $I_{encl} = I_{1}$. Para la 3, $I_{encl} = I_{1}  + J_{2}\pi(r^2 - b^2)$ y para la zona 4, $I_{encl} = I_{1} + I_{2}$. 
Finalmente consideramos los valores de las densidades:
$$
\begin{align}
J_{1} &  = \frac{I_{1}}{\pi a^2}  \\
J_{2}  & = \frac{I_{2}}{\pi (c^2-b^2)}
\end{align}
$$
Para encontrar el campo magnético en cada zona, tomamos caminos de integración circulares de radio r.

Empezando con la zona 1, planteamos:
$$
\begin{align}
\oint \vec{B} d \vec{l} = \mu_{0} I_{encl}
\end{align}
$$
Dado que el campo magnético resulta siempre tangente y constante en magnitud sea cual sea el punto del camino circular considerado, la magnitud de la integral es $B(2\pi r)$. Entonces:
$$
\begin{align}
B(2\pi r) &  = \mu_{0} I_{encl} \\
B  & = \frac{\mu_{0}(\frac{I_{1}}{\pi a^2})\pi r^2}{2\pi r} \\
B  & = \frac{\mu_{0}(\frac{I_{1}}{a^2})r}{2\pi} \\
B  & = \frac{\mu_{0}I_{1}r}{2\pi a^2 }
\end{align}
$$
Para la zona 2, tenemos un planteo similar, donde la integral de linea resulta $B(2\pi r)$:
$$
\begin{align}
B(2\pi r) &  = \mu_{0} I_{encl} \\
 & = \mu_{0} I_{1} \\
B  & = \frac{\mu_{0} I_{1}}{2\pi r} \\
\end{align}
$$
Para la zona 3, tenemos un planteo similar, donde la integral de linea resulta $B(2\pi r)$:
$$
\begin{align}
B(2\pi r) &  = \mu_{0} I_{encl} \\
B  & = \frac{\mu_{0}(I_{1}  + \frac{I_{2}}{\pi (c^2-b^2)}{\pi(r^2 - b^2)})}{2\pi r} \\
B  & = \frac{\mu_{0}(I_{1}  + I_{2}\frac{(r^2 - b^2)}{(c^2-b^2)})}{2\pi r} \\
\end{align}
$$
Para la zona 4, tenemos un planteo similar, donde la integral de linea resulta $B(2\pi r)$:
$$
\begin{align}
B(2\pi r) &  = \mu_{0} I_{encl} \\
B  & = \frac{\mu_{0}(I_{1} + I_{2})}{2 \pi r}
\end{align}
$$
Asumiendo que las corrientes fluyen a lo largo del eje longitudinal (dirección $+\hat{k}$ o $+\hat{z}$), la regla de la mano derecha dicta que el campo envuelve al cilindro. En coordenadas cilíndricas, ese giro está representado por el versor azimutal **$\hat{\phi}$** (en algunos textos llamado $\hat{\theta}$). Entonces, tenemos:

$$\vec{B}(r) = \begin{cases} \frac{\mu_{0}I_{1}r}{2\pi a^2 } \hat{\phi} & \text{si } r\leq a \\ \frac{\mu_{0} I_{1}}{2\pi r} \hat{\phi} & \text{si } a<r\leq b \\ \frac{\mu_{0}}{2\pi r} \left( I_{1} + I_{2}\frac{r^2 - b^2}{c^2-b^2} \right) \hat{\phi} & \text{si } b<r\leq c \\ \frac{\mu_{0}(I_{1} + I_{2})}{2 \pi r} \hat{\phi} & \text{si } r> c \end{cases}$$

_Nota: Si $I_1$ e $I_2$ llegaran a tener sentidos opuestos (por ejemplo, $I_2$ negativo), el signo matemático se encargará por sí solo de invertir la dirección del versor $\hat{\phi}$ si la corriente negativa es más grande._

#### b)
Usamos la Fuerza de Lorenz para obtener la fuerza que ejerce un campo magnético sobre una partícula con velocidad $\vec{v}$:
$$
\begin{align}
\vec{F}  & = q \vec{v} \times \vec{B}
\end{align}
$$
Teniendo en cuenta que para un electrón, $q = -1.6 \times 10^{-19}C$ y que la partícula se encuentra en la zona 4, específicamente con $r= 2c$. Pasando a coordenadas cartesianas para efectuar el prudcto cruz, consideramos que el campo durante todo el trayecto de la partícula mantiene una dirección hacia abajo de la misma. Aplicamos el producto cruz:
$$
\begin{align}
\vec{F} &  = -1.6 \times 10^{-19}C (v \hat{k} \times \frac{\mu_{0}(I_{1} + I_{2})}{4 \pi c} -\hat{i} ) \\
\vec{F}  & = -1.6 \times 10^{-19}C (v \frac{\mu_{0}(I_{1} + I_{2})}{4 \pi c} -\hat{j} ) \\
\vec{F}  & = 1.6 \times 10^{-19}C (v \frac{\mu_{0}(I_{1} + I_{2})}{4 \pi c} \hat{j} )
\end{align}
$$
Teniendo en cuenta el **Teorema del Trabajo y la Energía Cinética** ($W = \Delta E_c$):

$\vec{F}$ es el resultado de un producto vectorial entre $\vec{v}$ y $\vec{B}$. Por definición matemática, el resultado de un producto vectorial es **siempre perpendicular** a los vectores originales.

Por lo tanto, la fuerza magnética siempre empuja perpendicularmente a la velocidad del electrón ($\vec{F} \perp \vec{v}$).

Dado que el trabajo es $W = \int \vec{F} \cdot d\vec{r}$, y el desplazamiento va en la misma dirección que la velocidad, el producto escalar será cero. **Los campos magnéticos estáticos nunca realizan trabajo sobre las cargas, solo desvían su trayectoria.** ¿La conclusión para tu respuesta? La energía cinética no cambia en el tiempo; es constante.

**¿Fue correcto pasar a cartesianas?**

Sí, fue un paso lógico, seguro y físicamente válido. Al asignar que $\vec{B}$ apuntaba en $-\hat{i}$, implícitamente "congelaste" al electrón en el eje $+y$ de tu sistema de coordenadas, lo cual te permitió operar con vectores que conoces bien. Tu resultado matemático es impecable para ese punto específico.

**¿Se podía hacer directamente en coordenadas cilíndricas?**

¡Sí, y es mucho más fácil! No necesitas determinantes engorrosos. Los versores cilíndricos ($\hat{r}, \hat{\phi}, \hat{k}$) forman una base ortogonal (a $90^\circ$ entre sí) exactamente igual que ($\hat{i}, \hat{j}, \hat{k}$). Siguen su propia regla de la mano derecha cíclica:

- $\hat{r} \times \hat{\phi} = \hat{k}$
    
- $\hat{\phi} \times \hat{k} = \hat{r}$
    
- **$\hat{k} \times \hat{r} = \hat{\phi}$**
    

Si invertimos el orden de cualquiera de estos, el resultado cambia de signo (ej. $\hat{k} \times \hat{\phi} = -\hat{r}$).

Mira cómo sale el cálculo en dos líneas manteniendo la generalidad para cualquier punto del cilindro:

1. Tu velocidad es paralela al eje: $\vec{v} = v\hat{k}$
2. El campo en la zona 4 es azimutal: $\vec{B} = B\hat{\phi}$
3. La carga del electrón es negativa: $q = -e$
    
$$\vec{F} = (-e) (v\hat{k}) \times (B\hat{\phi})$$

$$\vec{F} = -evB (\hat{k} \times \hat{\phi})$$

Sabiendo que $\hat{k} \times \hat{\phi} = -\hat{r}$:
$$\vec{F} = -evB (-\hat{r}) = +evB\,\hat{r}$$

**Interpretación:** La fuerza apunta en $+\hat{r}$, es decir, **radialmente hacia afuera**, alejando al electrón del cilindro.

_(Nota lo genial de tu planteo en cartesianas: como habías "congelado" al electrón en el eje $+y$, la dirección hacia afuera en ese punto exacto es $+\hat{j}$. Tu resultado cartesiano coincide a la perfección con la realidad radial general)._
#### c

**1. "Nulo en la zona entre ambos cilindros"**
El campo en la Zona 2 es simplemente el generado por el cilindro interno:

$$B = \frac{\mu_{0} I_{1}}{2\pi r}$$

Para que este campo sea estrictamente nulo, la única relación posible es que **$I_1 = 0$**.

Físicamente tiene todo el sentido: en la zona hueca, tu curva de Ampere aún no ha encerrado nada del cilindro exterior ($I_2$). Al campo en esa zona no le importa en absoluto lo que pase con $I_2$, solo ve a $I_1$.

**2. "Nulo en algún radio mayor que el cilindro exterior" (Zona 4)**

Tu resolución aquí es **perfectamente correcta**:

$$I_1 = -I_2$$

según la fórmula de la Zona 4, el campo depende del término $(I_1 + I_2)$. Si $I_1 = -I_2$, el campo no solo es nulo en "algún" radio mayor, sino que es **nulo en absolutamente todo el espacio exterior** ($r > c$).

Esta es exactamente la razón de ser de los cables coaxiales reales (como los de la televisión o internet). La corriente va por el núcleo central ($I_1$) y retorna por la malla exterior ($I_2$). Al ser $I_1 = -I_2$, el campo magnético fuera del cable es cero, lo que evita interferencias con otros dispositivos electrónicos cercanos.

### Problema 8

Repetir el problema anterior si en lugar de dar como datos las corrientes $I_1$ e $I_2$, se dan las densidades volumétricas de corriente $\vec{J}_1$ y $\vec{J}_2$.

#### Resolución

Dado que ya dan $\vec{J}_1$ y $\vec{J}_2$ como datos primarios, las ecuaciones de corriente encerrada se vuelven directas:

El planteo de Ampere $\oint \vec{B} \cdot d\vec{l} = B(2\pi r) = \mu_0 I_{encl}$ se mantiene intacto. Solo cambian las expresiones de $I_{encl}$:

- **Zona 1 ($r \le a$):** $I_{encl} = J_1 (\pi r^2)$
    
    $B(2\pi r) = \mu_0 J_1 \pi r^2 \implies \vec{B} = \frac{\mu_0 J_1 r}{2} \hat{\phi}$
    
- **Zona 2 ($a < r \le b$):** $I_{encl} = J_1 (\pi a^2)$ _(Encierras todo el cilindro interno)_
    
    $B(2\pi r) = \mu_0 J_1 \pi a^2 \implies \vec{B} = \frac{\mu_0 J_1 a^2}{2r} \hat{\phi}$
    
- **Zona 3 ($b < r \le c$):** $I_{encl} = J_1 (\pi a^2) + J_2 \pi (r^2 - b^2)$
    
    $B(2\pi r) = \mu_0 \pi \left[ J_1 a^2 + J_2(r^2 - b^2) \right] \implies \vec{B} = \frac{\mu_0}{2r} \left[ J_1 a^2 + J_2(r^2 - b^2) \right] \hat{\phi}$
    
- **Zona 4 ($r > c$):** $I_{encl} = J_1 (\pi a^2) + J_2 \pi (c^2 - b^2)$
    
    $\vec{B} = \frac{\mu_0}{2r} \left[ J_1 a^2 + J_2(c^2 - b^2) \right] \hat{\phi}$

### Problema 9

**Estructura del Toroide:** Una bobina toroidal consiste en un alambre enrollado firmemente alrededor de una forma circular con sección transversal rectangular o circular. El campo magnético se encuentra completamente confinado en el interior del toro.

Calcular en todo el espacio el campo $\vec{B}$ creado por una bobina toroidal de $5000$ vueltas que transporta una corriente de $12\text{ mA}$.

**a)** Considerar que la sección del toro es rectangular ($R_{int} = 30\text{ cm}$, $R_{ext} = 50\text{ cm}$ y $h = 10\text{ cm}$). Grafique la componente relevante del campo $\vec{B}$ en función de la coordenada radial.

**b)** Repetir considerando que el campo $\vec{B}$ dentro del toro corresponde al evaluado con $R_m = 40\text{ cm}$ (radio medio).

**c)** Comparar cualitativa y cuantitativamente los resultados. Discutir.

### Resolución
Entender **por qué** el campo tiene que ser circular (azimutal) es el primer paso antes de meterse en las cuentas.

#### ¿Por qué las líneas de campo son concéntricas (azimutales)?

Imagina el toroide como una dona apoyada sobre una mesa (el plano $xy$). El centro del agujero de la dona es el origen de coordenadas $(0,0)$, y el eje $z$ atraviesa ese agujero hacia arriba.

Usaremos el argumento de las simetrías (las mismas que usaste para el cilindro macizo) en coordenadas cilíndricas $(r, \phi, z)$:

1. **Simetría Rotacional:** Si giras el toroide alrededor de su eje central (el eje $z$), la geometría y las corrientes se ven exactamente iguales desde cualquier ángulo. Esto significa que **el campo magnético no puede depender de la coordenada angular $\phi$**; su magnitud debe ser la misma en todos los puntos de cualquier círculo centrado en el origen.
2. **Inexistencia de Componente Radial ($B_r = 0$):** Supongamos que el campo tuviera una componente radial (apuntando hacia adentro o hacia afuera del agujero central). Si tomas una superficie cilíndrica cerrada que envuelva al toroide por dentro y por fuera, esas líneas de campo radiales entrarían o saldrían, creando un flujo magnético neto distinto de cero. Esto violaría la Ley de Gauss para el magnetismo ($\oint \vec{B} \cdot d\vec{A} = 0$, ¡no hay monopolos!). Por lo tanto, el campo no puede "escurrirse" hacia los costados.
3. **Inexistencia de Componente Axial ($B_z = 0$):** Imagina que el campo apunta hacia arriba (dirección $+\hat{k}$). Si inviertes la corriente en las espiras del toroide, la Ley de Biot-Savart te dice que el campo debe invertirse (apuntar hacia $-\hat{k}$). Sin embargo, si en lugar de invertir la corriente, simplemente "volteas" el toroide como un panqueque (lo que es físicamente idéntico si inviertes la corriente simultáneamente), una hipotética componente axial debería permanecer inalterada. La única forma de que no haya contradicciones lógicas es que la componente paralela al eje central sea cero.

**Conclusión:** Descartadas las direcciones radial y axial, al campo magnético no le queda otra opción física más que apuntar en la dirección circunferencial (tangencial a los círculos centrados en el eje). Es decir, $\vec{B} = B_\phi \hat{\phi}$.

Las líneas de campo son anillos cerrados perfectos que circulan "atrapados" dentro de la dona.

Ahora que sabemos que el campo describe círculos (dirección $\hat{\phi}$) y solo depende del radio $r$, la **Ley de Ampere** es la herramienta ideal. Tomaremos caminos de integración que sean circunferencias de radio $r$ centradas en el eje del toroide.
#### a) Toroide de sección rectangular

Al aplicar $\oint \vec{B} \cdot d\vec{l} = \mu_0 I_{encl}$ en una circunferencia de radio $r$, el lado izquierdo de la ecuación siempre será:

$$B (2\pi r) = \mu_0 I_{encl}$$

Debemos evaluar $I_{encl}$ en tres zonas del espacio:

- **Zona interior del "agujero" ($r < R_{int}$):** ¿Cuánta corriente atraviesa el área del círculo imaginario? Cero. Por lo tanto, por ley de Ampere, $\vec{B} = 0$.
    
- **Zona exterior al toroide ($r > R_{ext}$):** Si el círculo imaginario abraza todo el toroide por fuera, el área encierra cada vuelta de alambre _dos veces_: una vez cuando la corriente sube (entra a la dona) y otra vez cuando la corriente baja (sale de la dona). Se cancelan perfectamente. Corriente neta encerrada = 0. Por lo tanto, $\vec{B} = 0$. (Esto demuestra que el campo está "confinado").
    
- **Zona DENTRO del material del toroide ($R_{int} < r < R_{ext}$):** Esta es la importante. Tu círculo imaginario de radio $r$ está hundido en medio de la dona. Su área encierra a las espiras _solamente_ en su trayecto de bajada (o subida) por la pared interna del agujero central. Como el toroide tiene $N$ vueltas, estás encerrando la corriente $N$ veces.
    
    $$I_{encl} = N \cdot I$$
    
    Al despejar, obtenemos la fórmula exacta del campo dentro del toroide: $B(r)$.
	$$
	\begin{align}
	B(2\pi r) &  = \mu_{0} I_{encl} \\
	B(r) & = \frac{\mu_{0} N \cdot I}{2 \pi r} \\
	
	\vec{B(r) }& = \frac{\mu_{0} N \cdot I}{2 \pi r} \hat{\phi}
	\end{align}
	$$
    

Por tanto, tenemos que:
$$
\vec{B}(r) = \begin{cases}
0 & \text{si} & r \leq r_{\text{int}} \\
	\frac{\mu_{0} N \cdot I}{2 \pi r} \hat{\phi}  & \text{si} & r_{\text{int}}< r<r_{\text{ext}} \\
	0 & \text{si} & r\geq r_{\text{ext}}
\end{cases}
$$
- Nota que el campo _no_ es uniforme; depende de $r$. A menor radio (más cerca del agujero central), mayor campo. _(La altura $h$ de la sección transversal no afecta a la magnitud del campo en Ampere, es un distractor en este cálculo)_.
#### b) El modelo de "Radio Medio" ($R_m$)

El enunciado pide calcular el campo usando un único valor de radio.

El radio medio es el promedio aritmético entre el radio interno y externo: $R_m = \frac{30\text{ cm} + 50\text{ cm}}{2} = 40\text{ cm}$.


Si tomamos el radio promedio (efectivamente fijándolo a un solo número), podemos interpretar el término $\frac{N}{2\pi r}$ como el número de vueltas por unidad de longitud ($n$),  el campo podría ser escrito como:
$$
\begin{align}
\vec{B}(r) = \mu_{0}nI
\end{align}
$$
Igual que en el centro de un solenoide recto largo.

Toma la fórmula que obtuviste en el inciso (a), pero en lugar de dejar la variable $r$, evalúala numéricamente asumiendo que **todo** el campo dentro del toroide es constante y tiene el valor que tendría en $r = 40\text{ cm}$. Obtendrás un único número (un campo "uniforme").

#### c) Comparación
La ecuación del punto a demuestra que el campo no es uniforme dentro del toroide, pues va disminuyendo linealmente conforme a un factor r. Sin embargo, si el grueso del toroide ($r_{\text{ext} - r_{\text{int}}}$) es pequeño en comparación a la distancia del centro del eje axial del toroide, entonces se podría aplicar directamente la simplificación del punto b. Sin embargo, no sería aceptable asumir que el campo es constante dentro de un toroide grueso.
### Problema 10

Determinar la corriente, en valor y sentido, que debe circular por un alambre recto muy largo colocado en el eje del toroide del problema anterior para anular el campo $\vec{B}$ dentro del mismo. Graficar la componente relevante del campo en función del radio y dibujar las líneas de campo $\vec{B}$ en todo el espacio.

### Resolucion
Nace la intuición de preguntarte _"¿este ejercicio solo hace sentido si interpreto el r como constante?"_. La respuesta es un rotundo **NO**. De hecho, usar la simplificación del radio medio (constante) aquí arruinaría el ejercicio. Este problema está diseñado para mostrarte una coincidencia geométrica hermosa en el electromagnetismo.

Fíjate en la forma matemática de los dos campos magnéticos involucrados:

1. **Campo del toroide (en su interior):** $B_{tor} = \frac{\mu_0 N I_{tor}}{2\pi r}$

2. **Campo de un alambre infinito:** $B_{hilo} = \frac{\mu_0 I_{hilo}}{2\pi r}$
    

**¡Ambos campos tienen exactamente la misma dependencia espacial ($1/r$)!** Esto significa que si logras que se anulen en un radio específico (por ejemplo $r = 31\text{ cm}$), se anularán mágicamente en _absolutamente todos_ los radios dentro del toroide ($30 < r < 50$). No necesitas ninguna aproximación. Sus curvas hiperbólicas se calcan a la perfección.

#### 1. Determinar el valor de la corriente ($I_{hilo}$)

Para que el campo se anule dentro del toroide, la suma vectorial de ambos campos debe ser cero en la zona $R_{int} < r < R_{ext}$. Dado que ambos campos son azimutales, se opera directamente con las magnitudes:

$$B_{neto} = B_{tor} + B_{hilo} = 0$$

$$\frac{\mu_0 N I_{tor}}{2\pi r} + \frac{\mu_0 I_{hilo}}{2\pi r} = 0$$

Factorizando el término común $\frac{\mu_0}{2\pi r}$:

$$N I_{tor} + I_{hilo} = 0$$

$$I_{hilo} = -N I_{tor}$$

Insertando los datos numéricos de tu problema ($N = 5000$, $I_{tor} = 12\text{ mA} = 0.012\text{ A}$):

$$I_{hilo} = - (5000)(0.012\text{ A}) = \mathbf{-60\text{ A}}$$

El hilo central debe transportar una enorme corriente de $60\text{ A}$.

#### 2. Determinar el sentido

El signo negativo en la matemática nos dice que la corriente del hilo debe ir en tal sentido que genere un campo opuesto al del toroide.

- Si por la regla de la mano derecha el campo del toroide gira en sentido **antihorario** ($+\hat{\phi}$), el campo del hilo debe girar en sentido **horario** ($-\hat{\phi}$). En otras palabras, si la corriente del toroide va en el sentido $\hat{k}$, la corriente del hilo debe dirigirse en el sentido $- \hat{k}$. Para que un hilo vertical central genere un campo horario, su corriente debe fluir **hacia abajo** ($-\hat{k}$).

#### 3. El gráfico y el "plot twist" en todo el espacio

El problema te pide graficar el campo neto en _todo el espacio_. Aquí es donde el problema se vuelve fascinante.

Habíamos definido las zonas del toroide:

- **Zona Agujero ($r < 30\text{ cm}$):** El toroide aporta $B=0$. ¡Pero el hilo infinito existe allí! El campo neto es el del hilo: $B_{neto} = B_{hilo}$.
- **Zona Toroide ($30 < r < 50\text{ cm}$):** Ambos campos existen y se cancelan. $B_{neto} = 0$.
- **Zona Exterior ($r > 50\text{ cm}$):** El toroide aporta $B=0$. El campo del hilo sigue existiendo hasta el infinito. $B_{neto} = B_{hilo}$.

Con la introducción de ese hilo central para "limpiar" el campo dentro del toroide, terminaste **ensuciando todo el resto del universo**.
![Pasted image 20260624104746](assets/Pasted%20image%2020260624104746.png)