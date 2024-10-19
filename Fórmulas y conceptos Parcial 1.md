# Teoría de números enteros

## División

Un número entero divide a otro cuando:

$$b = a \times c + r \qquad 0 \le r \lt a$$

Cuando la división tiene resto 0, se dice que es una **división exacta**. Si un número divide a otro con resto 0, se denota como:

$$a|b \to b = a \times c + 0$$

Y se dice que *$a$ divide a $b$*. Algunos ejemplos:

* $2|4 \to 4 = 2 \times 2 + 0$
* **Contraejemplo:** $2|7 \to 7 = 3*2 + 1$ ($r \ne 0$, por lo tanto la división no es exacta).

### Propiedades de la división exacta:
* $a|a$
* $1|a$ para cualquier $a \in Z$
* $a|0$ para cualquier $a \in Z$
* $a|b \implies a|-b, -a|b, -a|-b$
* $a|b \implies a|bc$
* $a|b \land b|c \implies a|c$ *(transitividad)*

## Cambio de base

*// no sé cual es la definición de base, pero x lo menos explico cómo se hace.*

Dado un número $x_{10}$, para convertirlo a otra base $b$ se deben realizar los pasos:
1. Convertir $x$ a la forma $n = a \times b + r$
2. Se debe continuar haciendo esto hasta que se logre la igualdad con $a = 0$.
3. Finalmente, $x_{m}$ se obtiene tomando como dígitos a los restos obtenidos en los pasos anteriores, tales que $x_{m} = [r_n], [r_{n-1}]...[r_1]$.

Como no se entiende nada acá va un ejemplo:

Dado el número $256_{10}$, se lo quiere convertir a base $8$. Para esto se realizan los pasos:
* $256 = 32 \times 8 + 0$
* $32 = 4 \times 8 + 0$
* $32 = 0 \times 8 + 4$

Los restos fueron $4, 0, 0$.

$256_{10} = 400_{8}$

## Números enteros primos

Un número es primo si sus únicos divisores son triviales; es decir: $1, -1$ y él mismo. Todos los números no primos son compuestos.

1 y 0 no se consideran ni primos ni compuestos.

*// confío en que no van a tomar la criba de Eratóstenes*

## Máximo común divisor

El MCD entre dos enteros es el mayor número que divide a ambos sin dejar resto. Se denota como $(a,b)$ o $MCD(a,b)$.

Para todo par $a,b \in Z$ no nulos, existe un MCD $d > 0$ tal que:
* $d|a, d|b$
* Si existe un número $D$ que cumple $D|a, D|b$, entonces también $D|d$. *👈 de esta manera se garantiza que $d$ sea el máximo, ya que $D$ puede dividirlo y, por lo tanto, $D < d$*

Se dice que dos números $a,b \in Z$ son coprimos si $MCD(a,b) = 1$. Otra característica de los coprimos es que ninguno es múltiplo del otro; por lo tanto, si se da $a|mb$ es porque $a|m$.

### Descomposición en primos

Técnica para obtener el $MCD$ entre dos números. Consiste en descomponer los números en múltiplos de números primos y elegir el máximo factor en común.

Ejemplo con $(45,60)$:
* $45 = 15 \times 3 = 5 \times 3 \times 3 = 5\times 3^2$
* $60 = 3 \times 20 = 3 \times 5 \times 4 = 3 \times 5 \times 2 \times 2 = 3 \times 5 \times 2^2$

El mayor factor común es $5 \times 3$, por lo que $MCD(45,60) = 15$
* $45 \div 15 = 3$
* $60 \div 15 = 4$

### Algoritmo de Euclides

Otra técnica mucho más complicada. Consiste en obtener el $MCD$ de los restos de los números, siguiendo la cadena:

$$(a,b) = (b,r_1) = (r_1, r_2) = (r_2, r_3) = ... = (r_n, 0)$$

Una vez llegado al par $(r_n, 0)$, se sabe que $MCD(a,b) = r_n$.

*// para esto siempre se tiene que cumplir $a > b$, igual se pueden dar vuelta porque es conmutativo*

