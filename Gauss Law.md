---
id: 20260423163403
aliases: []
tags:
  - "#physics_eng"
created: 2026-04-23 16:34
status: draft
---
# Gauss Law
## Guia electroestatica 2.1
![Pasted image 20260424194004](assets/Pasted%20image%2020260424194004.png)
### Resolucion
Segun la ley de gauss, el flujo electrico sobre una superficie gaussiana es igual a:
$$
\begin{align}
\int {E_{\perp}}dA = \frac{Q_{encl}}{\epsilon_{0}}
\end{align}
$$
Entonces, para saber el flujo, no es necesario que calculemos la integral, pues podemos hacer $\frac{Q_{encl}}{\epsilon_{0}} = \frac{q}{\epsilon_{0}}$. Esta operación es igual a:
$$
\begin{align}
\phi_{E} = \frac{1\times 10^{-6} C}{8.9 \times 10^{-12} \frac{C^2}{N*m^2} } = 112359  \frac{N*m^2}{C}
\end{align}
$$

La cantidad no cambia al cambiar la superficie gaussiana, el flujo electrico no depende de la forma de la superficie elegida. 

## Guia electroestatica 2.2
![Pasted image 20260424194038](assets/Pasted%20image%2020260424194038.png)
### Resolucion
Dado que el campo electrico varia respecto a la coordenada, la distribucion de carga no es uniforme. Vamos a obtener el flujo electrico calculando el flujo por cada cara del cubo y luego sumaremos todos los resultados para obtener el flujo total en la superficie.
$$
\begin{align}
\phi_{total} = \phi_{top} + \phi_{bottom} + \phi_{right} + \phi_{left} + \phi_{front} + \phi_{back}
\end{align}
$$

Para calcular cada integral, necesitamos saber la orientación de $d \vec{A}$ en cada cara:
- Top (y=a): $d \vec{A} = dA\hat{j}$
- Bottom (y=0):  $d \vec{A} = -dA\hat{j}$
- Right (x=a): $d \vec{A} = dA\hat{i}$
- Left (x=0):  $d \vec{A} = -dA\hat{i}$
- Back (z=a):  $d \vec{A} = dA\hat{k}$
- Front (z=0):  $d \vec{A} = -dA\hat{k}$
#### Punto a)
Tenemos que $\vec{E} = E_{0}\hat{i}$. Dado que en la integral se usa producto punto, podemos descartar los flujos en top, bottom, back y front dado que forman un angulo de 180 grados con $d  \vec{A}$
$$
\begin{align}
\phi_{top} = \phi_{bottom} = \phi_{back} = \phi_{front} = 0
\end{align}
$$
Calculamos la integral para right y left:
$$
\begin{align}
\phi_{right}  & = \int \vec{E} \cdot d \vec{A} = \int E_{0} \hat{ i} \cdot dA \hat{i} = \int E_{0}dA \\
 & = E_{0} \int dA  = E_{0}A = E_{0}a^2
\end{align}
$$
Los resultados son similares para left, solo que cambia el signo:
$$
\begin{align}
\phi_{right}  & = \int \vec{E} \cdot d \vec{A} = \int E_{0} \hat{ i} \cdot -dA \hat{i} = \int -E_{0}dA \\
 & = -E_{0} \int dA  = -E_{0}A = -E_{0}a^2
\end{align}
$$
Por tanto, el flujo electrico total es:
$$
\begin{align}
\phi_{total} &  = \phi_{top} + \phi_{bottom} + \phi_{right} + \phi_{left} + \phi_{front} + \phi_{back} \\
 & =0 + 0 +E_{0}a^2 - E_{0}a^2 +0 +0 =0
\end{align}
$$
Este resultado hace sentido considerando que el flujo electrico entra por la cara izquierda y sale por la cara derecha.

Para obtener la carga total encerrada, usamos la ley de gauss:
$$
$$
$$
\begin{align}
\phi_{total}  & = \int {E_{\perp}}dA = \frac{Q_{encl}}{\epsilon_{0}} \\
Q_{encl}  & = \phi_{total} \epsilon_{0} = 0
\end{align}
$$
Para obtener la densidad de carga, usamos la forma diferencial de carga de la ley de gauss:
$$
\begin{align}
\nabla \cdot \mathbf{E} &  = \frac{\rho}{\epsilon_0} \\
\rho  & = \left( \frac{\partial E_{x}}{\partial x} + \frac{\partial E_{y}}{\partial y}  + \frac{\partial E_{z}}{\partial z}  \right) \epsilon_{0}
\end{align}
$$
En este caso, $\rho =0$, y hace sentido, dado que si no hay carga encapsulada, entonces la densidad de carga deberia ser 0.

