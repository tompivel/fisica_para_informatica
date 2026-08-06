---
id: 20260423015033
aliases: []
tags:
  - physics_eng
created: 2026-04-23 01:50
status: draft
---
# Electric Charge and Electric Field Exercises
## Sears: 21.63
Four identical charges $Q$ are placed at the corners of a square of side $L$ .
(a) In a free-body diagram, show all of the forces that act on one of the charges. 
(b) Find the magnitude and direction of the total force exerted on one charge by the other three charges.

### Resolution
## Sears 21.64
![Pasted image 20260423015325](assets/Pasted%20image%2020260423015325.png)
### Resolution

## Sears 21.78
![Pasted image 20260423015556](assets/Pasted%20image%2020260423015556.png)

## Guía Práctica Electroestática 1.4
![Pasted image 20260423015850](assets/Pasted%20image%2020260423015850.png)
### Resolución
Asumiendo que $q_{0}$ tiene carga positiva:
Adoptamos como ejes x e y en las direcciones de las fuerzas por comodidad. Buscamos los valores $q_{1}$ y $q_{2}$ para que la fuerza electrica sobre la carga puntual $q_{0}$ sea 0.
Esto significa que para la carga puntual $q_{0}$ se debe cumplir:
$$
\begin{align}
\sum F_{x} & = 0 \\
\sum F_{y}  & = 0
\end{align}
$$
Ahora ampliamos la expresion con los valores de las fuerzas individuales sobre $q_{0}$:
$$
\begin{align}
\sum F_{x} & = F_{q_{2}} -F_{q_{3}} = 0 \rightarrow F_{q_{2}} = k \frac{|q_{3}q_{0}|}{r^2} \\
\sum F_{y}  & = F_{q_{1}} - F_{q_{4}} = 0 \rightarrow F_{q_{1}} = k \frac{|q_{4}q_{0}|}{r^2}
\end{align}
$$
Ahora, descomponemos los valores con la ley de coulomb. Sea $l$ el lado del cuadrado, tenemos que $r^2 = 2\left( \frac{l}{2} \right)^2 = \frac{l^2}{2}$:
$$
\begin{align}
F_{q_{1}} & = k\frac{|q_{1}q_{0}|}{r^2}  = k \frac{|q_{3}q_{0}|}{r^2} \rightarrow |q_1| = |q_{3}| = |-1nC| = 1nC\\ 
F_{q_{2}} & = k\frac{|q_{2}q_{0}|}{r^2} = k \frac{|q_{4}q_{0}|}{r^2} \rightarrow |q_{2}| = |q_{4}| = 2nC\\
\end{align}
$$
La respuesta es unica y no depende del lado del cuadrado o del signo o valor de $q_{0}$. Los valores para $q_{1}$ y $q_{2}$ son $-1nC$ y $2nC$ respectivamente.

## Guía Práctica Electroestática 1.5
![Pasted image 20260423015819](assets/Pasted%20image%2020260423015819.png)
### Resolucion punto a
Se nos pide calcular la fuerza electrica ejercida por una carga lineal de largo $L$ y de densidad lineal uniforme $\lambda$ en una carga puntual $q_{o}$.

Para empezar, asumimos que la carga $Q$ es positiva. Colocamos la carga sobre el eje y desde $y=0$ hasta $y=L$. La carga lineal $\lambda = \frac{Q}{L}$ y la carga en un segmento $dQ = \lambda dy  = \frac{Q}{L}dy$.

