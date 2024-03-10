# Resumen del capítulo 1

Para esta primera entrega, se pretende brindar un resumen de lo que contiene el capítulo 1 del libro "Introductory Mathematical Analysis for Quantitative Finance". En este resumen, se incluyen los temas de Vectores, Topología de $\mathbb{R}^n$ y Límites de funciones.


## Vectores

En este capítulo, se introduce el espacio euclidiano $\mathbb{R}^n$, y elementos como axiomas, operaciones como productos internos y operaciones vectoriales básicas. Se define la base estándar de $\mathbb{R}^n$ y se explica la representación de vectores como combinaciones lineales.

Con la introducción de la base estándar de $\mathbb{R}^n$ dada como $\mathbb{E}_n = \\{ e_1, e_2, \ldots, e_n \\}$, la definición de combinación lineal para un vector genérico $x$ se da como:

$$ x = \sum_{j=1}^n x_j e_j = \sum_{j=1}^n x \cdot e_j e_j $$

Se explica luego el concepto de vectores paralelos y ortogonales; dado dos vectores $x, y \in \mathbb{R}^n$, si $x,y$ son paralelos se denotará como $x \\| y$ y se cumplirá que existe un $t\in\mathbb{R}$ tal que $x=ty$. Por otro lado, si $x,y$ son ortogonales se denotará como $x\perp y$ y se cumplirá que $x\cdot y = 0$.

> [!IMPORTANT]
> Se debe tener la consideración de que $x,y$ sean vectores no nulos.

Se define además la norma euclideana de $x$ como:

$$ || x || = \left( \sum_{k=1}^n x_k^2 \right)^{\frac12} $$

Teniendo además que $|| x ||^2 = x\cdot x$.

Posteriormente, se introduce la desigualdad de Cauchy dada por:

$$ | x\cdot y | \leq || x || \\; || y || $$

Y se lleva a cabo su demostración junto con algunas propiedades básicas de la norma Euclideana y sus demostraciones mediante dicha desigualdad.


## Topología de $\mathbb{R}^n$

En esta parte del capítulo, se explican conceptos de conjuntos abiertos y cerrados, y presenta propiedades básicas de estos conjuntos en $\mathbb{R}^n$. Incluye definiciones de bolas abiertas y cerradas, y teoremas relacionados con la topología.

La definición para bolas abiertas y cerradas se da de la siguiente manera:

**(i).** $\forall r > 0$, la bola **abierta** centrada en **a** y de radio $r$ es el conjunto de puntos:

$$ B_r(a) := \\{ x\in\mathbb{R}^n \\; | \\; ||x-a|| < r \\} $$

**(ii).** $\forall r \geq 0$, la bola **cerrada**, centrada en $a$ de radio $r$ es el conjunto de puntos:

$$ \overline{B}_r(a) := \\{ x\in\mathbb{R}^n \\; | \\; ||x-a||\leq r \\} $$

> [!NOTE]
> Se hace énfasis en que, cuando $n=1$, las bolas se representan como intervalos abiertos $(a-r, a+r)$ para las bolas abiertas y como intervalos cerrados $[a-r, a+r]$ para bolas cerradas. En $n=2$, las bolas se representan como circunferencias de línea punteada para bolas abiertas y como circunferencias de línea sólida para bolas cerradas.

Se determina además la unión e intersección de subconjuntos abiertos $\\{V_{\alpha}\\}_{\alpha\in A}$ y cerrados $\\{E_{\alpha}\\}_{\alpha\in A}$ de $\mathbb{R}^n$ donde $A$ es cualquier conjunto de índices. Se tiene entonces que:

$$
\begin{aligned}
    (i).& \bigcup_{\alpha\in A} V_{\alpha}\text{ es abierto}; \qquad& (iii).& \bigcap_{\alpha\in A} E_{\alpha}\text{ es cerrado};\\
    (ii).& \bigcap_{k=1}^p V_{k}\text{ es abierto}; \qquad& (iv).& \bigcup_{k=1}^p E_{k}\text{ es cerrado};\\
\end{aligned}
$$


## Límites de funciones

Aunque no se detalla en el contexto proporcionado, este apartado probablemente aborda la aproximación de funciones en Rn y la definición formal de límites en este espacio.