#### Punto b)
Tenemos que $\vec{E} = \frac{E_{0}x}{a}\hat{i}$. Dado que en la integral se usa producto punto, podemos descartar los flujos en top, bottom, back y front dado que forman un angulo de 90 grados con $d  \vec{A}$
$$
\begin{align}
\phi_{top} = \phi_{bottom} = \phi_{back} = \phi_{front} = 0
\end{align}
$$
Calculamos la integral para right y left:
$$
\begin{align}
\phi_{right}  & = \int \vec{E} \cdot d \vec{A} = \int \frac{E_{0}x}{a}\hat{i} \cdot dA \hat{i} = \int \frac{E_{0}x}{a}dA \\
 & = \frac{E_{0}x}{a} \int dA  = \frac{E_{0}x}{a}A = E_{0}xa
\end{align}
$$
Los resultados son similares para left, solo que cambia el signo:
$$
\begin{align}
\phi_{left}  & = \int \vec{E} \cdot d \vec{A} = \int \frac{E_{0}x}{a}\hat{i} \cdot -dA \hat{i} = \int -\frac{E_{0}x}{a}dA \\
 & = -\frac{E_{0}x}{a} \int dA  = -\frac{E_{0}x}{a}A = -E_{0}xa
\end{align}
$$
Sabemos, ademas, que $x=0$ para la cara izquierda y $x=a$ para la cara derecha, asi que el flujo electrico total es:
$$
\begin{align}
\phi_{total} &  = \phi_{top} + \phi_{bottom} + \phi_{right} + \phi_{left} + \phi_{front} + \phi_{back} \\
 & =0 + 0 +E_{0}a^2 - E_{0}0 +0 +0 =E_{0}a^2
\end{align}
$$
Para obtener la carga total encerrada, usamos la ley de gauss:
$$
\begin{align}
\phi_{total}  & = \int {E_{\perp}}dA = \frac{Q_{encl}}{\epsilon_{0}} \\
Q_{encl}  & = \phi_{total} \epsilon_{0} = E_{0}a^2\epsilon_{0}
\end{align}
$$
Para obtener la densidad de carga, usamos la forma diferencial de carga de la ley de gauss:
$$
\begin{align}
\nabla \cdot \mathbf{E} &  = \frac{\rho}{\epsilon_0} \\
\rho  & = \left( \frac{\partial E_{x}}{\partial x} + \frac{\partial E_{y}}{\partial y}  + \frac{\partial E_{z}}{\partial z}  \right) \epsilon_{0} \\
 & = \frac{E_{0}}{a} \epsilon_{0}
\end{align}
$$

#### Punto c)
Tenemos que $\vec{E} = \frac{E_{0}x^2}{a^2}\hat{i}$. Dado que en la integral se usa producto punto, podemos descartar los flujos en top, bottom, back y front dado que forman un angulo de 90 grados con $d  \vec{A}$
$$
\begin{align}
\phi_{top} = \phi_{bottom} = \phi_{back} = \phi_{front} = 0
\end{align}
$$
Calculamos la integral para right y left. Para la cara derecha, tenemos que $x=a$ y por tanto $\vec{E}(a)=\frac{E_{0}a^2}{a^2}\hat{i} = E_{0}\hat{i}$
$$
\begin{align}
\phi_{right}  & = \int \vec{E} \cdot d \vec{A} = \int E_{0}\hat{i} \cdot dA \hat{i} = \int E_{0}dA \\
 & = E_{0}\int dA  = E_{0}A = E_{0}a^2
\end{align}
$$
Para la cara izquierda, tenemos que $x=0$, por tanto $\vec{E}(0) = \frac{E_{0} \times 0}{a^2} \hat{ i} =0 \hat{ i}$.
$$
\begin{align}
\phi_{left}  & = \int \vec{E} \cdot d \vec{A} = 0
\end{align}
$$
El flujo electrico total es:
$$
\begin{align}
\phi_{total} &  = \phi_{top} + \phi_{bottom} + \phi_{right} + \phi_{left} + \phi_{front} + \phi_{back} \\
 & =0 + 0 +E_{0}a^2 + 0 +0 +0 =E_{0}a^2
