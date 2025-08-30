---
title: "Direcciones asintóticamente recurrentes de caminatas aleatorias"
permalink: /direcciones-recurrentes/
layout: single
author_profile: false
categories:
  - Probability
tags:
  - Spanish
---

Una caminata aleatoria se define como un proceso estocástico en tiempo discreto que evoluciona en función de saltos aleatorios idénticamente distribuidos. Es muy intuitivo pensar en una caminata aleatoria, pues se puede pensar que lo que modelamos es la posición de una partícula al momento $$n$$, como estamos hablando de modelo aleatoria nuestro interés es saber como evoluciona la posición de la particular y en que áreas de nuestro espacio será mas probable encontrarla.

Más específicamente una caminata aleatoria en $$\mathbb{R}^d$$ en tiempo discreto es un proceso estocástico dado por 

$$S_n=\sum_{i=1}^{n}\xi_i$$ 

donde $$(\xi_i)_{i\in\mathbb{N}}$$ son v.a.i.i.d. , este proceso resulta ser el más simple de todos los proceso de Markov, pues precisamente el proceso avanza un paso a la vez, dependiendo su siguiente posición solo de donde ha llegado.

Nuestro proceso empieza en $$S_0= 0$$, una de las preguntas más interesantes sobre las caminatas es la cantidad de veces que regresará a el origen. Decimos que $$x\in\mathbb{R}^d$$ es un valor <b>recurrente </b>si para cualquier $$\varepsilon\gt0$$, $$\mathbb{P}(\|S_n-x\|\lt;\varepsilon\text{ i.o.})=1$$ es decir que $$S_n$$ visita cualquier vecindad de $$x$$ una infinidad de veces con probabilidad. El siguiente teorema prueba que el conjunto de valores recurrentes o es el vació o un subgrupo de $$\mathbb{R}$$

### Teorema 1
El conjunto $$\mathcal{V}$$ de valores recurrentes es $$\emptyset$$ o un subgrupo cerrado de $$\mathbb{R}^d$$


Entonces para identificar una caminata aleatoria que visita una infinidad de veces el origen solo basta probar
que $$\mathcal{V}\neq\emptyset$$, en este caso la caminata es <b>recurrente</b>, cuando $$\mathcal{V}=\emptyset$$ la caminata es <b>trascendente</b>. Ahora nuestro objetivo sería identificar de alguna manera las caminatas aleatorias que son trascendentes y las que son recurrentes.

Algunos resultados interesantes para identificar el tipo de caminata aleatoria, son los siguientes:

### Teorema 2 
Una caminata aleatoria $$S_n$$ en $$\mathbb{R}^d$$ es recurrente bajo las siguientes condiciones:
(i) $$d=1$$ y $$n^{-1}S_n\overset{P}{\rightarrow}0$$
(ii) $$d=2$$, $$\mathbb{E}(\xi_i)=0$$ y $$\mathbb{E}|\xi|^2\lt;\infty$$

### Teorema 3
Sea $$S_n$$ una caminata aleatoria en $$\mathbb{R}^d$$ con distribución $$\mu(A)=\mathbb{P}(\xi\in A)$$, 
sea $$\varepsilon\gt;0$$, entonces $$S_n$$ es recurrente si y solo si 
$$$$\sup_{0\lt;r\lt;1}\int_{B_\varepsilon}\text{Re}\frac{1}{1-r\hat{\mu}_t}dt=\infty$$$$


### Teorema 4
Cualquier caminata aleatoria de dimensión efectiva $$d\geq3$$ es trascendente.


Dependiendo de los pasos $$\xi$$ es será mas fácil probar la recurrencia con alguno de los teoremas, notemos que el teorema 2 utiliza claramente el teorema del limite central y la ley fuerte de los grandes números.

Dependiendo de los saltos de la caminata $$\xi_i$$ esta puede tomar diferentes direcciones, para estudiar estas posibles direcciones consideramos el proceso $$\hat{S}_n=\frac{S_n}{\|S_n\|}$$, este proceso solo toma valores en la esfera $$\mathbb{S}^{d-1}=\{x\in\mathbb{R}^d:\|x\|=1\}$$ y denota la dirección que tiene la caminata al tiempo $$n$$. Este nuevo proceso pierde algunas de las propiedades, entre ellas que sea una proceso de Markov, esto porque los saltos que tenga ahora no solo dependen del anterior debido a la distancia que puede tener del origen.

