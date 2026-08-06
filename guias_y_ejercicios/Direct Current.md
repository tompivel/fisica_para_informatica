---
id: 20260604105041
aliases: []
tags:
  - uncataloged
created: 2026-06-04 10:50
status: draft
---
# Guía 3: Circuitos con Capacitores y con Corrientes Estacionarias - Corriente continua

### Ejercicio 1

Un alambre de cobre de 2 mm de radio y 1 m de largo se estira hasta cuadruplicar su longitud. Deduzca la expresión de la resistencia de un alambre recto. Suponiendo constante la resistividad del material, calcule la resistencia antes y después del estiramiento. Buscar en Internet las propiedades relevantes del cobre.

### Resolucion
$$
\begin{align}
\rho =  & \frac{E}{J} \implies \vec{E}  = \rho \vec{J} \\
I  & = JA \\
V  & = EL  \\
\frac{V}{L}  & = \frac{\rho I}{A} \implies V  = L  \frac{\rho I}{A} \\
R  & = L \frac{\rho}{A}
\end{align}
$$
La resistividad del cobre es $\rho = 1.72 \times 10^{-8}$. El area cross sectional $A$ es $\pi (0.002m)^2$. Por tanto, antes del estiramiento, la resistencia es:
$$
\begin{align}
R_1  &  = 1 \text{ m} \times \frac{1.72 \times 10^{-8} \ \Omega\text{m}}{\pi \times (0.002 \text{ m})^2} \approx 1.369 \times 10^{-3} \ \Omega \text{ (o } 1.37 \text{ m}\Omega \text{)}
\end{align}
$$
Estirar un conductor implica que su volumen se conserva, por tanto:

$$
\begin{align} 
\text{Volumen}  & = L_{1} A_{1} = L_{2} A_{2} \\
A_{2}  & = \frac{A_{1}L_{1}}{4L_{1}} = \frac{A_{1}}{4} = \frac{{ \pi (0.002m)^2}}{4} \\
R_2  & = \rho \frac{L_2}{A_2} = \rho \frac{4 L_1}{\frac{A_1}{4}} = 16 \left( \rho \frac{L_1}{A_1} \right) = 16 R_1 \\
R_2 & = 16 \times R_1 \approx 16 \times 1.369 \times 10^{-3} \ \Omega \approx 21.9 \times 10^{-3} \ \Omega \text{ (o } 21.9 \text{ m}\Omega \text{)}
\end{align}
$$
### Ejercicio 2

Dos conductores cilíndricos están conectados como muestra la figura. El azul tiene diámetro $d_1 = 1$ mm, largo $L_1 = 100$ cm y conductividad $\sigma_1 = 2 \times 10^{-8} \Omega^{-1} \text{m}^{-1}$. El rojo tiene diámetro $d_2 = 2$ mm, largo $L_2 = 200$ cm y conductividad $\sigma_2 = 1 \times 10^{-8} \Omega^{-1} \text{m}^{-1}$. La corriente circula en la dirección del eje de los cilindros y el voltaje entre los extremos del conductor azul es $V_1 = 0.1$ V. Calcular el voltaje $V_2$ entre los extremos del conductor rojo.
![Pasted image 20260604122931](../assets/Pasted%20image%2020260604122931.png)
**Descripción de la topología (Geometría 3D):**

- Dos cilindros sólidos coaxiales conectados en serie.
- **Cilindro 1 (Azul):** Situado a la izquierda, tiene el diámetro menor ($d_1$).
- **Cilindro 2 (Rojo):** Situado a la derecha, acoplado directamente a la cara plana derecha del cilindro azul, tiene el diámetro mayor ($d_2$).
    

### Resolucion
La corriente $I$ es la misma en ambos conductores dado que están conectados en serie.
$$
 \begin{align}
 \rho_{1}  & = \frac{1}{\sigma_{1}} = \frac{1 }{2 \times 10^{-8}} \Omega m \\
  \rho_{2}  & = \frac{1}{\sigma_{2}} = \frac{1 }{1 \times 10^{-8}} \Omega m
 \end{align}
$$
$$
\begin{align}
V_{1}   & = L_{1}  \frac{\rho_{1} I}{A_{1}} \\
I  & =  \frac{V_{1}A_{1}}{L_{1}\rho_{1}} \\
V_{2}   & = L_{2}  \frac{\rho_{2} I}{A_{2}} =   L_{2}\frac{\rho_{2} ( \frac{V_{1}A_{1}}{L_{1}\rho_{1}})}{A_{2}} \\
\end{align}
$$
O, simplificando los cáculos:
$$I = \frac{V_1}{R_1} = \frac{V_2}{R_2} \implies V_2 = V_1 \frac{R_2}{R_1}$$
Calculando las resistencias de cada tramo por separado usando la fórmula $R = \rho \frac{L}{A} = \frac{1}{\sigma} \frac{L}{\pi (d/2)^2}$:

**Resistencia del cilindro 1 (Azul):**

$$R_1 = \frac{1}{2 \times 10^{-8}} \times \frac{1}{\pi \times (0.5 \times 10^{-3})^2} = \frac{10^8}{2} \times \frac{1}{\pi \times 0.25 \times 10^{-6}} = \frac{2 \times 10^{14}}{\pi} \ \Omega$$

**Resistencia del cilindro 2 (Rojo):**

$$R_2 = \frac{1}{1 \times 10^{-8}} \times \frac{2}{\pi \times (1 \times 10^{-3})^2} = 10^8 \times \frac{2}{\pi \times 10^{-6}} = \frac{2 \times 10^{14}}{\pi} \ \Omega$$
Dado que $R_1 = R_2$, la relación de los voltajes resulta en:

$$V_2 = 0.1 \text{ V} \times \frac{R_2}{R_1} = 0.1 \text{ V} \times 1$$
### Ejercicio 3

Los bloques conductores de la figura tienen dimensiones $a = 10$ mm, $b = 20$ mm, $c = 30$ mm, $h = 50$ mm. El bloque azul tiene conductividad $\sigma_1 = 2 \times 10^{-8} \Omega^{-1} \text{m}^{-1}$ y el rojo $\sigma_2 = 1 \times 10^{-8} \Omega^{-1} \text{m}^{-1}$. Toda la base del conjunto se encuentra a un potencial $V_1 = 10$ V y la tapa superior a $V_2 = 20$ V. Calcular la corriente que circula por todo el conjunto.

**Descripción de la topología (Geometría 3D):**

