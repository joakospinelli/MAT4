# 1. Probar que no hay enteros simultáneamente pares e impares.
Un número $x$ es par si su división por 2 es exacta (con resto 0). Por otro lado, si el resto es distinto a 0, el número es impar.
* $Par: r(x/2) = 0$
* $Impar: r(x/2) \ne 0$

Un número cualquiera, al ser dividido por 2, siempre va a dar el mismo resultado, y por lo tanto, el mismo resto. Si hubiese números simultáneamente pares e impares, necesariamente tendría que obtener $r=0$ y $r\ne0$ a la vez, lo cual es un absurdo imposible.

Por lo tanto, no existen números que sean pares e impares a la vez.

# 2. Analizar si las siguientes afirmaciones son verdaderas o falsas:

## a. Si $a|1$, entonces $a=1$ o $a=-1$

$a|1$ implica que se cumple la fórmula $1 = a*c$.
* Si $a = 1$, se cumple $1=1*c \ \ \ c=1$
* Si $a = -1$, se cumple $1=(-1)*c \ \ \ c=-1$
* Para todo valor $|a| > 1$, la igualdad ya no se cumple, ya que $|a|*|c| > 1$ para todo valor de $a$ y $c$.

Por lo tanto, es verdadero que si se cumple $a|1$, entonces $a$ necesariamente debe ser $1$ o $-1$.

## b. $a|b$ y $b|c$ entonces $a|c$

$a|b: b=a*k$

$b|c: c=b*k$

$c=b*k$

$c=(a*k)*k$

$c=a*(k*k)$ *// $(k*k)$ da como resultado otro entero cualquiera*

$a|c: c=a*j$

* Si se cumple $a|b$, entonces $b$ es múltiplo de $a$.
* Si se cumple $b|c$, entonces $c$ es múltiplo de $b$.
* Los múltiplos cumplen con la propiedad de **transitividad**: si $c$ es múltiplo de $b$ y $b$ es múltiplo de $a$, entonces $c$ es múltiplo de $a$.
* Como $c$ es múltiplo de $a$, entonces $a|c$.

## c. $a(a-1)$ es par

$x = 2k$ *// definición de par*

$y = 2k + 1$ *// definición de impar*

Por definición, un número impar siempre va a tener como predecesor a un número par y viceversa: la fórmula de los impares coincide con la del sucesor de cualquier par.

En el caso de $a(a-1)$, como $(a-1)$ es el predecesor de $a$ siempre uno de los dos términos será par. Por lo tanto, asumiendo cualquier valor de $a$ par, la fórmula puede puede escribirse como:

$a(a-1) = (2k).(2k-1)$

$a(a-1)=2.k(2k-1)$

Por lo tanto, el resultado de $a(a-1)$ es par, ya que puede reducirse a una multiplicación por 2.

## d. $x|y$ e $y|z$ entonces $x|yz$

$x|y : y = x*c$

$y|z : z = y*c$

Ya demostramos en el inciso b que si se cumplen $x|y$ e $y|z$, entonces también se cumple $x|z$. Esto quiere decir que $y$ e $z$ son múltiplos de $x$.

Si multiplicamos $y*z$, siendo ambos múltiplos de $x$ obtendremos otro entero que, por transitividad, seguirá siendo múltiplo de $x$. Por lo tanto, el término $yz$ es múliplo de $x$ y se cumple $x|yz$.

# 3. Si a un número se lo divide por 5 con resto 3, y se lo divide por 7 con resto 4, ¿Cuál es el resto si se lo divide por 35?

*// este no sé cómo resolverlo je*

# 4. Sean $a$ y $b$ dos números enteros que al dividirlos por 11 tienen restos 4 y 7 respectivamente, hallar el resto de la división por 11 de $(a+b^2)$.

$a = 11.c_1 + 4$

$b = 11.c_2 + 7$

$b^2 = (11.c_2 + 7)^2 = 121.c_2^2 + 154.c_2 + 49$

