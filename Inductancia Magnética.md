---
id: 20260624105202
aliases: []
tags:
  - uncataloged
created: 2026-06-24 10:52
status: draft
---
# Inductancia Magnética

Física para Informática - 1er Cuatrimestre 2024

Guía 3: Inducción electromagnética

**1.** La bobina de la figura está dentro de un campo $\vec{B}$ normal a su plano que varía como $B=(0.04+0.01~t)~\text{T}$, para $t$ medido en segundos. Si la bobina tiene 50 espiras, determinar el valor de la f.e.m. inducida en la bobina en función del tiempo e indique el sentido de la corriente que se induciría en la bobina. Considere que $a=5~\text{cm}$ (ancho) y $b=10~\text{cm}$ (alto).
![Pasted image 20260624105815](assets/Pasted%20image%2020260624105815.png)

### Resolución 1
Interpretamos cada vuelta de la bobina como una espira que forma un circuito cerrado. Definimos el vector área $\vec{A}$ con dirección hacia adentro de la página $\hat{k}$, en la misma dirección que el campo $\vec{B}$.

De acuerdo a Sears:
"""
If we have a coil with N identical turns, and if the flux varies at the same rate $d \Phi_{B}$ through each turn, the total rate of change through all the turns is N times as large as for a single turn.
$$\mathcal{E} = -N \frac{d\Phi_B}{dt} \tag{29.4}$$
"""
Tenemos que el campo magnético es el mismo y uniforme a través de todo el bucle, de forma que para todo el bucle, el flujo puede ser calculado como $BA\cos\phi$, donde $\phi=0^\circ$:
$$
\begin{align}
 \frac{d\Phi_{B}}{d t}  & = A\frac{dB}{dt}  \\
  & = 0.01 (0.05m \times 0.1m) \implies \frac{d\Phi_{B}}{d t} >0 
\end{align}
$$
Esto significa que tanto la corriente como la f.e.m. es negativa. Según la regla de la mano derecha, una corriente positiva se movería clockwise. Pero dado que es negativa, se moverá counter-clockwise. Finalmente calculamos la magnitud con:
$$
\begin{align}
\mathcal{E} &  = -N \frac{d\Phi_B}{dt} \\
 & = -50 ( 0.01 (0.05m \times 0.1m)) V \\
 
  & = -0.0025V
\end{align}
$$


---

**2.** El cuadro de la figura de $5~\text{cm}$ de lado, que se mueve a una velocidad uniforme de $3~\text{m/s}$, penetra en una región de $20~\text{cm}$ de lado donde hay un campo $\vec{B}$, uniforme y normal a la dirección del movimiento, de intensidad $B=0.2~\text{T}$. Si el cuadro está formado por 50 espiras, determinar y graficar el valor de la f.e.m. inducida sobre él en función de su posición. Si el cuadro es de un material conductor, determinar el valor y el sentido de la corriente inducida.

![Pasted image 20260625124322](assets/Pasted%20image%2020260625124322.png)
### Resolución
El problema acá reside en que al recién penetrar a la región de 0.2m de lado, solo una parte del área del cuadrado estará siendo sometido al campo de la región. De manera análoga, este problema también ocurre al recién empezar a salir de la región. Mientras todo el cuadrado se encuentra contenido en la región, el campo y el área del cuadrado serán el mismo, y por tanto $d \frac{\Phi_{B}}{dt} =0$ y la f.e.m será 0. Es decir, en este problema no es $\vec{B}$ el que varía, sino el área del cuadrado $\vec{A}$.