Ejemplo con $(60,45)$:
* $r_1: 60 = 45 \times 1 + 15 \to (60,45) = (45,15)$
* $r_2: 45 = 15 \times 3 + 0 \to (15,0)$

$(60,45) = r_2 = 15$

### Identidad de Bézout

Esto es una fórmula que por sí sola no sirve para absolutamente nada pero a veces te sirve.

Dado un par de enteros $a,b \in Z$ y $d = (a,b)$, existen otros enteros $m,n$ tales que:

$$d = m \times a + n \times b$$

## Mínimo común múltiplo

El $MCM$ de dos o más números es el menor número natural que es múltiplo de ambos. Se denota como $MCM(a,b)$ ó $[a,b]$.

Para todo par de números $a,b \in Z$, existe un $MCM(a,b) m > 0$ tal que:
* $a|m, b|m$
* Si existe un número $M$ que cumple $a|M, b|M$, entonces también $m|M$. *👈 de esta manera se garantiza que $m$ sea el menor, ya que puede dividir a $M$ y, por lo tanto, $m < M$.*

# Números reales

Conjunto mayor de números que incluye a los racionales e irracionales, que permite realizar muchas más operaciones que el conjunto de los enteros.

Tiene algunas restricciones en las operaciones:
* Ningún número se puede dividir por 0.
* No pueden obtenerse logaritmos de números negativos.
* No puede obtener las raíces pares de números negativos. *👈 acá entran los imaginarios*

## Racionales

Son todos los números que pueden representarse como cociente de otros números enteros. Tienen el formato $\frac a b, b > 0$. Los números enteros están incluidos en este conjunto, representándolos como $\frac n 1$ con $n \in Z$.

Algunas operaciones y propiedades no tan obvias pero que son útiles:

* Dos fracciones $\dfrac a b; \dfrac c d$ son equivalentes si y sólo si $a \times d = b \times c$

* Dos fracciones $\dfrac a b; \dfrac c d$ están ordenadas de tal manera que $ad < bc$

* La suma, resta y muultiplicación son cerradas.

* El inverso de una fracción está dado por $(\dfrac a b) ^{-1} = \dfrac b a$
    * **NOTA PORQUE SIEMPRE ME CONFUNDO: el opuesto de $a$ es $-a$, el inverso es $a^{-1}$**

* La división de fracciones es el equivalente al producto con el inverso, tal que $\dfrac a b \div \dfrac c d = \dfrac a b \times \dfrac d c$

### Densidad

Para todo par de números racionales existe otro número entre ellos. Esto se demuestra como:

$$x < y$$

$$x + x < x + y < y +y = 2x < x+y < 2y$$

$$x < \dfrac {x+y} 2 < y$$

Por lo tanto, para dos pares de números racionales $x,y$ existe otro racional $\dfrac {x+y} 2$ exactamente entre ellos.

## Números irracionales

Otro conjunto dentro de los reales, formado por aquellos números que no pueden expresarse como una fracción racional $\frac m n$.

No son muy interesantes pero tienen estas propiedades:
* La suma y resta entre un racional y un irracional da un número irracional.
* El producto y cociente de un racional $\ne 0$ con un irracional da un número irracional.
    * Esto es porque 0 es racional y porque no podés dividir por 0.
* El inverso de un irracional es otro irracional.

# Números complejos

Otro conjunto que viene a resolver todos los problemas de los reales (no sé si todos, por lo menos las raíces de negativos). Tiene como subconjunto a los números reales, además de un nuevo conjunto de números denominados **imaginarios.**

Los números imaginarios se denotan como $i$ y se definen en base a:

$$x^2 + 1 = 0$$

$$x^2 = -1 \implies x = \sqrt {-1}$$

Esto los reales no lo pueden hacer ☝, por lo que se define a $i$ como:

$$i = \sqrt {-1}$$

## Forma binómica

Es la forma más básica de representar a los números complejos:

$$z = a + ib \qquad a,b \in R$$