$b^2 = 11(11.c^2 + 14.c_2) + 49$

$\dfrac {b^2} {11} = 11.c^2_2 + 14.c_2 + \dfrac {49} {11}$

Como $49$ es el único término no divisible por 11, el resto de $b^2$ será el resto de 49, el cual es $5$.

$(a+b^2) = (11.c_1+4) + (11.c_3 + 5)$ *// definiendo $c_3 = 11.c_2^2+14.c_2$*

$(a+b^2) = 11.c_1 + 11.c_3 + 9 = 11(c_1+c_3) + 9$

Por lo tanto, la división $\dfrac {(a+b^2)} {11}$ tendrá resto 9.

# 5. Convertir los siguientes números de base 10 a base 8

## a. 98

$98 = 12.8 + 2$

$12 = 8.1 + 4$

$1 = 8.0 + 1$

$98 = 142_8$

## b. 44

$44 = 5.8 + 4$

$5 = 0.8 + 5$

$44 = 54_8$

## c. 20

$20 = 2.8 + 4$

$2 = 0.8 + 2$

$20 = 24_8$

# 6. Calcular el máximo común divisor entre

*// los voy a hacer utilizando descomposición en primos*

## a. $(16,24)$

$16 = 8.2 = 4.2.2 = 2.2.2.2 = 2^4$

$24 = 8.3 = 4.2.3 = 2.2.2.3 = 2^3.3$

$MCD(16,24) = 8$

## b. $(70,50)$

$70 = 35.2 = 7.5.2$

$50 = 25.2 = 5.5.2 = 5^2.2$

$MCD(70,50) = 5.2 = 10$

*// era más rápido hacerlo así:*

$70 = 7.10 = 7.5.2$

$50 = 5.10 = 5.2.2$

$MCD(70,50)=10$

## c. $(121,88)$

$121 = 11.11 = 11^2$

$88 = 11.8 = 11.4.2 = 11.2.2.2 = 11.2^3$

$MCD(121,88) = 11$

## d. $(-90,90)$

$-90 = 30(-3) = 3.10(-3) = 3.5.2(-3) = 3.5.2.3(-1) = (3^2.5.2)(-1)$

$90 = 30.3 = 3.10.3 = 3.5.2.3 = 3^2.5.2$

$MCD(-90,90) = 3^2.5.2 = 90$

## e. $(980,224)$

$980 = 140.7 = 14.5.2.7 = 7.2.5.2.7 = 7^2.2^2.5$

$224 = 112.2 = 56.2.2 = 7.8.2.2 = 7.4.2.2.2 = 7.2.2.2.2.2 = 7.2^5 = 7.2^2.2^3$

$MCD(980, 224) = 7.2^2 = 28$

# 7. Probar que si $a,b$ son enteros:

## a. $a+b$ es coprimo con $a$.

Dos números son coprimos si su MCD es igual a 1.

Por lo tanto, el enunciado plantea que $(a, a+b) = 1$. Se intentará demostrar con un entrejemplo, a partir de un número $d > 1$ con el cual:
* $d|a+b$, por lo tanto $a+b = d.c_1$
* $d|a$, por lo tanto $a = d.c_2$

Esto también implica que $d|b$, siguiendo el razonamiento:

$$b = (a+b) - a = d.c_1 - d.c_2 = d(c_1 - c_2)$$

siendo $(c_1 - c_2)$ un número entero.

Por propiedades del MCD podemos deducir que

$$MCD(a, a+b) = MCD(a,(a+b)-a) = MCD(a,b)$$

Ya que restar un múltiplo de un término no afecta a la operación.

Por lo tanto, $(a,a+b)$ será coprimo cuando $(a,b)$ también lo sea.

## b. Si $a$ no es nulo, $(a,0) = |a|$.

Conociendo que $a \ne 0$, se quiere encontrar el $MCD(a,0)$.

