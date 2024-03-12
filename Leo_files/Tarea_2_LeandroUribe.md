# Ejercicios pares, capítulo 2

2. Para este problema se pide evaluar el límite punto a punto de la secuencia de funciones dada por:

$$ f_n(x) = \sqrt[n]{1 + x^n}, \quad x\geq 0 $$

Consideremos cada posible caso:

* Tenemos inicialmente que, si $x=0$, se tendrá que la función $f_n(0)=1$ para cualquier $n\in\mathbb{N}$.
* En el intervalo $0 < x \leq 1$, se tiene que el elemento $x^n \to 0$ y, aplicando la función en este intervalo, se tiene que $1\leq f_n(x)\leq \sqrt[n]{2}$, en donde se puede ver que:

$$ \lim_{n\to\infty} 1 = \lim_{n\to\infty} \sqrt[n]{2} = 1 $$

Y, por el teorema del sanduche, podemos decir entonces que para $0 < x \leq 1$ se cumple que

$$ \lim_{n\to\infty} f_n(x) = 1 $$

* Ahora, para $x>1$, notemos que podemos reescribir la secuencia de funciones como:

$$ f_n(x) = \sqrt[n]{1 + x^n} = \sqrt[n]{ x^n\left( \frac{1}{x^n} + 1 \right) } = x \sqrt[n]{ \frac{1}{x^n} + 1 } $$

Y, al aplicar el límite para $n\to\infty$, vemos que:

$$ \lim_{n\to\infty} x \sqrt[n]{ \frac{1}{x^n} + 1 } = x $$

Por lo que, juntando todo, hemos probado que:

$$ \lim_{n\to\infty} f_n(x) = f(x), \quad \text{donde } f(x) = 
\left\\{
    \begin{aligned}
        1 \quad & \text{si } x\leq 1 \\
        x \quad & \text{si } x > 1
    \end{aligned}
\right.
$$


4. Para este ejercicio, debemos demostrar que la siguiente secuencia de funciones converge uniformemente a $f(x)=0$:

$$ f_n(x) = \frac{ \sqrt{1-x^n} }{n^2}, \quad x\in[-1, 1] $$

Analizando la secuencia de funciones para el intervalo dado, la expresión $\sqrt{1-x^n}$ evaluada en $x=-1$ dará como resultado $\sqrt{2}$ para valores impares de $n$, mientras que el resultado será 0 tanto para valores pares de $n$ en $x=-1$ como para el extremo $x=1$ sin importar la paridad de $n$.

De lo anterior, podemos afirmar que $\sqrt{1-x^n} \leq \sqrt{2}$, por lo que se tendrá que:

$$ f_n(x) = \frac{ \sqrt{1-x^n} }{n^2} \leq \frac{\sqrt{2}}{n^2} $$

La desigualdad anterior no depende de $x \in [-1, 1]$, lo cual hace que al tomar el valor $\sup$ respecto a $x \in [-1, 1]$ garantice convergencia uniforme.


6. Se pide evaluar el siguiente límite:

$$ \lim_{n\to\infty} \int_1^{\infty} \frac{ ne^{-nx} }{ 1+nx } dx $$

El objetivo inicial será demostrar que existe convergencia uniforme para $f_n(x)$ para poder aplicar el teorema que permite introducir la expresión de un límite dentro de la integral, de modo que se tenga:

$$ \lim_{n\to\infty} \int_a^b f_n(x) dx = \int_a^b \lim_{n\to\infty} f_n(x) dx $$

Esto nos permitirá evaluar la expresión de una forma más sencilla.

Para esto, comenzamos definiendo la siguiente función decreciente con $x\in [1, +\infty)$:

$$ h_n(x) = \frac{n}{1+nx} $$

Se tiene que al calcular $h'_n(x)$ obtenemos la siguiente expresión:

$$ h'_n(x) = -\frac{ n^2 }{ (1+nx)^2 } < 0 $$

Considerando el límite para la función $h_n(x)$ tenemos:

$$ \lim_{x\to\infty} \frac{n}{1+nx} = 0 $$

y, tomando el $\sup$ para el intervalo dado:

$$ \sup_{x\in[1, \infty)} \frac{n}{1+nx} = h_n(1) = \frac{n}{1+n} $$

Con esto, podemos inferir que el valor de $h_n(1)$ se encuentra restringido por:

$$ |h_n(x)| \leq \frac{n}{1+n} < 1 $$

y, por lo tanto, si tomamos en consideración el elemento $e^{-nx}$ podemos afirmar que:

$$ \left| \frac{ne^{-nx}}{1+nx} \right| < e^{-nx} $$

Mostrando así que existe convergencia uniforme para $f_n(x)$. Con esto, podemos hacer uso del teorema que introduce el límite dentro de la integral y evaluar:

$$ \lim_{n\to\infty} \int_1^{\infty} \frac{ne^{-nx}}{1+nx} dx = \int_1^{\infty} \lim_{n\to\infty} \frac{ne^{-nx}}{1+nx} dx = \int_1^{\infty} 0 \\; dx = 0 $$