Tal que:
* $a$ representa a la **parte real** de $z$ (o $Re(z) = a$).
* $b$ representa a la **parte imaginaria** de $z$ (o $Im(z) = b$).

Entonces, un número real es un número complejo $z$ con $b = Im(z) = 0$, y un número imaginario es otro complejo $x$ con $a = Im(x) = 0$.

### Operaciones aritméticas

Siendo $z_1 = a_1 + b_2i, z_2 = a_2 + b_2i$

* $z_1 + z_2 = (a_1 + a_2) + i(b_1 + b_2)$

* $z_1 - z_2 = (a_1 - a_2) + i(b_1 - b_2)$

* $z_1 \times z_2 = a_1a_2 + (a_1b_2)i + (a_2b_1)i + (b_1b_2)i^2 = a_1a_2 +(a_1b_2)i + (a_2b_1)i - b_1b_2 =(a_1a_2 - b_1b_2) + i(a_1b_2 + a_2b_1)$

* $\overline z_1 = a_1 - b_1$ (conjugado)

* $z^{-1} = \dfrac {1 \times \overline z} {z \times \overline z} = \dfrac {a_1 - b_1} {(a_1 + b_1)(a_1 - b_1)}$ (inverso)

* $z_1 \div z_2 = z_1 \times z_2^{-1}  = \dfrac {(a_1 + b_1i)(a_2 - b_2i)} {(a_2 + b_2)(a_2 - b_2)} = \dfrac {(a_1a_2 - a_1b_2i + b_1a_2i - (b_1b_2i)^2)} {a_2^2 + b_2^2} = \dfrac {(a_1a_2 + b_1b_2) + (-a_1b_2 + b_1a_2)i} {a_2^2 + b_2^2}$

### Potencias

Esta es la parte más divertida de los números imaginarios y es que se pueden convertir de la siguiente manera:

* $i^0 = 1$
* $i^1 = \sqrt{-1}$
* $i^2 = -1$
* $1^3 = -i$
* $1^4 = 1$

Esta tabla se repite cíclicamente hasta el fin de los números. A partir de ella se puede convertir el valor de cualquier potencia de $i$, tal que:

$$i^m = i^{m\mod 4}$$

Un ejemplo con $i^{256}$:

* $256 \mod 4 = 0$
* $i^{256} = i^0 = 1$

☝ La manera "correcta" es ir descomponiéndolo en números de 4, capaz que si lo hago así se enojan en el examen.

# Plano complejo

Acá hay un montón de explicaciones del plano complejo que no nos interesan, lo importante es:

Dado $z = a + ib \in C$:
* $|z| = \sqrt {a^2 + b^2}$ (módulo de $z$)
* $\theta = \arctan(\frac b a)$ (ángulo o argumento de $z$; su valor tendría que estar entre $0 \le 2\pi$)

Que esto nos va a servir para representar a $z$ de otras formas que no sean la binómica.

Con esto se pueden otras cosas interesantes como:
* $\cos (\theta) = \dfrac a {|z|}$

* $\sin (\theta) = \dfrac b {|z|}$

Y si tenemos todo esto podemos obtener $Re(z), Im(z)$:

* $Re(z) = a = |z| \times \cos (\theta)$
* $Im(z) = b = |z| \times \sin (\theta)$

### Otras representaciones

A partir de $|z|$ y $\theta$ se pueden representar a los números complejos de nuevas formas:

* **Trigonométrica:** $z = |z|(\cos(\theta) + \sin(\theta)\times i)$
* **Polar:** $z = |z|_\theta$
* **Exponencial:** $z = |z|\times e^{i\theta}$

Que nos interesa la exponencial porque es con la que nos enseñaron a hacer las operaciones

### Operaciones en forma exponencial

Sean $z_1 = |z_1| \times e^{i\theta_1}; z_2 = |z_2| \times e^{i\theta_2}$

* **Producto:** $z_1 \times z_2 = (|z_1| \times e^{i\theta_1}) \times (|z_2| \times e^{i\theta_2}) = |z_1||z_2|\times e^{i(\theta_1 +\theta_2)}$