* Se sabe que si se cumple $x|y$, entonces $MCD(x,y) = y$ para todo par de números enteros $x,y$.
* $0$ es divisible por todos los números enteros, por lo tanto se cumple $a|0$ y, por lo tanto, $MCD(a,0) = a$.
* En el caso de que $a$ sea negativo, aún puede ser divisible por su opuesto (que es mayor que él), por lo tanto $MCD(a,0) = |a|$.

## c. Si $(a,b) = 1$ entonces $ma+nb=k$ con $m$, $n$, y $k$ enteros.

Este enunciado es una interpretación de la Identidad de Bézout, la cual dice que dado un par de números $a,b$ y su MCD $d$, existen dos enteros tales que $d = ma+nb$. En este caso, $d$ toma el valor de $1$.

# 8. Hallar $MCD(5k + 3; 3k+2)$ para cualquier $k$ entero.

$a = 5k+3$

$b = 3k+2$

Mediante el algoritmo de Euclides:

1. $r_1 = 5k+3 - c_1(3k+2) = 2k + 1 \to (a,b) = (b,r_1)$ *// asumiendo $c_1=1$ ya que $a > b$*
2. $r_2 = 3k+2 - c_2(2k+1) = k+1 \to (b,r_1) = (r_1,r_2)$ *// asumiendo $c_2=1$*
3. $r_3 = 2k+1 - c_2(k+1) = 0-1 \to (r_1,r_2) = (r_2, -1)$ *// asumiendo $c_2=2$ ya que $k \times 2 = 2k$*

Para todo entero se cumple $MCD(x,-1) = |1|$, por lo tanto:

$$(5k+3;3k+2) = (3k+2,r_1) = (r_1,r_2) = (r_2, -1) = (-1,0) = 1$$

# 9. Sean $a,b \in Z$ y $p$ primo, demostrar que si $p|ab$ entonces $p|a$ ó $p|b$. Mostrar que no se cumple cuando $p$ no es primo.

Dado $p|ab$ con $p$ primo, se da que $p=c_1 \times ab$ con resto 0. Se quiere demostrar que, al cumplirse esto, necesariamente debe cumplirse $p|a$ o $p|b$.

Si $p$ es primo, quiere decir que no puede descomponerse en factores de números más pequeños a él, por lo tanto si $p|ab$ se cumple es porque necesariamente alguno de los dos factores es divisible por $p$.

Por otro lado, cuando $p$ no es primo, existen factores que dan como resultado $p$, los cuales podrían dividir a $a$ ó $b$ individualmente sin necesidad de que $p$ pueda hacerlo; el caso más común de esto es cuando algunos de los factores que descomponen a $p$ se encuentra en $a$ ó $b$.

Cuando $p$ no es primo, la demostración puede realizarse simplemente con un contraejemplo:

$a = 5 \\ b=2 \\ p=10$

Se cumple $10|2 \times 5$. Sin embargo no se cumplen $10|2$ ni $10|5$ ya que 2 y 5 se obtienen de descomponer a $p$, por lo que son menores a él y no pueden ser divididos.

# 10. Hallar, si existe, un número entero $q$ tal que $7290q$ es el cubo de un entero.

*// no sé de dónde pretendían quue saque esto sin mi amigazo gpt*

Se busca encontrar un número tal que $x^3 = 7290q$. Esto puede realizarse descomponiendo 7290 en números primos, tal que:

* $7290 = 3645 \times 2$
* $3645 = 1215 \times 3$
* $1215 = 405 \times 3$
* $405 = 135 \times 3$
* $135 = 45 \times 3$
* $45 = 15 \times 3$
* $15 = 5 \times 3$
* $5 = 5 \times 1$

Por lo que 7290 puede descomponerse en $2 \times 3^6 \times 5$.

Para obtener un cubo perfecto, los primos que componen a 7290 deberían tener exponente 3 o un múltiplo de este. Esto puede realizarse multiplicándo por los factores restantes, obteniendo así el valor de $q$:

$$ q = 2^2 \times 3^0 \times 5^2 = 4 \times 1\times 25 = 100 $$

