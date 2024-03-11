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