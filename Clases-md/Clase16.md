## Ecuaciones diofantinas

A lo largo de esta sección, sólo se trabajará con números enteros.

**Definición.** Una ecuación diofantina es una ecuación en *dos* incógnitas, de la forma $$ax+by=c$$ con $a,b,c$ cantidades fijas ($a,b\neq 0$) y $x,y$ incógnitas.
Una *solución* de esta ecuación es un par de valores $(x_0,y_0)$ tales que la sustitución $x=x_0$, $y=y_0$ satisface la ecuación original.

Asociados a una ecuación hay tres problemas:

- **Determinar existencia de soluciones.** Decidir si acaso una ecuación tiene alguna solución o no.

	Un ejemplo de esto último sería $2x+4y=5$, donde como el lado izquierdo es par y el lado derecho impar es imposible que haya soluciones. Pero se necesita un método más general que estudiar pares/impares.

- **Encontrar una solución.** Una cosa es saber si una ecuación tiene soluciones - pero otra es encontrar alguna de estas soluciones. Podría ser que hubiera múltiples, pero se necesita empezar con alguna.

- **Resolver la ecuación.** Una ecuación se considera resuelta cuando se tienen descritas *todas* sus soluciones, sean cuántas sean (incluso si son cero - en ese caso la resolución es la justificación de por qué no hay).

---

**Propiedad.** La ecuación $ax+by=c$ tiene soluciones si y sólo si $\operatorname{MCD}(a,b) \mid c$.

> Demostración.
>
> Si la ecuación tiene alguna solución, entonces evaluando en esa solución se puede ver que el lado izquierdo es divisible por $\operatorname{MCD}(a,b)$. Entonces el lado derecho, $c$, también debe serlo.
> 
> Si $\operatorname{MCD}(a,b) \mid c$, entonces a partir de la expresión dada por el teorema de Bézout se puede amplificar para hacer que el lado derecho sea igual a $c$.

---

**Propiedad.** Sean $(x_1,y_1)$, $(x_2,y_2)$ dos soluciones de una ecuación $ax+by=c$. Entonces $(x_2-x_1 , y_2-y_1)$ es solución de la ecuación $ax+by=0$.

> Demostración.
>
>$$\begin{array}{cccccccc} &&ax_2&+&by_2&=&c&\\ -&(&ax_1&+&by_1&=&c&) \\[2mm] \hline \\[-2mm] &&a(x_2-x_1)&+&b(y_2-y_1)&=&0&&\end{array}$$

---

*Definición.* Dada la ecuación $ax+by=c$, la ecuación $ax+by=0$ se conoce como su *ecuación homogénea asociada*.

---

### Método para resolver ecuaciones diofantinas de la forma $Ax+By=C$

1. Verificar existencia de soluciones usando el $MCD$. Si las hay, simplificar la ecuación por el $MCD$.

2. Determinar una solución particular deshaciendo el algoritmo de Euclides.
	- Despejar restos
	- Reemplazar desde la última ecuación hacia la primera
	- Amplificar al final si resulta necesario

3. Determinar las soluciones de la ecuación homogénea asociada.
	- Verificar coprimalidad
	- Atención a los signos!

4. Construir el conjunto de todas las soluciones sumando la solución particular con cada solución homogénea.

---

*Ejemplo.* Se compran paquetes de galletas, a $500 cada uno, y botellas de bebida, a $1.100 cada una. En total se gastan $24.000. Determinar todas las compras posibles que logran este valor.

---

**Teorema (chino del resto).** Sean $A$, $B$ dos números coprimos, y sean $r$ un resto posible de la división por $A$ y $s$ un resto posible de la división por $B$.
Existen números que, simultáneamente, dejan resto $r$ al ser divididos por $A$ y resto $s$ al ser divididos por $B$.

*Ejemplo.* Determinar los números que dejan resto $6$ al ser divididos por $15$ y resto $3$ al ser divididos por $17$.
