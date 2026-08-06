---
id: 20260626192640
aliases: []
tags:
  - uncataloged
created: 2026-06-26 19:26
status: draft
---
# Corriente Alterna

    

### Problema 1
**1.** Un circuito está formado por una resistencia $R = 400\,\Omega$ y una inductancia $L = 1\text{ Hy}$. El mismo es alimentado por un generador de voltaje $V_g(t) = 311 \cos(2\pi \cdot 50\text{ Hz} \cdot t)\text{ V}$. Determinar, en régimen permanente:

a) la corriente $I(t)$ que circula,
b) la caída de tensión $V_R(t)$ sobre $R$ y $V_L(t)$ sobre $L$,
c) Calcular la potencia instantánea $P(t) = V_g(t)I(t)$

Análisis previo:
- Analiza un resistor y un inductor alimentados por una fuente alterna, solicitando corriente, tensiones y potencia instantánea. Consultar el **Capítulo 31 (Corriente alterna)**, leyendo las Secciones 31.1 (Fasores y corrientes alternas), 31.2 (Resistencia y reactancia) y 31.4 (Potencia en circuitos de corriente alterna).
### Resolución
### Problema 2
**2.** En el circuito anterior se reemplaza la inductancia por un capacitor $C = 10\,\mu\text{F}$. Recalcular las consignas (a), (b) y (c) del problema anterior.

Análisis previo:
- Adapta el circuito anterior reemplazando el inductor por un capacitor. Consultar el **Capítulo 31**, Secciones 31.2 (prestando atención a la reactancia capacitiva y su desfase) y 31.4 (Potencia).
### Resolución
### Problema 3 

**3.** Calcular la impedancia equivalente de los siguientes casos:

Datos: $R_1 = 10\,\Omega$; $R_2 = 50\,\Omega$; $L = 5 \cdot 10^{-4}\text{ Hy}$; $C = 0.1\,\mu\text{F}$; $f = 50\text{ Hz}$.

```
* Circuito Ejercicio 3 - Caso 1 (Izquierda)
R1 1 2 10
L1 2 0 5e-4
R2 2 0 50

* Circuito Ejercicio 3 - Caso 2 (Centro)
R1 1 0 10
R2 1 2 50
C1 2 0 0.1uF

* Circuito Ejercicio 3 - Caso 3 (Derecha)
R1 1 2 R_val
L1 2 0 5e-4
C1 2 0 0.1uF
```

Análisis previo:
- Pide calcular la impedancia compleja equivalente en tres arreglos mixtos (serie y paralelo). Consultar el **Capítulo 31**, Sección 31.3 (El circuito L-R-C en serie). _Nota: Dado que el libro base se centra principalmente en serie, deberás combinar el uso de impedancia compleja ($Z$) de este capítulo con las reglas de mallas y nodos del Capítulo 26 aplicadas algebraicamente a números complejos._
### Resolución
### Problema 4 

**4.** Un circuito RLC serie con $L = 0.5\text{ H}$, $R = 300\,\Omega$ y $C = 10\,\mu\text{F}$ es alimentado por un generador $V_g(t)$. Se mide una corriente $I(t) = 5.2\text{ A} \cos(100\text{ Hz} \cdot t + 60^\circ)$.

a) Encontrar la ecuación diferencial que describe el comportamiento del circuito con los coeficientes numéricos,
b) calcular $V_g(t)$,
c) la potencia instantánea $P(t) = V_g(t)I(t)$,
d) El valor de $C$ que lleve el circuito a resonancia.

Análisis previo:
- Evalúa un circuito RLC serie a partir de la corriente medida, pidiendo la ecuación diferencial, el voltaje de la fuente, potencia y la capacitancia de resonancia. Consultar el **Capítulo 31**, Secciones 31.3 (El circuito L-R-C en serie), 31.4 (Potencia) y 31.5 (Resonancia en circuitos de corriente alterna).
### Resolución
### Problema 5 
**5.** En el circuito de la figura calcular la corriente y la caída sobre la resistencia.

¿Cuál es la potencia activa que entrega la fuente?
```
* Circuito Ejercicio 5
V_source 1 0 AC V0 omega
R1 1 2 R1_val
R2 2 0 R2_val
C1 2 0 C_val
```

Análisis previo:
-  Presenta un circuito mixto R-LC y pide corriente, tensiones y la potencia activa entregada por la fuente. Consultar el **Capítulo 31**, Secciones 31.3 (Impedancia) y 31.4 (Potencia activa y factor de potencia).
### Resolución
### Problema 6 
**6.** El circuito de la figura está alimentado por la red domiciliaria de nuestro país. Considerando régimen alterno permanente, se pide:

a) Calcular la reactancia y la impedancia compleja de cada elemento y del circuito serie total, expresándolas en sus formas binómica y exponencial. Indicar si el circuito tiene comportamiento inductivo, capacitivo o resistivo.
b) Indicar en forma exponencial los valores complejos asociados a la corriente y los voltajes sobre cada elemento y su relación con las respectivas impedancias complejas.
c) Calcular los valores de potencia activa y potencia reactiva.
d) Calcular potencia aparente y factor de potencia.
e) Dibujar el diagrama fasorial de corriente y voltajes.
f) Calcular la frecuencia de resonancia. Describir el comportamiento del circuito en la condición de resonancia.