- Dos bloques rectangulares paralelos unidos físicamente por una de sus caras laterales.
- **Bloque 1 (Azul):** Lado izquierdo. Dimensiones en la base: ancho $a$ y profundidad $c$.
- **Bloque 2 (Rojo):** Lado derecho. Dimensiones en la base: ancho $b$ y profundidad $c$.
- Ambos bloques comparten la misma altura $h$.
### Resolucion
Dado que "toda la base del conjunto" se encuentra a $V_1 =$ 10 V y "la tapa superior" a $V_2 =$ 20 V, la diferencia de potencial se aplica a lo largo del eje vertical (la altura $h$). El flujo de corriente va desde la superficie de mayor potencial (20 V) hacia la de menor potencial (10 V). Esto significa que la corriente viaja perpendicular a las tapas, de arriba hacia abajo.

La corriente que circula por un bloque no necesariamente es la misma que circula por el otro. Por tanto, analizamos la corriente por cada bloque. Para el bloque azul, tenemos:
$$
\begin{align}
I_{\text{azul}}  & =  \frac{VA_{1}}{L\rho_{1}} = \frac{{10V \times 0.01m \times 0.03m}}{0.05m \times  \frac{1}{2 \times 10^{-8} \Omega\text{m}}} \\
I_{\text{rojo}}  & =  \frac{VA_{2}}{L\rho_{2}} = \frac{{10V \times 0.02m \times 0.03m}}{0.05m \times  \frac{1}{1 \times 10^{-8} \Omega\text{m}}} \\
\end{align}
$$
Por tanto, $I_{\text{total}} = I_{\text{azul}} + I_{\text{rojo}}$. 
$$I_{\text{total}} = 1.2 \times 10^{-9}\text{ A} + 1.2 \times 10^{-9}\text{ A} = 2.4 \times 10^{-9}\text{ A}$$

### Ejercicio 4

Determinar la resistencia equivalente de los circuitos de la figura:
![Pasted image 20260605105411](../assets/Pasted%20image%2020260605105411.png)
#### Circuito 1 (Izquierda)

#### Definición de Nodos

- **Nodo A:** Terminal de entrada A.
- **Nodo B:** Terminal de salida B (tomado como nodo de referencia/tierra para la parte inferior izquierda).
- **Nodo 1:** Unión entre la resistencia de $5\ \Omega$, la de $10\ \Omega$ y la de $8\ \Omega$ superior.
- **Nodo 2:** Esquina superior derecha, unión entre la resistencia de $8\ \Omega$ superior y la de $8\ \Omega$ vertical derecha.
- **Nodo 3:** Esquina inferior derecha, unión entre la resistencia de $8\ \Omega$ vertical derecha y la de $12\ \Omega$ inferior.
#### Netlist (Formato SPICE / Tabla)

| **Componente** | **Nodo (+)** | **Nodo (-)** | **Valor (Ω)** | **Descripción**                                          |
| -------------- | ------------ | ------------ | ------------- | -------------------------------------------------------- |
| **R_A_1**      | A            | 1            | 5             | Resistencia de entrada desde la terminal A               |
| **R_1_B**      | 1            | B            | 10            | Resistencia en la rama vertical central                  |
| **R_1_2**      | 1            | 2            | 8             | Resistencia superior de la malla derecha                 |
| **R_2_3**      | 2            | 3            | 8             | Resistencia vertical derecha de la malla derecha         |
| **R_3_B**      | 3            | B            | 12            | Resistencia inferior de la malla derecha que regresa a B |

#### Circuito 2 (Derecha)

#### Definición de Nodos

- **Nodo A:** Terminal de entrada A.
- **Nodo B:** Terminal de salida B.
- **Nodo 1:** Punto de división después de la primera resistencia, conecta la de $10\ \Omega$ de la entrada, la de $20\ \Omega$ superior y la de $12\ \Omega$ inferior.
- **Nodo 2:** Nodo centralizado por el cortocircuito vertical; une el final de la resistencia de $20\ \Omega$, el inicio de la de $50\ \Omega$ y el inicio de la de $10\ \Omega$ central.
- **Nodo 3:** Punto de encuentro antes de la salida; conecta el final de la de $50\ \Omega$, el final de la de $10\ \Omega$ central, el final de la de $12\ \Omega$ inferior y el inicio de la de $20\ \Omega$ final.
#### Netlist (Formato SPICE / Tabla)

| **Componente**   | **Nodo (+)** | **Nodo (-)** | **Valor (Ω)** | **Descripción**                                        |
| ---------------- | ------------ | ------------ | ------------- | ------------------------------------------------------ |
| **R_in**         | A            | 1            | 10            | Resistencia inicial conectada a la terminal A          |
| **R_top_izq**    | 1            | 2            | 20            | Resistencia superior de la primera sección en paralelo |
| **R_inf**        | 1            | 3            | 12            | Resistencia que va por toda la rama inferior           |
| **R_centro_sup** | 2            | 3            | 50            | Resistencia superior del par en paralelo interno       |
| **R_centro_inf** | 2            | 3            | 10            | Resistencia inferior del par en paralelo interno       |
| **R_out**        | 3            | B            | 20            | Resistencia final conectada a la terminal B            |

### Resolucion
#### Circuito 1
Para el circuito 1 (el de la izquierda), empezamos reduciendo partes del circuito: $R_{12}, R_{23}$  y $R_{3B}$están en serie, entonces: $R_{\text{eq1}}=2\times{8} + 12=28 \Omega$. 
Luego, tenemos que $R_{eq_{1}}$ está en paralelo con $R_{1B}$, asi que reducimos: 
$$R_{eq2} = \frac{28 \times 10}{28 + 10} = \frac{280}{38} \approx 7.37$$
Por último, tenemos en serie $R_{eq_{2}}$ con $R_{A_{1}}$. Por tanto:
$$R_{eq} = 7.37 + 5 = 12.37$$
#### Circuito 2
$R_{\text{centro inf}}$ está en paralelo con $R_{\text{centro sup}}$, reducimos:
$$R_{\text{eq1}} = \frac{50 \times 10}{50 + 10} = \frac{500}{60} = \frac{25}{3} \approx 8.33 \ \Omega$$
Luego, $R_{eq_{1}}$ está en serie con $R_{\text{top izq}}$, reducimos con suma:
$$R_{\text{eq2}} = \frac{25}{3} + 20 = \frac{85}{3} \approx 28.33 \ \Omega$$
Luego, $R_{eq_{2}}$ esta en paralelo con $R_{inf}$, reducimos:
$$R_{\text{eq3}} = \frac{\frac{85}{3} \times 12}{\frac{85}{3} + 12} = \frac{340}{\frac{121}{3}} = \frac{1020}{121} \approx 8.43 \ \Omega$$
Finalmente, $R_{eq_{3}}$ se encuentra en serie con $R_{in}$ y $R_{out}$, reducimos:
$$R_{\text{eq}} = \frac{1020}{121} + 10 + 20 = 30 + 8.43 = 38.43 \ \Omega$$

