---
title: "Volumen de Pirámide Hexagonal"
permalink: /volumen-piramide/
layout: single
author_profile: false
categories:
  - Calculus
tags:
  - Spanish
---

Hallar el volumen de la pirámide hexagonal en función de la altura y del área de la base.

Para calcular el volumen de la pirámide usaremos el calculo integral, como es de apreciar, ningún solido en revolución genera este volumen, por lo que los métodos tradicionales para el calculo de volúmenes no nos serán de utilidad.

Si consideramos el siguiente volumen hexagonal el cual recorrerá a la pirámide desde su base hasta su altura y calculamos su diferencial de volumen obtendremos el volumen de la pirámide.

Para comenzar notemos el área del hexágono en función del apotema esta definida por

$$\frac { p(a) }{ 2 } =\frac { 6L(a) }{ 2 } =3L(a)$$

Siendo $$P = Perímetro$$.

Usando el teorema de pitagoras (el cual ya a sido demostrado en este blog), para encontrar el valor de $$L$$

$$a=\sqrt { { L }^{ 2 }-{ (\cfrac { L }{ 2 } ) }^{ 2 } } \rightarrow { a }^{ 2 }=\frac { 3 }{ 4 } { L }^{ 2 }\\ { L }^{ 2 }=\frac { 4 }{ 3 } { a }^{ 2 }\quad L=\frac { 2\sqrt { 3 } }{ 3 } a$$

Donde finalmente concluimos que el área del hexágono en función del apotema es

$$3L(a)=3(\frac { 2\sqrt { 3 } }{ 3 } a)(a)=2\sqrt { 3 } { a }^{ 2 }$$

Si analizamos el diferencial de volumen (dv del solido hexagonal que consideramos, obtenemos lo siguiente

$$dv=\frac { p(a) }{ 2 } dy\\ dv=2\sqrt { 3 } { a }^{ 2 }dy\\ v=\int _{ 0 }^{ h }{ 2\sqrt { 3 } { a }^{ 2 }dy } \\ v=\int _{ 0 }^{ h }{ 2\sqrt { 3 } { x }^{ 2 }dy }$$

Para poder resolver esta integral la variable $$x$$ debe de estar en función de $$y$$ para poderla integrar

para ello usaremos la ecuación de la recta con los puntos $${ P }_{ 1 }$$ y $${ P }_{ 2 }$$

$$y-{ y }_{ 1 }=m(x-{ x }_{ 1 })\\ y-{ y }_{ 1 }=(\frac { { y }_{ 2 }-{ y }_{ 1 } }{ { x }_{ 2 }-{ x }_{ 1 } } )(x-{ x }_{ 1 })$$

Sustituyendo los puntos $${ P }_{ 1 }$$ y $${ P }_{ 2 }$$

$$y-h=\frac { 0-h }{ a-0 } (x-0)=\frac { -h }{ a } x\rightarrow \quad x=a-\frac { ay }{ h }$$

Así

$$\begin{aligned}
\int _{ 0 }^{ h }{ 2\sqrt { 3 } { x }^{ 2 }dy } &=2\sqrt { 3 } \int _{ 0 }^{ h }{ (a-\frac { ay }{ h } { ) }^{ 2 }dy } \\
&=2\sqrt { 3 } \int _{ 0 }^{ h }{ [{ a }^{ 2 }-\frac { 2{ a }^{ 2 }y }{ h } +\frac { { a }^{ 2 }y }{ { h }^{ 2 } } ]dy } \\
&=2\sqrt { 3 } { a }^{ 2 }{ y | }_{ 0 }^{ h }-{ \frac { 4{ \sqrt { 3 } a }^{ 2 }{ y }^{ 2 } }{ 2h } | }_{ 0 }^{ h }+{ \frac { 2{ \sqrt { 3 } a }^{ 2 }{ y }^{ 3 } }{ 3{ h }^{ 2 } } | }_{ 0 }^{ h } \\
&=2\sqrt { 3 } { a }^{ 2 }h-2\sqrt { 3 } { a }^{ 2 }h+\frac { 2{ \sqrt { 3 } a }^{ 2 }h }{ 3 } \\
&=\frac { 1 }{ 3 } (2{ \sqrt { 3 } a }^{ 2 })h \\
&=\frac { 1 }{ 3 } ({ A }_{ BASE })h
\end{aligned}$$

Quedando así demostrado que el volumen de una pirámide de base hexagonal es un tercio del área de su base por su altura