Para modelar este problema, planteamos un sistema de coordenadas cartesianas, donde la región se encuentra ubicada en el origen, con límites horizontales en $x=0m$ y $x =0.2m$. El cuadrado, de alto $l$ y ancho $a$, se mueve con velocidad $\vec{v} = 3 \frac{m}{s} \hat{i}$. Tomamos en consideración el límite derecho del cuadrado para posicionarlo como una partícula en el sistema. En el segundo 0, el cuadrado se encuentra en $x=0$.
$$
\begin{align}
x = & 3 \frac{m}{s} t \\
\end{align}
$$
Usando esta fórmula, calculamos límites en el tiempo de interés. Empezamos con el punto en el que el cuadrado es sumergido por completo en la región.
$$
\begin{align} \\
\frac{0.05m}{3 \frac{m}{s}}  & =  t_{1} \\
\end{align}
$$
Para obtener el tiempo en el que el ancho de cuadrado sometido al campo empieza a reducirse, calculamos el instante en el que el cuadrado alcanza el límite derecho de la región.
$$
\begin{align} \\
\frac{0.2m}{3 \frac{m}{s}}  & =  t_{2} \\
\end{align}
$$
Luego, calculamos el punto en el cuadrado deja la región por completo:
$$
\begin{align} \\
\frac{0.25m}{3 \frac{m}{s}}  & =  t_{3} \\
\end{align}
$$
Usamos estos límites de tiempo para definir el ancho sometido al campo de la región en términos de t:
$$
a(t)= \begin{cases} \\
3 \frac{m}{s}t  & \text{si} &  0\leq t_{1}\\
0.05 m  & \text{si} & t_{1}<t\leq t_{2}\\
0.05m - \left( 3 \frac{m}{s}t \right)-0.2m   & \text{si} & t_{2}<t\leq t_{3} \\
0m  & \text{si} & t>t_{3}
\end{cases}
$$

 Si definimos la dirección del vector área del cuadrado $\vec{A}$, en la misma dirección que el campo, tenemos que el flujo viene dado por:
$$
\begin{align}
\Phi_{B} = \int \vec{B} \cdot \vec{A} = BA\cos \phi = Bha
\end{align}
$$
de forma que:
$$
\begin{align}
\frac{d\Phi_{B}}{dt} = Bh \frac{da}{dt}
\end{align}
$$
Entonces:
$$
\frac{d\Phi_{B}}{dt} =  \begin{cases}
Bh \cdot 3 \frac{m}{s}  & \text{si} & t\leq t_{1} \\
0 & \text{si} & t_{1}<t\leq t_{2} \\
- Bh \cdot 3 \frac{m}{s} & \text{si}&t_{1}<t\leq t_{2} \\
0 & \text{si}& t> t_{2}
\end{cases}
$$
Finalmente, obtenemos la f.e.m:
$$
\mathcal{E} =\begin{cases}
-Bh \cdot 3 \frac{m}{s}  & \text{si} & t\leq t_{1} \\
0 & \text{si} & t_{1}<t\leq t_{2} \\
Bh \cdot 3 \frac{m}{s} & \text{si}&t_{1}<t\leq t_{2} \\
0 & \text{si}& t> t_{2}
\end{cases}
$$
Mientras el cuadrado va entrando a la región, obtiene una f.e.m en dirección counter-clockwise por la regla de la mano derecha. La corriente (si fuera un material conductor) seguiría este mismo sentido. Una vez ya dentro de la región, no experimenta f.e.m dado que el flujo mágnetico que cruza por el cuadrado no varía. Al empezar a salir, sin embargo, obtiene una f.e.m en dirección clockwise por la regla de la mano derecha. La corriente (si fuera un material conductor) seguiría este mismo sentido. 

### Resolución con respecto a la posición
El problema acá reside en que al recién penetrar a la región de 0.2m de lado, solo una parte del área del cuadrado estará siendo sometido al campo de la región. De manera análoga, este problema también ocurre al recién empezar a salir de la región. Mientras todo el cuadrado se encuentra contenido en la región, el campo y el área del cuadrado serán el mismo, y por tanto $d \frac{\Phi_{B}}{dt} =0$ y la f.e.m será 0. Es decir, en este problema no es $\vec{B}$ el que varía, sino el área del cuadrado $\vec{A}$.

Para modelar este problema, planteamos un sistema de coordenadas cartesianas, donde la región se encuentra ubicada en el origen, con límites horizontales en $x=0m$ y $x =0.2m$. El cuadrado, de alto $l$ y ancho $a$, se mueve con velocidad $\vec{v} = 3 \frac{m}{s} \hat{i}$. Tomamos en consideración el límite derecho del cuadrado para posicionarlo como una partícula en el sistema. 

Tenemos 4 posiciones de interés que definen el ancho de la espira dentro del campo en términos de la posición $x$ de su arista derecha:

