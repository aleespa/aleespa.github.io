---
title: "Seno y Coseno de Suma de Ángulos "
permalink: /seno-coseno/
layout: single
author_profile: false
---

Las funciones seno y coseno las podemos expandir a ser una función con dominio complejo gracias a las series de funciones complejas en el que encontramos igualdades que son interesantes y podemos deducir resultados aun mas interesantes, ahora veremos que las propiedades básicas de ambas funciones se cumplen también para complejos. Veamos que:

$$\forall z,w\in C\\ \cos { (z+w) } =\cos { z } \cos { w } -\sin { z } \sin { w } \\ \sin { (z+w) } =\sin { z } \cos { w } +\sin { w } \cos { z }$$

Como se demostró en una antigua publicación, la función exponencial la podemos poner en función de senos y cosenos, también se puede de manera inversa:

$${ e }^{ iz }=\cos { z } +i\sin { z } \\ { e }^{ -iz }=\cos { z } -i\sin { z } \\ { e }^{ iz }+{ e }^{ -iz }=2\cos { z } \\ { e }^{ iz }-{ e }^{ -iz }=2i\sin { z } $$

$$\therefore  \quad \cos { z } =\frac { { e }^{ iz }+{ e }^{ -iz } }{ 2 } ;\quad \sin { z } =\frac { { e }^{ iz }-{ e }^{ -iz } }{ 2i }$$

## DEMOSTRACIÓN

La demostración sera completamente directa y algebraica. a partir de un lado de la igualdad llegaremos al otro, empezamos con $$\cos { z } \cos { w } -\sin { z } \sin { w }$$ usando lo anterior:

$$\begin{aligned}
\cos { z } \cos { w } -\sin { z } \sin { w } &=(\frac { { e }^{ iz }+{ e }^{ -iz } }{ 2 } \cdot \frac { { e }^{ iw }+{ e }^{ -iw } }{ 2 } )-(\frac { { e }^{ iz }-{ e }^{ -iz } }{ 2i } \cdot \frac { { e }^{ iw }-{ e }^{ -iw } }{ 2i } ) \\
&=\frac { { e }^{ i(z+w) }+{ e }^{ i(z-w) }+{ e }^{ i(w-z) }+{ e }^{ -i(z+w) } }{ 4 } +\frac { { e }^{ i(z+w) }-{ e }^{ i(z-w) }-{ e }^{ i(w-z) }+{ e }^{ -i(z+w) } }{ 4 } \\
&=\frac { 2({ e }^{ i(z+w) }+{ e }^{ -i(z+w) }) }{ 4 } \\
&=\frac { { e }^{ i(z+w) }+{ e }^{ -i(z+w) } }{ 2 } \\
&=\cos { (z+w) }
\end{aligned}$$

Solo se hizo uso de leyes de los exponentes y de que $${i}^{2}=-1$$, de manera similar ocurre con:

$$\begin{aligned}
\sin { z } \cos { w } +\sin { w } \cos { z } &=(\frac { { e }^{ iz }-{ e }^{ -iz } }{ 2i } \cdot \frac { { e }^{ iw }+{ e }^{ -iw } }{ 2 } )+(\frac { { e }^{ iw }-{ e }^{ -iw } }{ 2i } \cdot \frac { { e }^{ iz }+{ e }^{ -iz } }{ 2 } ) \\
&=\frac { { e }^{ i(z+w) }-{ e }^{ i(z-w) }+{ e }^{ i(w-z) }-{ e }^{ -i(z+w) } }{ 4i } +\frac { { e }^{ i(z+w) }+{ e }^{ i(z-w) }-{ e }^{ i(w-z) }-{ e }^{ -i(z+w) } }{ 4i } \\
&=\frac { 2({ e }^{ i(z+w) }-{ e }^{ -i(z+w) }) }{ 4i } \\
&=\frac { { e }^{ i(z+w) }-{ e }^{ -i(z+w) } }{ 2i } \\
&=\sin { (z+w) }
\end{aligned}$$

Con esto queda demostrado, es mucho mas sencillo que algunas demostraciones de geometría analítica o calculo de variable real.