A partir del cual podemos deducir también el valor de $x$:

$ x^3 = 100 \times 7290$

$x = \sqrt[3] {729000 }$

$x = 90$

# 11. Demostrar que, dados los números $a,b$ en $Q$ tales que $a < b$, existe otro número racional $x$ tal que $a < x < b$.

Partiendo de $a < b$, se puede demostrar la existencia de $x$ tal que $a < x < b$ a través de los siguientes pasos:
* $a < b$
* $\exists x: x=a+b;a < x < b$
* $a < b = a+a < x < y+y = 2a < x < 2y$
* $\dfrac {2a} 2 < \dfrac {x} 2 < \dfrac {2b} 2$
* $a < \dfrac {x} 2 < b$

De esta manera, se demostró que para todo par de números $a,b \in Q$ tales que $a < b$, existe otro número $x$ que existe entre ambos, y siempre tomará el valor de $\dfrac {a+b} 2$.

**Ejemplo:**
$$a = 2, b = 4 \qquad x=\dfrac {2+4} 6 = 3$$

# 12. Probar que no existe un número racional cuyo cubo sea igual a 2.

Se quiere demostrar que no existe ningún número racional $r$ tal que $r^3 = 2$.

Como ya sabemos, todo número racional está formado por el cociente de dos números enteros, por lo que $r = \dfrac a b$ y, por lo tanto, $r^3 = (\dfrac a b)^3$, siendo $\dfrac a b$ la forma irreducible de $r$.

Haciendo una serie de pasos esto se puede traducir a:
* $(\dfrac a b)^3 = \dfrac {a^3} {b^3} = 2$
* $a^3 = 2(b^3)$

Se sabe que $a$ es par, debido a que su cubo es también un número par. Por lo tanto:
* $a = 2k$.
* $(2k)^3 = 2(b^3)$
* $8k^3 = 2(b^3)$
* $\dfrac {8k^3} 2 = b^3$
* $4k^3 = b^3$

A partir de lo cual deducimos que $b$ también es par, ya que $b^3$ es divisible por 4. Esto implicaría que tanto $a$ como $b$ son pares, y por lo tanto la función aún puede reducirse al tener factor común 2. Esto entra en una contradicción con nuestra hipótesis, ya que se planteó que $\dfrac a b$ era irreducible.

## 13. Indique la parte real $Re(z)$ y la parte imaginaria $Im(z)$ de los siguientes complejos:

## a.

$\sqrt {-49} = \sqrt {7^2 \times (-1)} = 7 \times \sqrt {-1} = 7i$

* $Re(z) = 0$
* $Im(z) = 7i$

## b.

$ \sqrt {-20} = \sqrt {20 \times (-1)} = \sqrt {20} \times \sqrt {-1} = 4.4721i$

* $Re(z) = 0$
* $Im(z) = 4.4721i$

## c.

$\sqrt {- \dfrac 9 {16}} = \sqrt {\dfrac 9 {16} \times (-1)}=\sqrt \dfrac 9 {16} \times \sqrt {-1} = \dfrac 3 4 i$

* $Re(z) = 0$
* $Im(z) = \dfrac 3 4$

## d.

$z = -8$

* $Re(z) = -8$
* $Im(z) = 0$

## e.

$z = 7i$

* $Re(z) = 0$
* $Im(z) = 7$

## f.

$z = (3+i) + (5-4i) = (3+5)+(i-4i)=8-3i$

* $Re(z) = 8$
* $Im(z) = -3$

## g.

$z = 3i-(5-2i) = 3i+2i-5=5i-5$

* $Re(z) = -5$
* $Im(z) = 5$

## h.

* $a_1 = 1 \qquad b_1=3$
* $a_2 = 3 \qquad b_2=-1$

$\dfrac {1+3i} {3-i} = \dfrac {(1\times3 + 3(-1)) + i(-1(-1)+3\times3)} {3^2 + (-1)^2} = \dfrac {0 + 10i} {10} = \dfrac {10i} {10} = i$

