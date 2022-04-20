## Conteo y combinatoria

### Principio de inclusión-exclusión

*Problema.* En general, $|A\cup B| \neq |A| + |B|$, puesto que un elemento que esté presente en $A$ y en $B$ se contará dos veces en la suma del lado derecho.

**Teorema (inclusión-exclusión para dos conjuntos).** Sean $A,B$ conjuntos finitos. Se tiene
$$
|A\cup B| = |A| + |B| - |A\cap B|
$$

**Teorema (inclusión-exclusión para tres conjuntos).** Sean $A,B,C$ conjuntos finitos. Se tiene
$$
|A\cup B\cup C| = |A| + |B| + |C| - |A\cap B| - |A\cap C| - |B\cap C| + |A\cap B\cap C|
$$

*Demostración.* Directa, por casos. Se distinguen ocho casos, dependiendo de la pertenencia o no a cada conjunto:

- **Caso 000** Si un elemento no pertenece a $A$ ni a $B$ ni a $C$, aporta $0$ al lado izquierdo y $0$ al lado derecho.

- **Caso 100** Si un elemento pertenece a $A$ pero no a $B$ ni a $C$, aporta $1$ al lado izquierdo y $1+0+0-0-0-0+0$ al lado derecho.

- **Caso 010** Si un elemento no pertenece a $A$, sí a $B$, pero no a $C$, aporta $1$ al lado izquierdo y $0+1+0-0-0-0+0$ al lado derecho.
- **Caso 001**

- **Caso 110** Si un elemento pertenece a $A$ y a $B$, pero no a $C$, aporta $1$ al lado izquierdo y $1+1+0-1-0-0+0$ al lado derecho.
- **Caso 101**
- **Caso 011**
- **Caso 111** Si un elemento pertenece a $A$, a $B$ y a $C$, aporta $1$ al lado izquierdo y $1+1+1-1-1-1+1$ al lado derecho.

**Caso para cuatro conjuntos.**
$$|A\cup B\cup C\cup D| =$$ $$|A|+|B|+|C|+|D|$$ $$-|A\cap B|-|A\cap C|-|A\cap D|-|B\cap C|-|B\cap D|-|C\cap D| $$ $$ +|A\cap B\cap C|+|A\cap B\cap D|+|A\cap C\cap D|+|B\cap C\cap D|$$ $$- |A\cap B\cap C\cap D|$$

---

### Combinatoria

*Problema general.* Dada una situación que se puede ejecutar de diversas formas, contar el número de formas en que se puede realizar.

*Situación.* Se debe realizar un número $n$ de elecciones en orden.
- La primera elección es de una opción de entre $k_1$ posibilidades.
- La segunda elección es de una opción de entre $k_2$ posibilidades.
- La tercera elección es de una opción de entre $k_3$ posibilidades.
$$\vdots$$
- La $n$-ésima elección es de una opción de entre $k_n$ posibilidades.

**Teorema.** La cantidad de formas posibles de realizar las elecciones de la situación anterior es $$k_1\cdot k_2\cdot k_3\cdot\ldots\cdot k_n$$

*Demostración.* Por inducción sobre $n$.

*Ejemplo.* Si $|A|=m$ y $|B|=n$, determinar la cantidad de funciones que existen con dominio $A$ y codominio $B$.

*Ejemplo.* Si $|A|=n$, determinar la cantidad de subconjuntos que tiene $A$.

*Ejemplo.* Si se tienen $n$ personas, determinar la cantidad de formas en que se sentar en una hilera de $n$ asientos.

*Ejemplo.* Si se tienen $n$ personas, determinar la cantidad de formas en que se sentar alrededor de una mesa redonda con $n$ asientos (con simetría!).

*Ejemplo.* De un grupo de $n$ elementos se debe escoger un subgrupo ordenado de $k$ elementos. Determinar la cantidad de formas en que se puede hacer esto.

---

### Coeficiente combinatorio

*Situación.* De un grupo de $n$ elementos se debe escoger un subgrupo de $k$ elementos. No importa el orden de estos elementos.

**Teorema.** La cantidad de formas de realizar la elección de la situación es $$\frac{n!}{k!(n-k)!}$$ lo que se escribe $n\choose k$ y se conoce como el *coeficiente combinatorio de n sobre k*.

*Observación.* El coeficiente combinatorio $n\choose k$ tiene una definición recursiva para $n\ge k\ge 0$: $$\begin{cases} {n\choose 0 }= 1 \\ {n+1\choose k+1} = \frac{n+1}{k+1}{n\choose k}\end{cases}$$




