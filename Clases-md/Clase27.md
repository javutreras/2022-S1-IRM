## Conjuntos numerables y el teorema de Cantor

**Definición.** Un conjunto se dice numerable si es equipotente a $\mathbb{N}$.

*Ejemplo.* El conjunto $\mathbb{Z}$ es numerable.

---

### Numerabilidad de los números racionales

**Teorema.** $\mathbb{Q}$ es numerable.

*Demostración.* Por el teorema de Cantor-Bernstein-Schröder.

- Como la función $f:\mathbb{N}\to\mathbb{Q}$ dada por $f(x)=x$ es inyectiva, vemos que $|\mathbb{N}|\le |\mathbb{Q}|$.

- Si un número racional positivo $q$ se escribe en su forma más simplificada como $\frac{a}{b}$, definimos $g(q)=2^a3^b$ y $g(-q)=2^a3^b5$. Si además hacemos $g(0)=0$, tenemos $g:\mathbb{Q}\to\mathbb{N}$ inyectiva y por consiguiente $|\mathbb{Q}|\le |\mathbb{N}|$.

---

### No-numerabilidad de los números reales

**Teorema (Cantor).** Una función $\mathbb{N}\to [0,1]$ no puede ser sobreyectiva.

**Corolario.** Una función $\mathbb{N}\to\mathbb{R}$ no puede ser biyectiva. Si lo fuera se podría componer con la función sobreyectiva $x\mapsto\begin{cases}0& x<0\\ x&x\in[0,1] \\ 1& x>1\end{cases}$ y se obtendría una función que contradice el teorema.

*Demostración del teorema.* Supongamos que existe una función $f:\mathbb{N}\to [0,1]$ sobreyectiva...

---

### Teorema de Cantor

**Teorema.** Sea $X$ un conjunto. No existe una función $X\to\mathcal{P}(X)$ sobreyectiva.

**Corolario.** $|X|<|\mathcal{P}(X)|$.

*Demostración del teorema.* Supongamos que existe una función $f:X\to\mathcal{P}(X)$ sobreyectiva. Definimos el conjunto
$$C=\{x\in X\,:\, x\not\in f(x)\}$$

Claramente $C\subset X$, luego $C\in\mathcal{P}(X)$. Como $f$ es sobreyectiva, existe $u\in X$ tal que $C=f(u)$.

- Si $u\in C$, entonces $u\in f(u)$ y en consecuencia $u\not\in C$. Contradicción.

- Si $u\not\in C$, entonces $u\not\in f(u)$ y en consecuencia $u\in C$. Contradicción.

En conclusión $u$ no puede existir, es decir, $f$ no puede ser sobreyectiva.