$$a(x)= \begin{cases} x & \text{si } x \leq 0.05\text{ m} \\ 0.05\text{ m} & \text{si } 0.05\text{ m} < x \leq 0.20\text{ m} \\ 0.20\text{ m} - (x-0.05\text{ m}) & \text{si } 0.20\text{ m} < x \leq 0.25\text{ m} \\ 0\text{ m} & \text{si } x > 0.25\text{ m} \end{cases}$$

Si definimos la dirección del vector área del cuadrado $\vec{A}$ en la misma dirección que el campo, el flujo para una sola espira viene dado por:

$$\Phi_{B} = \int \vec{B} \cdot d\vec{A} = BA\cos(0^\circ) = Bha$$

Por la Ley de Faraday para $N$ espiras, y aplicando la regla de la cadena:

$$\mathcal{E} = -N \frac{d\Phi_{B}}{dt} = -N \cdot Bh \frac{da}{dt} = -N \cdot Bh \frac{da}{dx} \frac{dx}{dt}$$

Sabiendo que $\frac{dx}{dt} = v = 3\frac{\text{m}}{\text{s}}$ y derivando $a(x)$ respecto a $x$:

$$\frac{da}{dx} = \begin{cases} 1 & \text{si } x \leq 0.05\text{ m} \\ 0 & \text{si } 0.05\text{ m} < x \leq 0.20\text{ m} \\ -1 & \text{si } 0.20\text{ m} < x \leq 0.25\text{ m} \\ 0 & \text{si } x > 0.25\text{ m} \end{cases}$$

Multiplicando por los factores constantes (donde $N \cdot B \cdot h \cdot v = 50 \cdot 0.2\text{ T} \cdot 0.05\text{ m} \cdot 3\frac{\text{m}}{\text{s}} = 1.5\text{ V}$), obtenemos la f.e.m. en función de la posición:

$$\mathcal{E}(x) = \begin{cases} -1.5\text{ V} & \text{si } 0\text{ m} < x \le 0.05\text{ m} \text{ (Entrando)}\\ 0\text{ V} & \text{si } 0.05\text{ m} < x \le 0.20\text{ m} \text{ (Adentro)} \\ 1.5\text{ V} & \text{si } 0.20\text{ m} < x \le 0.25\text{ m} \text{ (Saliendo)} \\ 0\text{ V} & \text{si } x > 0.25\text{ m} \text{ (Afuera)} \end{cases}$$

Mientras el cuadrado va entrando a la región, obtiene una f.e.m en dirección counter-clockwise por la regla de la mano derecha. La corriente (si fuera un material conductor) seguiría este mismo sentido. Una vez ya dentro de la región, no experimenta f.e.m dado que el flujo mágnetico que cruza por el cuadrado no varía. Al empezar a salir, sin embargo, obtiene una f.e.m en dirección clockwise por la regla de la mano derecha. La corriente (si fuera un material conductor) seguiría este mismo sentido. 


---

**3.** Una bobina rectangular con lados $a=5~\text{cm}$ y $b=10~\text{cm}$, formada por 100 espiras gira con una frecuencia angular constante de $1500~\text{r.p.m.}$ en un campo $\vec{B}$ uniforme con $B=1~\text{T}$ Graficar el valor de la f.e.m. inducida en función del ángulo de giro y hallar sus valores en las posiciones 1, 2 y 3.

![Pasted image 20260625124430](assets/Pasted%20image%2020260625124430.png)

### Resolución
El campo que atraviesa la bobina va a depender del ángulo en el cual la misma se encuentra posicionada con respecto al campo, efectivamente alterando el flujo magnético a medida que la bobina recorre distintos ángulos. Tomaremos el vector del área $\vec{A}$ siguiendo las líneas del campo en la posición 1, también tendremos en consideración que el campo es uniforme y forma el mismo ángulo para cada punto de la bobina en cada posición determinada. Lo que significa que para una posición determinada:

$$
\Phi_{B} = BA\cos \phi
$$

Consideremos las 3 posiciones propuestas:
- Posición 1: la bobina forma un ángulo de 90 grados con el campo. El vector área forma un ángulo $\phi = 0^\circ$ con el campo, por tanto: $\Phi_{B} = BA$
- Posición 2: la bobina forma un ángulo de 45 grados con el campo. El vector área forma un ángulo $\phi = 45^\circ$ con el campo, por tanto: $\Phi_{B} = BA \cos 45^\circ$
- Posición 3: la bobina forma un ángulo de 0 grados con el campo. El vector área forma un ángulo $\phi = 90^\circ$ con el campo, por tanto: $\Phi_{B} = 0$
Con esto comprobamos existe una variación constante en el flujo magnético.

