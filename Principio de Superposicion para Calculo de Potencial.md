---
id: 20260529110800
aliases: []
tags:
  - uncataloged
created: 2026-05-29 11:08
status: draft
---
# Principio de Superposicion para Calculo de Potencial
Se puede aplicar el principio de superposicion para el calculo de potenciales en distintas regiones. En este caso analizamos el punto d del ejercicio: 
[Examen Parcial Fisica 2026-1C](Examen%20Parcial%20Fisica%202026-1C.md)

El principio de superposición **no excluye ni ignora** ninguna superficie en ninguna región. El hecho de que para $r > r_b$ el resultado sea visualmente idéntico al de una única carga puntual no es una decisión arbitraria, sino el resultado de una **cancelación matemática exacta**.

Para aplicar superposición en esferas concéntricas, debes tener grabada la regla del potencial de un cascarón esférico de radio $R$ y carga $Q$:

- **Afuera del cascarón ($r > R$):** El potencial decae con la distancia, como si fuera una carga puntual. $V = \frac{Q}{4\pi\epsilon_0 r}$
- **Adentro del cascarón ($r \leq R$):** El campo eléctrico es nulo, por lo que el potencial se "congela" y es constante e igual al de la superficie. $V = \frac{Q}{4\pi\epsilon_0 R}$

Si aplicamos rigurosamente la superposición (sumando las 3 cargas en todo momento) para las tres zonas, ocurre lo siguiente:

### 1. Para la región exterior ($r > r_b$)

Evalúas las tres fuentes considerando que tu posición $r$ está **afuera** de todas ellas:

- Carga puntual $+q$: $V_1 = \frac{q}{4\pi\epsilon_0 r}$
- Superficie interna $-q$: Como $r > r_a$, $V_2 = \frac{-q}{4\pi\epsilon_0 r}$
- Superficie externa $+q$: Como $r > r_b$, $V_3 = \frac{q}{4\pi\epsilon_0 r}$

$$V(r) = V_1 + V_2 + V_3 = \frac{q}{4\pi\epsilon_0 r} - \frac{q}{4\pi\epsilon_0 r} + \frac{q}{4\pi\epsilon_0 r} = \frac{q}{4\pi\epsilon_0 r}$$
Las contribuciones de las dos superficies inducidas ($-q$ y $+q$) se anulan perfectamente entre sí. No las ignoraste; su suma algebraica dio cero.

### 2. Para la región del conductor ($r_a < r \leq r_b$)

Evalúas considerando que estás **afuera** de la cavidad pero **adentro** de la superficie externa:

- Carga puntual $+q$: $V_1 = \frac{q}{4\pi\epsilon_0 r}$
    
- Superficie interna $-q$: Como $r > r_a$, $V_2 = \frac{-q}{4\pi\epsilon_0 r}$
    
- Superficie externa $+q$: Como **$r \leq r_b$**, estás adentro, es un valor constante. $V_3 = \frac{q}{4\pi\epsilon_0 r_b}$
    

$$V(r) = \frac{q}{4\pi\epsilon_0 r} - \frac{q}{4\pi\epsilon_0 r} + \frac{q}{4\pi\epsilon_0 r_b} = \frac{q}{4\pi\epsilon_0 r_b}$$

La carga puntual y la superficie interna se cancelan, dejando solo la constante de la superficie externa.

### 3. Para la cavidad interna ($0 < r \leq r_a$)

Evalúas considerando que estás **adentro** de los dos cascarones:

- Carga puntual $+q$: $V_1 = \frac{q}{4\pi\epsilon_0 r}$
- Superficie interna $-q$: Como **$r \leq r_a$**, es un valor constante. $V_2 = \frac{-q}{4\pi\epsilon_0 r_a}$
- Superficie externa $+q$: Como **$r \leq r_b$**, es un valor constante. $V_3 = \frac{q}{4\pi\epsilon_0 r_b}$
    

$$V(r) = \frac{q}{4\pi\epsilon_0 r} - \frac{q}{4\pi\epsilon_0 r_a} + \frac{q}{4\pi\epsilon_0 r_b}$$

Aquí ninguna se cancela, porque dependes de radios distintos.

### ¿Qué approach te recomiendo para un examen?

Te recomiendo enfáticamente mantener el enfoque de **Integración de Línea (Deltas de potencial)** que usaste en tu última resolución.

- **Pros de la Integración (tu método):** Es mecánicamente robusto, demuestra comprensión profunda de la física (el potencial como trabajo acumulado en el espacio) y te obliga a arrastrar la continuidad desde el infinito. Si tu función de campo eléctrico $\vec{E}$ está bien, integrar por partes casi garantiza que el potencial estará bien. Además, en la corrección de un parcial, muestra un procedimiento analítico claro.
    
- **Contras de la Superposición:** Es extremadamente rápido (un solo paso algebraico), pero propenso a errores letales de memoria. Si en medio del nerviosismo te confundes y pones una $r$ minúscula en lugar de la $R$ constante cuando estás evaluando el interior de un cascarón, el resultado de toda esa zona y las siguientes estará mal.
    

Usa la Integración para desarrollar el ejercicio en papel y usa la Superposición mentalmente como una prueba de escritorio rápida para verificar que tu resultado final tenga sentido físico.