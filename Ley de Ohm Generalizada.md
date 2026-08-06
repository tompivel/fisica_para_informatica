---
id: 20260607105841
aliases: []
tags:
  - uncataloged
created: 2026-06-07 10:58
status: draft
---
# Ley de Ohm Generalizada
### La Regla de Oro de la Polaridad

La Ley de Ohm generalizada se puede resumir en una sola fórmula infalible para cualquier rama:

$$I = \frac{V_{\text{origen}} - V_{\text{destino}} + \sum V_{\text{baterías}}}{R}$$

El verdadero secreto está en **qué signo** le pones a ese voltaje de la batería. Para no equivocarte nunca en un examen, debes usar la técnica de "caminar por la rama".

### La Técnica de "Caminar por la Rama"

Cuando planteas una corriente como $I_{AB}$, estás asumiendo matemáticamente que los electrones van a viajar desde el Nodo A (origen) hasta el Nodo B (destino).

Imagina que caminas sobre el cable desde A hacia B. Al encontrarte con una batería en tu camino, fíjate en qué terminal "chocas" primero:

- **Si chocas con el polo POSITIVO primero (la barra larga):** Estás yendo de mayor a menor potencial dentro de la pila. Es una caída de tensión. Por lo tanto, debes **RESTAR** el valor de la fuente en tu ecuación ($-V$). La pila está "empujando en contra" de tu camino.
- **Si chocas con el polo NEGATIVO primero (la barra corta):** Estás yendo de menor a mayor potencial. Es una ganancia de tensión. Por lo tanto, debes **SUMAR** el valor de la fuente en tu ecuación ($+V$). La pila te está "dando un empujón a favor" en tu camino.
    
Esa es toda la magia de la Ley de Ohm generalizada. Planteas el camino (Origen - Destino) y simplemente sumas o restas las baterías según con qué polo te tropieces primero en ese recorrido.
# Deducción Ley de Ohm Generalizada

> sigo sin entender esta regla de ohm generalizada, ¿en qué se fundamenta? Suena a un truco o atajo que podría llegar a complicar en un examen. Antes de usarla, me gustaría entenderla.

No es un truco ni un atajo arbitrario. La "Ley de Ohm generalizada" es simplemente la combinación rigurosa de la definición de diferencia de potencial y la Ley de Ohm clásica, analizadas desde la perspectiva de la conservación de la energía en un circuito (las bases de Kirchhoff KCL).

Para demostrar que es infalible en un examen, vamos a deducirla paso a paso.

### La deducción física

La Ley de Ohm fundamental establece que la corriente a través de una resistencia depende estrictamente de la diferencia de potencial **entre los bornes exactos de esa resistencia**:

$$I = \frac{\Delta V_{R}}{R} = \frac{V_{\text{entrada}} - V_{\text{salida}}}{R}$$

Imagina una rama típica de tu Ejercicio 7 (como la rama B). Tienes un nodo superior (Nodo 1) a un potencial $V_1$, una batería con su polo positivo mirando hacia arriba ($V_f = 10\text{V}$), una resistencia $R$, y finalmente la conexión a Tierra ($0\text{V}$).

Si recorremos la rama desde el Nodo 1 hacia la Tierra para calcular qué voltaje "ve" realmente la resistencia:

1. **Punto de partida:** Estás en el Nodo 1. El potencial eléctrico allí es $V_1$.
    
2. **Atravesando la batería:** Caminas hacia la resistencia y atraviesas la batería desde el polo positivo al negativo. Como vas de mayor a menor potencial dentro de la fuente, experimentas una caída de tensión igual al valor nominal de la batería. Al salir de la batería, el nuevo potencial eléctrico en ese punto intermedio del cable es exactamente $V_1 - V_f$.
    
3. **Llegando a la resistencia:** El borne superior de la resistencia está conectado a ese punto intermedio. Por lo tanto, el voltaje a la entrada de la resistencia es $V_{\text{entrada}} = V_1 - V_f$.
    
4. **Saliendo de la resistencia:** El borne inferior de la resistencia está conectado directamente a Tierra. Por lo tanto, su voltaje de salida es $V_{\text{salida}} = 0\text{V}$.
    

Ahora, sustituimos estos valores reales en la Ley de Ohm fundamental:

$$I = \frac{(V_1 - V_f) - 0}{R}$$

$$I = \frac{V_1 - V_f}{R}$$

Como puedes ver, la ecuación no "inventa" nada. Simplemente calcula cuál es el voltaje efectivo que empuja los electrones a través del resistor tras descontar el salto de potencial que fuerza la batería.

### Inversión de polaridad

Si la batería estuviera conectada al revés (polo negativo hacia el Nodo 1), al caminar desde el nodo hacia la resistencia subirías un escalón de potencial. El voltaje a la entrada de la resistencia sería $V_1 + V_f$.