Ahora, transformemos la frecuencia angula en rpm a radianes por segundo:

$$
\begin{align}
w &  = 1500 \frac{\text{revolutions}}{1m} \times \frac{1m}{60s} \times  \frac{2\pi}{\text{revolution}} \\
  & = \frac{2\pi}{60} 1500 \frac{\text{radianes}}{s}

\end{align}
$$

Nos piden $\mathcal{E}(\theta)$, siendo $\theta$ el ángulo de giro. Primero intentamos buscar una expresión de la tasa de cambio del flujo magnético dependiente del ángulo de giro. Aplicaremos regla de la cadena:
$$
\begin{align}
 \frac{d\Phi_{B}}{dt}  & =\frac{d}{dt} ( BA\cos\theta )  \\
  & = BA \frac{d \cos \theta}{dt} 
\end{align}
$$
Asumiendo que empezamos en posición 1, con $t=0$ y $\theta=0$, tenemos que:
$$
\begin{align}
\theta(t) &  = \vec{w}t \\
\cos(\theta) &  = \cos(wt) \\
\frac{d \cos \theta}{dt}  & = \frac{d \cos(wt)}{dt} \frac{d (wt)}{dt} \\
& = -w \sin(wt)  \\
& = -w \sin(\theta) 
\end{align}
$$
Por tanto:
$$
\begin{align}
\frac{d\Phi_{B}}{dt}  & = BA \frac{d \cos \theta}{dt} \\
 & = -BAw\sin(\theta) 
\end{align}
$$
Por tanto:
$$
\begin{align}
\mathcal{E}(\theta)  & = -N( -BAw\sin(\theta) ) \\
  &= NBA w \sin \theta \\
   & = 100 \times 1 T \times (0.05m \times 0.1m) \times w \sin(\theta)
\end{align}
$$

**2. Valores numéricos**

Primero, resolvemos el escalar de la frecuencia angular $\omega$:

$$\omega = \frac{2\pi}{60} 1500~\text{rad/s} = 50\pi~\text{rad/s} \approx 157.08~\text{rad/s}$$

Calculamos la amplitud máxima ($\mathcal{E}_{max} = NBA\omega$):

$$\mathcal{E}_{max} = 100 \times 1~\text{T} \times (0.005~\text{m}^2) \times 50\pi~\text{rad/s} = 25\pi~\text{V} \approx 78.54~\text{V}$$

La ecuación final queda definida como:

$$\mathcal{E}(\theta) = 25\pi \sin(\theta)~\text{V}$$

Evaluamos en las posiciones indicadas:

- **Posición 1 ($\theta = 0^\circ$):**
    
    $$\mathcal{E}(0^\circ) = 25\pi \sin(0^\circ) = 0~\text{V}$$
    
- **Posición 2 ($\theta = 45^\circ$):**
    
    $$\mathcal{E}(45^\circ) = 25\pi \sin(45^\circ) = 25\pi \frac{\sqrt{2}}{2}~\text{V} \approx 55.54~\text{V}$$
    
- **Posición 3 ($\theta = 90^\circ$):**
    
    $$\mathcal{E}(90^\circ) = 25\pi \sin(90^\circ) = 25\pi~\text{V} \approx 78.54~\text{V}$$

El problema también requiere "Graficar el valor de la f.e.m. inducida en función del ángulo de giro". Debes incluir un gráfico de una onda senoidal estándar partiendo del origen $(0,0)$, con un pico máximo de $78.54~\text{V}$ en $\theta = \frac{\pi}{2}$ ($90^\circ$) y cruzando el eje horizontal en $\theta = \pi$ ($180^\circ$).
![Pasted image 20260625142553](assets/Pasted%20image%2020260625142553.png)

--- 
**4.** Un conductor rectilíneo muy largo lleva una corriente variable en el tiempo $I(t)$.