\end{align}
$$
Para obtener la carga total encerrada, usamos la ley de gauss:
$$
\begin{align}
\phi_{total}  & = \int {E_{\perp}}dA = \frac{Q_{encl}}{\epsilon_{0}} \\
Q_{encl}  & = \phi_{total} \epsilon_{0} = E_{0}a^2\epsilon_{0}
\end{align}
$$
Para obtener la densidad de carga, usamos la forma diferencial de carga de la ley de gauss:
$$
\begin{align}
\nabla \cdot \mathbf{E} &  = \frac{\rho}{\epsilon_0} \\
\rho  & = \left( \frac{\partial E_{x}}{\partial x} + \frac{\partial E_{y}}{\partial y}  + \frac{\partial E_{z}}{\partial z}  \right) \epsilon_{0} \\
 & = 2\frac{E_{0}x}{a} \epsilon_{0}
\end{align}
$$

#### Punto D
Tenemos que $\vec{E} = \frac{E_{0}}{a}(y\hat{i} + x\hat{j})$. 
Calculamos la integral para top y bottom. Para la cara superior, tenemos $y=a$ y para la cara inferior tenemos $y=0$. Por tanto $\vec{E} = \frac{E_{0}}{a}(a \hat{i} + x \hat{j}) = E_{0} \hat{i} + \frac{E_{0}x}{a} \hat{j}$ para la cara superior. Teniendo en cuenta que en este caso $dA = dxdz$, integramos:
$$
\begin{align}
\phi_{top}  & = \int \vec{E} \cdot d \vec{A} = \int \left( E_{0} \hat{i} + \frac{E_{0}x}{a} \hat{j} \right) \cdot dA \hat{j} = \int \frac{E_{0}x}{a}dA \\
 & = \int_{0}^a \int_{0}^a \frac{E_{0}x}{a}dxdz = \frac{E_{0}}{a} \int_{0}^a \int_{0}^a xdxdz \\
  & =  \frac{E_{0}}{a}\frac{a^2}{2}\int_{0}^a dz = \frac{E_{0}}{a}\frac{a^2}{2}a = \frac{E_{0}a^2}{2}
\end{align}
$$

Para la cara inferior, $\vec{E} = \frac{E_{0}}{a}(0 \hat{i} + x \hat{j}) =  \frac{E_{0}x}{a} \hat{j}$ . Entonces:
$$
\begin{align}
\phi_{bottom}  & = \int \vec{E} \cdot d \vec{A} = \int \left( \frac{E_{0}x}{a} \hat{j} \right) \cdot -dA \hat{j} = -\int \frac{E_{0}x}{a}dA\\ \\
 & = -\frac{E_{0}a^2}{2}
\end{align}
$$
Ahora calculamos la integral para front y back. Para la cara del frente tenemos que $z=0$ y para la cara trasera tenemos que $z=a$. Por tanto, para la ambas caras tenemos que $\vec{E} = \frac{E_{0}}{a}(y\hat{i} + x \hat{j}) = \frac{E_{0}y}{a} \hat{i} + \frac{E_{0}x}{a} \hat{j}$. Teniendo en cuenta que en este caso $dA = dxdy$, calculemos la integral de superficie:
$$
\begin{align}
\phi_{front}  & = \int \vec{E} \cdot d \vec{A} = \int \left( \frac{E_{0}y}{a} \hat{i} + \frac{E_{0}x}{a} \hat{j} \right) \cdot dA \hat{k} = \int 0dA = 0 \\
\end{align}
$$
Para la cara trasera, tenemos:
$$
\begin{align}
\phi_{back}  & = \int \vec{E} \cdot d \vec{A} = \int \left( \frac{E_{0}y}{a} \hat{i} + \frac{E_{0}x}{a} \hat{j} \right) \cdot -dA \hat{k} = \int 0dA = 0 \\
\end{align}
$$
Calculamos la integral para right y left. Para la cara derecha, tenemos que $x=a$, por tanto $\vec{E} = \frac{E_{0}}{a}y \hat{i} + E_{0} \hat{j}$. Teniendo en cuenta que en este caso $dA=dydz$, calculamos la integral de superficie:
$$
\begin{align}
\phi_{right}  & = \int \vec{E} \cdot d \vec{A} = \int \left( \frac{E_{0}}{a}y \hat{i} + E_{0} \hat{j} \right)\cdot dA\hat{i}= \int \frac{E_{0}y}{a}dA \\
& = \int_{0}^a \int_{0}^a \frac{E_{0}y}{a}dydz = \frac{E_{0}}{a} \int_{0}^a \int_{0}^a ydydz \\
  & =  \frac{E_{0}}{a}\frac{a^2}{2}\int_{0}^a dz = \frac{E_{0}}{a}\frac{a^2}{2}a = \frac{E_{0}a^2}{2}
