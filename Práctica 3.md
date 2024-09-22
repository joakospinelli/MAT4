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