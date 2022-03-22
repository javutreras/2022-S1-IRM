## Métodos de demostración

### Estructura de un teorema

El enunciado de un teorema consta de dos afirmaciones o conjuntos de afirmaciones: la(s) *hipótesis* y la(s) *tesis*.

Un teorema afirma que, en aquellas situaciones donde las hipótesis sean verdaderas, las tesis deben ser también verdaderas.

*Importante.* Si en una situación no se cumplen las hipótesis de un teorema, entonces el teorema no se puede utilizar para concluir que las tesis sean verdaderas o falsas.

*Ejemplos.*

- Teorema:
	- Hipótesis: $\triangle ABC$ es un triángulo rectángulo, $a,b$ son las longitudes de sus catetos y $c$ la longitud de su hipotenusa.
	- Tesis: $a^2+b^2=c^2$.

- Teorema:
	- Hipótesis: $n$ es un número natural y la escritura de $n$ termina en los dígitos $0$ ó $5$.
	- Tesis: $n$ es múltiplo de $5$.

- Teorema:
	- Hipótesis: $a$ y $b$ son dos números naturales de la misma paridad, es decir, ambos pares o ambos impares.
	- Tesis: $a+b$ &nbsp;y&nbsp; $a-b$&nbsp; son pares.

---

### Demostración directa

**Razonamiento.** La implicación $H\rightarrow T$ se busca demostrar obteniendo deducciones a partir de $H$ hasta llegar a $T$.

**Proposición.** Sean $A$, $B$, $C$ tres conjuntos. Si $A\subseteq B$ y $B\subseteq C$, entonces $$A\subseteq C$$

*Demostración.* Queremos demostrar que todo elemento de $A$ está en $C$:
- Sea $x\in A$ *(preparación de una generalización)*.
- Sabemos que $A\subseteq B$ *(dato del problema)*.
	- Es decir, todo elemento de $A$ está en $B$.
- Se deduce que $x\in B$.
- Sabemos que $B\subseteq C$ *(dato del problema)*.
	- Es decir, todo elemento de $B$ está en $C$.
- Se deduce que $x\in C$, que era a lo que se quería llegar.

*Otra forma de presentarla.* Sea $x\in A$. Como $A\subseteq B$, se deduce que $x\in B$. De la misma forma, como $B\subseteq C$, se deduce que $x\in C$. Por consiguiente, todo elemento de $A$ está en $C$, y se concluye que $A\subseteq C$, como se pedía.

---

### Demostración por contrarrecíproco

**Razonamiento.** La implicación $H\rightarrow T$ se busca demostrar obteniendo deducciones a partir de $\sim T$ hasta llegar a $\sim H$.

**Proposición.** Sean $A$, $B$ dos conjuntos. Si $B\subseteq A$, entonces $$A\cap B=B$$

*Demostración.* Procederemos por contrarrecíproco; es decir, se planea demostrar que si $A\cap B\neq B$ entonces $B\not\subseteq A$.

- $A\cap B\neq B$ (dato). La desigualdad de conjuntos puede ser dada por dos motivos:
	- o hay elementos en $A\cap B$ que no están en $B$;
	- o hay elementos en $B$ que no están en $A\cap B$.
- Es imposible que haya elementos en $A\cap B$ que no estén en $B$, puesto que esto significaría que están en $A$ y en $B$ y no en $B$ al mismo tiempo.
- Se deduce que hay elementos en $B$ que no están en $A\cap B$.
	- Es decir, hay elementos en $B$ que no están en $A$ y $B$ al mismo tiempo.
- Se deduce que hay elementos en $B$ que no están en $A$.
	- Es decir, $B\not\subseteq A$, como se quería demostrar.

---

### Demostración por reducción al absurdo

**Razonamiento.** La implicación $H\rightarrow T$ se busca demostrar por descarte: se deduce a partir de $H\,\wedge\,\sim T$ hasta llegar a una contradicción, algo imposible.

**Proposición.** Sean $A$, $B$ dos conjuntos. Si $A\cap B=B$, entonces $$B\subseteq A$$

*Demostración.* Supongamos que no es así. Existirían dos conjuntos $A$, $B$ tales que $A\cap B=B$ pero $B\not\subseteq A$.

- $B\not\subseteq A$ *(dato)*.
- deducción: existe un elemento $x\in B$ que cumple $x\not\in A$.
- $A\cap B=B$ *(dato)*.
- deducción: como $x\in B$, entonces $x\in A\cap B.$
	- es decir, $x\in A$ &nbsp;y &nbsp;$x\in B$.
- deducción: $x\not\in A$ &nbsp;y &nbsp;$x\in A$.

Como se deduce una contradicción, la proposición es verdadera.

---

### Contraejemplos

**Razonamiento.** Si una implicación $H\rightarrow T$ no es verdadera, significa que existe alguna situación donde $H$ y $\sim T$ se cumplen simultáneamente.

**¿Posible proposición?.** Sean $A$, $B$ dos conjuntos. Si $A\cap B=A$, entonces $$B\subseteq A$$

*Contraejemplo.* Notamos que con $A=\{1,2,3\}$ &nbsp;y&nbsp; $B=\{1,2,3,4,5\}$ se cumple que $A\cap B=A$ pero no se cumple la conclusión $B\subseteq A$.

*Conclusión.* No es cierto que si $A\cap B=A$ entonces $B\subseteq A$.
