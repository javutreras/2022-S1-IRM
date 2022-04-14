## Ejemplo: compresión de datos sin pérdida

El objetivo de este material adicional es mostrar una aplicación adicional del principio del palomar. Se presentan algunas ideas de forma intuitiva y sin detalles para no sobrecargar la exposición.

### Propiedades básicas

- Un archivo está formado por código, y almacenar este código es lo que gasta espacio en un disco.
- Dado un tamaño $T$ de archivo (1 GB, 100kB, etc), el conjunto de todos los archivos posibles de tamaño menor o igual a $T$ es un conjunto finito $X_T$.
- La compresión de archivos se puede pensar como una función $f$ que convierte un archivo en otro archivo.

### Desarrollo del ejemplo

- Es de esperar que, al aplicar la compresión a un archivo de tamaño menor o igual a $T$, resulte un archivo de tamaño menor o igual a $T$. Esto sería porque **la compresión no debería aumentar el tamaño de un archivo**.
- Para algún tamaño $T$, es de esperar que algún archivo $\omega$ de tamaño mayor que $T$, al ser comprimido, resulte en otro archivo de tamaño menor o igual a $T$. Esto sería porque **la compresión debería disminuir el tamaño de algunos archivos**.
- Pero entonces ocurre lo siguiente: $$f:X_T\cup\{\omega\}\to X_T$$ y entonces el dominio tiene cardinalidad mayor en uno que el codominio.
- Por el principio del palomar, esto significa que existen dos archivos distintos $x,y$ que, al comprimirse, resultan en el mismo archivo comprimido $f(x)=f(y)$. Esto significaría que **la compresión pierde datos, no siempre es posible recuperar exactamente el archivo original**.

### Conclusiones

- El último punto destacado no suena deseable - al comprimir archivos, se espera poder recuperar el archivo original al descomprimir. Para evitarlo, necesitamos alterar alguna de las suposiciones anteriores.
- Una solución que evita el problema es alterar la segunda suposición: *la compresión debería disminuir el tamaño de algunos archivos*. Esta solución implicaría que los archivos, al comprimirse, pesan lo mismo que antes de ser comprimidos. Esto evita el problema, sí, pero es inútil para lo que se quiere usar la compresión.
- La otra solución es alterar la primera suposición: *la compresión no debería aumentar el tamaño de un archivo*. Esta es la solución práctica: siempre existirán archivos que un sistema de compresión hará *mayores* que los archivos originales. El diseño de un sistema de compresión, entonces, radica en optimizarlo para que comprima los archivos que el público objetivo utilice y, a cambio, expanda archivos que no se espera que sean utilizados, o al menos no con frecuencia.
