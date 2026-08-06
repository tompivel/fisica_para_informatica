---
id: 20260628153659
aliases: []
tags:
  - uncataloged
created: 2026-06-28 15:36
status: draft
---
# Examen 2do Parcial 2025-2C
# CB024 Física para Informática – Segundo parcial

**Tema 1**

**2do Cuatrimestre 2025**

## Ejercicio 1

En el circuito de la figura, todas las resistencias son múltiplos de $R$ y la pila tiene un voltaje $V_0$. En el estado **estacionario**, calcular:
![Pasted image 20260628153950](../assets/Pasted%20image%2020260628153950.png)

a. La potencia que entrega la pila.

- i. 43 W
- ii. 16 W
- iii. 5 W
- iv. 27 W
- v. Ninguna de las anteriores.

b. La potencia disipada por la resistencia $R_1$.

- i. 2 W
- ii. 7 W
- iii. 18 W
- iv. 23 W
- v. Ninguna de las anteriores.

c. La corriente que circula por la resistencia $R_2$.

- i. 0.3 A
- ii. 1.1 A
- iii. 1.5 A
- iv. 2.1 A
- v. Ninguna de las anteriores.

d. La carga y la polaridad del voltaje sobre el capacitor, cuya capacidad es $C$.

- i. $Q = 8.9 \cdot 10^{-6}$ C, $V_A > V_B$
- ii. $Q = 8.9 \cdot 10^{-8}$ C, $V_A < V_B$
- iii. $Q = 1.4 \cdot 10^{-7}$ C, $V_A > V_B$
- iv. $Q = 1.4 \cdot 10^{-7}$ C, $V_A < V_B$
- v. Ninguna de las anteriores.

Datos: $R_1 = R$; $R_2 = 2R$; $R_3 = R$; $R_4 = 3R$; $C$ = 1 μF; $V_0$ = 10 V; $R$ = 1 Ω

**[Descripción de la figura para la IA]:**

El esquema muestra un circuito de corriente continua. En la rama izquierda hay una fuente de voltaje $V_0$. Desde su terminal positivo (arriba), la corriente fluye hacia la derecha pasando por una resistencia $R_1$ en serie hasta llegar a un nodo de derivación que llamaremos **Nodo A** (marcado con un punto y la letra A).

Desde el Nodo A, el circuito se divide en tres trayectorias:

1. Hacia abajo: una rama que pasa por la resistencia $R_2$ y se conecta directamente al cable inferior de retorno (conectado al terminal negativo de la fuente).
2. Hacia la derecha: dos ramas en paralelo que conectan el Nodo A con otro nodo marcado como **Nodo B**. La rama superior contiene una resistencia $R_3$ y la rama inferior contiene un capacitor $C$.
Finalmente, desde el Nodo B, una rama desciende pasando por la resistencia $R_4$ hasta conectarse también al cable inferior de retorno.

## Ejercicio 2

Dos bobinados de $N_1$ y $N_2$ vueltas respectivamente se hallan enrollados en un núcleo magnético largo de sección circular de radio $r$ y permeabilidad relativa $\mu_r$, como indica la figura.

a. Calcular la autoinductancia de cada uno de los bobinados y la inductancia mutua de los mismos, suponiendo válida la aproximación de solenoide infinito. **Indique claramente** cómo calcula las magnitudes que necesita calcular, justificando todas y cada una de las suposiciones que realiza.

b. El primer bobinado es alimentado con una fuente de corriente $I_1(t) = K \cdot t$, con $K$ = 5 A/s. Suponiendo que el primer bobinado tiene una autoinductancia $L_1 = 10^{-4}$ Hy, el segundo $L_2 = 4 \cdot 10^{-2}$ Hy, que la inductancia mutua es $M = 2 \cdot 10^{-3}$ Hy, que los bornes A y B son homólogos y que $R$ = 10 Ω, escriba la ecuación que rige la evolución temporal de la corriente $I_2$, cuando se cierra la llave.

c. Si $t=0$ es el instante en que se cierra la llave, ¿cuál de los siguientes gráficos representa la evolución temporal de la corriente $I_2$?

**[Descripción de la figura para la IA]:**

La imagen consta de dos partes:

1. **Esquema físico:** Muestra un núcleo magnético cilíndrico vertical continuo de radio $r$ y permeabilidad $\mu_r$. Sobre él hay dos bobinados. El superior ($L_1$) tiene $N_1$ vueltas, longitud $l_1$, y está alimentado por una corriente entrante $I_1(t)$. El inferior ($L_2$) tiene $N_2$ vueltas, longitud $l_2$, y sus terminales se etiquetan como A (arriba) y B (abajo). Estos terminales A y B forman un circuito secundario cerrado que incluye una resistencia $R$ y un interruptor ("llave"). Se indica una corriente inducida $I_2(t)$ fluyendo por este secundario.
    
