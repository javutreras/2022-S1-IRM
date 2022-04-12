## Demostración por inducción

Recordar el quinto axioma de los números naturales:

- Se cumple la *propiedad inductiva*: para cualquier propiedad $\mathtt{P}$ que puedan tener los números naturales, si
	- el elemento mínimo $0$ tiene la propiedad $\mathtt{P}$ y además
	- siempre que algún número $n$ tenga la propiedad $\mathtt{P}$, su sucesor $S(n)$ también la tendrá

	entonces todos los números naturales tendrán la propiedad $\mathtt{P}$.

---

A partir de esta propiedad se puede idear un nuevo método de demostración.

### Inducción

Sea $\texttt{P}$ una propiedad de los números naturales, o de objetos indexados por los números naturales. Si el número/objeto $0$ tiene la propiedad $\texttt{P}$, y además se tiene $$n\in\texttt{P}\Rightarrow n+1\in \texttt{P}$$
entonces todos los números/objetos tienen la propiedad $\texttt{P}$.

*Ejemplo.* De la clase pasada: para $n\ge 0$, 
$$\begin{cases}a_0=1 \\ a_{n+1}=\displaystyle\frac{a_n^2+1}{2a_n+2}\end{cases}$$

Mostraremos formalmente que todos los términos $a_n$ son positivos.

Sea $\texttt{P}=\{n\in\mathbb{N}\,:\,a_n >0\}$. Claramente $0\in\mathtt{P}$.

Supongamos que para algún número natural $n$ se tiene $n\in\texttt{P}$. Esto significa que $a_n>0$. Pero entonces $$a_{n+1}=\displaystyle\frac{a_n^2+1}{2a_n+2} >0$ (por las leyes de los signos), y entonces $a_{n+1}\in\texttt{P}$.

Conclusión: $\texttt{P}=\mathbb{N}$, es decir, para todo natural $n$ se tiene $a_n>0$.

---

### Inducción generalizada

Sea $\mathtt{P}$ una propiedad que puedan tener los números naturales. Si se cumple que

- algún número $n_0$ tiene la propiedad $\mathtt{P}$; y

- cada vez que un número $n$ tiene la propiedad $\mathtt{P}$, su sucesor $n+1$ también la tiene,

entonces todos los números naturales mayores o iguales a $n_0$ tienen la propiedad $\mathtt{P}$.

*Ejemplo.* En un polígono con todos sus ángulos interiores menores que $180^\circ$ la suma de sus ángulos exteriores es $360^\circ$.

*Demostración.* Sea $\texttt{P}$ el conjunto de todos los números naturales $n$ tales que todos los polígonos de $n$ lados cumplen el enunciado.

- El caso base es $n=3$ --- sabido por propiedades de triángulos.
- El paso inductivo requiere ser explicado con un dibujo.

---

### Inducción fuerte

Sea $\mathtt{P}$ una propiedad que puedan tener los números naturales. Si se cumple que

- algún número $n_0$ tiene la propiedad $\mathtt{P}$; y

- si los números menores a $n$ tienen la propiedad $\mathtt{P}$, entonces $n$ también la tiene,

entonces todos los números naturales mayores o iguales a $n_0$ tienen la propiedad $\mathtt{P}$.

*Ejemplo.* Mostrar que con suficientes monedas de \$3 y \$5 se puede hacer cualquier monto exacto desde \$8 en adelante.

---

**Teorema (buen orden).** Todo subconjunto no vacío de los números naturales tiene un menor elemento.

*Demostración.* Por contrarrecíproco. Sea $X$ un subconjunto de los números naturales sin menor elemento. Sea $\texttt{P}$ el conjunto de números que no están en $X$.

- $0\in \texttt{P}$; de lo contrario sería el menor elemento de $X$.
- Si todos los números menores a algún $n$ están en $\texttt{P}$, entonces ninguno de ellos está en $X$; entonces $n$ tampoco está en $X$, o si no sería su menor elemento. Por consiguiente $n\in\texttt{P}$.

Conclusión: $\texttt{P}=\mathbb{N}$, y luego $X=\emptyset$.
