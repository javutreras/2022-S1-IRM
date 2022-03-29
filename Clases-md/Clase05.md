## Propiedades de las relaciones binarias

**Definición.** Sea $R$ una relación binaria entre elementos de $A$ y $B$. Se definen los conjuntos *imagen directa de $a\in A$*: $$R(a)=\{x\,:\,(a,x)\in R\}$$
e *imagen inversa de $b\in B$*: $$R^{-1}(b)=\{x\,:\,(x,b)\in R\}$$

**Definición.** La misma definición anterior se puede realizar a subconjuntos. Se definen la *imagen directa de $A_0\subseteq A$*: $$R(A_0)=\bigcup_{a\in A_0}R(a)$$
y la *imagen inversa de $B_0\subseteq B$*: $$R^{-1}(B_0)=\bigcup_{b\in B_0}R^{-1}(b)$$

---

**Definición.** Sea $R$ una relación binaria entre elementos de $A$ y $B$. Si para cada $a\in A$ el conjunto imagen directa $R(a)$ tiene exactamente un elemento, decimos que $R$ es una *función* $R:A\to B$, y a ese único elemento lo llamamos *la imagen* de $a$ bajo $R$, y lo denotamos también como $R(a)$.

---

*Notación.* Si $R$ es una relación binaria entre un conjunto $A$ y un conjunto $B$, el conjunto $A$ se llama el *dominio* de $R$, y el conjunto $B$ el *codominio* de $R$.

*Notación.* Una *relación binaria sobre un conjunto* $A$ es una relación cuyo dominio y codominio son ambos el conjunto $A$.

---

*Ejemplos.* Considerar las siguientes relaciones binarias sobre $\R$:

- $R_1 = \{(x,y)\,:\,x\le y\}$

- $R_2 = \{(x,y)\,:\,x+y=0\}$
- $R_3=\{(x,y)\,:\,|x|=|y|\}$
- $R_4=\{(x,y)\,:\,y=x^2\}$

---

### Clasificación de las relaciones binarias sobre un conjunto

**Definiciones.** Sea $R$ una relación sobre un conjunto $A$.

- Se dice que $R$ es *reflexiva* si para todo $x\in A$ se tiene $(x,x)\in R$.

- Se dice que $R$ es *simétrica* si cada vez que $(x,y)\in R$ se tiene $(y,x)\in R$.
- Se dice que $R$ es *antisimétrica* si cada vez que $(x,y)\in R\,\wedge\,(y,x)\in R$ se tiene $x=y$.
- Se dice que $R$ es *transitiva* si cada vez que $(x,y)\in R\,\wedge\, (y,z)\in R$ se tiene $(x,z)\in R$.

---

**Definiciones.** 
- Una relación es *de equivalencia* si es reflexiva, simétrica y transitiva.
	- Si $R$ es una relación de equivalencia y $(a,b)\in R$, se dice que $a$ y $b$ son *equivalentes*. Se escribe $a\equiv_R b$.

- Una relación es *de orden* si es reflexiva, antisimétrica y transitiva.
	- Si $R$ es una relación de orden y $(a,b)\in R$, se dice que $a$ es *menor o igual que* $b$, *según* $R$. Se escribe $a\le_R b$.

---

*Ejemplos.*
- La relación *dejar el mismo resto al dividir por* $2$ es una relación de equivalencia en $\mathbb{N}^+$.

- La relación *dividir a* es una relación de orden en $\mathbb{N}^+$.
