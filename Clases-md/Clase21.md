## Congruencia numérica (continuación)

### Criterios de divisibilidad:

Considerar el número de escritura $abcde$, es decir,
$$10000a+1000b+100c+10d+e$$

Se tienen las siguientes congruencias:

- $10000a+1000b+100c+10d+e\equiv e \quad(\textrm{mod }2)$

- $10000a+1000b+100c+10d+e\equiv a+b+c+d+e \quad(\textrm{mod }3)$
- $10000a+1000b+100c+10d+e\equiv 2d + e \quad(\textrm{mod }4)$
- $10000a+1000b+100c+10d+e\equiv e \quad(\textrm{mod }5)$
- La divisibilidad por $6$ es equivalente a la divisibilidad por $2$ y por $3$, porque son factores coprimos.
- $10000a+1000b+100c+10d+e\equiv 10(1000a+100b+10c+d-2e) \quad(\textrm{mod }7)$
- $10000a+1000b+100c+10d+e\equiv 4c+2d+e \quad(\textrm{mod }8)$
- $10000a+1000b+100c+10d+e\equiv a+b+c+d+e \quad(\textrm{mod }9)$
- La divisibilidad por $10$ es equivalente a la divisibilidad por $2$ y por $5$, porque son factores coprimos.
- $10000a+1000b+100c+10d+e\equiv a-b+c-d+e \quad(\textrm{mod }11)$
- La divisibilidad por $12$ es equivalente a la divisibilidad por $4$ y por $3$, porque son factores coprimos.
- $10000a+1000b+100c+10d+e\equiv 10(1000a+100b+10c+d-9e) \quad(\textrm{mod }13)$

---

### Pequeño teorema de Fermat

**Teorema (Fermat).** Sean $p$ un número primo y $a$ un entero no divisible por $p$. Se tiene
$$ a^{p-1}\equiv 1\quad (\textrm{mod }p)$$

*Ejemplo.* Si $a$ y $b$ son coprimos con $91$, entonces $a^{12}-b^{12}$ es divisible por $91$.