\end{align}
$$
Para la cara izquierda, tenemos que $x=0$, por tanto $\vec{E} = \frac{E_{0}}{a}y \hat{i}$.
$$
\begin{align}
\phi_{left}  & = \int \vec{E} \cdot d \vec{A} = \int \left( \frac{E_{0}}{a}y \hat{i} \right)\cdot -dA\hat{i}= -\int \frac{E_{0}y}{a}dA \\
 & = - \phi_{right} = -\frac{E_{0}a^2}{2}
\end{align}
$$
El flujo electrico total es:
$$
\begin{align}
\phi_{total} &  = \phi_{top} + \phi_{bottom} + \phi_{right} + \phi_{left} + \phi_{front} + \phi_{back} \\
 & = \frac{E_{0}a^2}{2}  -\frac{E_{0}a^2}{2} +  \frac{E_{0}a^2}{2} -  \frac{E_{0}a^2}{2}  +0 +0=0
\end{align}
$$
Dado que el flujo electrico es nulo, la carga total encerrada tambien sera cero, confirmemoslo usando la ley de gauss:
$$
\begin{align}
\phi_{total}  & = \int {E_{\perp}}dA = \frac{Q_{encl}}{\epsilon_{0}} \\
Q_{encl}  & = \phi_{total} \epsilon_{0} = 0\epsilon_{0} =0
\end{align}
$$
Para obtener la densidad de carga, usamos la forma diferencial de carga de la ley de gauss:
$$
\begin{align}
\nabla \cdot \mathbf{E} &  = \frac{\rho}{\epsilon_0} \\
\rho  & = \left( \frac{\partial E_{x}}{\partial x} + \frac{\partial E_{y}}{\partial y}  + \frac{\partial E_{z}}{\partial z}  \right) \epsilon_{0} \\
 & = 0  \epsilon_{0} =0
\end{align}
$$

## Guia electroestatica 2.3
![Pasted image 20260425034445](assets/Pasted%20image%2020260425034445.png)
### Resolucion
Asumiendo que la superficie descrita (el hemisferio) es una superficie abierta (sin la tapa circular plana del hemisferio), planteamos lo siguiente: Si añadimos la tapa circular plana al hemisferio para convertirla en una superficie cerrada, hemos creado una superficie sin carga interior, y por tanto el flujo electrico total de esta superficie sera 0. Podemos descomponer este flujo total como la suma de los flujos de las caras individuales del hemisferio cerrado (la curva y la cara plana)
$$
\begin{align}
\phi_{total} = \phi_{curva} + \phi_{plana} = 0
\end{align}
$$
Por tanto,
$$
\begin{align}
\phi_{curva} = - \phi_{plana}
\end{align}
$$
Esto hace sentido con lo que propone la ley de Gauss. En una superficie cerrada sin carga interior, el flujo electrico que entra termina tambien saliendo, cancelandose a si mismo. Por tanto, si el hemisferio fuera cerrado, todo el flujo que entra por la cara curva, termina saliendo por la cara plana. Resulta mucho mas facil calcular el flujo sobre la cara plana, puesto que representa un problema en 2d (calcular el flujo sobre la cara curva hubiera representando un problema en 3d).

Sabemos que la cara plana contiene un radio R y que el campo electrico es uniforme por sobre toda la superficie, mantiendo una direccion paralela al eje del hemisferio. Por tanto, si decidimos poner nuestro eje x justo sobre el eje del hemisferio, tenemos que $\vec{E} = E \hat{i}$. Ademas, sabemos que en cada punto de la cara plana del hemisferio, $d \hat{A} = -dA \hat{i}$. Dado esto, podemos calcular la integral:
$$
\begin{align}
\phi_{plana} &  = \int \vec{E} \cdot d \vec{A} = \int E \hat{i} \cdot -dA \hat{i} \\
 & = -EA
