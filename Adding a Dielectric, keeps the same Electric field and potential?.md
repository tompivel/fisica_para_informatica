---
id: 20260528104313
aliases: []
tags:
  - uncataloged
created: 2026-05-28 10:43
status: draft
---
# Adding a Dielectric, keeps the same Electric field and potential?

> Pregunta: los potenciales en ambos conductores se deben matener, lo que significa que el diferencial debe ser el mismo, es decir V =10V. Eso signficaria que el campo electrico tambien se debe mantener, o sea que E' = E. Lo cual me extrañaria porque implicaria que la capacitancia de un capacitor no cambia en absoluto al introducir un dielectrico dado que $C = Q/V_{ab}$ Por tanto, ¿en que camino conceptual estoy errando?

El error conceptual radica en la premisa: _"los potenciales en ambos conductores se deben mantener, lo que significa que el diferencial debe ser el mismo, es decir $V = 10\text{V}$"_.

Esa afirmación es falsa. Eso solo ocurre si la pila sigue conectada. Al desconectar la pila, el sistema queda aislado. En un sistema aislado, la magnitud que se conserva estrictamente es la **carga total $Q$**, no la diferencia de potencial $V$. Decir que un conductor es un "volumen equipotencial" significa que existe **uniformidad espacial**, no invarianza temporal.

Significa que toda la placa superior se encuentra a un único potencial $V_{\text{sup}}$, y toda la placa inferior a un único potencial $V_{\text{inf}}$. Por lo tanto, la _nueva_ diferencia de potencial $V' = V_{\text{sup}} - V_{\text{inf}}$ se aplica por igual a la sección que tiene vacío y a la que tiene dieléctrico ($V_{\text{vacio}}' = V_{\text{dielec}}' = V'$).

Ambas secciones experimentan el mismo $V'$ y el mismo campo $E'$, pero este nuevo $V'$ ya no es de $10\text{V}$.

### Cómo se resuelve la paradoja de la capacitancia

Tu deducción sobre la capacitancia es el camino correcto para ver la falla física:

1. **La capacitancia aumenta:** Al introducir un material dieléctrico (con $\epsilon_r > 1$) en cualquier porción del espacio entre las placas, la capacitancia total del sistema inevitablemente aumenta ($C' > C_{\text{inicial}}$) dado que $C = \frac{\epsilon_{r}\epsilon_{0}A}{d}$. El sistema ahora tiene mayor "capacidad" para almacenar carga por cada voltio.
2. **La carga está atrapada:** Como desconectaste la pila, los electrones no tienen a dónde ir. $Q_{\text{total}}$ es una constante inamovible.
3. **El voltaje debe caer:** Analizando la definición de capacitancia $V' = \frac{Q_{\text{total}}}{C'}$, si el numerador ($Q$) se mantiene constante y el denominador ($C$) aumenta, el cociente ($V'$) necesariamente disminuye. $V'$ será menor al original $V$.
4. **El campo eléctrico debe caer:** Dado que la distancia $d$ es fija y $E' = \frac{V'}{d}$, si el voltaje cae, el nuevo campo eléctrico uniforme en todo el espacio interior también será menor al original.


> Pero, eso sería en un sistema aislado, al introducir un diélectrico entre dos placas conductoras conectadas a una pila, el diferencial de potencial se debería mantener, ¿no es así? ¿Sería entonces la carga la que cambia en ese caso para mantener la equipotencialidad?

Es exactamente así. Al mantener la pila conectada, el diferencial de potencial $V$ es una constante innegociable impuesta por la fuente.

El mecanismo físico y matemático funciona de la siguiente manera:

1. **La capacitancia aumenta:** Al introducir el dieléctrico (con permitividad relativa $\epsilon_r > 1$), la capacidad del sistema para almacenar carga se multiplica: $C' = \epsilon_r C_0$.
2. **La carga debe adaptarse:** Dada la definición fundamental $C = \frac{Q}{V}$, si la capacitancia $C$ aumenta y el voltaje $V$ está fijado por la pila, el numerador necesariamente debe crecer en la misma proporción. La nueva carga será $Q' = \epsilon_r Q_0$.
    

**¿Qué hace la pila físicamente?**

Cuando el dieléctrico entra entre las placas, sus moléculas se polarizan y generan un campo eléctrico propio que se opone al campo original. Esto debilita momentáneamente el campo neto y hace caer la diferencia de potencial.

La pila "detecta" que el diferencial entre las placas ahora es menor a su propio voltaje (por ejemplo, menor a los $10\text{V}$). Para restaurar el equilibrio, la pila realiza trabajo y actúa como una bomba: arranca más electrones de una placa y los deposita en la otra. Inyecta esta nueva carga hasta que el campo eléctrico neto recupera su fuerza original ($E = \frac{V}{d}$) y el diferencial de potencial vuelve a igualar exactamente al de la fuente.