### Ejercicio 5
Hallar las corrientes en todas las ramas del circuito de la figura.
![Pasted image 20260605112701](../assets/Pasted%20image%2020260605112701.png)
#### Definición de Nodos

- **Nodo 0 (Tierra):** Conecta el polo negativo de la fuente de 10V y el extremo izquierdo de la resistencia inferior de $10\ \Omega$.
- **Nodo 1:** Conecta el polo positivo de la fuente de 10V y el extremo izquierdo de la resistencia de $5\ \Omega$.
- **Nodo 2:** Nodo extendido en la parte inferior derecha. Une el extremo derecho de la resistencia inferior de $10\ \Omega$, la base de la resistencia vertical de $20\ \Omega$, la base de la resistencia diagonal de $10\ \Omega$ y la base de la resistencia derecha de $20\ \Omega$.
- **Nodo 3:** Punto de unión central superior. Une el extremo derecho de la resistencia de $5\ \Omega$, la parte superior de la de $20\ \Omega$ vertical, la parte superior de la de $10\ \Omega$ diagonal y el extremo izquierdo de la de $10\ \Omega$ superior derecha.
- **Nodo 4:** Esquina superior derecha. Une el extremo derecho de la resistencia superior de $10\ \Omega$ con la parte superior de la resistencia derecha de $20\ \Omega$.

#### Netlist (Formato SPICE / Tabla)

| **Componente**    | **Nodo (+)** | **Nodo (-)** | **Valor**   | **Descripción**                           |
| ----------------- | ------------ | ------------ | ----------- | ----------------------------------------- |
| **V1**            | 1            | 0            | 10 V        | Fuente de voltaje principal               |
| **R_top_izq**     | 1            | 3            | 5 $\Omega$  | Resistencia en la rama superior izquierda |
| **R_inf_izq**     | 0            | 2            | 10 $\Omega$ | Resistencia en la rama inferior izquierda |
| **R_centro_vert** | 3            | 2            | 20 $\Omega$ | Resistencia vertical central              |
| **R_diagonal**    | 3            | 2            | 10 $\Omega$ | Resistencia cruzada en diagonal           |
| **R_top_der**     | 3            | 4            | 10 $\Omega$ | Resistencia horizontal superior derecha   |
| **R_der_vert**    | 4            | 2            | 20 $\Omega$ | Resistencia vertical del extremo derecho  |

### Resolucion
Calcularemos la resistencia equivalente total, aplicando la Ley de Ohm para encontrar la corriente principal, y luego ir "desarmando" la topología hacia atrás utilizando la Ley de Ohm en cada nodo para hallar las corrientes de cada rama individual.
#### Primer paso: Reducción
Empezamos reduciendo $R_{\text{top der}}$ y $R_{\text{der ver}}$, las cuales se encuentran en serie:
$$
R_{eq_{1}} = 10 \Omega + 20 \Omega = 30 \Omega
$$
Luego, reducimos $R_{eq_{1}}, R_{\text{diagonal}}$ y $R_{\text{centro vert}}$, las cuales se encuentran en paralelo:
$$
R_{eq_{2}} = \frac{1}{\frac{1}{R_{eq_{1}}} + \frac{1}{R_{\text{diagonal}}} + \frac{1}{R_{\text{centro vert}}}}
$$
$$R_{eq_{2}} = \frac{1}{\frac{1}{30} + \frac{1}{10} + \frac{1}{20}} = \frac{1}{\frac{2 + 6 + 3}{60}} = \frac{1}{\frac{11}{60}} = \frac{60}{11}\ \Omega \approx 5.45\ \Omega$$
Finalmente, tenemos que $R_{\text{top izq}}, R_{\text{inf izq}}$ y $R_{eq_{2}}$ se encuentran en serie, las reducimos:
$$
R_{eq} = 5 \Omega + R_{eq_{2}} + 10 \Omega
$$
$$R_{eq} = 5\ \Omega + \frac{60}{11}\ \Omega + 10\ \Omega = \frac{225}{11}\ \Omega \approx 20.45\ \Omega$$
Por tanto:
$$
I = \frac{V}{R} 
$$
$$I_{\text{total}} = \frac{10\text{V}}{\frac{225}{11}\ \Omega} = \frac{110}{225}\text{A} = \frac{22}{45}\text{A} \approx 0.489\text{A}$$
#### 2do Paso: Desarmando
La corriente total se la misma para el circuito en serie  $R_{\text{top izq}}, R_{\text{inf izq}}$ y $R_{eq_{2}}$.  Esto hace sentido, la corriente que sale desde la pila es la misma que termina regresando, la carga total se conserva.
$$I_{\text{top izq}} = I_{\text{inf izq}} = \frac{22}{45}\text{A}$$
Sin embargo, el potencial se distribuye de forma distinta:
$$
\begin{align}
V_{\text{total}}  & =  V_{\text{top izq}} + V_{\text{eq2}} + V_{\text{inf izq}} \\ \\
V_{\text{eq2}}  & = V_{total} - V_{\text{top izq}} - V_{\text{inf izq}}  \\
 & = 10V - I_{\text{total}}\times 15 \Omega
\end{align}
$$
Podemos calcular $V_{eq_{2}}$ directamente:
$$V_{eq_{2}} = I_{\text{total}} \times R_{eq_{2}} = \left(\frac{22}{45}\text{A}\right) \times \left(\frac{60}{11}\ \Omega\right) = \frac{1320}{495}\text{V} = \frac{8}{3}\text{V} \approx 2.667\text{V}$$
Entonces tenemos que para $R_{eq_{2}}$, la corriente que circula es $I_{\text{total}}$ y el voltaje es $V_{eq_{2}}$. La corriente se distribuye en los tres ramales paralelos que reduce $R_{eq_{2}}$ : $R_{eq_{1}}, R_{\text{diagonal}}$ y $R_{\text{centro vert}}$, mientras que el diferencial de potencial $V_{eq_{2}}$ se mantiene. Por tanto:
$$
\begin{align}
I_{\text{total}}  & = I_{eq_{1}} + I_{\text{diagonal}} + I_{\text{centro vert}} \\
 & = \frac{V_{eq_{2}}}{R_{eq_{1}}} + \frac{V_{eq_{2}}}{R_{\text{diagonal}}} + \frac{V_{eq_{2}}}{R_\text{centro vert}}