La fórmula sigue siendo robusta si tratas el voltaje de la fuente con su signo correspondiente respecto al sentido en el que asumes la corriente.

> OK, pero esta deduccion que me acabas de dar seria para la corriente en un resistor en aquella rama, ¿por que debería deducir tambien que es la corriente de toda la rama? ¿Porque la corriente es la misma en toda la rama por conservacion de carga?

¡Exactamente! Has dado en el clavo.

La corriente que calculas para la resistencia es, por definición, la corriente de **toda esa rama**.

Aquí está la justificación física de por qué esto es así:

- **Componentes en serie:** En esa rama específica (desde el Nodo 1 hasta la Tierra), la batería y la resistencia están conectadas una detrás de la otra, formando un único camino continuo. Es decir, están en serie.
    
- **Conservación de la carga:** Como bien intuyes, los electrones no tienen otro lugar a donde ir. No hay bifurcaciones intermedias en esa rama donde la corriente pueda dividirse, ni los electrones pueden acumularse o desaparecer en el medio del cable. Por lo tanto, la cantidad de carga que pasa por la batería por segundo tiene que ser exactamente igual a la cantidad de carga que pasa por la resistencia por segundo.
    

Es como el flujo de agua en una manguera que no tiene pinchazos: aunque el agua pase primero por una bomba (la batería) y luego por una boquilla estrecha (la resistencia), los litros por minuto (la corriente) que circulan por cualquier punto de esa manguera son exactamente los mismos.

Por eso, al calcular la corriente que logra atravesar el obstáculo principal (la resistencia) usando la diferencia de potencial efectiva, automáticamente has descubierto la corriente que fluye por cada milímetro de esa rama.


## Deducción a partir de KCL
> Ok, entiendo la aplicación de signos, pero no me termina de quedar clara esta ley. ¿esta ley solo se puede usar en una rama que va desde un nodo a hasta un nodo b, sin intersecciones de otras ramas en la mitad? ¿verdad? ¿Por que es posible agrupar todas las posibles resistencias de la rama en un solo término R si pueden estar intercaladas con las fuentes?

La ley de Ohm generalizada solo se puede aplicar a una rama que consiste en un **camino en serie puro** entre dos nodos principales, sin ninguna intersección o bifurcación en el medio.

Si existe una intersección por donde puede entrar o salir corriente (un nuevo nodo), la corriente $I$ deja de ser constante a lo largo de todo el trayecto. Al haber distintas corrientes antes y después de la intersección, es matemáticamente imposible usar una única variable $I$ en la ecuación. En ese caso, la rama original se ha convertido en dos ramas distintas, y debes aplicar la fórmula por separado para cada tramo.

### Agrupación de Resistencias Intercaladas

La capacidad de agrupar todas las resistencias en un solo término del denominador ($R_{\text{eq}} = R_1 + R_2 + \dots$), independientemente de si hay baterías mezcladas entre ellas, se fundamenta en la **propiedad conmutativa de la suma** dentro de la Ley de Voltajes de Kirchhoff (KVL).

Dado que la rama no tiene bifurcaciones (es un circuito en serie), la corriente $I$ que atraviesa el primer componente es exactamente la misma que atraviesa el último.

Para demostrarlo, imagina una rama que va del Nodo A al Nodo B. En el camino, la corriente $I$ atraviesa una resistencia $R_1$, luego una batería que aporta un potencial $V_{\text{bat}}$ (chocando con el polo negativo primero), y finalmente otra resistencia $R_2$.

Si planteamos el recorrido paso a paso (KVL):

$$V_A - \Delta V_{R_1} + V_{\text{bat}} - \Delta V_{R_2} = V_B$$

Sustituyendo la caída en cada resistencia por la Ley de Ohm local ($\Delta V = I \cdot R$):

$$V_A - (I \cdot R_1) + V_{\text{bat}} - (I \cdot R_2) = V_B$$

Dado que la corriente $I$ es el factor común en las caídas de tensión, puedes agrupar esos términos mediante álgebra simple:

$$V_A + V_{\text{bat}} - V_B = I \cdot R_1 + I \cdot R_2$$

Sacando factor común $I$:

$$V_A - V_B + V_{\text{bat}} = I(R_1 + R_2)$$

Al despejar $I$, el orden físico de los componentes desaparece de la ecuación y se consolida la Ley de Ohm generalizada:

$$I = \frac{V_A - V_B + V_{\text{bat}}}{R_1 + R_2}$$

Físicamente, el voltaje es una medida de energía potencial. El orden en el que restas energía (resistencias) o sumas energía (baterías) no importa; el balance energético total para ir del punto A al punto B requiere exactamente la misma tasa de flujo (corriente) sin importar la secuencia de los obstáculos.