- **a)** Si el cuadro se aleja con velocidad constante $\vec{v}$, calcular la fuerza electromotriz inducida y el sentido de la corriente inducida en el cuadro si $I(t)$ es creciente. Considerar $x(0)=D$ (ver figura).
- **b)** Repetir el cálculo si la velocidad del cuadro es paralela al conductor rectilíneo.
    
![Pasted image 20260625142607](assets/Pasted%20image%2020260625142607.png)

### Resolucion
_(Asumiremos por convención estándar que la figura muestra una espira rectangular de altura $a$ paralela al cable, y ancho $b$ perpendicular al cable. El cable largo coincide con el eje $y$)._
#### a) El cuadro se aleja con velocidad $\vec{v}$ perpendicular al hilo

**Paso 1: Escribir el flujo magnético dependiente del tiempo**

El campo magnético del hilo a una distancia $x$ es $B = \frac{\mu_0 I(t)}{2\pi x}$.

La posición de la arista más cercana de la espira es dependiente del tiempo: $x(t) = D + vt$. La arista lejana está en $x(t) + b$.

Integrando el campo sobre el área de la espira, el flujo total en un instante $t$ es:

$$\Phi_B(t) = \int_{x(t)}^{x(t)+b} \frac{\mu_0 I(t)}{2\pi x} a \, dx = \frac{\mu_0 a I(t)}{2\pi} \ln\left( \frac{x(t) + b}{x(t)} \right)$$

**Paso 2: Derivar aplicando la regla del producto**

Aquí es donde la matemática te revela la física. Tienes dos funciones que dependen del tiempo multiplicándose: $I(t)$ y el término del logaritmo natural (que depende de $x(t)$).

$$\mathcal{E} = -\frac{d\Phi_B}{dt} = - \frac{\mu_0 a}{2\pi} \left[ \underbrace{ \frac{dI(t)}{dt} \ln\left( \frac{x(t) + b}{x(t)} \right) }_{\text{FEM por Transformación}} + \underbrace{ I(t) \frac{d}{dt} \ln\left( \frac{x(t) + b}{x(t)} \right) }_{\text{FEM por Movimiento}} \right]$$


Para derivar $\ln\left( \frac{x(t) + b}{x(t)} \right)$ respecto al tiempo, la forma más segura y rápida de evitar errores con la regla del cociente es aplicar las propiedades de los logaritmos para separarlo primero en una resta:

$$f(t) = \ln(x(t) + b) - \ln(x(t))$$

Ahora, derivamos ambos términos respecto al tiempo aplicando la regla de la cadena elemental (y recordando que $\frac{dx}{dt} = v$):

$$\frac{df}{dt} = \left( \frac{1}{x(t) + b} \cdot v \right) - \left( \frac{1}{x(t)} \cdot v \right)$$

Sacamos $v$ como factor común y buscamos denominador común para juntar las fracciones:

$$\frac{df}{dt} = v \left[ \frac{x(t) - (x(t) + b)}{x(t)(x(t) + b)} \right]$$

$$\frac{df}{dt} = v \left[ \frac{-b}{x(t)(x(t) + b)} \right] = \frac{-b \cdot v}{x(t)(x(t) + b)}$$

Si insertamos esta derivada correcta en tu planteo original de la Ley de Faraday, la fuerza electromotriz total queda:

$$\mathcal{E} = - \frac{\mu_0 a}{2\pi} \left[ \frac{dI(t)}{dt} \ln\left( \frac{x(t) + b}{x(t)} \right) - I(t) \frac{b \cdot v}{x(t)(x(t) + b)} \right]$$

Si I es creciente, el primer término es positivo, y el segundo término es negativo. Para determinar la dirección de la corriente inducida (y del la fem), se precisa determinar cuál de los dos términos es dominante. Si el primer término lo es, la corriente circulará counter-clockwise. Si el segundo término lo es, la corriente circulará clockwise.
#### b) El cuadro se mueve paralelo al hilo

Si la velocidad es paralela al cable (por ejemplo, en el eje $y$), la distancia $x$ entre el cable y la espira **no cambia**.

$$x(t) = D = \text{constante}$$

Si observas la ecuación de tu flujo magnético, el término $\ln\left( \frac{D + b}{D} \right)$ se convierte en una constante espacial estática.

Al derivar para obtener la FEM, la derivada de esa constante es cero. La "FEM de movimiento" desaparece por completo (geométricamente, las aristas cortan líneas de campo de forma que se anulan entre sí).