* **Cociente:** $\dfrac {z_1} {z_2} = \dfrac {|z_1| \times e^{i\theta_1}} {|z_2| \times e^{i\theta_2}} = \dfrac {|z_1|} {|z_2|} \times e^{i(\theta_1 - \theta_2)}$

Lo más importante de esto son las potencias y las raíces. sean $z = |z|\times e^{i\theta}; w = |w|\times e^{i\phi}$ y un número natural $n$ tal que $w^n = z$:

* **Potencia:** $z^x = (|z|^{i\theta})^n = |z|^n \times e^{ni\theta}$

La raíz es un poco más complicada:
* $|z| = |w|^n = \sqrt[n] {|z|}$

* $\phi k = \dfrac {\theta + 2k\pi} n; 0 \le k \le n-1$

Entonces $z$ va a tener $k$ raíces, tales que:

$$w_k = |w| \times e^{i\phi_k}$$

Un ejemplito (lo saqué de la práctica):

$z = -1 + i$

$|z| = \sqrt {(-1)^2 + 1^2} = \sqrt {1+1} = \sqrt 2$

$\theta = \arctan(\dfrac {1} {-1}) = \dfrac 7 4 \pi$

$|w| = \sqrt[4] {|z|} = \sqrt[4] {\sqrt 2} = \sqrt[8] 2$

$\phi_k = \dfrac {\frac 7 4 \pi + 2k\pi} {4} \qquad 0 \le k \le 3$

* $\phi_0 = \dfrac {\frac 7 4 \pi + 2.0\pi} {4} = \dfrac {\frac 7 4 \pi} {4} = \dfrac {7} {16}\pi$

* $\phi_1 = \dfrac {\frac 7 4 \pi + 2.1\pi} {4} = \dfrac {\frac 7 4 \pi + 2\pi} {4} = \dfrac {\frac {15} {4} \pi} {4} = \dfrac {15} {16} \pi$

* $\phi_2 = \dfrac {\frac 7 4 \pi + 2.2\pi} {4} = \dfrac {\frac 7 4 \pi + 4\pi} {4} = \dfrac {\frac {23} 4 \pi} {4} = \dfrac {23} {16} \pi$

* $\phi_3 = \dfrac {\frac 7 4 \pi + 2.3\pi} {4} = \dfrac {\frac 7 4 \pi + 6\pi} {4} = \dfrac {\frac {31} 4 \pi} {4} = \dfrac {31} {16} \pi$

$w_k = |w| \times e^{i\phi_k}$

A partir de lo que obtenemos las raíces cuartas de $z$:

* $w_0 = \sqrt[8] 2\times e^{\frac 7 {16} \pi i}$

* $w_1 = \sqrt[8] 2\times e^{\frac {15} {16} \pi i}$

* $w_2 = \sqrt[8] 2\times e^{\frac {23} {16} \pi i}$

* $w_3 = \sqrt[8] 2\times e^{\frac {31} {16} \pi i}$

# Relaciones entre conjuntos

Una relación entre conjuntos es un subconjunto de su producto cartesiano, que selecciona sus elementos por una condición específica. Las más comunes son las relaciones binarias, que son exclusivas entre 2 conjuntos.

## Algunos conceptos que no sé si sirven

Las relaciones entre los conjuntos $A, B$ poseen elementos en el formato $(x,y)$, con $x \in A$ e $y \in B$.

* El dominio de la relación está dado por los elementos $x$ de $A$ que pertenezcan a una tupla $(x,y) \in R$
* La imagen de la relación está dada por los elementos $y$ de $B$ que pertenezcan a una tupla $(x,y) \in R$
* Una relación inversa se define a partir de una relación en $A \times B$, y es exactamente igual pero en $B \times A$, de manera que $R^{-1} = \{ (y,x) : (x,y) \in R \}$

## Matriz

La matriz de una relación está dada por las columnas $a_i$ (representando a los elementos $a \in A$) y las filas $b_i$ (representando a $b \in B$). Las celdas $m_{ij}$ puede tomar los valores:
* $1$ si $(a_i, b_j) \in R$
* $0$ si $(a_i, b_j) \notin R$

