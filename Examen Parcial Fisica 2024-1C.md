---
id: 20260524084133
aliases: []
tags:
  - uncataloged
created: 2026-05-24 08:41
status: draft
---
# Examen Parcial Fisica 2024-1C
## Ejercicio 1

Una partícula puntual de masa $m_{1}$ parte del reposo desde el extremo superior de un plano inclinado con rozamiento despreciable, como se indica en la figura. Al llegar a la parte más baja impacta sobre otra partícula de masa $m_{2}$ la que se encontraba en reposo. Como consecuencia del impacto, la masa $m_1$ queda detenida en ese lugar y la otra partícula comienza a moverse.
![Pasted image 20260524084345](assets/Pasted%20image%2020260524084345.png)

- **a)** ¿Con qué velocidad impacta la masa 1 a la masa 2?
    
- **b)** ¿Cuál es la velocidad de la partícula 2 después del impacto?
    
- **c)** ¿Cuál es la relación entre las energías cinéticas del sistema de partículas, antes y después del impacto? ¿Qué relación de masas debe darse para que el choque pueda ser considerado elástico?
    
- **d)** Si la relación $m_{2}/m_{1}$ es menor que 1, ¿puede ocurrir la situación descripta en el enunciado? Justifique.

### Resolución
#### Punto A
Para este punto, tenemos que considerar que durante el trayecto de la masa $m_{1}$, la energía mecánica de $m_{1}$ se conserva, debibo a que no existen fuerzas no conservativas realizando trabajo sobre el sistema. Por tanto, podemos igualar la energía mecánica inicial $E_{A}$ con la energía $E_{B}$ en el punto  en el que la masa $m_{1}$ impacta a $m_{2}$. Si usamos el piso con $U=0$ como referencia para la energía potencial, tenemos:
$$
\begin{align}
E_{A} &  = E_{B}  \\
K_{A} + U_{A} &  = K_{B} + U_{B} \\
m_{1}gy_{1_{A}}  & = \frac{1}{2}m_{1}v_{1_{B}}^2
\end{align}
$$
Despejamos $v_{1_{B}}$:
$$
\begin{align}
m_{1}gy_{1_{A}}  & = \frac{1}{2}m_{1}v_{1_{B}}^2 \\
v_{1} & = \sqrt{ 2gy_{1_{A}}} \\
v_{1} & = \sqrt{ 2gH}
\end{align}
$$
#### Punto B
Justo antes del impacto (Estado B) y justo después (Estado C), se conserva el momento lineal del sistema $m_{1} + m_{2}$. Por tanto, igualamos ambos momentos y despejamos.
$$
\begin{align}
\vec{p}_{B} &  = \vec{p}_{C} \\
m_{1}v_{1_{B}}  & = m_{2}v_{2_{C}} \\
v_{2_{C}}  & = \frac{m_{1}}{m_{2}}v_{1_{B}} \\
v_{2_{C}}  & = \frac{m_{1}}{m_{2}}\sqrt{ 2gH}
\end{align}
$$
#### Punto C
$$
\begin{align}
K_{B} & = \frac{1}{2}m_{1}v_{1_{B}}^2 = \frac{1}{2}m_{1}2gH \\
K_{B} & = m_{1}gH  \\
K_{C}  & = \frac{1}{2}m_{2}v_{2_{C}}^2 =  \frac{1}{2}m_{2}(\frac{m_{1}}{m_{2}})^22gH \\
K_{C}  & = \frac{m_{1}^2}{m_{2}}gH
\end{align}
$$
Por tanto, la relación entre las energías cinéticas viene dado por:
$$
\begin{align}
\frac{K_{C}}{K_{B}}  & = \frac{{ \frac{m_{1}^2}{m_{2}}gH}}{m_{1}gH} \\
\frac{K_{C}}{K_{B}}  & = \frac{m_{1}}{m_{2}}
\end{align}
$$
Para que el choque pueda considerarse elástico, la energía cinética inicial y final deben ser iguales. Entonces:
$$
\begin{align}
K_{B} & = K_{C} \\
m_{1}gH & =\frac{m_{1}^2}{m_{2}}gH \\
m_{1} & =\frac{m_{1}^2}{m_{2}} \\
m_{1} & = m_{2}
\end{align}
$$
Por tanto, se tiene que cumplir que las masas deben ser iguales para que el choque sea elástico.
#### Punto D
 $\frac{m_{2}}{m_{1}} < 1 \implies m_{1}> m_{2}$. 
 Si la masa $m_{1}$ es mayor que $m_{2}$, la situación descrita en el enunciado no puede suceder. La velocidad de $m_{2}$ después del impacto será mayor que la velocidad de $m_{1}$, afectando directamente a la relación de energías cinéticas obtenida: $\frac{K_{C}}{K_{B}}=\frac{m_{1}}{m_{2}}$. Es decir, la energía cinética final sería mayor a la inicial, sin una reducción en la energía potencial gravitatoria, lo cuál sería imposible en este caso dado que no existen fuentes de energía interna afectando la energía mecánica del sistema durante la colisión.
## Ejercicio 2
Un hilo muy largo se encuentra cargado con una densidad lineal de carga $\lambda$, uniformemente distribuida.
![Pasted image 20260524094359](assets/Pasted%20image%2020260524094359.png)

- **a)** Calcular el campo eléctrico que genera en todo el espacio.
    