\end{align}
$$
Con esta tensión, se calcula la corriente por cada una de las tres ramas del paralelo utilizando la Ley de Ohm ($I = \frac{V}{R}$):
**1. Rama central vertical:**

$$I_{\text{centro vert}} = \frac{V_{eq_{2}}}{R_{\text{centro vert}}} = \frac{\frac{8}{3}\text{V}}{20\ \Omega} = \frac{8}{60}\text{A} = \frac{2}{15}\text{A} \approx 0.133\text{A}$$
**2. Rama diagonal:**

$$I_{\text{diagonal}} = \frac{V_{eq_{2}}}{R_{\text{diagonal}}} = \frac{\frac{8}{3}\text{V}}{10\ \Omega} = \frac{8}{30}\text{A} = \frac{4}{15}\text{A} \approx 0.267\text{A}$$
Finalmente, la corriente que circula por las resistencias en serie $R_{\text{top der}}, R_{\text{der ver}}$ es la misma que $I_{eq_{1}}$.
$$I_{\text{top der}} = I_{\text{der vert}} = \frac{V_{eq_{2}}}{R_{eq_{1}}} = \frac{\frac{8}{3}\text{V}}{30\ \Omega} = \frac{8}{90}\text{A} = \frac{4}{45}\text{A} \approx 0.089\text{A}$$
### Ejercicio 6

Para el siguiente circuito, calcular: 
![Pasted image 20260605121330](../assets/Pasted%20image%2020260605121330.png)
#### Definición de Nodos

- **Nodo 0:** Rama vertical del extremo derecho. Conecta los terminales derechos de la resistencia superior (6 Ω), la central (3 Ω) y la inferior (6 Ω). Se toma como nodo de referencia (Tierra).
- **Nodo 1:** Rama vertical del extremo izquierdo. Conecta el polo positivo de la fuente de 12V, el terminal izquierdo del interruptor L y el terminal izquierdo de la resistencia inferior (6 Ω).
- **Nodo 2:** Conexión en la rama superior entre el polo negativo de la fuente de 12V y el terminal izquierdo de la resistencia superior (6 Ω).
- **Nodo 3:** Nodo interno de la rama central. Conecta el terminal derecho del interruptor L con el terminal izquierdo de la resistencia de 3 Ω.
    

#### Netlist (Formato SPICE / Tabla)

| **Componente** | **Nodo A** | **Nodo B** | **Valor** | **Descripción**                                        |
| -------------- | ---------- | ---------- | --------- | ------------------------------------------------------ |
| **V1**         | 1          | 2          | 12 V      | Fuente de voltaje (Polo positivo en el Nodo 1)         |
| **R_sup**      | 2          | 0          | 6 Ω       | Resistencia de la rama superior                        |
| **SW_L**       | 1          | 3          | -         | Interruptor de control L                               |
| **R_cent**     | 3          | 0          | 3 Ω       | Resistencia de la rama central (activa si SW_L cierra) |
| **R_inf**      | 1          | 0          | 6 Ω       | Resistencia de la rama inferior                        |

- a. La potencia entregada por la batería (de resistencia interna despreciable) con la llave L abierta.
- b. La caída de tensión sobre la resistencia de 3 $\Omega$ y la potencia disipada en la misma. 
- c. La potencia entregada por la batería con L cerrada.
- d. El consumo en kWh luego de dos días de funcionamiento con L abierta y con L cerrada.

### Resolucion
#### a)
Las resistencias de $6 \Omega$ se encuentran en serie (cuando la llave L se mantiene abierta), entonces la resistencia equivalente del circuito resulta: $R_{eq} = 12 \Omega$ y dado que el voltaje entregado por la batería son $12V$, calculamos:
$$
\begin{align}
P & = \frac{V^2}{R} = 12W
\end{align}
$$
#### b)
Dada que la resistencia del aire se puede asumir como infinita, siguiendo la ley de ohm ($V = IR$), nos damos cuenta que la caída de potencial en esta resistencia es nula mientras la llave esté abierta. Lo mismo sucede con la potencia disipada, dado que no fluye corriente y ni existe caída de potencial sobre la resistencia ($P = V \times I$).
#### c)
Cuando L se cierra, buscamos la nueva resistencia equivalente:
- $6 \Omega$ y $3 \Omega$ en paralelo: $R_{eq_{1}} = \frac{{6\Omega \times 3 \Omega}}{9 \Omega} = 2 \Omega$
- $R_{eq_{1}}$ y  $6 \Omega$ en serie: $R_{eq} = R_{eq_{1}} + 6 \Omega = 2\Omega$. 
La potencia nueva entregada es:
$$
P = \frac{{12V}^2}{2 \Omega}= 18 W
$$
#### d)
 2 días de funcionamiento equivalen:
 $$
 \begin{align}
 2 \text{dias} \times \frac{24 \text{horas}}{1 \text{dia}} = 48 \text{horas}
 \end{align}
 $$
Multiplicamos ambas expresiones encontradas de potencia por la duración encontrada:
$$P_{L_{\text{abierta}}} (\text{en kW}) = \frac{12\text{ W}}{1000} = 0.012\text{ kW}$$

$$Consumo_{L_{\text{abierta}}} = 0.012\text{ kW} \times 48\text{ h} = 0.576\text{ kWh}$$

$$P_{L_{\text{cerrada}}} (\text{en kW}) = \frac{18\text{ W}}{1000} = 0.018\text{ kW}$$

$$Consumo_{L_{\text{cerrada}}} = 0.018\text{ kW} \times 48\text{ h} = 0.864\text{ kWh}$$
### Ejercicio 7

Para el circuito de la figura, calcular las diferencias de potencial de los puntos A, B y C respecto a la referencia tierra cuando la llave L está abierta y cuando L está cerrada. Todas las resistencias son de 10 $\Omega$ y las baterías de 10 V.