La única FEM que sobrevive es la "FEM de transformación" provocada por la derivada $\frac{dI(t)}{dt}$. En este caso, no hay competencia: como $I(t)$ crece, el flujo total sin dudas aumenta, y la corriente inducida tendrá un único sentido claro para oponerse a ese aumento.


--- 

**5.** La barra metálica AB de largo $L=20~\text{cm}$ y resistencia $R=10~\Omega$ desliza sobre un par de rieles conductores muy largos y de resistencia despreciable y se desplaza con velocidad constante $v=10~\text{m/s}$, con dirección paralela al largo de los rieles. Todo el conjunto se encuentra inmerso en un campo $B_{0}=1~\text{T}$ que apunta hacia adentro de la página, perpendicular al plano de los rieles. Calcular:

- **a)** la fuerza electromotriz inducida, la corriente inducida y el sentido de la misma.
- **b)** el valor de la fuerza necesaria para que la velocidad de la barra se mantenga constante.
- **c)** la potencia disipada por la resistencia y la entregada por el agente externo que hace que se mueva con velocidad constante.
- **d)** ¿Cómo evoluciona la velocidad de la barra en función del tiempo si se suprime la fuerza ejercida por el agente externo?

### Resolución

#### a) FEM, Corriente y Sentido

Tus fórmulas son las correctas. Al ser la velocidad, el campo magnético y la longitud de la barra mutuamente perpendiculares, la integral de la Ley de Faraday se reduce exactamente a tu expresión.

**1. Fuerza electromotriz inducida:**

$$ \mathcal{E} = v B L = (10\text{ m/s}) (1\text{ T}) (0.2\text{ m}) = 2\text{ V} $$

**2. Corriente inducida:**

Aplicando la Ley de Ohm para el circuito completo:

$$ I = \frac{\mathcal{E}}{R} = \frac{2\text{ V}}{10\ \Omega} = 0.2\text{ A} $$

**3. Sentido de la corriente:**

Asumiendo que la barra se mueve hacia la derecha, el área del circuito rectangular aumenta, incrementando el flujo magnético hacia adentro de la página. Por la **Ley de Lenz**, el circuito inducirá una corriente que genere un campo magnético propio hacia _afuera_ de la página para oponerse a este cambio. Por la regla de la mano derecha, la corriente debe circular en **sentido antihorario**.

_(Alternativamente: usando la Fuerza de Lorentz $\vec{F} = q\vec{v} \times \vec{B}$ sobre las cargas positivas de la barra, $\hat{i} \times (-\hat{k}) = +\hat{j}$, por lo que la corriente fluye hacia arriba por la barra)._

### b) Fuerza del agente externo

Como indicaste, para que la velocidad sea constante, la aceleración debe ser cero. Esto implica que la fuerza externa aplicada debe contrarrestar exactamente a la fuerza magnética de frenado sobre la barra.

$$ \vec{F}_{mag} = I \vec{L} \times \vec{B} $$ Como la barra es perpendicular al campo: $$ F_{mag} = I L B = (0.2\text{ A}) (0.2\text{ m}) (1\text{ T}) = 0.04\text{ N} $$

Por lo tanto, la fuerza del agente externo debe ser de **$0.04\text{ N}$** en la misma dirección que la velocidad.

### c) Potencias

Tu argumento sobre la conservación de la energía es el núcleo de este inciso. La potencia inyectada al sistema como trabajo mecánico debe igualar exactamente a la potencia extraída del sistema como calor en la resistencia.

**1. Potencia disipada (efecto Joule):**

$$ P_{disipada} = I^2 R = (0.2\text{ A})^2 (10\ \Omega) = 0.04 \times 10 = 0.4\text{ W} $$

**2. Potencia mecánica entregada:**

$$ P_{externa} = F_{ext} v = (0.04\text{ N}) (10\text{ m/s}) = 0.4\text{ W} $$

Ambos valores coinciden a la perfección.

### d) Evolución de la velocidad

Tu razonamiento es cualitativamente correcto: la barra desacelera debido a la fuerza magnética opuesta. Para que la respuesta sea rigurosa a nivel universitario, se puede demostrar cómo es esa desaceleración planteando la Segunda Ley de Newton.

