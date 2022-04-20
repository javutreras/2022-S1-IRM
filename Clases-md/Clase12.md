## Coeficiente combinatorio

**Propiedades.**

Las siguientes propiedades se pueden ver a partir de la fórmula, pero también se pueden entender del punto de vista combinatorio:

- ${n\choose 0} = 1$

- ${n\choose n} = 1$ 
- ${n\choose 1} = n$
- ${n\choose k} = {n\choose n-k}$
- Definición recursiva alternativa: $$\begin{cases} {n\choose 0}=1 \\ {n+1\choose k+1} = \frac{n+1}{k+1}{n\choose k}\end{cases}$$
- Definición recursiva alternativa: $$\begin{cases} {n\choose 0} = 1 \\{n\choose n} = 1 \\ {n+1\choose k+1}={n\choose k} + {n\choose k+1}\end{cases}$$
- $\displaystyle\sum_{i=0}^n {n\choose i} = 2^n$

**Corolario.** Triángulo de Pascal.

**Corolario.** $\displaystyle\sum_{i=0}^n (-1)^n{n\choose i} = 0$

**Corolario (Inclusión-exclusión).**

**Corolario (Teorema del binomio).** Para $n\in\mathbb{N}$,$$(a+b)^n = \sum_{i=0}^n{n\choose i}a^ib^{n-i}$$
