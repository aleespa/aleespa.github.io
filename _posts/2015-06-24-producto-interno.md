---
title: "Producto Interno"
permalink: /producto-interno/
layout: single
author_profile: false
---

El producto interno en un espacio lineal se puede definir de varias maneras, siempre y cuando se tengan las características de la definición el mas conocido puede ser el producto punto en que simplemente estaba definido como la suma de cada producto de valores.

En esta ocacion vamos a demostrar que la siguiente expresión es un producto interno.

$$\left< f,g \right> =\int _{ a }^{ b }{ f(t)g(t)dt }$$

Pero primero tenemos que definir el espacio lineal, usaremos funciones continua es cierto intervalo $$[a,b]$$:

$$V(a,b)=\{ f(x)|\lim _{ x\rightarrow c }{ f(x)=f(c)\quad \forall c\in [a,b]\} }$$

Forma el espacio lineal con la suma común de funciones y la multiplicación por algún numero real (o imaginario, formando un espacio euclidiano complejo). En seguida demostraremos que la formula anterior es un producto interno para ese espacio lineal.

## DEMOSTRACIÓN

En cada propiedad sera demostrado tomando por un hecho varios teoremas de la integral de funciones continuas

**1) $$\left< f,g \right>=\left< g,f \right>$$ (conmutatividad o simetría)**

$$\left< f,g \right>=\int _{ a }^{ b }{ f(t)g(t)dt } =\int _{ a }^{ b }{ g(t)f(t)dt } =\left< g,f \right>$$

**2) $$\left< f,g+h \right>=\left< f,g \right>+\left< f,h \right>$$ (distributividad o linealidad)**

$$\begin{aligned}
\left< f,g+h \right>&=\int _{ a }^{ b }{ f(t)[g+h](t)dt } \\
&=\int _{ a }^{ b }{ f(t)[g(t)+h(t)]dt } \\
&=\int _{ a }^{ b }{ f(t)g(t)dt } +\int _{ a }^{ b }{ f(t)h(t)dt } \\
&=\left< f,g \right>+\left< f,h \right>
\end{aligned}$$

**3) $$c\left< f,g \right>=\left< cf,g \right>$$ (asociatividad u homogeneidad)**

$$c\left< f,g \right> =c\int _{ a }^{ b }{ f(t)g(t)dt } =\int _{ a }^{ b }{ cf(t)g(t)dt } =\left< cf,g \right>$$

**4) $$\left< f,f \right> >0$$ si $$f\neq 0$$ (positividad)**

$$\left< f,f \right> =\int _{ a }^{ b }{ f(t)f(t)dt } =\int _{ a }^{ b }{ { f }^{ 2 }(t)dt } \\ { f }^{ 2 }(t)\ge 0\quad \Rightarrow \int _{ a }^{ b }{ { f }^{ 2 }(t)dt } \ge 0\\ \int _{ a }^{ b }{ { f }^{ 2 }(t)dt } =0\quad \Leftrightarrow \quad f(t)=0$$

Por lo tanto cumple todos los axiomas de producto interno y $$V(a,b)$$ es espacio euclidiano.

De esto se pueden concluir cosas interesantes como la desigualdad de Cauchy-Schwarz y establecer una metrica de funciones continuas, calcular normas y establecer la ortogonalidad de funciones.

$${ (\int _{ a }^{ b }{ f(t)g(t)dt } ) }^{ 2 }\le \int _{ a }^{ b }{ { f }^{ 2 }(t)dt } \int _{ a }^{ b }{ { g }^{ 2 }(t)dt } \\ \left\| f(t) \right\| =\sqrt { \int _{ a }^{ b }{ { f }^{ 2 }(t)dt } }$$

Gracias por su visita, espero sus comentarios.