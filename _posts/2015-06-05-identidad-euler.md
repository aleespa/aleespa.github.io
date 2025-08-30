---
title: "Identidad de Euler"
permalink: /identidad-euler/
layout: single
author_profile: false
categories:
  - Calculus
tags:
  - Spanish
---

En esta publicación daré una demostración muy simple de la identidad de Euler

$${ e }^{ i\pi }+1=0$$

### Demostración

Primero consideraremos el numero complejo $$z=a+bi$$ ($$a$$ es la parte real y $$b$$ la imaginaria) con modulo 1, en su forma polar tenemos que $$z=(\cos(t)+i\sin(t))$$ calculado la derivada

$$z=\cos { \theta } +i\sin { \theta } \\ dz=(-\sin { \theta } +i\cos { \theta } )d\theta $$

Se puede factorizar un $$i$$ ya que $$i^2=-1$$

$$dz=i(\cos { \theta } +i\sin { \theta } )d\theta \\ dz=izd\theta $$

Se deja de la forma:

$$\frac { dz }{ z } =id\theta $$

Integrando:

$$\int { \frac { dz }{ z } } =\int { id\theta } \\ \Rightarrow \ln { z } =i\theta $$

Lo que nos demuestra que

$${ e }^{ i\theta }=z\\ { e }^{ i\theta }=\cos{\theta}+i\sin{\theta}$$

Y en un caso particular en el que el angulo es pi obtenemos la identidad

$${ e }^{ i\pi }+1=0$$

A partir de este resultado podemos concluir varias cosas interesantes como el calculo de logaritmos de números negativos.

$$\ln { (-1) } =i\pi \\ \ln { (-\beta ) } =\ln { \beta } +\ln { (-1) } =\ln { \beta } +i\pi $$

Gracias por su visita, me gustaría ver sus comentarios.