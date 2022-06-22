## Cardinalidad y el infinito

**Definición.** Sean $A$, $B$ dos conjuntos.
- Si existe una función $f:A\to B$ inyectiva diremos que $A$ es *subpotente* a $B$, lo que se escribe $|A|\le |B|$.

- Si existe una función $f:A\to B$ biyectiva diremos que $A$ y $B$ son *equipotentes*, lo que se escribe $|A| = |B|$.

**Teorema (Cantor-Bernstein-Schröder).** Si $A$ es subpotente a $B$ y $B$ es subpotente a $A$ entonces $A$ y $B$ son equipotentes.

*Observación.* A partir de la notación se podría pensar que este teorema es obvio, pero es al revés: la notación existe gracias a este teorema. La demostración de este teorema requiere construir una biyección a partir de funciones inyectivas en ambas direcciones.

---

*Ejemplo.* La función $f:\mathbb{N}\to \mathbb{Z}$ dada por $f(n)=\frac{n}{2}$ si $n$ es par y $f(n)=-\frac{n+1}{2}$ si $n$ es impar es una biyección.

Por consiguiente $\mathbb{N}$ y $\mathbb{Z}$ son equipotentes.

---

### Conjuntos finitos e infinitos

**Definición.** $|\emptyset| = 0$.

**Definición.** Sea $n$ un número natural positivo. Si un conjunto $C$ es equipotente a $\{1,2,\ldots ,n\}$, diremos que $|C|=n$.

**Definición.** Si $|C|=n$ para algún número natural $n$, diremos que $C$ es un *conjunto finito*. En caso contrario se dice que $C$ es un *conjunto infinito.*

---

*Observación.* Si se tienen dos conjuntos que cumplen $A\subseteq B$, entonces la función $f:A\to B$ dada por $f(x)=x$ es inyectiva. Se puede garantizar que $|A|\le |B|$.

Pero incluso si $B-A\neq\emptyset$ no se puede garantizar que $|A|$ sea estrictamente menor que $|B|$.