![Pasted image 20260605224418](../assets/Pasted%20image%2020260605224418.png)
#### Definición de Nodos

- **Nodo 0 (Tierra):** Línea vertical central (marcada con el símbolo de tierra). Conecta el extremo derecho del resistor de la rama A, el extremo derecho del resistor de la rama B, el extremo derecho del resistor de la rama C, el extremo izquierdo del resistor superior derecho y el retorno inferior del interruptor L.
- **Nodo 1:** Línea vertical izquierda que une los puntos A, B y C en un único potencial. Conecta el extremo izquierdo del resistor de la rama A, el polo positivo de la batería de la rama B y el polo positivo de la batería de la rama C.
- **Nodo 2:** Nodo interno de la rama central (B), ubicado entre el polo negativo de su batería y el resistor de esa misma rama.
- **Nodo 3:** Nodo interno de la rama inferior (C), ubicado entre el polo negativo de su batería y el resistor de esa misma rama.
- **Nodo 4:** Nodo de la rama superior derecha, ubicado entre el resistor superior derecho y el polo positivo de la batería de esa rama.
- **Nodo 5:** Nodo interno de la rama derecha, ubicado entre el polo negativo de la batería derecha y el terminal superior del interruptor L.
#### Netlist (Formato SPICE / Tabla)

| **Componente** | **Nodo (+)** | **Nodo (-)** | **Valor** | **Descripción**                                     |
| -------------- | ------------ | ------------ | --------- | --------------------------------------------------- |
| **R_A**        | 1            | 0            | -         | Resistor de la rama superior izquierda (Terminal A) |
| **V_B**        | 1            | 2            | -         | Fuente de voltaje de la rama central (B)            |
| **R_B**        | 2            | 0            | -         | Resistor de la rama central (B)                     |
| **V_C**        | 1            | 3            | -         | Fuente de voltaje de la rama inferior (C)           |
| **R_C**        | 3            | 0            | -         | Resistor de la rama inferior (C)                    |
| **R_top_der**  | 0            | 4            | -         | Resistor de la rama superior derecha                |
| **V_der**      | 4            | 5            | -         | Fuente de voltaje de la rama derecha                |
| **SW_L**       | 5            | 0            | -         | Interruptor de control L                            |

### Resolucion
#### Llave abierta
Empezando con la llave L abierta, tenemos a la parte derecha del circuito desconectado, y por ende no afecta a nuestros calculamos. Asumimos tierra con $V=0$. En esta configuracion, aplicamos ley de Kirchhoff al nodo 1:
$$
\begin{align}
I_{A} + I_{B} + I_{C}  & = 0  \tag{1}\\
\end{align}
$$
Ademas, se puede apreciar que el voltaje del nodo 1 es el mismo en los puntos A, B y C dado que comparten el mismo conductor sin intereferencias de resistencias o pilas que generen algún diferencial, de manera que $V_{A} = V_{B}= V_{C} = V_{1}$. Por tanto, podemos calcular las corrientes de cada rama usando la ley de ohm generalizada ([Ley de Ohm Generalizada](../notas/Ley%20de%20Ohm%20Generalizada.md)).
$$
I = \frac{V_{\text{nodo}} - V_{\text{fuente}}}{R} \tag{2}
$$
 Juntamos (1) y (2):
$$
\begin{align}
\frac{V_{1}}{10 \Omega} + \frac{V_{1}-10V}{10 \Omega} + \frac{V_{1} - 10V}{10 \Omega}  & = 0 \\
3V_{1} -20V  & =0 \\
V_{1}  & = \frac{20}{3}V
\end{align}
$$
Dado que el potencial de referencia final que estamos usando ($V_{\text{tierra}} =0$) es nulo, el diferencial de potencial $\Delta V$ en las tres ramas resulta $V_{1}-0 =\frac{20}{3}V$.
#### Llave cerrada 
El diferencial de potencial en las ramas exploradas en el inciso anterior no se ven afectadas dado que el análisis sobre el Nodo 1 es idéntico. Sin embargo, ahora tenemos una nueva rama. Analizando el diferencial de potencial en esta rama, vemos que el punto de referencia es la tierra ($V=0$). Por tanto, la ley de ohm nos indica que:
$$
I_{D} = \frac{V_{fuente}}{R} = \frac{10V}{10 \Omega} = 1A
$$
Por tanto, el diferencial de potencial en esta rama adicional es el que provoca la pila: $10V$.
### Ejercicio 8
La figura representa un trozo de circuito en el que se conocen las corrientes $I_1$ e $I_2$ y la diferencia de potencial entre los puntos B y C ($I_1 = 4$ A; $I_2 = 2$ A; $V_B - V_C = 12$ V). Sabiendo que $R = 10\ \Omega$ determinar: 

- a) El sentido y valor de la corriente en la resistencia $R_y$.
- b) Los valores de $R_x$ y $R_y$.
- c) La diferencia de potencial $V_A - V_D$. ¿Cuál es la fem equivalente que habría que aplicar al circuito con extremos en A y D para conseguir las mismas corrientes? 
- d) Calcular la potencia entregada al circuito.
![Pasted image 20260605224431](../assets/Pasted%20image%2020260605224431.png)
#### Definición de Nodos

- **Nodo A:** Terminal de entrada A. Conecta el extremo izquierdo del resistor $R$.
- **Nodo B:** Punto de unión de la primera bifurcación. Conecta el extremo derecho del resistor $R$, el polo positivo (barra larga) de la fuente de $10\text{ V}$ y el extremo izquierdo del resistor $R_y$.
- **Nodo 1 (Interno):** Ubicado en la rama central superior, entre el polo negativo (barra corta) de la fuente de $10\text{ V}$ y el extremo izquierdo del resistor $R_x$.
- **Nodo C:** Punto de unión de la segunda bifurcación. Conecta el extremo derecho del resistor $R_x$, el extremo derecho del resistor $R_y$ y el polo positivo (barra larga) de la fuente de $15\text{ V}$.
- **Nodo D:** Terminal de salida D. Conecta el polo negativo (barra corta) de la fuente de $15\text{ V}$.
    

#### Netlist (Formato SPICE / Tabla)