Ejemplo:

- $A = \{ 1, 2, 3 \}$
- $B = \{ r, s \}$
- $R=\{ (1,r); (2,s); (3,r) \}$

$M_R = \begin{pmatrix}
1&0 \\
0&1 \\
1&0
\end{pmatrix}$ ya que existen en $R$ $(1,r);(2,s);(3,r)$ y no existen $(1,s);(2,r);(3,s)$.

# Relaciones binarias en un mismo conjunto

Una relación $R$ está definida en un único conjunto si se cumple que $R \subset A \times A$.

## Propiedades

Estas son re importantes:

* **Reflexividad:** si para todo $x \in A$ se cumple $xRx$ (*cada $x$ se relaciona con sí mismo mediante $R$)*.
* **Simétrica:** si para todo $x,y \in A$, $xRy$ implica lógicamente a $yRx$. Esto puede darse de dos maneras:
    * $xRy \in R: xRy \implies yRx \to V \implies V = V$
    * $xRy \notin R: xRy \implies yRx \to F \to yRx = V$
* **Antisimétrica:** si cuando se cumple $xRy \implies yRx$, necesariamente se cumple $x=y$. En otras palabras, $R$ sólo es simétrica cuando $x=y$.
* **Transitiva:** si cuando $xRy \land yRz$ implican lógicamente a $xRz$.
    * $xRy \in R; yRz \in R \to xRy \land yRz \implies xRz = V \land V \implies V$

## Relaciones de orden

Una relación es un preorden si es **reflexiva y transitiva**.

Una relación es de orden si es **reflexiva, transitiva y anti-simétrica.**

Si un conjunto tiene una relación de orden, es un conjunto ordenado. Que tiene los siguientes elementos:
* $a$ es un **máximo** si $x < a$ para todo $x \in A$.
* $b$ es un **mínimo** si $x > b$ para todo $x \in A$.
* $c$ es una **cota superior** si es el máximo de un subconjunto del conjunto ordenado.
* $d$ es una **cota inferior** si es el mínimo de un subconjunto del conjunto ordenado.

## Relaciones de equivalencia

Una relación es de equivalencia si es **reflexiva, simétrica y transitiva.** Se denota como $A \equiv B$.

### Clases de equivalencia

Están formadas por todos los elementos de $A$ que se relacionan con otro $a \in A$ mediante $R$. Se denota como $R(a)$.

### Particiones

Conjunto de partes no vacías, disjuntas y tales que su unión coincide con $A$. Sus propiedades son:
* No existen partes vacías.
* Un elemento no puede estar en dos o más partes a la vez.
    * La intersección entre 2 partes debe ser vacía.
* No puede haber elementos que no pertenezcan a ninguna parte.
    * La unión de las partes debe ser igual a $A$.

## Relaciones de congruencia

Tipo de relaciones equivalentes entre números enteros.

Un entero $a$ es congruente con otro $b$ mediante el módulo de $m$ si se cumple $m|a-b$; o de otra manera, existe un entero $k$ tal que $a-b = k \times m$.

Se denota como $a \equiv b \pmod m$ ó $a \equiv_m b$. Algunas demostraciones:
* Es reflexiva ya que $a-a = k \times m=0\times m$ para todo $a \in Z$.
* Es simétrica ya que:
    * $a-b = k \times m$
    * $b-a = -(a-b)$
    * $a-b = k \times m \implies -(a-b) = -(k \times m)$
* Es transitiva ya que:
    * $a-b = k \times m$
    * $b-c = j \times m$
    * $a-c = a + (-b + b) - c = (a-b) + (b-c) = k \times m + j \times m = (k+j)\times m$
    * $(k+j)$ es un nuevo entero tal que $a \equiv_m c$

### Cositas de la congruencia

* Un número pertenece a la clase de equivalencia $R(n)$ si al dividrlo por $m$ obtiene como resto a $n$.
* Dos números son congruentes entre sí ($a \equiv_m b$) si pertenecen a la misma clase de equivalencia.