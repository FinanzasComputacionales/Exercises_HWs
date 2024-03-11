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
\begin{aligned}
    \left\\{
        1 \quad & \text{si } x\leq 1 \\
        x \quad & \text{si } x > 1
    \right.
\end{aligned}
$$