| **Componente** | **Nodo (+)** | **Nodo (-)** | **Valor**     | **Descripción**                                                       |
| -------------- | ------------ | ------------ | ------------- | --------------------------------------------------------------------- |
| **R**          | A            | B            | -             | Resistor de entrada de la corriente $I_1$                             |
| **V1**         | B            | 1            | $10\text{ V}$ | Fuente de voltaje superior central                                    |
| **R_x**        | 1            | C            | -             | Resistor de la rama superior central (corriente $I_2$)                |
| **R_y**        | B            | C            | -             | Resistor de la rama inferior central en paralelo con la rama de $R_x$ |
| **V2**         | C            | D            | $15\text{ V}$ | Fuente de voltaje de la rama derecha                                  |
### Resolucion
#### a)
Analizemos el nodo B, planteando KCL, tomando la convención de la corriente que entra a un nodo es negativa, y la que sale positiva:
$$
\begin{align}
\sum_{B} I &  = 0 \\
-I_{1} + I_{2} + I_{y}   & = 0 \\
I_{y}  & = 4A - 2A = 2A
\end{align}
$$
Por tanto, $I_{y}$ es igual a 2A y circula en el mismo sentido que $I_{2}$ (sale del nodo).
#### b)
Aplicamos ley de ohm para obtener la resistencia $R_{y}$:
$$
R_{y}= \frac{V_{B-C}}{I_{y}} = \frac{12V}{2A} = 6\Omega
$$
Para encontrar la resistencia $R_{x}$, aplicamos la ley de ohm generalizada (teniendo en cuenta el diferencial de potencial que provoca la fuente):
$$
R_{x} = \frac{(V_{B}-V_{\text{fuente}}) - V_{C}}{I_{2}} = \frac{V_{B-C} - V_{\text{fuente}}}{I_{2}} = \frac{12V-10V}{2A} =1\Omega 
$$
#### c)
El diferencial de potencial entre el punto A y D, se puede calcular como:
$$
\Delta V_{A-D} = \Delta V_{A-B} + \Delta V_{B-C} + \Delta V_{C-D}
$$
Tenemos que:
$$
\Delta V_{A-B} = I_{1}R = 4A \times 10 \Omega = 40 V
$$
y dado que en el trozo de circuito C-D solo contamos con una pila con su borne postivo primero, tenemos que el diferencial de potencial en este tramo resulta:
$$
\Delta V_{C-D} = 15V
$$
Por tanto:
$$
\Delta V_{A-D} = 40V + 12V + 15V = 67V
$$
Esto quiere decir, asumiendo una fuente de energía ideal (sin resistencia interna), la fuerza electromotriz $\varepsilon$ necesaria para empujar la misma corriente (4A) a través del circuito A-D es $67V$.
#### d)
La potencia otorgada al circuito resulta:
$$
P = V_{A-D} \times I_\text{generado} = 67V \times 4A = 268 W
$$
### Ejercicio 9

En el circuito de la figura los dos amperímetros marcan 1.70 A y la potencia entregada por la fuente es de 300 W. Determinar $R_1$, $R_2$ y la tensión de la fuente.
![Pasted image 20260605224536](../assets/Pasted%20image%2020260605224536.png)

#### Definición de Nodos

- **Nodo 0 (Tierra):** Línea horizontal inferior (a la derecha de $R_1$). Conecta el polo negativo de la batería, el extremo derecho del resistor $R_1$, y los terminales inferiores de los resistores de $95\ \Omega$, $R_2$ y $154,3\ \Omega$.
- **Nodo 1:** Punto de unión inmediatamente superior de la batería. Conecta el polo positivo de la batería, el extremo derecho del resistor de $28\ \Omega$ y el terminal izquierdo del amperímetro superior.
- **Nodo 2:** Esquina superior izquierda. Conecta el extremo izquierdo del resistor de $28\ \Omega$ con el terminal superior del amperímetro izquierdo.
- **Nodo 3:** Esquina inferior izquierda. Conecta el terminal inferior del amperímetro izquierdo con el extremo izquierdo del resistor $R_1$.
- **Nodo 4:** Línea horizontal superior derecha (después del amperímetro). Conecta el terminal derecho del amperímetro superior y los extremos superiores de los resistores en paralelo de $95\ \Omega$, $R_2$ y $154,3\ \Omega$.
    

#### Netlist (Formato SPICE / Tabla)