Colocamos nuestra carga puntual en un lugar arbitrario del espacio ($x_{0}, y_{o}$), de tal forma que las componentes del campo electrico paralelas a la carga no se cancelan. La distancia $r$ entre un segmento a la altura $y$ y la carga puntual es:
$$
r^2 = x_{0}^2 + (y-y_{0})^2 \rightarrow r = (x_{0}^2 + (y_{0}-y)^2)^{1/2}
$$
De esta forma, la magnitud del campo en la carga puntual dado el segmento a la altura $y$ es:
$$
\begin{align}
dE &  = \frac{1}{4\pi \epsilon_{0}} \frac{dQ}{r^2} = \frac{1}{4\pi \epsilon_{0}} \frac{Q}{L} \frac{dy}{x_{0}^2  + (y_{0}-y)^2}
\end{align}
$$
Tambien sabemos que las componentes de $dE$ son $dE_{x} = dE\cos \theta$ y $dE_{y} = dE \sin \theta$, donde $\cos \theta = \frac{x_{0}}{r}$ y $\sin \theta = \frac{y_{0}-y}{r}$. Entonces, tenemos que:
$$
\begin{align}
dE_{x} & = \frac{1}{4\pi \epsilon_{0}} \frac{Q}{L} \frac{x_{0}dy}{(x_{0}^2  + (y_{0}-y)^2)^{3/2}} \\
dE_{y} & = \frac{1}{4\pi \epsilon_{0}} \frac{Q}{L} \frac{(y_{0}-y)dy}{(x_{0}^2  + (y_{0}-y)^2)^{3/2}}
\end{align}
$$
Entonces, integrando por sobre todos los segmentos infinitesimales, tenemos:
$$
\begin{align}
E_{x}  & = \frac{1}{4\pi \epsilon_{0}}  \frac{Q}{L}x_{0} \int_{0}^{L} \frac{ dy}{(x_{0}^2  + (y_{0}-y)^2)^{3/2}} \\
E_{y} &  = \frac{1}{4\pi \epsilon_{0}}  \frac{Q}{L} \int_{0}^{L} \frac{(y_{0}-y)dy}{(x_{0}^2  + (y_{0}-y)^2)^{3/2}}
\end{align}
$$
#### Resolviendo $E_{x}$
Empecemos resolviendo $E_{x}$. Dejamos de lado las constantes por un momento. Planteamos la sustitucion $u = y-y_{0}$. Entonces $du = dy$. 
$$
\begin{align}
\int \frac{du}{(x_{0}^2  + u^2)^{3/2}}
\end{align}
$$
Luego,  planteamos que $\tan \theta = \frac{u}{x_{0}} \rightarrow u = \tan \theta x_{0}$ y $du = x_{0}\sec^2\theta d\theta$. Reemplazamos:
$$
\begin{align}
\int \frac{du}{(x_{0}^2  + u^2)^{3/2}} \rightarrow \int \frac{x_{0}\sec^2\theta d\theta}{(x_{0}^2  + x^2_{0}\tan^2 \theta)^{3/2}} \rightarrow \int \frac{x_{0}\sec^2\theta d\theta}{(x_{0}^2(1+\tan^2\theta))^{3/2}}
\end{align}
$$
Aplicando la regla trigonometrica $1+\tan^2 \theta= \sec^2 \theta$, tenemos:
$$
\begin{align}
\int \frac{x_{0}\sec^2\theta d\theta}{(x_{0}^2(1+\tan^2\theta))^{3/2}} \rightarrow \int \frac{x_{0}\sec^2\theta d\theta}{(x_{0}^2(\sec^2\theta))^{3/2}} \rightarrow \int \frac{x_{0}\sec^2\theta d\theta}{x_{0}^3\sec^3\theta} 
\end{align}
$$
Simplificando terminos, nos quedamos con:
$$
\begin{align}
\int \frac{x_{0}\sec^2\theta d\theta}{x_{0}^3\sec^3\theta} \rightarrow \frac{1}{x^2_{0}} \int \frac{d\theta}{\sec\theta} 
\end{align}
$$
Sabiendo que $\cos \theta = \frac{1}{\sec \theta}$, resolvemos la antiderivada:
$$
\begin{align}
\frac{1}{x^2_{0}} \int \frac{d\theta}{\sec\theta} \rightarrow \frac{1}{x^2_{0}} \int \cos \theta d\theta = \frac{1}{x_{0}^2}\sin \theta
\end{align}
$$
Reconstruyendo la expresion con u, sabemos que $\sin \theta = \frac{u}{(x_{0}^2 + u^2)^{1/2}}$. Entonces tenemos que:
$$
\begin{align}
\frac{1}{x_{0}^2}\sin \theta = \frac{u}{x_{0}^2 \sqrt{x_{0}^2 + u^2}}
\end{align}
$$
Y tambien tenemos que $u = y-y_{o}$, aplicando los limites de integracion originales, asi que nos quedamos con:
$$
\begin{align}
\int_{0}^{L} \frac{ dy}{(x_{0}^2  + (y_{0}-y)^2)^{3/2}} = \left. \frac{(y-y_{0})}{x_{0}^2 \sqrt{x_{0}^2 + (y-y_{0})^2}} \right|_{0}^L
\end{align}
$$

