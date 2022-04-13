## Principios de conteo

**Definición (informal).** La *cardinalidad* de un conjunto es "la cantidad de elementos que contiene". Se denota $|A|$ o $\operatorname{card}(A)$.

---

**Teorema (Principio del palomar).** Si se reparten $m$ elementos entre $n$ grupos, y $m>n$, entonces siempre habrá un grupo con más de un elemento.

*Demostración.* Por reducción al absurdo. Supongamos que es posible repartirlos de otra forma, es decir, haciendo que en cada grupo hayan 0 ó 1 elementos. Entonces el total de elementos sería a lo más $1\cdot n = n$, lo que contradice el hecho de que $m>n$.

*Ejemplo.* Si se escogen cinco números del conjunto $\{1,2,\ldots ,8\}$, hay dos de ellos que suman 9.

*Ejemplo.* En una reunión de 5 personas algunas se saludan entre sí antes de comenzar. Mostrar que hay dos personas que realizan la misma cantidad de saludos.

---

*Observación.* En términos de funciones, el principio del palomar dice: si $A$, $B$ son conjuntos finitos y $|A|>|B|$, entonces toda función $f:A\to B$ debe repetir valores, es decir, debe haber dos elementos distintos $x,y\in A$ tales que $f(x)=f(y)$.

---

*Definición/notación.* Si $r$ es un número real, el menor entero mayor o igual a $r$ se denota $\lceil r\rceil$.
Se tiene:
- $\lceil r\rceil\in\mathbb{Z}$

- $\lceil r\rceil -1 <r\le \lceil r\rceil$

*Ejemplos.*
- $\lceil 3\rceil = 3$

- $\lceil \frac{5}{4}\rceil = 2$
- $\lceil -\frac{7}{2}\rceil = -3$ (recordar que $-4<-3.5<-3$)

**Teorema (principio del palomar fuerte).** Si se reparten $m$ elementos entre $n$ grupos, entonces siempre habrá un grupo con al menos $\lceil\frac{m}{n}\rceil$ elementos.

*Ejemplo*. En un estadio con 80000 personas, hay al menos 219 que están de cumpleaños el mismo día.