Al suprimir la fuerza externa, la única fuerza en el eje de movimiento es la fuerza magnética, la cual no es constante, sino que depende de la velocidad instantánea $v$:

$$ F_{neta} = - F_{mag} = - I L B = - \left( \frac{vBL}{R} \right) L B = - \frac{B^2 L^2}{R} v $$

Aplicando $\sum F = m a$:

$$ - \frac{B^2 L^2}{R} v = m \frac{dv}{dt} $$

$$ \frac{dv}{dt} = - \left( \frac{B^2 L^2}{mR} \right) v $$

Esta es una ecuación diferencial ordinaria de primer orden. Su solución indica que la velocidad no decae linealmente, sino de forma **exponencial decreciente**:

$$ v(t) = v_0 e^{-t/\tau} \qquad \text{donde} \qquad \tau = \frac{mR}{B^2 L^2} $$

La velocidad evoluciona decayendo exponencialmente hasta detenerse por completo cuando $t \to \infty$. Toda la energía cinética inicial de la barra ($\frac{1}{2}mv_0^2$) se terminará disipando como calor en la resistencia.


**6.** Un alambre conductor de longitud ajustable rodea el Ecuador de un globo esférico de $10~\text{cm}$ de diámetro formando una espira en el plano $xy$, en una región del espacio donde existe un campo uniforme $\vec{B}=B_{0}\hat{z}$.

- **a)** Si el globo se está inflando en forma esférica junto con la espira de alambre, ¿se induce una corriente? Si su respuesta es afirmativa, justifique qué sentido tiene la corriente inducida. Si su respuesta es negativa, justifique su respuesta.
    
- **b)** Si la magnitud del campo fuera $0.30~\text{T}$ y el diámetro de la espira aumentara de $10~\text{cm}$ a $20~\text{cm}$ en un tiempo de $0.040~\text{s}$, ¿cuál sería valor promedio de la fem inducida en la espira?
    

**7.** Los trazos amarillos de la figura son conductores cuya resistencia por unidad de longitud es $2~\Omega/\text{m}$. El conjunto está inmerso en un campo uniforme $\vec{B}=(-1.5+0.1~\frac{1}{\text{s}}t)\hat{z}~\text{T}$. Si $a=50~\text{cm}$, determinar la corriente inducida en el tramo PQ.

**8.** La figura muestra un toroide de radio interior $a=4~\text{cm}$, exterior $b=5~\text{cm}$ y altura $h=1~\text{cm}$. El núcleo es de un material de permeabilidad $\mu_{r}=1000$. Arrolladas sobre el toroide hay $N_{1}=100$ vueltas de alambre por las que circula corriente, la que determina un campo como marca la flecha azul. El trazo rojo representa $N_{2}=200$ vueltas de alambre superpuestas de resistencia $R=10~\Omega$ bobinadas sobre un cuadrado de lado $L=10~\text{cm}$. Si la corriente que circula por el toroide está dada por $I(t) = 10~\text{A}~e^{-t/\tau}$ ($\tau=0.5~\text{s}$), determinar la corriente inducida en el trazo rojo.

**9.** La circunferencia roja, de radio $R=2~\text{cm}$, es la traza de un solenoide muy largo de 1000 vueltas por metro por el que circula una corriente que crece linealmente con el tiempo a razón de $10~\text{A/s}$ y que determina un campo $\vec{B}$ saliente al plano del papel. Determinar:

- **a)** La corriente inducida en las resistencias.
    
- **b)** La lectura de los voltímetros.
    

**10.** Obtener el valor aproximado de la autoinductancia por unidad de longitud de un solenoide de radio $R=1~\text{cm}$ y largo $L=1~\text{m}$. ¿Qué suposiciones realiza para calcularlo?

**11.**

- **a)** Calcular la inductancia mutua entre un conductor recto de largo $10~\text{m}$ y una bobina rectangular, de $10~\text{cm}$ por $15~\text{cm}$, como la indicada en la figura.
    
- **b)** Si la resistencia de la bobina es $R=10~\Omega$ y por el conductor recto circula una corriente $i=5\cos(9t)$ (donde $i$ está en Ampere y $t$ en segundos) calcular la fem y corriente inducida en la bobina. Discutir el signo de las mismas y su dependencia con el sentido de la corriente en el conductor recto.
    