Evaluamos el limite superior y restamos el inferior:
$$
\begin{align}
\left. \frac{(y-y_{0})}{x_{0}^2 \sqrt{x_{0}^2 + (y-y_{0})^2}} \right|_{0}^L = \frac{(L-y_{0})}{x_{0}^2 \sqrt{x_{0}^2 + (L-y_{0})^2}} + \frac{y_{0}}{x_{0}^2 \sqrt{x_{0}^2 + y_{0}^2}}
\end{align}
$$

Uniendo este resultado con el resto de la expresion para $E_{x}$, tenemos:
$$
\begin{align}
E_{x}  & = \frac{1}{4\pi \epsilon_{0}}  \frac{Q}{L} \frac{1}{x_{0}} \left(\frac{L-y_{0}}{\sqrt{x_{0}^2 + (L-y_{0})^2}} + \frac{y_{0}}{\sqrt{x_{0}^2 + y_{0}^2}} \right)
\end{align}
$$

#### Resolviendo $E_{y}$
La integral que queremos resolver (quitando constantes) es:
$$
\begin{align}
\int_{0}^{L} \frac{(y_{0}-y)dy}{(x_{0}^2  + (y_{0}-y)^2)^{3/2}}
\end{align}
$$
Planteamos la sustitucion $w = (x_{0}^2  + (y_{0}-y)^2$, de tal forma que $dw = 2(y_{0}-y)(-1)dy = -2(y_{0}-y)dy$. Sustituyendo esto en la antiderivada, tenemos:
$$
\begin{align}
\int \frac{(y_{0}-y)dy}{(x_{0}^2  + (y_{0}-y)^2)^{3/2}} \rightarrow \frac{1}{-2}\int \frac{dw}{w^{3/2}} = \frac{1}{-2}\int w^{-3/2}dw 
\end{align}
$$
Resolviendo la antiderivada, tenemos
$$
\begin{align}
\frac{1}{-2}\int w^{-3/2}dw = \frac{1}{-2}\left(-2w^{-1/2} \right) = w^{-1/2}
\end{align}
$$
Reemplazando con nuestra expresion original $w = (x_{0}^2  + (y_{0}-y)^2$ y evaluando en los limites de integracion, tenemos:
$$
\begin{align}
\left. \frac{1}{\sqrt{ x_{0}^2  + (y_{0}-y)^2 }} \right|_{0}^L = \frac{1}{\sqrt{ x_{0}^2  + (y_{0}-L)^2 }} - \frac{1}{\sqrt{ x_{0}^2  + y_{0}^2 }}
\end{align}
$$
Uniendo este resultado con el resto de la expresion para $E_{y}$, tenemos:
$$
\begin{align}
E_{y} &  = \frac{1}{4\pi \epsilon_{0}}  \frac{Q}{L} \left(\frac{1}{\sqrt{ x_{0}^2  + (y_{0}-L)^2 }} - \frac{1}{\sqrt{ x_{0}^2  + y_{0}^2 }}\right)
\end{align}
$$

Finalmente, sabiendo que $F =  Eq_{0}$, tenemos que:
$$
\begin{align}
F_{x}  & =  \frac{1}{4\pi \epsilon_{0}}  \frac{Q}{L} \frac{q_{0}}{x_{0}} \left(\frac{L-y_{0}}{\sqrt{x_{0}^2 + (L-y_{0})^2}} + \frac{y_{0}}{\sqrt{x_{0}^2 + y_{0}^2}} \right)\\
F_{y}  & = \frac{q_{0}}{4\pi \epsilon_{0}}  \frac{Q}{L} \left(\frac{1}{\sqrt{ x_{0}^2  + (y_{0}-L)^2 }} - \frac{1}{\sqrt{ x_{0}^2  + y_{0}^2 }}\right)
\end{align}
$$
### Resolucion punto b
Como estamos en el plano mediatriz, $y_{0} = \frac{L}{2}$. Los valores de $x_{0}$ seran 2m, 0.1m y 0.05m.
La expresion cuando nos encontramos en el plano mediatriz viene dada por:
$$
\begin{align}
F_{x}  & =  \frac{1}{4\pi \epsilon_{0}}  \frac{Q}{L} \frac{q_{0}}{x_{0}} \left(\frac{\frac{L}{2}}{\sqrt{x_{0}^2 + \frac{L^2}{4}} } + \frac{\frac{L}{2}}{\sqrt{x_{0}^2 + \frac{L^2}{4}}} \right) = \frac{1}{4\pi \epsilon_{0}}  Q \frac{q_{0}}{x_{0}} \left(\frac{1}{\sqrt{x_{0}^2 + \frac{L^2}{4}} } \right)\\
F_{y}  & = \frac{q_{0}}{4\pi \epsilon_{0}}  \frac{Q}{L} \left(\frac{1}{\sqrt{ x_{0}^2  + (y_{0}-L)^2 }} - \frac{1}{\sqrt{ x_{0}^2  + y_{0}^2 }}\right) = 0
\end{align}
$$

#### Caso 2m
$$
\begin{align}
F_{x}  &  = \frac{1}{4\pi \epsilon_{0}}  Q \frac{q_{0}}{2m} \left(\frac{1}{\sqrt{4m^2 + \frac{L^2}{4}} } \right)\\
F_{y}  & = 0
\end{align}
$$
Resolviendo con $\lambda L = Q$, $F_{x}= 16745q_{0}N$
#### Caso 0.1m
$$
\begin{align}
F_{x}  &  = \frac{1}{4\pi \epsilon_{0}}  Q \frac{q_{0}}{0.1m} \left(\frac{1}{\sqrt{0.01m^2 + \frac{L^2}{4}} } \right)\\
F_{y}  & = 0
\end{align}
$$
Resolviendo con $\lambda L = Q$, $F_{x}= 2506887q_{0}N$
#### Caso 0.05m
$$
\begin{align}
F_{x}  &  = \frac{1}{4\pi \epsilon_{0}}  Q \frac{q_{0}}{0.05m} \left(\frac{1}{\sqrt{2.5\times 10^{-3}m^2 + \frac{L^2}{4}} } \right)\\
F_{y}  & = 0
\end{align}
$$
Resolviendo con $\lambda L = Q$, $F_{x}= 5295135q_{0}N$

Se puede observar, como a medida que la distancia disminuye en el eje x, la componente de la fuerza electrica en este eje se hace mas grande gracias al factor $\frac{1}{x_{0}}$. El valor $x_{0}^2$ empieza a hacerse despreciable comparado con $y_{0}^2$. Sin embargo, no hace diferencia en el eje y.
### Resolucion punto c
Como estamos en el plano mediatriz, $y_{0} = \frac{L}{2}$. Los valores de $x_{0}$ seran 2m, 0.1m y 0.05m.
La expresion cuando nos encontramos en el plano mediatriz viene dada por:
$$
\begin{align}
F_{x}  & =  \frac{1}{4\pi \epsilon_{0}}  \frac{Q}{L} \frac{q_{0}}{x_{0}} \left(\frac{\frac{L}{2}}{\sqrt{x_{0}^2 + \frac{L^2}{4}} } + \frac{\frac{L}{2}}{\sqrt{x_{0}^2 + \frac{L^2}{4}}} \right) = \frac{1}{4\pi \epsilon_{0}}  Q \frac{q_{0}}{x_{0}} \left(\frac{1}{\sqrt{x_{0}^2 + \frac{L^2}{4}} } \right)\\
F_{y}  & = \frac{q_{0}}{4\pi \epsilon_{0}}  \frac{Q}{L} \left(\frac{1}{\sqrt{ x_{0}^2  + (y_{0}-L)^2 }} - \frac{1}{\sqrt{ x_{0}^2  + y_{0}^2 }}\right) = 0
\end{align}
$$
Pero ahora se nos pide evaluar estas expresiones en el limite cuando L tiende a infinito.
$$
\begin{align}
\lim_{ L \to \infty } F_{x}  & =  \lim_{ L \to \infty }  \frac{1}{4\pi \epsilon_{0}}  \lambda \frac{q_{0}}{x_{0}} \left(\frac{L}{\sqrt{x_{0}^2 + \frac{L^2}{4}} } \right) \\
\lim_{ L \to \infty } F_{y}  & = \frac{q_{0}}{4\pi \epsilon_{0}}  \frac{Q}{L} \left(\frac{1}{\sqrt{ x_{0}^2  + \left( \frac{L}{2}-L \right)^2 }} - \frac{1}{\sqrt{ x_{0}^2  + \frac{L}{2}^2 }}\right) = 0
\end{align}
$$
Enfocandonos en el limite para $F_{x}$, intentamos sacar factor comun en el denominador:
$$
\begin{align}
\lim_{ L \to \infty } F_{x}  & =  \frac{1}{4\pi \epsilon_{0}}  \lambda \frac{q_{0}}{x_{0}} \lim_{ L \to \infty }  \left(\frac{L}{\sqrt{\frac{L^2}{4}\left(  \frac{{4x_{0}^2}}{L^2} + 1 \right)} } \right)  \\
 & =   \frac{1}{4\pi \epsilon_{0}}  \lambda \frac{q_{0}}{x_{0}} \lim_{ L \to \infty }  \left(\frac{2}{\sqrt{\left(  \frac{{4x_{0}^2}}{L^2} + 1 \right)} } \right)  = \frac{2}{4\pi \epsilon_{0}}  \lambda \frac{q_{0}}{x_{0}} \\
\end{align}
$$
Por tanto, nuestra expresion para la fuerza electrica en un punto de campo en el plano mediatriz de una linea infinita de carga es:
$$
\begin{align}
F_{x}  & = \frac{2}{4\pi \epsilon_{0}}  \lambda \frac{q_{0}}{x_{0}} \\
F_{y}  & = 0
\end{align}
$$
Para los casos 2m, 0.1m y 0.05m, tenemos:
- $F_{x} = 135000q_{0}$ para 2m
- $F_{x} = 2700000q_{0}$ para 0.1m
- $F_{x} = 5400000q_{0}$ para 0.05m
### Resolucion punto d
comparamos las diferencias porcentuales
- Para 0.05m: $\frac{F_{xc}-F_{xb}}{Fxc}\times 100 = 1.94\%$
- Para 0.1m: $\frac{F_{xc}-F_{xb}}{Fxc}\times 100 = 7.15\%$
- Para 2m: $\frac{F_{xc}-F_{xb}}{Fxc}\times 100 = 87.6\%$
Podemos concluir que cuando $L\gg x$, es aproximadamente equivalente a la realidad tratar la carga como si estuviera distribuida infinitamente.
## Guía Práctica Electroestática 1.6
![Pasted image 20260423015609](assets/Pasted%20image%2020260423015609.png)
### Resolucion punto a
Para analizar el campo electrico sobre todo punto sobre el eje x, utilizamos la superposicion de campos: $\vec{E_{1} + \vec{E_{2}} = \vec{E}}$.
Podemos observar a simple vista que la direccion de $\vec{E}$ sera paralela al eje x y por tanto tendra una componente sobre el eje y nula. Es decir $\vec{E} = k \hat{i}$.
Entonces, calculamos las magnitudes de las componentes individuales de cada carga en un punto de campo arbitrario sobre el eje x:
$$
\begin{align}
E_{1} &  = \frac{1}{4\pi \epsilon_{0}} \frac{q}{r_{1}^2}\\
 E_{2}  & = \frac{1}{4\pi \epsilon_{0}} \frac{q}{r_{2}^2}
\end{align}
$$
Las direcciones en todos los casos son en contra de la carga positiva y a hacia la carga negativa. Asumiendo carga positiva el punto de prueba, los signos varian dependiendo de la posicion del punto, analicemos los casos:
##### $x < \frac{-d}{2}$
$$
\begin{align}
\vec{E} = -E_{1}\hat{i}  + E_{2} \hat{i}
\end{align}
$$
Dado que r es mayor para $E_{2}$ en este caso, $\vec{E}$ terminara apuntando hacia la izquierda.
##### $\frac{-d}{2} < x < \frac{d}{2}$
$$
\begin{align}
\vec{E} = +E_{1}\hat{i}  + E_{2} \hat{i}
\end{align}
$$
Dado que ambas componentes apuntan hacia la derecha  en este caso, $\vec{E}$ terminara apuntando hacia la derecha.
##### $\frac{d}{2} < x$
$$
\begin{align}
\vec{E} = E_{1}\hat{i}  - E_{2} \hat{i}
\end{align}
$$
Dado que r es mayor para $E_{1}$ en este caso, $\vec{E}$ terminara apuntando hacia la izquierda.

Por tanto, si, el sentido de $\vec{E}$ varia sobre el eje.

### Resolucion punto b
En eje y, la componente del campo electrico tambien es nula por simetria. La componente en el eje x siempre apunta hacia la derecha. Es decir, tenemos $\vec{E} = E_{x}\hat{i}$, donde:
$$
\begin{align}
E_{1x} = E_{2x} = E_{1}\cos \theta = \frac{1}{4\pi \epsilon_{0}} \frac{|q|}{r_{1}^2} \cos \theta
\end{align}
$$
Por tanto, $\vec{E}$ es:
$$
\begin{align}
\vec{E} = 2(\frac{1}{4\pi \epsilon_{0}} \frac{|q|\cos \theta}{r_{1}^2})\hat{i}
\end{align}
$$

	