- **b)** Se tiene una esfera abstracta (no material) de radio $R$ que rodea al hilo, como indica la figura. Calcular el flujo del campo eléctrico a través de la superficie de la esfera.
    
- **c)** Suponga ahora que el hilo se corta a una longitud $L=4R$, manteniendo la esfera matemática centrada en la mitad del hilo. ¿Se modifica el campo eléctrico en la superficie de la esfera, respecto del calculado en a)? ¿Se modifica el flujo del campo a través de la esfera, respecto del calculado en b? Justifique.
### Resolución
#### Punto A
Para calcular el campo eléctrico que produce el hilo muy largo, usaremos la ley de gauss, definiendo una superficie gaussiana cilíndrica concéntrica al hilo, de largo l y radio r. Dada la distribución de la carga $\lambda$ en el hilo, el campo eléctrico no tiene preferencia horizontal sobre la la superficie que definimos, teniendo una dirección radial en todo punto de la misma, de tal forma que $\vec{E}\cdot \hat{n} = E$. Este el caso para la superficie cilíndrica, en el caso de las "tapas" de la superficie, tenemos: $\vec{E} \cdot \hat{n} = 0$. Utilizamos esta simetría a nuestro favor para simplificar los cálculos del campo:
$$
\begin{align}
\Phi_{E}  & = \iint_{S} \vec{E} \cdot d \vec{S} \\
\Phi_{E}  & = \iint_{S} E \hat{r} \cdot dS \hat{r} = \iint_{S} EdS = E \iint_{S} dS \\
\Phi_{E}  & = E \times 2\pi r l = \frac{Q_{encl}}{\epsilon_{0}} \\
E  & = \frac{Q_{encl}}{\epsilon_{0} 2 \pi rl}
\end{align}
$$
Siendo que $Q_{encl} = \lambda \times l$, nos quedamos con que $E = \frac{\lambda}{\epsilon_{0} 2 \pi r}$  en todo el espacio. Finalmente:
$$
\begin{align}
\vec{E}(r) & = \frac{\lambda}{\epsilon_{0} 2 \pi r} \hat{r}
\end{align}
$$

#### Punto B
Para este punto, usamos una superficie gaussiana idéntica a la esfera abstracta descrita, con radio R. Para todo $dA$ de la esfera, acá no se cumple que $\vec{E} \cdot \hat{n}=E$, y tampoco que se cumple que la magnitud se mantiene constante. Por ejemplo, existen puntos de intersección entre el hilo y la esfera, donde $E \to \infty$, y otros puntos donde $\vec{E} \cdot \hat{n} \neq E$ dado que el ángulo $\theta$ no es 0. Para calcular el flujo, seguimos usando la ley de Gauss, pero esta vez trabajando directamente con la expresión $\frac{Q_{encl}}{\epsilon_{0}}$:
$$
\begin{align}
\Phi_{E}  & = \frac{Q_{encl}}{\epsilon_{0}} \\
\end{align}
$$
La pregunta que nos surge entonces es: ¿Cuál es la carga del hilo que encierra la esfera? Si consideramos las dos intersecciones que la superficie de la esfera tiene con el hilo, nos damos cuenta que ocurren en puntos a distancia R del centro de la esfera. Por tanto, la distancia total encerrada del hilo es 2R. Por tanto:
$$
\begin{align}
\Phi_{E} = \frac{\lambda \times 2R}{\epsilon_{0}}
\end{align}
$$
#### Punto C
El campo eléctrico cambia, el flujo eléctrico no:
- La ley de Coulomb expresa que el campo eléctrico generado por un diferencial de carga $dq$ decae con una relación $1/r^2$. La cantidad de carga de un lado o del otro de un punto depende de la longitud $l$ de ese segmento. Si consideramos un punto en la superficie de la esfera que no se encuentra en el plano medio del hilo, la distancia a los extremos es asimétrica. Debido a la fuerte dependencia con $1/r^2$, el campo eléctrico axial generado por el segmento más corto y cercano supera al del segmento más largo y lejano. Por lo tanto, las componentes axiales no se cancelan, modificando la dirección y magnitud del campo eléctrico respecto a la expresión obtenida en el **punto a**.
- Respecto al flujo eléctrico obtenido, la carga encerrada sigue siendo la misma, siendo determinada por la longitud del hilo que encierra la superficie. Por tanto, no se ve alterado.
## Ejercicio 3

Dos capacitores plano-paralelos tienen la misma superficie ($S=700\text{ mm}^{2}$) y la misma separación entre placas ($d=0,2\text{ mm}$). El capacitor $C_{1}$ tiene aire entre sus placas, mientras que el capacitor $C_{2}$ tiene un dieléctrico de permitividad relativa $\epsilon_{r}=3$ (recordar que la permitividad relativa modifica el valor de la permitividad del medio, llevando a $\epsilon=\epsilon_r \epsilon_0$).

- **a)** Calcular el valor de la capacidad de ambos capacitores.
- **b)** Los capacitores están conectados en paralelo a una batería ideal de $12\text{ V}$ como se muestra en la figura. ¿Cuál es el valor de las cargas libres que adquieren cada uno de los capacitores al conectarse a la batería?
- **c)** Si, una vez cargados, se desconecta la batería, ¿se modifica el valor de las cargas calculadas en b)? Justifique.
### Resolución
#### Punto A
#### Punto B
#### Punto C