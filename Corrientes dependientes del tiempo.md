---
id: 20260626192603
aliases: []
tags:
  - uncataloged
created: 2026-06-26 19:26
status: draft
---
# Corrientes dependientes del tiempo
## Guía: Corrientes dependientes del tiempo

    
- **Ejercicio 2:** Se requiere analizar el crecimiento de la corriente en un circuito R-L cerrado por una llave, evaluando voltajes transitorios, la potencia y la energía almacenada. Consultar el **Capítulo 30 (Inductancia)**, centrándose en la Sección 30.4 (El circuito R-L) para el transitorio y la Sección 30.2 (Energía de un campo magnético) para el almacenamiento en el inductor.
    
- **Ejercicio 3:** Plantea el escenario análogo al anterior pero para un circuito R-C, requiriendo calcular el transitorio de corriente, caídas de potencial y energía. Consultar el **Capítulo 26 (Circuitos de corriente continua)** en su Sección 26.4 (Circuitos R-C, parte de carga del capacitor) y el **Capítulo 24 (Capacitancia y dieléctricos)** en la Sección 24.3 (Energía de un capacitor).
    
- **Ejercicio 4:** Pide calcular el valor de una resistencia con base en el tiempo y el porcentaje de corriente durante la descarga de un capacitor. Consultar el **Capítulo 26**, Sección 26.4 (Circuitos R-C, centrándose exclusivamente en la deducción matemática de la descarga).
    
- **Ejercicio 5:** Relaciona la energía límite ($t \to \infty$) de una inductancia para deducir la constante de tiempo de un circuito RL. Consultar el **Capítulo 30**, Secciones 30.2 (Energía de un campo magnético) y 30.4 (El circuito R-L para interpretar el límite asintótico de la corriente).
    
- **Ejercicio 6:** Requiere extraer información de un gráfico de crecimiento de corriente en un circuito RL para el instante en que alcanza el 63% de su valor final. Consultar el **Capítulo 30**, Sección 30.4 (El circuito R-L), prestando especial atención al concepto visual y matemático de la constante de tiempo inductiva ($\tau = L/R$).
    
- **Ejercicio 7:** Exige analizar un gráfico de descarga de un capacitor marcando el punto del 37% de la corriente inicial. Consultar el **Capítulo 26**, Sección 26.4 (Circuitos R-C), para interpretar gráficamente la constante de tiempo capacitiva ($\tau = RC$).
    
- **Ejercicio 8:** Es un problema complejo que involucra dos capacitores y una resistencia, exigiendo calcular redistribución de cargas, corrientes transitorias y diferencias de energía disipada como calor. Consultar el **Capítulo 26**, Sección 26.2 (Reglas de Kirchhoff) y 26.4 (Circuitos R-C), combinándolo con los balances de energía del **Capítulo 24**, Sección 24.3.
## Problema 1

**1.** Para el tramo de circuito de la figura, determinar:

a) La caída de voltaje en función del tiempo $(V_A(t) - V_B(t))$.
b) La potencia, $P_{AB}(t) = (V_A(t) - V_B(t)) \cdot I(t)$, entregada a dicho tramo.
$I(t) = 4 \exp(-t / 1\text{ s})$

```
* Circuito Ejercicio 1
R1 A C 10
L1 C B 1
```

### Resolución 
## Problema 2

**2.** El circuito consta de una batería $E = 100\text{ V}$ una resistencia $R = 10\,\Omega$ y una inductancia $L = 1\text{ H}$. La llave K se cierra en el instante $t = 0\text{ s}$.

a) Hallar y graficar la corriente $I(t)$ y los voltajes sobre la resistencia $V_R(t)$ y el inductor $V_L(t)$.

b) El instante en que la corriente alcanza la mitad de su valor final.

c) La potencia $P_R(t)$ disipada en el resistor y la energía $E_L(t)$ almacenada en el inductor.

Code snippet

```
* Circuito Ejercicio 2
V_E 1 0 DC 100
R_1 1 2 10
SW_K 2 3  ; Se cierra en t=0
L_1 3 0 1
```
## Problema 2

**3.** Si ahora se reemplaza el inductor del problema anterior por un capacitor $C = 20\,\mu\text{F}$

a) Hallar y graficar la corriente $I(t)$ y los voltajes sobre la resistencia $V_R(t)$ y el capacitor $V_C(t)$.

b) El instante en que la corriente alcanza la mitad de su valor inicial.

c) La potencia disipada en el resistor $P_R(t)$ y la energía $E_C(t)$ almacenada en el capacitor.
## Problema 2

**4.** Un capacitor $C = 10\,\mu\text{F}$ se descarga sobre una resistencia $R$ a partir del momento $t = 0\text{ s}$. En $t = 20\text{ ms}$ la corriente que circula por la resistencia es el $13.53\%$ de la máxima.

Calcular el valor de $R$.
## Problema 2

**5.** En el circuito de la figura la resistencia vale $R = 1\,\Omega$. A $t = 0\text{ s}$ se cierra la llave. Se sabe que luego de mucho tiempo de haber cerrado la llave, la energía almacenada en la inductancia es $10\text{ J}$. Calcular la constante de tiempo del circuito.

Code snippet

```
* Circuito Ejercicio 5
V_1 1 0 DC 10
SW_1 1 2  ; Se cierra en t=0
R_1 2 3 1
L_1 3 0 L_unknown
```

**6.** El gráfico muestra la corriente, $I(t)$, que circula por una inductancia $L = 10\text{ H}$ alimentada por una pila $V_0$ a través de una resistencia $R$. El punto del gráfico que se indica con línea punteada corresponde al instante ($t$) en el que $I(t) = 0.63 \times I(t = \infty)$. Calcular el valor de la pila que alimenta el circuito y de la resistencia.

_(Gráfico: Curva de crecimiento asintótica con asíntota en $2000\text{ mA}$. Punto punteado en $t = 1\,\mu\text{s}$)._
## Problema 2

**7.** El gráfico muestra la corriente de descarga $I(t)$ de un capacitor $C = 10\,\mu\text{F}$ sobre una resistencia $R$. El punto del gráfico que se indica con línea punteada marca el instante ($t$) en el que $I(t) = 0.37 \cdot I(t=0)$. Calcular la carga inicial $Q$ del capacitor y el valor de la resistencia.

_(Gráfico: Curva de decaimiento exponencial con ordenada al origen en $100\text{ mA}$. Punto punteado en $t = 1\text{ ms}$)._
## Problema 2

**8.** Un capacitor $C_1 = 20\,\mu\text{F}$, tiene una carga inicial de $200\,\mu\text{C}$. En el instante $t = 0$ se cierra la llave. Suponiendo que inicialmente $C_2$ está descargado:

a) Obtenga la corriente $i(t)$.

b) Obtenga $V_{C1}(t)$ y $V_{C2}(t)$ y las respectivas cargas finales en los mismos.

c) Evalúe la energía de campo inicial del capacitor $C_1$ y la final total del conjunto de capacitores $C_1$ y $C_2$.

d) Verifique que la diferencia coincide con la energía disipada en forma de calor por el resistor entre el instante inicial $t=0$ y $t$ tendiendo a infinito.

e) Demuestre que los resultados obtenidos en d) son independientes del valor del resistor.

f) Verifique que los resultados obtenidos para la carga final de los capacitores, coincide con los que se obtienen aplicando el método de mallas e islas estudiado oportunamente.

Code snippet

```
* Circuito Ejercicio 8
C1 1 0 20uF IC=10V
SW1 1 2 ; Se cierra en t=0
R1 2 3 10
C2 3 0 40uF IC=0V
```
## Problema 2

