## Máximo común divisor

**Definición.** El *máximo común divisor* de dos números naturales, al menos uno de ellos positivo, es el mayor de todos sus divisores comunes. Se denota por $\operatorname{MCD}$.

*Observación.* Para garantizar que todo par de números tiene un máximo común divisor, hay que sortear dos obstáculos: que siempre haya algún divisor común, y que no crezcan sin cota al infinito.

El primer obstáculo se resuelve observando que el número $1$ siempre es divisor común. El segundo obstáculo se resuelve al notar que los divisores comunes de $a$ y $b$ son $\le a$ y $\le b$.

---

*Problema.* Determinar el máximo común divisor de dos números dados sin tener que encontrar las listas de divisores de ambos.

**Propiedad.** Si la división $a\div b$ es exacta, entonces $$\operatorname{MCD}(a,b)=b$$

**Propiedad.** Si la división $a\div b$ deja resto $r$, entonces $$\operatorname{MCD}(a,b) = \operatorname{MCD}(b,r)$$

---

### Algoritmo de Euclides para el máximo común divisor

En base a las dos propiedades señaladas, se puede construir el siguiente algoritmo para determinar $\operatorname{MCD}(a,b)$, con $a>b$:

- Si $b\mid a$, entonces $\operatorname{MCD}(a,b)=b$.

- Si $a\div b$ deja un resto $r$, entonces se calcula $\operatorname{MCD}(b,r)$, que es el mismo problema pero con números menores.

Por descenso infinito, este método obtiene el máximo común divisor buscado.

---

*Ejemplo.* Encontrar $\operatorname{MCD}(513,378)$ usando el algoritmo de Euclides.

---

**Teorema (Bézout).** Sea $d=\operatorname{MCD}(a,b)$. Existen números enteros $s,t$ tales que $$sa + tb = d$$

*Demostración.* "Deshacer" el algoritmo de Euclides!

---

**Definición.** Dos números se dicen *coprimos* si su máximo común divisor es $1$. Si $a$ y $b$ son coprimos, se escribe $a\,\perp\,b$.

**Teorema.** Si $a\mid bc$ &nbsp;y&nbsp; $a\,\perp\,b$, entonces $a\mid c$&nbsp;.

---

### Ecuaciones diofantinas

*Problema.* Resolver la ecuación $$15x+6y=22$$ en los números enteros.

*Problema.* Resolver la ecuación $$15x+6y=21$$ en los números enteros.