\end{align}
$$
Siendo el area de la cara plana igual a $\pi R^2$. Entonces $-EA = -E\pi R^2$.
Entonces sigue que el flujo que atraviesa la cara curva del hemisferio es $- (-E\pi R^2) = E\pi R^2$.

## Guia electroestatica 2.4
![Pasted image 20260425041608](assets/Pasted%20image%2020260425041608.png)
### Resolucion
#### punto a
Se sabe que una distribucion lineal infinita de carga con densidad lineal uniforme $\lambda$ distribuye un campo electrico radial hacia afuera (si la densidad es positiva). Usando coordenadas cilindricas, podemos argumentar que por la simetria de traslacion, el campo no depende de la coordenada z, y por la simetria cilindrica, el campo no depende del angulo $\theta$. El campo electrico en algun punto del espacio solo termina dependiendo de la distancia $r$  del cable. Por tanto, las caracteristicas de simetria en el campo electrico generado sugiere que hagamos uso de una superficie gaussiana cilindrica, de radio r y longitud l, coaxial con la carga y con sus extremos perpendiculares a la carga.

Usando la superposicion de campos electricos, podemos describir el campo electrico total sobre la superficie gaussiana como la suma del campo electrico sobre los extremos y sobre la superficie cilindrica. En ambos extremos del cilindro, tenemos que el flujo electrico es 0, dado que $\vec{E}\cdot \vec{n} = 0$. En cambio, en la parte cilindrica, tenemos lo contrario: $\vec{E} \cdot \vec{n} = E = E_{\perp}.$  El area de la cara cilindrica de la superficie es $2\pi rl$. Por tanto, el flujo electrico total de la superficie es $E 2\pi rl$. Entonces, aplicando la ley de gauss, tenemos:
$$
\begin{align}
\phi_{E} &  = 2E\pi rl = \frac{Q_{encl}}{\epsilon_{0}} \\
 E  & = \frac{Q_{encl}}{2\pi\epsilon_{0}rl}
\end{align}
$$
Ademas, tenemos que $Q_{encl} = \lambda l$. Por tanto, sustituyendo, tenemos:
$$
\begin{align}
E=\frac{\lambda}{2\pi \epsilon_{0}r}\hat{r} \end{align} $$ Si la densidad de lineal no fuera uniforme, las componentes verticales no se cancelarian en cada punto, y por tanto la integral del flujo electrico no se podria simplificar, dado que el campo electrico variaria dependiendo de la posicion.  
#### punto b
Tenemos una distribucion plana infinita de carga con densidad superficial uniforme $\sigma$. Usando un sistema de coordenadas cartesiano, podemos describir facilmente las caracteristicas de simetria del campo electrico generado. En cualquier punto del espacio, por simetria en el eje x e y, el campo no depende de estas coordenadas. Dadas estas caracteristicas, usaremos una superficie gaussiana cilindrica de longitud l y radio r, con sus extremos paralelos al plano, atravesada por su punto medio por el plano de carga.

Usando la superposicion de campos electricos, podemos describir el campo electrico total sobre la superficie gaussiana como la suma del campo electrico sobre los extremos y sobre la superficie cilindrica. En la cara cilindrica de la superficie tenemos que $\vec{E} \cdot \vec{n}=0$, dado que el angulo entre el vector normal a la superficie y el campo electrico es de 90 grados. Sin embargo, para los extremos del cilindro, se da el caso contrario, el angulo es de 0 grados en todos los puntos del mismo, por tanto $\vec{E} \cdot \vec{n} = E$. El area de cada cara es $\pi r^2$, y por tanto el flujo electrico total en la superficie gaussiana termina siendo: $$ \begin{align} \phi_{E} =  2E\pi r^2 =\frac{Q_{encl}}{\epsilon_{0}} \end{align} $$ Sabemos que la densidad superficial uniforme viene dada por $\sigma= \frac{Q_{encl}}{A}= \frac{Q_{encl}}{\pi r^2}$. Entonces tenemos: $$ \begin{align} E =\frac{\sigma}{2\epsilon_{0}} \end{align} $$ 

Podemos obsevar como el campo electrico generado no depende de ninguna coordenada. Sin embargo, este resultado es altamente dependiente de la uniformidad de la densidad superficial, dado que si la reparticion de carga no fuera uniforme, no habria simetria en los ejes x e y, y por tanto la integral no se podria simplicar dado que el campo electrico variaria en direccion por cada punto de la superficie gaussiana.