Para estudiar las direcciones que visita la caminata definimos el siguiente conjunto: $$$$\mathcal{D}=\{u\in\mathbb{S}^{d-1}:\liminf_{n\rightarrow\infty}\|\hat{S}_n-u\|=0\text{ a.s}\}$$$$
Es el conjunto de direcciones recurrentes, son las direcciones que visita una infinidad de veces o que se aproxima a ellas. Se puede probar que es un conjunto cerrado y no vació, por lo tanto cualquier caminata aleatoria tiene al menos una dirección, algunos resultados interesantes sobre $$\mathcal{D}$$
### Proposición 1 
Si $$S_n$$ es recurrente entonces $$\mathcal{D}=\mathbb{S}^{d-1}$$

### Proposición 2
Sea $$\mathcal{D}$$ el conjunto de direcciones recurrentes de $$S_n = \sum_{ i=1}^{n} X_i$$ en $$\mathbb{R}^ d$$ . Entonces para cualquier transformación ortogonal $$B$$ en $$\mathbb{R}^d$$ la caminata aleatoria $$S'_n = \sum_{ i=1}^{n} BX_i$$ tiene direcciones recurrentes $$B\mathcal{D}$$ .

### Proposición 3
Supongamos que existe una variablea aleatoria $$\zeta\in\mathbb{S}^{d-1}$$ tal que $$\hat S_n\overset{d}{\rightarrow}\zeta$$. Entonces $$\text{supp } \zeta \subseteq \mathcal{D}$$


### Proposición 4
Supongamos que $$\mathbb{E}\|\xi\|\lt;\infty$$ y $$\mu=\mathbb{E}\xi_i$$ entonces
(i) Si $$\mu\neq 0$$ entonces $$\mathcal{D}=\{\hat\mu\}$$
(ii) Si $$\mu=0$$ entonces $$\#\mathcal{D}\geq 2$$

Con estas proposiciones se cubren una gran cantidad de ejemplos en donde $$\xi$$ tiene un comportamiento común, el caso en el que $$S_n$$ es reurrrente el problema es trivial ya que visitara en algún momento cualquier dirección, entonces nos podemos concentrar cuando es trascendente. Si los saltos tienen primer momento $$\mu$$ se puede usar la ley fuerte de los grandes numeros para probar que $$\lim_{n\rightarrow\infty}\|\hat S_n-\hat \mu\|=0\text{ a.s.}$$ entonces $$\hat \mu$$ es su dirección recurrente.

Es natural explorar cuáles son las propiedades de $$\mathcal{D}$$, aparte de ser cerrado y no vacío. Es intuitivo pensar que tendría cierta convexidad, ya que los saltos no pueden llevarnos de una dirección a otra completamente distinta con un solo salto. Pues resulta que este no es el caso y cualquier subconjunto cerrado de $$\mathbb{S}^{d-1}$$ puede ser el conjunto de direcciones recurrentes de alguna caminata aleatoria, el siguiente teorema lo enuncia.

### Teorema 5
Sea $$A$$ un conjunto no cerrado de $$\mathbb{S}^{d-1}$$, supongamos que los saltos de la caminata aleatoria son $$X=Q\xi$$ donde $$Q\in\mathbb{S}^{d-1}$$ y $$\xi\in\mathbb{R}_{+}$$ independientes tal que $$\text{supp }Q=A$$ y $$\mathbb{P}(\xi\gt;r)=(\log \log r)^{-1}$$ para $$r\gt;e^e$$. Entonces la caminata $$S_n=\sum_{i=1}^{n}X_i$$ tiene direcciones recurrentes $$\mathcal{D}=A$$

Este teorema no solo nos asegura que existe una caminata aleatoria para cada subconjunto $$A$$, también nos dice la forma en la que se consigue tal caminata, notemos que $$\xi$$ en este caso es una variable aleatoria con una distribución con <b>cola extremadamente pesada</b>, es decir que la probabilidad de que tenga valores grandes decrece demasiado lento. Para probar el teorema 5 es necesaria esta distribución que tiene la propiedad de que un solo salto puede ser más grande que el resto de los saltos y esto ocurre infinitamente seguido, osea que nuestra caminata aleatoria puede cambiar de dirección en cualquier momento, sin importar que tan alejada este del origen.

### Bibliografía
- R. Durrett, Probability: Theory and Examples, 4th ed., Cambridge University Press,
Cambridge, 2010.
- O. Kallenberg, Foundations of Modern Probability. 2nd ed., Springer, New York,
2002.
