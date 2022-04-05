## Axiomas de los números naturales

*Objetivo.* Describir el conjunto de los números naturales a partir de sus propiedades más básicas.

Se desea llegar a una lista óptima de propiedades básicas: donde ninguna sea redundante y a la vez todas sean suficientes: esto significa que sólo el conjunto de los números naturales debe cumplirlas todas.

---

### Axiomas de Dedekind-Peano para el conjunto $\mathbb{N}$

- Hay un elemento $0\in\mathbb{N}$.

>*Nota.* Como veremos, la presentación de los números naturales requiere de un "menor elemento". Se podría realizar de igual manera empezando del número 1 en vez del 0, pero la definición estándar es ésta.

- Hay una función $S:\mathbb{N}\to\mathbb{N}$, la función *sucesor*.

>*Nota.* Recordando la diferencia entre una relación cualquiera y una función, vemos que esto significa que cada elemento $x$ de $\mathbb{N}$ tiene un, y exactamente un, sucesor $S(x)$.

- Números distintos deben tener sucesores distintos.

>*Nota.*  Esto se puede expresar $$n\neq m\Rightarrow S(n)\neq S(m)$$o también por su contrarrecíproco $$S(n)=S(m)\Rightarrow n=m$$
- El número $0$ no es sucesor de ningún número.

>*Nota*. Esto se puede expresar $$\forall n\,S(n)\neq 0$$Esto justifica la idea de que 0 es el "menor elemento" del conjunto $\mathbb{N}$.
- Se cumple la *propiedad inductiva*: para cualquier propiedad $\mathtt{P}$ que puedan tener los números naturales, si
	- el elemento mínimo $0$ tiene la propiedad $\mathtt{P}$ y además
	- siempre que algún número $n$ tenga la propiedad $\mathtt{P}$, su sucesor $S(n)$ también la tendrá

	entonces todos los números naturales tendrán la propiedad $\mathtt{P}$.

>*Nota.* La propiedad inductiva se puede entender intuitivamente como 
>> No hay ningún natural al que no se pueda llegar desde 0 después de suficientes sucesores.

---

*Observación.* Los axiomas se pueden escribir reemplazando el elemento $0$ con el $1$, y resulta una definición equivalente. Lo importante es que haya un elemento "especial" que no sea sucesor de ningún otro y del cual comiencen las propiedades $\mathtt{P}$ del axioma inductivo.

---

### Definiciones recursivas

*Ejemplo.* Se intenta definir una función $f_1:\mathbb{N}\to\mathbb{N}$ de la forma siguiente: $$\begin{cases}f_1(0) = 1 \\ f_1(n+1) = 2\cdot f_1(n)\textrm{ si }n\ge 0 \end{cases}$$

¿Está esta definición completa? ¿Se puede calcular, por ejemplo, $f_1(5)$?

*Observación.* Este tipo de definición, donde se define una operación o propiedad para el/los caso(s) básico(s) y, para los demás casos, se indica cómo simplificar la operación o propiedad para acercarse a los casos iniciales, se conoce como *definición recursiva*.
Se basan en el hecho que, desde cualquier número natural, se puede retroceder en los sucesores hasta llegar al inicio.

