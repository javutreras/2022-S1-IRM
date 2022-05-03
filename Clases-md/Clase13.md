## Coeficiente combinatorio y teorema del binomio

**Corolario.** SI $n\ge 1$, entonces $\displaystyle\sum_{i=0}^n (-1)^i{n\choose i} = 0$

**Corolario (Inclusión-exclusión).**

---

**Corolario (Teorema del binomio).** Para $n\in\mathbb{N}$,$$(a+b)^n = \sum_{i=0}^n{n\choose i}a^ib^{n-i}$$

*Problema.* En general, determinar cómo son los términos de la forma $c\cdot a^ib^j$ que aparecen al desarrollar $(a+b)^n$.

- Condiciones sobre $i,j$
- Cantidad de sumandos
- Valor de cada coeficiente $c$

Tenemos:

- Antes de agrupar términos semejantes, hay $2^n$ sumandos en el desarrollo de $(a+b)^n$. Ésto se deduce por combinatoria: cada sumando posible se obtiene del producto $$(a+b)\cdot (a+b)\cdot\ldots \cdot (a+b)$$ escogiendo, de cada factor, un término de entre dos posibles. O sea, $2\cdot 2\cdot\ldots\cdot 2$ combinaciones posibles.

- En cada una de las $n$ elecciones del item anterior se escoge una $a$ o una $b$ para construir un sumando. En consecuencia, en cada sumando $a^ib^j$ se ha de cumplir $i+j=n$.

- Deducción: los términos son de la forma $c\cdot a^{n-k}b^k$

- Si de los $n$ binomios $(a+b)$ se pretende escoger *exactamente* $k$ veces el término $b$, se obtendrá el sumando $a^{n-k}b^k$; ésto se puede hacer de ${n\choose k}$ formas distintas.
- El término $a^{n-k}b^k$ aparece ${n\choose k}$ veces en la suma; por consiguiente ${n\choose k}$ es su coeficiente.

