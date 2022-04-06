## Más ejemplos de definiciones recursivas

### Ejemplo básico: definición de la suma

Notar que los axiomas de Dedekind-Peano no mencionan ninguna operación aparte del sucesor. Esto significa que las demás operaciones se pueden deducir de los axiomas. Para $n\ge 0$ se define:

$$\begin{cases} m + 0 = m \\ m + S(n) = S(m+n)\end{cases}$$

*Ejercicio.* Calcular $4+3$ a partir de la definición.

### Un ejemplo aplicado: aproximación de una solución de una ecuación

**Problema.** Considerar la función $f(x)=x^2+2x-1$ y la ecuación $f(x)=0$.

> Como $f(0)=-1<0$&nbsp; y &nbsp;$f(1)=2>0$, sabemos que tiene una solución (en los números reales) entre cero y uno.

Considerar la siguiente sucesión infinita de números, construida de forma recursiva para $n\ge 0$: $$\begin{cases}a_0=1 \\ a_{n+1}=\displaystyle\frac{a_n^2+1}{2a_n+2}\end{cases}$$

*Propiedad.* Todos los términos $a_n$ son positivos.
*Idea.* $a_0$ es positivo. Por las leyes de los signos, esto implica que $a_1$ es positivo. Por las leyes de los signos, esto implica que $a_2$ es positivo. Por las leyes de los signos, esto implica que $a_3$ es positivo. Y así sucesivamente.

 *Propiedad.* Todos los términos $a_n$ son menores o iguales a $1$.
 *Idea.* La presentación recursiva se puede escribir de la forma$$\begin{cases}a_0=1 \\ a_{n+1}=\displaystyle\frac{a_n^2+1}{2a_n+2}=\displaystyle\frac{a_n-1}{2}+\displaystyle\frac{1}{a_n+1}\end{cases}$$

*Propiedad.* Todos los términos $a_n$, al ser evaluados en la función $f$, tienen imágenes positivas.
*Idea.* Observar lo siguiente (pasos algebraicos omitidos):
$$\begin{cases}f(a_0)=2 \\ f(a_{n+1}) = f\left(\displaystyle\frac{a_n^2+1}{2a_n+2}\right)=\displaystyle\frac{\left(f(a_n)\right)^2}{4(a_n+1)^2}\end{cases}$$

*Propiedad.* El valor de $f(a_n)$ se hace cada vez más cercano a cero al aumentar $n$.
*Idea.* Observar lo siguiente:
$$\begin{cases}f(a_0)=2 \\ f(a_{n+1}) = \displaystyle\frac{\left(f(a_n)\right)^2}{4(a_n+1)^2}=f(a_n)\cdot\frac{1}{4}\cdot \displaystyle\frac{a_n^2+2a_n-1}{a_n^2+2a_n+1}<f(a_n)\cdot\frac{1}{4}\end{cases}$$

**Conclusión.** Los términos $a_n$ aproximan una solución de la ecuación $f(x)=0$.  Ninguno de ellos es la solución, pero son cada vez más precisos.

---

*Algunas observaciones.*

- Este método parece ser superfluo, porque existe la fórmula cuadrática. Pero con este método llegamos a valores numéricos con operaciones simples: para encontrar valores numéricos en la fórmula cuadrática habría de todas maneras que aproximar una raíz.
- Este método sirve para más ecuaciones que la cuadrática, pero las propiedades se vuelven más difíciles de demostrar.  Por ejemplo, para aproximar la solución de $x^3+2x-1=0$ se utiliza la sucesión recursiva $$\begin{cases}a_0=1 \\ a_{n+1}=\displaystyle\frac{2a_n^3+1}{3a_n^2+2}\end{cases}$$
- Observar que las distintas propiedades de la sucesión recursiva se demostraron también de forma recursiva --- a partir del hecho de que se cumplen para $n=0$, se fueron "transmitiendo" de sucesor en sucesor hasta cubrir todos los números naturales.