* $Re(z) = 0$
* $Im(z) = 1$

## i.

$\dfrac {1-i} {(1+i)^2} = \dfrac {1-i} {1 + 2i + i^2} = \dfrac {1-i} {2i}$

* $a_1 = 1 \qquad b_1 = -1$
* $a_2 = 0 \qquad b_2 = 2$

$\dfrac {(1\times0 + (-1)\times2) + i(-1\times2 + 0\times(-1))} {0^2 + 2^2} = \dfrac {-2 +2i} 4 = \dfrac {-1+i} 2$

* $Re(z) = -\dfrac 1 2$
* $Im(z) = \dfrac 1 2$

# 14. La suma de un número complejo y su conjugado es -8, y la suma de sus módulos es 10. De qué números complejos se trata?

A partir de un número $z$, se sabe que:
* $z + \overline z = -8$
* $|z| + |\overline z| = 10$

Sabiendo que $z = a + bi$, podemos despejar $a$ a partir de la operación $z + \overline z$, ya que la parte imaginaria se anula con el conjugado:

* $z + \overline z = -8$
* $a+bi + (a-bi) = -8$
* $2a = -8$
* $a = \dfrac {-8} 2 = -4$

Con el valor de $a$ se puede buscar el valor de $b$ a partir de la segunda operación:
* $|z| + |\overline z| = 10$
* $\sqrt {a^2 + b^2} + \sqrt {a^2 + (-b)^2} = 10$
* $\sqrt {a^2 + b^2} + \sqrt {a^2 + b^2} = 10$
* $2 \sqrt {a^2 + b^2} = 10$
* $\sqrt {a^2 + b^2} = 5$
* $\sqrt {(-4)^2 + b^2} = 5$
* $\sqrt {16 + b^2} = 5$
* $16 + b^2 = 25$
* $b^2 = 25-16$
* $b^2 = 9$
* $b = 3$

El valor de $b$ es el mismo tanto para $z$ como $\overline z$, los cuales son:

$z = -4 + 3i$

$\overline z = -4 - 3i$

# 15. Hallar, si existe, un número $x$ real tal que $Re(z) = Im(z)$, siendo $z = \dfrac {x+2i} {4-3i}$

Primero se intentará resolver $z$:

$z = \dfrac {x+2i} {4-3i} = \dfrac {(x+2i)(4+3i)} {(4-3i)(4+3i)} = \dfrac {(4x + 3xi +8i + 6i^2)} {16+12i-12i-9i^2}$

$\dfrac {(4x + 3xi +8i + 6i^2)} {16+12i-12i+9i^2} = \dfrac {4x + 3xi + 8i +6(-1)} {16-9(-1)} = \dfrac {4x + 3xi + 8i -6} {25}$

$\dfrac {4x + 3xi + 8i -6} {25} = \dfrac {4x - 6 + i(3x+8)} {25}$

Con esta forma de $z$ podemos ver que:
* $Re(z) = \dfrac {4x-6} {25}$
* $Im(z) = \dfrac {3x+8} {25}$

Se quiere encontrar un número $x$ tal que $Re(z) = Im(z)$, por lo que se usará esta igualdad para encontrar $x$:

$Re(z) = Im(z)$

$\dfrac {4x-6} {25} = \dfrac {3x+8} {25}$

$4x-6 = 3x+8$

$4x = 3x+8+6 = 3x+14$

$4x - 3x = 14$

$x = 14$

Por lo tanto, existe un número complejo $z = \dfrac {14 + 2i} {4-3i}$ tal que:

* $Re(z) = \dfrac {4\times14 - 6} {25} = \dfrac {56-6} {25} = \dfrac {50} {25} = 2$

* $Im(z) = \dfrac {3\times14 + 8} {25} = \dfrac {42+8} {25} = \dfrac {50} {25} = 2$

Cumpliendo con la hipótesis inicial $Re(z) = Im(z)$.