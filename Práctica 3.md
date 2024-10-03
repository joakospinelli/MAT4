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