#### punto c
Tenemos una distribucion esferica con densidad volumetrica de carga uniforme $\rho$. Usando coordenadas esfericas, podemos denotar la simetria de la esfera en el angulo polar $\theta$ y el azimutal $\alpha$. El campo electrico generado entonces sera radial, dirigido estricamente en la coordenada $r$. Teniendo esto en cuenta, usaremos una superficie gaussiana esferica con radio r que englobe la distribucion, compartiendo origen en el sistema de coordenadas. Distingamos el radio R de la esfera vs el radio r de la superficie gaussiana.

**Para el caso en el que $R>r$, tenemos:**
Podemos asegurar que en cada punto de la superficie gaussiana, el vector normal a la superficie sera paralelo al del campo vectorial en ese punto, dando lugar a la nocion de que el flujo electrico es:
$$
\begin{align}
\phi_{E} = 4\pi r^2E = \frac{Q_{encl}}{\epsilon_{0}}
\end{align}
$$
Teniendo en cuenta que $Q_{encl} = \rho{V} = {\rho}{\frac{4}{3}\pi r^3}$. Entonces, reemplazamos y despejamos el campo electrico:
$$
\begin{align}
E  & = \frac{{\rho}{\frac{4}{3}\pi r^3}}{\epsilon_{0} 4\pi r^2} \\
E  & = \frac{\rho r}{\epsilon_{0} 3} \hat{r}
\end{align}
$$
**Para el caso en el que r> R, tenemos:**
$$
\begin{align}
\phi_{E} = 4\pi r^2E = \frac{Q_{encl}}{\epsilon_{0}}
\end{align}
$$
Teniendo en cuenta que $Q_{encl} = \rho{V} = {\rho}{\frac{4}{3}\pi R^3}$. Entonces, reemplazamos y despejamos el campo electrico:
$$
\begin{align}
E  & = \frac{{\rho}{\frac{4}{3}\pi R^3}}{\epsilon_{0} 4\pi r^2} \\
E  & = \frac{{\rho}{ R^3}}{3\epsilon_{0} \pi r^2} \\
\end{align}
$$
Para aplicar la Ley de Gauss de esta forma, **no es estrictamente necesario exigir uniformidad constante** (ρ=cte). Solo se exige **simetría esférica**, es decir, que la densidad de carga dependa a lo sumo de la distancia radial ρ(r), pero no de las coordenadas angulares. Si dependiera de los ángulos, se perdería la simetría y el campo dejaría de ser netamente radial.

#### punto d
Esto parece describir un conductor: distribucion cilindrica infinita de carga con densidad superficial de carga uniforme $\sigma$. Asumimos que la carga es positiva y que el cilindro tiene radio R.

Usando coordenadas cilindricas, nos damos cuenta de la simetria en los ejes $\theta$ y z, de tal forma que el vector del campo electrico termina siendo radial a la carga. Por tanto, usamos una superficie gaussiana coaxial con el eje de simetria del cilindro, de radio r y largo l, con sus extremos perpendiculares a la carga.

Para el caso en el que $r<R$, encontrar el campo electrico resulta trivial, dado que la carga se encuentra solo en la superficie, y por tanto la ley de gauss en este caso nos indica que el campo electrico es 0.

Para el caso en el que $r>R$, tenemos en cuenta que el vector del campo electrico en todos los puntos de la parte cilindrica de la superficie es paralelo al vector normal, y perpendicular en los extremos, asi que el calculo termina siendo similar al punto a).

El area de la cara cilindrica es $2\pi rl$. Entonces, aplicando la ley de gauss, tenemos:
$$
\begin{align}
\phi_{E} &  = 2E\pi rl = \frac{Q_{encl}}{\epsilon_{0}} \\
 E  & = \frac{Q_{encl}}{2\pi\epsilon_{0}rl}
\end{align}
$$
Ademas, tenemos que $Q_{encl} = \sigma 2\pi Rl$. Por tanto, sustituyendo, tenemos:
$$
\begin{align}
E=\frac{\sigma R}{\epsilon_{0}r}\hat{r} \end{align} $$
Es fundamental que la distribucion de la carga sobre la superficie sea uniforme de tal forma que garantize la simetria en las coordenadas $\theta$ y $z$ del cilindro.