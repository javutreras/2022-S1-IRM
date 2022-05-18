## Teorema fundamental de la aritmética

**Teorema (factorización única).** Todo número mayor que $1$ se puede escribir como un producto de números primos de forma **única** (salvo el orden de los factores).

---

### Orden de un número en un primo

*Definición.* Si $p$ es un número primo y $x\neq 0$ un número natural, el *orden de $p$ en $x$*, $\operatorname{ord}_p(x)$, es la cantidad de veces que aparece $p$ en la factorización prima de $x$.

*Ejemplos.*

- $\operatorname{ord}_2 (12) = 2$

- $\operatorname{ord}_5(1000)=3$
- $\operatorname{ord}_7(10)=0$
- $\operatorname{ord}_p(1) = 0$ para cualquier primo $p$.

---

**Propiedad.** Sean $n,m$ dos números naturales. $n$ divide a $m$ si y sólo si, para todo primo $p$, $\operatorname{ord}_p(n)\le\operatorname{ord}_p(m)$.

**Propiedad.** Sean $n,m$ dos números naturales. Para todo primo $p$, $$\operatorname{ord}_p(\operatorname{MCD}(m,n)) = \min(\operatorname{ord}_p(m),\operatorname{ord}_p(n))$$


