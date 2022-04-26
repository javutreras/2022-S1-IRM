## Coeficiente combinatorio y teorema del binomio

**Corolario.** SI $n\ge 1$, entonces $\displaystyle\sum_{i=0}^n (-1)^n{n\choose i} = 0$

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

- Si de los $n$ binomios $(a+b)$ se pretende escoger *exactamente* $k$ veces el término $b$, se obtendrá el sumando $a^{n-k}b^k$; esto se puede hacer de ${n\choose k}$ formas distintas.
- El término $a^{n-k}b^k$ aparece ${n\choose k}$ veces en la suma; por consiguiente ${n\choose k}$ es su coeficiente.

---

### Bonus: versión multinomial

**Definición.** Si $k_1+k_2+\ldots +k_n=n$, el *coeficiente multinomial* se define $${n\choose k_1,k_2,\ldots ,k_n} = \frac{n!}{k_1!k_2!\ldots k_n!}$$

Las propiedades del coeficiente binomial tienen versiones más complejas, por ejemplo:

- si $k_1,k_2>0$, $${n+1\choose k_1,k_2,0} = {n\choose k_1-1,k_2,0} + {n\choose k_1,k_2-1,0}$$
- pero si $k_1,k_2,k_3>0$, $${n+1\choose k_1,k_2,k_3} = {n\choose k_1-1,k_2,k_3} + {n\choose k_1,k_2-1,k_3} + {n\choose k_1,k_2,k_3-1}$$

Y el teorema de la potencia queda
$$
\left(\sum_{i=0}^ma_i\right)^n = \sum_{k_i\ge 0, \sum_{i=1}^mk_i=n}{n\choose k_1,k_2,\dots ,k_m}\prod_{i=1}^ma_i^{k_i}
$$

---

## Divisibilidad

Se trabajará en el conjunto de los números naturales con el cero.

**Definiciones.** Sean $a,b\in\mathbb{N}$.
- Si existe $k$ tal que $a+k=b$, se dice que $a$ es *menor o igual que* $b$, y se escribe $a\le b$.

- Si existe $k$ tal que $a\cdot k=b$, se dice que $a$ *divide a* $b$, y se escribe $a\mid b$.

Se puede ver que ambas relaciones son relaciones de orden.

*Observación.* La *división* es una operación que tiene como resultado un número; la *divisibilidad* es una propiedad que puede ser verdadera o falsa:
- $2\mid 6$ es verdadero.

- $3\mid 5$ es falso.

- $10\div 5 = 2$.

---

**Propiedad (de los tres términos).**
Sean $a,b,c\in\mathbb{N}$ tales que $$a+b=c$$ Si $d\in\mathbb{N}$ divide a dos de los términos de esa relación, entonces debe dividir al tercero.