2. **Gráficos cartesianos (opciones para el inciso c):** Se muestran cuatro gráficos de $I_2(t)$ en el eje Y (en mA) en función del tiempo $t$ en el eje X (en ms). Todos muestran curvas exponenciales transitorias:
    
    - **Arriba a la izquierda:** La curva inicia en 0 mA en $t=0$ y decrece exponencialmente hacia una asíntota en -20 mA.
    - **Arriba a la derecha:** La curva inicia en -20 mA en $t=0$ y asciende exponencialmente hacia una asíntota en 0 mA.
    - **Abajo a la izquierda:** La curva inicia en 0 mA en $t=0$ y asciende exponencialmente hacia una asíntota en 20 mA.
    - **Abajo a la derecha:** La curva inicia en 20 mA en $t=0$ y decrece exponencialmente hacia una asíntota en 0 mA.
        

## Ejercicio 3

Contestar verdadero (V) o falso (F) en cada una de las siguientes afirmaciones.

a. Si en un circuito, un nodo está conectado a tierra, la suma algebraica de las corrientes que llegan o salen de él son siempre nulas.

b. La presencia de un capacitor en una rama de un circuito alimentado por una batería implica que la corriente que circula por esa rama es nula desde el instante que se efectúa la conexión.

c. Dados dos solenoides acoplados magnéticamente (inductancia mutua no nula), agregar un núcleo magnético a uno de ellos modifica la autoinductancia del propio solenoide, pero no influye sobre el valor de la inductancia mutua.

d. Si queremos aumentar el tiempo característico de un circuito de carga R-C, bastará con alimentarlo con una fuente de mayor voltaje.

_(Este ejercicio no cuenta con figura asociada)._

## Ejercicio 4
![Pasted image 20260628154033](../assets/Pasted%20image%2020260628154033.png)

Una instalación eléctrica domiciliaria puede representarse por una resistencia equivalente $R$ ($R$ = 100 Ω) en serie con una autoinductancia $L$ ($L$ = 0.32 Hy). Si la compañía eléctrica alimenta la instalación con una corriente alterna de $V_{ef}$ = 220 V y $f$ = 50 Hz, encuentre:

a. La potencia activa y la potencia reactiva que entrega la fuente.

- i. $P_{ac}$ = 122 W y $P_{reac}$ = 115 VA
- ii. $P_{ac}$ = 122 W y $P_{reac}$ = -115 VA
- iii. $P_{ac}$ = 241 W y $P_{reac}$ = -242 VA
- iv. $P_{ac}$ = 241 W y $P_{reac}$ = 242 VA
- v. Ninguna de las anteriores.

b. La compañía eléctrica quiere que la instalación tenga un factor de potencia ($\cos \varphi$) igual a 1. Para ello, les pide que coloquen un capacitor en paralelo con la fuente de alimentación, de modo que obtener un desfasaje nulo entre el voltaje de entrada y la corriente que entrega. ¿Qué valor debe tomar ese capacitor?

- i. $C$ = 6 μF
- ii. $C$ = 16 μF
- iii. $C$ = 25 μF
- iv. $C$ = 42 μF
- v. Ninguno de los anteriores.

c. En la configuración del punto b) ¿Cuánto vale la energía media almacenada por la autoinductancia?

- i. $U_L$ = 1.3 J
- ii. $U_L$ = 2.85 J
- iii. $U_L$ = 0.39 J
- iv. $U_L$ = 4.25 J
- v. Ninguna de las anteriores.

**[Descripción de las figuras para la IA]:**

Hay dos esquemas de circuitos de corriente alterna que acompañan el problema:

- **Circuito superior (corresponde a la situación inicial / inciso a):** Muestra una fuente de tensión alterna ($V_{ef}, \omega$) conectada en un lazo simple en serie con una resistencia $R$ y una autoinductancia $L$.
    
- **Circuito inferior (corresponde a la configuración del inciso b y c):** Es el mismo circuito anterior pero se le ha agregado un capacitor $C$ conectado en paralelo directamente a los bornes de la fuente alterna. En consecuencia, la rama que contiene la combinación en serie de la resistencia $R$ y la inductancia $L$ queda ahora en paralelo con el capacitor $C$.

---

![Pasted image 20260628153921](../assets/Pasted%20image%2020260628153921.png)
![Pasted image 20260628153928](../assets/Pasted%20image%2020260628153928.png)