```
* Circuito Ejercicio 6
V_red 1 0 AC 220 50Hz ; Asumiendo red de Argentina
L_1 1 2 60mH
R_1 2 3 10
C_1 3 0 300uF
```

Análisis previo:
- Es un ejercicio integrador para un circuito RLC serie que exige notación fasorial (binómica/exponencial), cálculo de potencias (activa, reactiva, aparente), factor de potencia y resonancia. Consultar íntegramente el **Capítulo 31** de principio a fin, prestando especial atención a la diagramación fasorial en la Sección 31.2 y el triángulo de potencias derivado de la Sección 31.4.
### Resolución
### Problema 7 

**7.** El circuito de la figura ($R_1 = 5\,\Omega$, $R_2 = 500\,\Omega$) está alimentado por la red domiciliaria de nuestro país. Un voltímetro conectado sobre el capacitor mide $V_C = 120\text{ V}$.

Calcular:

a) la corriente que circula por la fuente.
b) la capacidad $C$.
c) la potencia activa $P$.
d) la potencia reactiva $Q$.
e) la potencia aparente $S$.

```
* Circuito Ejercicio 7
V_source 1 0 AC 220 50Hz
R1 1 2 5
R2 2 0 500
C1 2 0 C_unknown
```
Análisis previo:
- Analiza un circuito mixto donde se brinda la medición de un voltímetro sobre un capacitor para escalar el circuito, solicitando corriente, capacidad y todas las potencias (P, Q, S). Consultar el **Capítulo 31**, Secciones 31.2 (Relaciones eficaces rms), 31.3 y 31.4 (Potencia).
### Resolución
### Problema 8 

**8.** En el circuito de la figura (para la fuente: $V_{\text{eficaz}} = 200\text{ V}$, $f = 50\text{ Hz}$) dos voltímetros ideales miden las caídas de voltaje $V_R$ y $V_C$ sobre $R$ y $C$ respectivamente.

a) ¿Cuál es la lectura del voltímetro $V_C$ si $V_R = 150\text{ V}$?
b) ¿Qué relación hay entre $R$ y $X_C$?
c) Si la corriente eficaz es $I = 1\text{ A}$ calcular $R$ y $C$.
d) ¿Qué ocurre con $\cos(\phi)$ si se duplica $R$?

```
* Circuito Ejercicio 8
V1 1 0 AC 200 50Hz
R1 1 2 R_unknown
C1 2 0 C_unknown
```
Análisis previo:
- Estudia un circuito RC serie mediante mediciones de voltímetros ideales, relación de impedancias y factor de potencia. Consultar el **Capítulo 31**, Secciones 31.2 (Valores eficaces en mediciones), 31.3 (Diagramas fasoriales de tensión) y 31.4 (Relación entre $R$, impedancia y $\cos(\phi)$).
### Resolución
### Problema 9 

**9.** En un circuito RLC serie ($L = 50\text{ mH}$) se aplica una tensión eficaz de $100\text{ V}$ y frecuencia $50\text{ Hz}$, y circula una corriente de $25\text{ A}$ atrasada $45^\circ$ respecto de la tensión. Calcular:

a) los valores de $R$ y de $C$.
b) la tensión sobre cada elemento.
c) verificar la segunda ley de Kirchoff con un diagrama fasorial.
d) evaluar el triángulo de potencias.

Análisis previo:
- Pide hallar los valores de los componentes de un RLC serie partiendo de su desfase angular de 45 grados y verificar la segunda ley de Kirchhoff con un diagrama. Consultar el **Capítulo 31**, Sección 31.3 (Ángulo de fase en diagramas fasoriales) y 31.4 (Triángulo de potencias).
### Resolución
### Problema 10 

**10.** El circuito de la figura es alimentado por un generador de tensión eficaz $120\text{ V}$ y frecuencia $60\text{ Hz}$. Dentro de la caja punteada hay componentes ($R$ y/o $L$ y/o $C$) conectados en serie. La potencia aparente medida es $S = 50.9\text{ VA}$ y la reactiva $|Q| = 36\text{ VAR}$ (inductiva) ¿Qué hay dentro de la caja?

```
* Circuito Ejercicio 10
V1 1 0 AC 120 60Hz
R1 1 2 100
X_caja_punteada 2 0  ; Subcircuito desconocido
```

Análisis previo:
- Consiste en una "caja negra" donde, dados los valores de potencia aparente y reactiva, se debe deducir qué elementos están en serie en su interior. Consultar el **Capítulo 31**, Sección 31.4 (Potencia en circuitos de CA, enfocándose en cómo el signo de la potencia reactiva y el factor de potencia definen la naturaleza inductiva o capacitiva del circuito).
### Resolución