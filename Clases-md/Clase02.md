## Conjuntos

**Definición (intuitiva).** Un *conjunto* es un contenedor de elementos especificado únicamente por los elementos que contiene.

*Ejemplos.* Los siguientes son todos el mismo conjunto:
- $\{1,2,3,4\}$
- $\{1,3,4,2\}$
- $\{1,2,4,1,2,3,1\}$
- El conjunto de todos los números enteros del $1$ al $4$, extremos incluidos.

---

**Notación.** Si un elemento $x$ pertenece a un conjunto $C$, se escribe $x\in C$ y se dice que $x$ *pertenece a* $C$.
En caso contrario, se escribe $x\not\in C$ y se dice que $x$ *no pertenece a* $C$.

---

**Definiciones.** Sean $C$, $D$ dos conjuntos. 
- Se dice que $C$ es un *subconjunto* de $D$, o que $C$ está *incluido* en $D$, si todo elemento que pertenece a $C$ pertenece también a $D$. Se denota $C\subseteq D$.
- La *unión* de $C$ y $D$ es el conjunto formado por todos los elementos que estén en al menos uno de los dos conjuntos. Se denota $C\cup D$.  
- La *intersección* de $C$ y $D$ es el conjunto formado por todos los elementos que estén en ambos conjuntos simultáneamente. Se denota $C\cap D$.

*Observación.*
- La inclusión es una *relación* entre dos conjuntos; el hecho que un conjunto sea subconjunto de otro puede ser verdadero o falso. La pertenencia de un elemento a un conjunto también es una relación.
- La unión y la intersección son *operaciones* entre dos conjuntos. Entregan otro conjunto como resultado.

---

### Herramienta clave para demostrar: la generalización

*Idea.* Si se quiere probar que todos los elementos de un conjunto $X$ tienen una propiedad $P$, se puede, en vez de eso, mostrar que un elemento *arbitrario* y *general* del conjunto $X$ tiene la propiedad $P$.

**Ejemplo.** Si $A$ y $B$ son dos conjuntos y se tiene $A\cap B = B$, mostrar que $B\subseteq A$.

*Desarrollo.* Consultando la definición: se quiere poder concluir que todo elemento que pertenece a $B$ pertenece también a $A$.

| | Afirmación | Justificación |
|----|----|----|
|**(A1)**| Sea $x\in B$ arbitrario. | Preparar una generalización sobre todos los elementos de $B$|
|**(A2)**| $A\cap B=B$ | Dato del problema|
|**(A3)** | $x\in A\cap B$ | Deducción a partir de **(A1)** y **(A2)**|
|**(A4)** | $x\in A$ &nbsp;y&nbsp; $x\in B$ | Definición de intersección en **(A3)**|
|**(A5)** | $x\in A$ | Deducción a partir de **(A4)**

A partir de **(A1)** se deduce **(A5)**. Es decir, se tiene que si $x\in B$ entonces $x\in A$.  Como $x$ es un elemento cualquiera de $B$, por generalización se concluye que todo elemento de $B$ está en $A$.

Es decir, $B\subseteq A$.