- **c)** ¿Cómo se modifican los valores obtenidos en b) si la bobina rectangular tiene $N_{1}$ espiras estrechamente arrolladas?
    

**12.**

- **a)** Calcular la autoinductancia de un toroide de sección cuadrada ($R_{1}=2~\text{cm}$ y $R_{2}=3~\text{cm}$ y $h=1~\text{cm}$).
    
- **b)** Repita el cálculo si $R_{1}=2.9~\text{cm}$ y $R_{2}=3~\text{cm}$ y $h=10~\text{cm}$.
    
- **c)** Compare los resultados y discuta la diferencia que se obtendría al considerar que el campo es uniforme en el toroide.
    

**13.** Sobre el toroide delgado ($\mu_{r}=1200$) se han bobinado dos arrollamientos: uno con $N_{1}=500$ espiras, por el que circula una corriente $I_{1}=(20+0.2~t)~\text{A}$, con $t$ en segundos, y otro con $N_{2}=200$ espiras, cuyos bornes están desconectados. La sección es $S=1~\text{cm}^{2}$, y los radios interior y exterior de $7~\text{cm}$ y $8~\text{cm}$, respectivamente. Calcular $L_{1}$, $L_{2}$, $M$ y el valor de la f.e.m. inducida en la bobina 2 y su polaridad, indicando bornes homólogos.

**14.** Para el mismo núcleo del Problema 13, calcular la energía almacenada cuando las corrientes son $I_{1}=20~\text{A}$ y $I_{2}=2~\text{A}$. Considere las distintas posibilidades de bornes homólogos.

**15.** Un aparato de resonancia magnética para realizar imágenes del cuerpo humano es, en esencia, un solenoide. Suponga un equipo de $1~\text{m}$ de diámetro y $2~\text{m}$ de longitud, con un devanado de 10000 vueltas por metro. En su interior el campo magnético es de $1.5~\text{T}$. Calcule:

- **a)** La autoinductancia del solenoide.
    
- **b)** La intensidad de corriente eléctrica necesaria para obtener el campo magnético de $1.5~\text{T}$.
    
- **c)** La energía magnética almacenada en la bobina.
    
- **d)** Si la resistencia por unidad de longitud del hilo que forma la bobina es de $0.1~\Omega~\text{m}^{-1}$, calcule la potencia que se disipa en forma de calor.
    

**16.** Dos solenoides $N_{1}$ y $N_{2}$ se hallan enfrentados como muestra la figura. Si $L_{1}=1~\text{H}$; $L_{2}=5~\text{H}$; $M=1.5~\text{H}$ y por $N_{1}$ circula la corriente $I_{1}=(2+0.5~t)~\text{A}$, y $N_{2}$ está abierto, calcular las expresiones de la f.e.m. inducida sobre $N_{2}$ y la energía almacenada.

**17.** Por dos solenoides con $L_{1}=2~\text{H}$, $L_{2}=5~\text{H}$, $M=2.2~\text{H}$ (como los del Problema 16) circulan las corrientes $I_{1}=5~\text{A}$, $I_{2}=10~\text{A}$, respectivamente. Determinar:

- **a)** La energía magnética almacenada en el sistema.
    
- **b)** La energía magnética que tendría el sistema si $L_{2}$ se encontrara muy alejado de $L_{1}$.
    
- **c)** El trabajo necesario para traer $L_{2}$ desde el infinito hasta la posición original.
    

**18.** Un núcleo cuadrado de material ferromagnético de $30~\text{cm}$ de lado posee una sección (también cuadrada) de $1~\text{cm}^{2}$. Sobre el núcleo se colocan dos arrollamientos de $N_{1}=100$ y $N_{2}=500$ espiras. Por el primero circula una corriente $I_{1}=I_{0}\exp(-t/\tau)$ siendo $I_{0}=10~\text{A}$ y $\tau=5~\text{s}$, y el segundo está abierto. Suponga que se puede considerar al material con una permeabilidad relativa $\mu_{r}=1000$. Determine en qué sentido circularía la corriente ($I_{2}$) si el segundo arrollamiento estuviera cerrado, sabiendo que P y S son bordes homólogos (¿sentido de P a Q o de Q a P?). Fundamente mediante la Ley de Lenz.