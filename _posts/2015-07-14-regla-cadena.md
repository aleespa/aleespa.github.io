---
title: "Regla de la Cadena en Campos Escalares"
permalink: /regla-cadena/
layout: single
author_profile: false
categories:
  - Calculus
tags:
  - Spanish
---

La regla de la cadena es de mucha utilidad en funciones de una dimensión, y tiene gran importación, puede ser extendida a campos escalares.

## Teorema

Sea $$f:S\rightarrow R,\quad S\subseteq { R }^{ n }$$ y $$\vec { r } :J\rightarrow S\quad J\subseteq { R }$$ funcion vectorial

definimos $$g(t)=f[\vec { r } (t)]$$ si $$t\epsilon J$$; si $$\vec { r' } (t)$$ existe y $$f$$ es diferenciable en $$r(t)$$ entonces $$g'(t)$$ existe y:

$$g'(t)=\left< \nabla f(\vec { a } ),\vec { r' } (t) \right> \quad \text{ donde }\quad \vec { a } =\vec { r } (t)$$

Para demostrarlo vamos a usar la formula de la diferenciación de un campo escalar:

$$f(\vec { a } +\vec { b } )=f(\vec { a } )+{ T }_{ a }(\vec { v } )+\left\| \vec { v } \right\| E(\vec { a } ,\vec { v } )\\ { T }_{ a }(\vec { v } )=\left< \nabla f(\vec { a } ),\vec { v } \right>$$

Donde $$E(\vec { a } ,\vec { v } )$$ tiende a 0 cuando $$\left\| \vec { v } \right\|$$ tiende a 0. $$T_a$$ es una transformación lineal y es diferencial de $$f$$ en $$\vec { a }$$, como en la hipótesis se asegura que la diferenciabilidad en $$\vec { r } (t)$$ y $$t$$ existen se podrá hacer uso de esa definición, $$S$$ es un conjunto abierto. Usaremos el producto punto tradicional de un campo escalar:

$$\left< \vec { x } ,\vec { y } \right> =\sum _{ k=1 }^{ n }{ { x }_{ k }{ y }_{ k } } \quad \forall \vec { x } ,\vec { y } \in { R }^{ n }$$

## DEMOSTRACIÓN

Como $$S$$ es un conjunto abierto existe una n-bola dentro de $$S$$ y sea algun $$h$$ muy pequeño tal que $$\vec { r } (t+h)$$ esta contenida en tal n-bola, definamos $$\vec { y } =\vec { r } (t+h)-\vec { r } (t)$$ notese que $$\vec { y }$$ tiende a 0 cuando $$h$$ tiende a 0 y definamos tambien desde un principio que $$\vec { a } =\vec { r } (t)$$. Podemos establecer lo siguiente:

$$g(t+h)-g(t)=f[\vec { r } (t+h)]-f[\vec { r } (t)]=f(\vec { a } +\vec { y } )-f(\vec { a } )$$

Todo esto es valido, solo es cambiar las variables, ahora ya podemos aplicar la formula de la diferenciación vista al principio.

$$f(\vec { a } +\vec { y } )-f(\vec { a } )=\left< \nabla f(\vec { a } ),\vec { y } \right> +\left\| \vec { y } \right\| E(\vec { a } ,\vec { y } )$$

Podemos regresar a las variables iniciales ya que hemos llegado a esta expresión, y dividir entre $$h$$:

$$\frac { g(t+h)-g(t) }{ h } =\left< \nabla f(\vec { a } ),\frac { \vec { r } (t+h)-\vec { r } (t) }{ h } \right> +(\frac { \left\| \vec { r } (t+h)-\vec { r } (t) \right\| }{ h } )E(\vec { a } ,\vec { r } (t+h)-\vec { r } (t))$$

Podemos aplicar el proceso de limite, y no queda indefinido ya que $$E(\vec { a } ,\vec { y } )$$ esta definida en el 0 es decir $$E(\vec { a } ,\vec { 0 } )$$ y en lo demas queda lo deseado:

$$\lim _{ h\rightarrow 0 }{ \frac { g(t+h)-g(t) }{ h } } =\lim _{ h\rightarrow 0 }{ [\left< \nabla f(\vec { a } ),\frac { \vec { r } (t+h)-\vec { r } (t) }{ h } \right> +(\frac { \left\| \vec { r } (t+h)-\vec { r } (t) \right\| }{ h } )E(\vec { a } ,\vec { r } (t+h)-\vec { r } (t))] } \\ g'(t)=\left< \nabla f(\vec { a } ),\vec { r' } (t) \right>$$

Por lo tanto queda demostrado el teorema.

La expresión puede expresarse en términos menos generales que faciliten los cálculos:

$$\begin{aligned}
g'(t)&=\left< \nabla f(\vec { a } ),\vec { r' } (t) \right> \\
\nabla f(\vec { a } )&=(\frac { \partial f(\vec { a } ) }{ \partial { x }_{ 1 } } ,\frac { \partial f(\vec { a } ) }{ \partial { x }_{ 2 } } ,...,\frac { \partial f(\vec { a } ) }{ \partial { x }_{ n } } ) \\
\vec { r } '(t)&=(r'_{ 1 }(t),{ r' }_{ 2 }(t),..,{ r' }_{ n }(t)) \\
g'(t)&=\frac { \partial f(\vec { a } ) }{ \partial { x }_{ 1 } } r'_{ 1 }(t)+\frac { \partial f(\vec { a } ) }{ \partial { x }_{ 2 } } { r' }_{ 2 }(t)+...+\frac { \partial f(\vec { a } ) }{ \partial { x }_{ n } } { r' }_{ n }(t) \\
&=\sum _{ k=1 }^{ n }{ \frac { \partial f(\vec { a } ) }{ \partial { x }_{ k } } { r' }_{ k }(t) }
\end{aligned}$$

Gracias por su visita, espero sus comentarios.
