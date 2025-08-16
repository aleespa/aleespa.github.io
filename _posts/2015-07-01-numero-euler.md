---
title: "Número de Euler"
permalink: /numero-euler/
layout: single
author_profile: false
---

El numero de Euler puede ser definido de varias maneras según la rama de las matemáticas en la que se este estudiando, lo podemos ver como el limite de una sucesión. Al final todos valen lo mismo, se esta hablando del mismo numero, en esta ocasión me gustaría demostrar a partir de una definición distinta el limite de esta sucesión:

$$a_n= (1+\frac { 1 }{ n } ) ^{ n }$$


Para la demostración vamos a partir de la definición del calculo diferencial en donde la base del logaritmo natural es igual a $$e$$, de donde se deriva la función inversa al logaritmo, la exponencial, cuya derivada es ella misma, el echo de que su derivada sea ella misma es muy fuerte, cuando queremos expresar la forma polinomica de la función exponencial, llegamos a una expresión sencilla.

$$f(x)=\sum _{ n=0 }^{ \infty }{ \frac { { f }^{ n }(0){ x }^{ n } }{ n! } } ;\quad { e }^{ x }=\sum _{ n=0 }^{ \infty }{ \frac { { x }^{ n } }{ n! } } \quad e=\sum _{ n=0 }^{ \infty }{ \frac { 1 }{ n! } }$$

Y así es como podemos aproximar el valor de $$e$$ ($$e=2.7182...$$ pero eso en realidad no importa).

Vamos a usar el binomio de Newton en la demostración, su demostración, podría quedar para otra publicación futura.

$${ (x+y) }^{ n }=\sum _{ k=0 }^{ n }{ \frac { n! }{ k!(n-k)! } } { x }^{ n-k }{ y }^{ k }$$

## DEMOSTRACIÓN

Tomemos la sucesión $${a}_{n}$$

$${a}_{n}={(1+\frac { 1 }{ n } ) }^{ n }$$

Expandiendo el binomio tenemos que:

$${ a }_{ n }=\sum _{ k=0 }^{ n }{ \frac { n! }{ k!(n-k)!{ n }^{ k } } }$$

De ahi se pueden simplificar y re-acomodar algunos términos

$${ a }_{ n }=\sum _{ k=0 }^{ n }{ \frac { n! }{ k!(n-k)!{ n }^{ k } } } =\sum _{ k=0 }^{ n }{ \frac { 1\cdot 2\cdot 3\cdot \cdot \cdot (n-k)\cdot \cdot \cdot n }{ k!\cdot 1\cdot 2\cdot 3\cdot \cdot \cdot (n-k){ n }^{ k } } } =\sum _{ k=0 }^{ n }{ \frac { (n-(k+1))\cdot \cdot \cdot n }{ k!n^{ k } } }$$

En el numerador hay exactamente $$k$$ elementos al igual que en la parte de abajo, hay exactamente k elementos, podemos re-acomodarlos en $$k$$ fracciones.

$$\sum _{ k=0 }^{ n }{ \frac { (n-(k+1))\cdot \cdot \cdot n }{ k!n^{ k } } } =\sum _{ k=0 }^{ n }{ \frac { 1 }{ k! } \cdot \frac { n }{ n } \cdot \frac { n-1 }{ n } \cdot \frac { n-2 }{ n } \cdot \cdot \cdot \frac { n-(k+1) }{ n } }$$

Se puede simplificar aun mas, o bueno dejarlo en términos que sean agradables para lo que se busca.

$${ a }_{ n }=\sum _{ k=0 }^{ n }{ \frac { 1 }{ k! } \cdot (1-\frac { 1 }{ n } )\cdot (1-\frac { 2 }{ n } )\cdot \cdot \cdot (1-\frac { k+1 }{ n } ) }$$

De esa manera en la que esta escrito ya es posible calcular el limite, teniendo en cuenta los teoremas de limites (como la suma y la multiplicación), podemos tomar el limite de cada sumando y después de el de la suma completa.

$$\begin{aligned}
\lim _{ n\rightarrow \infty }{ { a }_{ n } } &=\lim _{ n\rightarrow \infty }{ \sum _{ k=0 }^{ n }{ \frac { 1 }{ k! } \cdot (1-\frac { 1 }{ n } )\cdot (1-\frac { 2 }{ n } )\cdot \cdot \cdot (1-\frac { k+1 }{ n } ) } } \\
&=\lim _{ n\rightarrow \infty } \frac { 1 }{ k! } \cdot (1-\frac { 1 }{ n } )\cdot (1-\frac { 2 }{ n } )\cdot \cdot \cdot (1-\frac { k+1 }{ n } ) \\
&=\lim _{ n\rightarrow \infty }{ \frac { 1 }{ k! } } \cdot \lim _{ n\rightarrow \infty }{ (1-\frac { 1 }{ n } ) } \cdot \lim _{ n\rightarrow \infty }{ (1-\frac { 2 }{ n } ) } \cdot \cdot \cdot \lim _{ n\rightarrow \infty }{ (1-\frac { k+1 }{ n } ) }
\end{aligned}$$

$$\forall i\in \{ m|0<m<t+1;\quad m\in { Z }\} \quad \lim _{ n\rightarrow \infty  }{ (1-\frac { i }{ n } )= } \lim _{ n\rightarrow \infty  }{ 1 } -i\lim _{ n\rightarrow \infty  }{ (\frac { 1 }{ n } )}$$

El ultimo limite ya es uno conocido, fácil de demostrar con la definición de limite:

$$\forall \varepsilon >0\quad \exists N\quad t.q.\quad \frac { 1 }{ N } <\varepsilon \rightarrow \quad si\quad n>N\quad \frac { 1 }{ n } <\frac { 1 }{ N } <\varepsilon \\ \therefore \left| \frac { 1 }{ n } -0 \right| <\varepsilon \quad \Rightarrow \lim _{ n\rightarrow \infty }{ (\frac { 1 }{ n } ) } =0\quad ;\quad \lim _{ n\rightarrow \infty }{ (1-\frac { i }{ n } ) } =1$$

Por lo tanto aplicando el limite a cada producto de la sumatoria es igual a 1 solo vamos a tener que

$$\lim _{ n\rightarrow \infty }{ ({ a }_{ n }) } =\sum _{ k=0 }^{ \infty }{ \frac { 1 }{ k! } } =e$$

Quedando demostrado.

Con esto se llega también a muchos resultados subsecuentes

$$\lim _{ n\rightarrow \infty }{ { (1+\frac { x }{ n } ) }^{ n } } =\lim _{ m\rightarrow \infty }{ { (1+m) }^{ \frac { x }{ m } } } =\sum _{ k=0 }^{ \infty }{ \frac { x }{ k! } } =\frac { { d }^{ n }{ e }^{ x } }{ d{ x }^{ n } } ={ e }^{ x }$$

Gracias por su visita espero ver sus comentarios.
