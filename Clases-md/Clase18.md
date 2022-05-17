## Números primos

**Teorema (lema de Euclides).** Sea $n>1$ un número natural. Las siguientes dos propiedades son equivalentes:

- $st=n\,\Rightarrow\,s=1\,\vee\,t= 1$ *(irreducibilidad)*

- $n\mid ab\,\Rightarrow\, n\mid a\,\vee\,n\mid b$ *(primalidad)*

**Definición.** Un número natural que satisface las condiciones del teorema anterior se conoce como un *número primo*.

*Observación.* El contrarrecíproco de la segunda condición dice: "si ningún factor es múltiplo de un primo $p$, es imposible que el producto de ellos sea múltiplo de $p$"

---

Con esto los números naturales quedan separados en subconjuntos:

- la *unidad*, que es el número $1$, que en términos de divisibilidad divide a todos los números naturales;
- el *cero*, que en términos de divisibilidad no divide a ningún otro número;

- los *números primos*; y
- los *números compuestos*, que son los números mayores que $1$ que no son primos.

---

**Lema.** Todo número compuesto es divisible por algún número primo.

**Teorema (Euclides).** Existen infinitos números primos.

---

*Problema.* ¿Es posible encontrar una fórmula que entregue números primos?

Por un tiempo se estudió $n^2-n+41$, pensando que al evaluarse en distintos valores de $n$ entregaría sólo números primos. Esto porque ocurre para los valores pequeños de $n$, pero al evaluar en $n=41$ se ve que el resultado ha de ser múltiplo de $41$.

En general, no se puede construir una fórmula polinomial en una variable que entregue sólo valores primos; al evaluar $n$ en el término libre, como en el ejemplo anterior, se construirá un múltiplo de ese valor.

---

*Problema.* ¿Se podrá con algo más complicado que un polinomio?

**Proposición (Fermat).** Si un número $n$ no es una potencia de $2$, entonces $2^n+1$ es compuesto.

Fermat estudió entonces el recíproco: ¿podemos asegurar que $2^{2^n}+1$ siempre será primo? Lo verificó manualmente hasta $n=4$, pero un siglo después Euler mostró que $$2^{2^5}+1 = 4294967297 = 641\cdot 6700417$$

---

**Lema.** Todo número mayor que $1$ se puede escribir como un producto de números primos.

**Lema.** Si $p, q$ son números primos y $p\mid q$, entonces $p=q$.

**Teorema (factorización única).** Todo número mayor que $1$ se puede escribir como un producto de números primos de forma **única** (salvo el orden de los factores).

---

*Definición.* Si $p$ es un número primo y $x\neq 0$ un número natural, el *orden de $p$ en $x$*, $\operatorname{ord}_p(x)$, es la cantidad de veces que aparece $p$ en la factorización prima de $x$.
