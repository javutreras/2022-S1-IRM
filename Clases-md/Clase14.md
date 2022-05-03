## Coeficiente combinatorio

### Bonus: versión multinomial

**Definición.** Si $k_1+k_2+\ldots +k_n=n$, el *coeficiente multinomial* se define $${n\choose k_1,k_2,\ldots ,k_n} = \frac{n!}{k_1!k_2!\ldots k_n!}$$

Las propiedades del coeficiente binomial tienen versiones más complejas, por ejemplo:

- si $k_1,k_2>0$, $${n+1\choose k_1,k_2,0} = {n\choose k_1-1,k_2,0} + {n\choose k_1,k_2-1,0}$$
- pero si $k_1,k_2,k_3>0$, $${n+1\choose k_1,k_2,k_3} = {n\choose k_1-1,k_2,k_3} + {n\choose k_1,k_2-1,k_3} + {n\choose k_1,k_2,k_3-1}$$

Y el teorema de la potencia queda
$$
\left(\sum_{i=0}^ma_i\right)^n = \sum_{k_i\ge 0, \sum_{i=1}^mk_i=n}{n\choose k_1,k_2,\dots ,k_m}\prod_{i=1}^ma_i^{k_i}
$$

---

## Divisibilidad

Se trabajará en el conjunto de los números naturales con el cero.

**Definiciones.** Sean $a,b\in\mathbb{N}$.
- Si existe $k$ tal que $a+k=b$, se dice que $a$ es *menor o igual que* $b$, y se escribe $a\le b$.

- Si existe $k$ tal que $a\cdot k=b$, se dice que $a$ *divide a* $b$, y se escribe $a\mid b$.

Se puede ver que ambas relaciones son relaciones de orden.

*Observación.* La *división* es una operación que tiene como resultado un número; la *divisibilidad* es una propiedad que puede ser verdadera o falsa:
- $2\mid 6$ es verdadero.

- $3\mid 5$ es falso.

- $10\div 5 = 2$.

---

**Propiedad (de los tres términos).**
Sean $a,b,c\in\mathbb{N}$ tales que $$a+b=c$$ Si $d\in\mathbb{N}$ divide a dos de los términos de esa relación, entonces debe dividir al tercero.

---

### División euclidiana (división con resto)

**Teorema.** Dados dos números naturales $D\ge 0$ (el *dividendo*) y $d\ge 1$ (el *divisor*), existen **únicos** números $q\ge 0$ (el *cuociente*)&nbsp; y &nbsp;$0\le r<d$ (el *resto*) tales que $$D=qd+r$$

*Observación.* Esto también funciona con $D$ entero; en este caso $q$ también es entero. El resto sigue igual entre $0$ y $d-1$.

*Ejemplo.* Encontrar cuociente y resto para $D=-11$, $d=3$.

> Notamos que $11\div 3$ da $3$ con resto $2$. SImplemente cambiar el signo no funciona: porque $3\cdot 3 < 11$ pero $3\cdot (-3) > -11$.
> Lo que hay que notar es que $3\cdot (-4) < -11$. El cuociente de $(-11) \div 3$ es $-4$, y su resto es lo que le falta a $-12$ para llegar a $-11$, que es $1$.
> $$(-11)=(-4)\cdot 3 + 1$$