|**Componente**|**Nodo (+)**|**Nodo (-)**|**Valor**|**Descripción**|
|---|---|---|---|---|
|**V1**|1|0|-|Fuente de voltaje central|
|**R_sup_izq**|2|1|$28\ \Omega$|Resistor en la rama superior izquierda|
|**A_izq**|2|3|-|Amperímetro de la rama vertical izquierda|
|**R_1**|3|0|-|Resistor $R_1$ en la rama inferior izquierda|
|**A_sup**|1|4|-|Amperímetro en la rama horizontal superior|
|**R_para_1**|4|0|$95\ \Omega$|Primer resistor del bloque en paralelo derecho|
|**R_2**|4|0|-|Resistor $R_2$ (central del bloque en paralelo derecho)|
|**R_para_3**|4|0|$154,3\ \Omega$|Resistor del extremo derecho del bloque en paralelo|
### Resolucion
#### Encontrando la tensión
Nos damos cuenta que en el nodo 1 circula la corriente total ofrecida por la batería. Aplicando KCL en el nodo 1:
$$
\begin{align}
\sum_{1} I  & = 0 \\ 
-I_{total} + I_{\text{izq}} + I_{\text{sup der}}  & = 0 \\
I_{\text{total}}  & = I_{izq} + I_{\text{sup der}}
\end{align}
$$
Dado que ambos amperímetros (el de la izquierda y el superior derecho) dan 1.70 A, entonces:
$$
I_{total} = 2\times1.70 A
$$
Y por tanto, la tensión total que ofrece la fuente es:
$$
\begin{align}
P_{\text{total}} &  = I_{\text{total}} \times V_{\text{total}} \\
V_{\text{total}} &  = \frac{P_{\text{total}}}{I_{\text{total}}}= \frac{300W}{2\times 1.70A} = \frac{1500}{17}V
\end{align}
$$
#### Encontrando R1
Aplicamos KVL a la malla 1 (izquierda):
$$
\begin{align}
V_{\text{total}} - 28 \Omega \times 1.70A  - R_{1} \times 1.70 A  & = 0 \\
R_{1}  & = \frac{{V_{\text{total}} - 28 \Omega \times 1.70A}}{1.70A} \\
R_{1}  & = \frac{6908}{289} \Omega
\end{align}
$$
#### Encontrando R2
Todo el bloque derecho (resistencias $95 \Omega, R_{2}, 154,3 \Omega$ se encuentran en paralelo, conectadas superiormente en el nodo 1 al borne positivo de la fuente y conectadas inferiormente al nodo 0 (borne negativo de la fuente). Dado que se encuentran en paralelo, podemos definir la resistencia equivalente de todo el bloque como:
$$
\begin{align}
\frac{1}{R_{\text{eq der}}} = \frac{1}{95 \Omega} + \frac{1}{R_{2}} + \frac{1}{154,3 \Omega}
\end{align}
$$
Finalmente, definimos:
$$
\begin{align}
V_{\text{der}}  & = V_{\text{total}} = I_{\text{sup der}}\times R_{\text{eq der}} \\
R_{\text{eq der}}  & = \frac{V_{\text{total}}}{I_{\text{sup der}}} \implies R_{2} = 442,58 \Omega
\end{align}
$$
### Ejercicio 10
¿Cuál es la diferencia de potencial entre los puntos P y Q?
![Pasted image 20260605224549](../assets/Pasted%20image%2020260605224549.png)

#### Circuito 1 (Izquierda)

##### Definición de Nodos

- **Nodo 0 (Tierra):** Puntos conectados al símbolo de masa. Conecta el polo negativo de la fuente de 6V y el extremo inferior del resistor de $2\ \Omega$.
- **Nodo 1:** Rama superior. Conecta el polo positivo de la fuente de 6V con el extremo superior del resistor de $1\ \Omega$.
- **Nodo P:** Punto de conexión central P. Conecta el extremo inferior del resistor de $1\ \Omega$ con el extremo superior del resistor de $2\ \Omega$.

##### Netlist (Formato SPICE / Tabla)

| **Componente** | **Nodo (+)** | **Nodo (-)** | **Valor**  | **Descripción**                            |
| -------------- | ------------ | ------------ | ---------- | ------------------------------------------ |
| **V1**         | 1            | 0            | 6 V        | Fuente de voltaje (Polo negativo a Tierra) |
| **R_sup**      | 1            | P            | 1 $\Omega$ | Resistor superior de la rama               |
| **R_inf**      | P            | 0            | 2 $\Omega$ | Resistor inferior conectado a Tierra       |

#### Circuito 2 (Derecha)

##### Definición de Nodos

- **Nodo 0 (Tierra):** Puntos conectados al símbolo de masa. Conecta el extremo superior del resistor de $4\ \Omega$ y el polo positivo (barra larga) de la fuente de 6V.
- **Nodo Q:** Punto de conexión central Q. Conecta el extremo inferior del resistor de $4\ \Omega$ con el extremo superior del resistor de $2\ \Omega$.
- **Nodo 1:** Línea inferior de retorno. Conecta el extremo inferior del resistor de $2\ \Omega$ con el polo negativo (barra corta) de la fuente de 6V.

##### Netlist (Formato SPICE / Tabla)

| **Componente** | **Nodo (+)** | **Nodo (-)** | **Valor**  | **Descripción**                            |
| -------------- | ------------ | ------------ | ---------- | ------------------------------------------ |
| **R_sup**      | 0            | Q            | 4 $\Omega$ | Resistor superior conectado a Tierra       |
| **R_inf**      | Q            | 1            | 2 $\Omega$ | Resistor inferior                          |
| **V2**         | 0            | 1            | 6 V        | Fuente de voltaje (Polo positivo a Tierra) |
### Resolucion
#### Encontrando potencial en P
Averiguamos la corriente total del circuito con:
$$
\begin{align}
I_{\text{total P}} =  \frac{6 V}{3 \Omega} = 2A
\end{align}
$$
Ahora calculamos la caída de potencial en la resistencia $1 \Omega$:
$$
\begin{align} 
\Delta V_{R_{sup}} = I_{\text{total P}} \times 1 \Omega = 2V
\end{align}
$$
Por tanto, en el punto P nos encontramos a $6V -2V=4V$
#### Encontrando potencial en Q 
Averiguamos la corriente total del circuito con:
$$
\begin{align}
I_{\text{total D}} =  \frac{6 V}{6 \Omega} = 1A
\end{align}
$$
Ahora calculamos la caída de potencial en la resistencia $2 \Omega$:
$$
\begin{align} 
\Delta V_{R_{sup}} = I_{\text{total P}} \times 2 \Omega = 2V
\end{align}
$$
Por tanto, en el punto Q nos encontramos a $6V -2V=4V$

Esto quiere decir que la diferencia entre el potencial de P con respecto a Q es 0.
### Ejercicio 11

Para la porción del circuito que se ilustra calcule las corrientes en las ramas AB, AC y CB y las diferencias de potencial entre estos puntos. Indique por qué no puede realizarse en este caso un balance de potencias.

![Pasted image 20260605224602](../assets/Pasted%20image%2020260605224602.png)

#### Definición de Nodos

- **Nodo 0 (Tierra) / Nodo C:** Punto inferior central con el símbolo de masa. Conecta el polo negativo de la fuente de $20\text{ V}$ y el extremo inferior de la resistencia de $5\ \Omega$.
- **Nodo A:** Terminal izquierda. Conecta la entrada externa de corriente de $2\text{ A}$, el extremo izquierdo de la resistencia de $1\ \Omega$ y el extremo superior de la resistencia de $3\ \Omega$.
- **Nodo B:** Terminal derecha. Conecta la salida externa de corriente de $1\text{ A}$, el polo negativo de la fuente de $10\text{ V}$ y el extremo superior de la resistencia de $5\ \Omega$.
- **Nodo 1 (Interno rama A-B):** Ubicado en la rama superior, entre el extremo derecho de la resistencia de $1\ \Omega$ y el polo positivo de la fuente de $10\text{ V}$.
- **Nodo 2 (Interno rama A-C):** Ubicado en la rama diagonal izquierda, entre el extremo inferior de la resistencia de $3\ \Omega$ y el polo negativo de la fuente de $20\text{ V}$.

### Resolucion
#### Corriente en AB

#### Netlist (Formato SPICE / Tabla)

| **Componente** | **Nodo (+)** | **Nodo (-)** | **Valor**     | **Descripción**                                      |
| -------------- | ------------ | ------------ | ------------- | ---------------------------------------------------- |
| **I_in**       | A            | Ext*         | $2\text{ A}$  | Corriente entrante al Nodo A desde el exterior       |
| **I_out**      | Ext*         | B            | $1\text{ A}$  | Corriente saliente desde el Nodo B hacia el exterior |
| **R_top**      | A            | 1            | $1\ \Omega$   | Resistencia de la rama superior                      |
| **V_top**      | 1            | B            | $10\text{ V}$ | Fuente de voltaje de la rama superior                |
| **R_diag_izq** | A            | 2            | $3\ \Omega$   | Resistencia de la rama diagonal izquierda            |
| **V_diag_izq** | 0            | 2            | $20\text{ V}$ | Fuente de voltaje de la rama diagonal izquierda      |
| **R_diag_der** | B            | 0            | $5\ \Omega$   | Resistor de la rama diagonal derecha                 |

_Nota: "Ext" representa las conexiones externas o del resto del circuito no dibujado por donde entran y salen las corrientes especificadas._
### Resolucion
Para el nodo A, tenemos que KCL dice:
$$
- 2A + I_{{AB}} + I_{{AC}}=0 \tag{1}
$$
Aplicamos ley de ohm generalizada para las ramas AB y AC:
$$
\begin{align}
I_{AB} = \frac{V_{A} - 10V - V_{B}}{1 \Omega} \tag{2} \\
I_{AC} = \frac{V_{A} + 20V - 0}{3 \Omega} \tag{3}
\end{align}
$$
Para el nodo B, tenemos que KCL dice:
$$
\begin{align}
- I_{AB} +1A + I_{BC} &  =0 \\
I_{BC}  & = I_{AB} - 1 \tag{4}
\end{align}
$$
Aplicamos ley de ohm generalizada para las ramas BC:
$$
\begin{align}
I_{BC} = \frac{V_{B} - 0}{5 \Omega} \tag{5} \\
\end{align}
$$

Usamos estas ecuaciones y despejamos, empezamos con (5), (4) y (2):
$$
\begin{align}
\frac{V_{B}}{5\Omega} &  =  \frac{V_{A}-10V -V_{B}}{1 \Omega} - 1A \\
\frac{V_{B}}{5\Omega} + \frac{5V_{B}}{5\Omega} &  =  \frac{V_{A}-10V}{1 \Omega} - 1A  \\
V_{B}  & = \frac{5\Omega}{6}({\frac{V_{A}-10V}{1 \Omega} - 1A})
\end{align}
$$

El despeje de (5), (4) y (2) se puede reducir así:

$$\begin{align} \frac{V_{B}}{5} & = V_{A} - 10 - V_{B} - 1 \\ \frac{V_{B}}{5} + V_{B} & = V_{A} - 11 \\ \frac{6V_{B}}{5} & = V_{A} - 11 \\ V_{B} & = \frac{5}{6}(V_{A} - 11) \end{align}$$
Usando (1), (2), (3), tenemos:
$$
\begin{align}
\frac{V_{A} + 20V}{3 \Omega}  & = - \frac{V_{A} - 10V - V_{B}}{1 \Omega} + 2A \\
\end{align}
$$

Sustituyendo esto en la ecuación del Nodo A reducida:

$$\begin{align} \frac{V_{A} + 20}{3} & = - (V_{A} - 10 - V_{B}) + 2 \\ \frac{V_{A} + 20}{3} & = -V_{A} + 12 + \frac{5}{6}(V_{A} - 11) \\ \frac{V_{A} + 20}{3} & = -V_{A} + 12 + \frac{5}{6}V_{A} - \frac{55}{6} \\ \frac{V_{A} + 20}{3} & = -\frac{1}{6}V_{A} + \frac{17}{6} \end{align}$$

Multiplicando toda la ecuación por 6 para eliminar los denominadores:

$$\begin{align} 2(V_{A} + 20) & = -V_{A} + 17 \\ 2V_{A} + 40 & = -V_{A} + 17 \\ 3V_{A} & = -23 \\ V_{A} & = -\frac{23}{3}\text{ V} \approx -7.67\text{ V} \end{align}$$

Con $V_A$ despejado, los resultados finales que debes obtener al reemplazar hacia atrás son:

- **Voltaje en B:** $V_B = -\frac{140}{9}\text{ V} \approx -15.56\text{ V}$
- **Corriente AC:** $I_{AC} = \frac{37}{9}\text{ A} \approx 4.11\text{ A}$ (Hacia abajo)
- **Corriente AB:** $I_{AB} = -\frac{19}{9}\text{ A} \approx -2.11\text{ A}$ (El signo negativo indica que la corriente fluye de B hacia A, no de A hacia B)
- **Corriente BC:** $I_{BC} = -\frac{28}{9}\text{ A} \approx -3.11\text{ A}$ (Fluye de tierra hacia el Nodo B)

Para que la sumatoria de potencias entregadas y disipadas sea exactamente igual a cero (conservación de la energía), el circuito debe estar completamente cerrado y aislado.

En este esquema, tienes $2\text{ A}$ inyectándose en el Nodo A y $1\text{ A}$ extrayéndose en el Nodo B provenientes de un resto del circuito que es invisible o "caja negra". Como no conoces qué componentes externos están generando o consumiendo esa energía exterior, ni a qué potencial absoluto se encuentran las fuentes externas que empujan esos amperios, es físicamente imposible contabilizar el balance total de energía del sistema. Solo puedes calcular el comportamiento local de esta porción específica.
### Ejercicio 12

Entre los puntos A y B del circuito de la figura se conecta un amperímetro de resistencia R. Hallar la corriente medida en función de V, $R_1$, $R_2$, $R_3$ y $R_4$, y determinar para qué valores de estos parámetros la corriente se anula. Nota: Este es el circuito conocido como "Puente de Wheatstone" que se usa para comparar resistencias desconocidas con resistencias patrón.

**Descripción del circuito (Puente de Wheatstone Estándar):**

Plaintext

```
- Fuente de tensión continua (V) conectada a un arreglo en forma de rombo.
- El terminal superior de la fuente (V) se ramifica hacia las resistencias R1 y R3.
- El terminal inferior de la fuente se ramifica hacia las resistencias R2 y R4.
- La resistencia R1 se conecta entre el extremo superior y el Nodo A (ubicado en el vértice izquierdo).
- La resistencia R2 se conecta entre el Nodo A y el extremo inferior.
- La resistencia R3 se conecta entre el extremo superior y el Nodo B (ubicado en el vértice derecho).
- La resistencia R4 se conecta entre el Nodo B y el extremo inferior.
- Un Amperímetro transversal (con resistencia interna R) puentea el Nodo A y el Nodo B.
```