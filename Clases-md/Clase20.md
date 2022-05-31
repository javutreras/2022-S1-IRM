## Congruencia numérica

**Definición.** Sea $m>1$. Sean $a,b\in\mathbb{Z}$. Si $m\mid (a-b)$, diremos que *$a$ y $b$ son congruentes módulo $m$*, lo que se escribirá
$$a\equiv b\quad(\textrm{mod }m)$$
o también
$$a\equiv_m b$$

**Propiedad.** Dos números son congruentes módulo $m$ si y sólo si dejan el mismo resto al ser divididos por $m$.

**Teorema.** Sea $m>1$ fijo.
- La congruencia módulo $m$ es una relación de equivalencia.

- La congruencia módulo $m$ preserva las operaciones de suma y multiplicación.

- Todo número entero es congruente módulo $m$ a exactamente un elemento del conjunto $\{x\in\mathbb{Z}\,:\,0\le x<m\}$.

---

### Tablas de adición y multiplicación

Gracias a la última propiedad del teorema, se ve que todos los números enteros módulo $m$ son descritos por un conjunto de $m$ elementos. Se pueden escribir estos elementos, y describir las operaciones entre ellos.

---

*Ejemplos.*

- Resolver la ecuación $x^2+1\equiv 0$ módulo $m$, con $m$ entre $2$ y $6$ (ambos inclusive).

- Resolver la ecuación $3x\equiv 0$ módulo $m$, con $m$ entre $2$ y $6$ (ambos inclusive).

---

**Teorema.** Si $m$ es un número primo, la congruencia módulo $m$ satisface la propiedad
$$ xy\equiv_m 0 \Longrightarrow x\equiv_m 0\,\vee\, y\equiv_m 0 $$
Si $m$ es compuesto, no la satisface.

**Teorema.** Si $m$ es un número primo, todo elemento distinto de cero tiene un inverso multiplicativo módulo $m$. Si $m$ es compuesto, no todo elemento tiene inverso.

---

### Colección de resultados varios

- La ecuación $2x^2-3y^2=7$ no tiene soluciones enteras.
- Todo número positivo es congruente módulo $9$ a la suma de sus dígitos.
- *(ONM 2003)* Al número $2^{2003}$ se le suman todos sus dígitos. Al resultado se le suman todos sus dígitos, y así sucesivamente hasta llegar a un solo dígito. Indicar qué digito es.

- Pequeño teorema de Fermat: si $a$ es coprimo con un primo $p$, entonces $$a^{p-1}\equiv 1\quad(\textrm{mod }p)$$
- Si $a$ y $b$ son coprimos con $91$, entonces $a^{12}-b^{12}$ es divisible por $91$.
