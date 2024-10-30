# Hallar los resultados de las siguientes operaciones realizadas entre enteros módulo 4 y 5:

## a. $\overline 3 + \overline 1$

**Módulo 4:**
* $\overline 3 + \overline 1 = (3+1) \mod 4$
* $4 \mod 4 = 0$
* $\overline 3 + \overline 1 = \overline 0$

**Módulo 5:**
* $\overline 3 + \overline 1 = (3+1) \mod 5$
* $4 \mod 5 = 4$
* $\overline 3 + \overline 1 = \overline 4$

## b. $\overline 5 + \overline 9$

**Módulo 4:**
* $\overline 5 + \overline 9 = (5+9) \mod 4$
* $14 \mod 4 = 2$
* $\overline 5 + \overline 9 = \overline 2$

**Módulo 5:**
* $\overline 5 + \overline 9 = (5+9) \mod 5$
* $14 \mod 5 = 4$
* $\overline 5 + \overline 9 = \overline 4$

## c. $\overline {40} \times \overline 3$

**Módulo 4:**
* $\overline 40 \times \overline 3 = (40 \times 3) \mod 4$
* $120 \mod 4 = 0$
* $\overline 40 \times \overline 3 = \overline 0$

**Módulo 5:**
* $\overline 40 \times \overline 3 = (40 \times 3) \mod 5$
* $120 \mod 5 = 0$
* $\overline 40 \times \overline 3 = \overline 0$

## d. $(\overline 3 + \overline 2)(\overline 6 \times \overline 8)$

**Módulo 4:**
* $(\overline 3 + \overline 2)(\overline 6 \times \overline 8) = ((3+2)(6 \times 8)) \mod 4$
* $6 \times 48 \mod 4 = 288 \mod 4 = 0$
* $(\overline 3 + \overline 2)(\overline 6 \times \overline 8) = \overline 0$

**Módulo 5:**
* $(\overline 3 + \overline 2)(\overline 6 \times \overline 8) = ((3+2)(6 \times 8)) \mod 5$
* $6 \times 48 \mod 4 = 288 \mod 5 = 3$
* $(\overline 3 + \overline 2)(\overline 6 \times \overline 8) = \overline 3$

# 2. Construir las tablas de sumar y multiplicar de los enteros módulo 2 y 5

## Módulo 2

$Z_2 = \{ 0, 1 \}$

* $\overline 0 + \overline 0 = \overline 0$
* $\overline 0 + \overline 1 = \overline 1$
* $\overline 1 + \overline 0 = \overline 1$
* $\overline 1 + \overline 1 = \overline 0$

| + | $\overline 0$ | $\overline 1$ |
| - | ------------- | ------------- |
| $\overline 0$ | $\overline 0$ | $\overline 1$ |
| $\overline 1$ | $\overline 1$ | $\overline 0$ |

* $\overline 0 \times \overline 0 = \overline 0$
* $\overline 0 \times \overline 1 = \overline 0$
* $\overline 1 \times \overline 0 = \overline 0$
* $\overline 1 \times \overline 1 = \overline 0$

| $\times$ | $\overline 0$ | $\overline 1$ |
| -------- | ------------- | ------------- |
| $\overline 0$ | $\overline 0$ | $\overline 0$ |
| $\overline 1$ | $\overline 0$ | $\overline 1$ |

## Módulo 5

$Z_5 = \{ 0, 1, 2, 3, 4 \}$

| + | $\overline 0$ | $\overline 1$ | $\overline 2$ | $\overline 3$ | $\overline 4$ |
| - | - | - | - | - | - |
| $\overline 0$ | $\overline 0$ | $\overline 1$ | $\overline 2$ | $\overline 3$ | $\overline 4$ |
| $\overline 1$ | $\overline 1$ | $\overline 2$ | $\overline 3$ | $\overline 4$ | $\overline 0$ |
| $\overline 2$ | $\overline 2$ | $\overline 3$ | $\overline 4$ | $\overline 0$ | $\overline 1$ |
| $\overline 3$ | $\overline 3$ | $\overline 4$ | $\overline 0$ | $\overline 1$ | $\overline 2$ |
| $\overline 4$ | $\overline 4$ | $\overline 0$ | $\overline 1$ | $\overline 2$ | $\overline 3$ |

| $\times$ | $\overline 0$ | $\overline 1$ | $\overline 2$ | $\overline 3$ | $\overline 4$ |
| ------- | - | - | - | - | - |
| $\overline 0$ | $\overline 0$ | $\overline 0$ | $\overline 0$ | $\overline 0$ | $\overline 0$ |
| $\overline 1$ | $\overline 0$ | $\overline 1$ | $\overline 2$ | $\overline 3$ | $\overline 4$ |
| $\overline 2$ | $\overline 0$ | $\overline 2$ | $\overline 4$ | $\overline 1$ | $\overline 3$ |
| $\overline 3$ | $\overline 0$ | $\overline 3$ | $\overline 1$ | $\overline 4$ | $\overline 2$ |
| $\overline 4$ | $\overline 0$ | $\overline 4$ | $\overline 3$ | 2 | $\overline 1$ |

# 3. Analizar si las siguientes son estructuras de grupo:

## a. $(Z_4, +)$. Enteros módulo 4 con la suma modular.

* La suma modular es una operación cerrada, ya que $x + y$ da como resultado otro elemento en $Z_4 \quad \forall x,y \in Z_4$. Por lo tanto, está bien definida.
* La suma modular es asociativa *(no lo voy a demostrar)*.
* Existe un elemento neutro $e=0$ para la suma modular en $Z_4$, tal que $x + e = x \quad \forall x \in Z_4$
* Cada elemento tiene un inverso $a' \in Z_4$, tal que $a + a' = 0$:
    * $0 + 0 = 0 \mod 4 = 0$
    * $1 + 3 = 4 \mod 4 = 0$
    * $2 + 2 = 4 \mod 4 = 0$
    * $3 + 1 = 4 \mod 4 = 0$

Por lo tanto, $(Z_4, +)$ es un grupo. Como la suma modular también es conmutativa, es un **grupo abeliano**.

## b. $(Z_4, \times)$. Enteros módulo 4 con el producto modular.

* El producto es una operación cerrada, ya que $x \times y$ da como resultado otro elemento en $Z_4 \quad \forall x,y \in Z_4$. Por lo tanto, está bien definida.
* El producto modular es asociativo *(tampoco lo voy a demostrar)*.
* Existe un elemento neutro $e=1$ para el producto modular en $Z_4$, tal que $x \times e = x \quad \forall x \in Z_4$
* No existe un inverso para cada elemento de $Z_4$: no existen elementos que, al operar con 2 y 0, den como resultado el elemento neutro.

Por lo tanto, $(Z_4, \times)$ **no** es un grupo.

## c. $(Z_3, \times)$. Enteros módulo 3 con el producto modular.

* El producto es una operación cerrada, ya que $x \times y$ da como resultado otro elemento en $Z_3 \quad \forall x,y \in Z_3$. Por lo tanto, está bien definida.
* El producto modular es asociativo *(otra vez lo voy a demostrar)*.
* Existe un elemento neutro $e=1$ para el producto modular en $Z_3$, tal que $x \times e = x \quad \forall x \in Z_3$
* No existe un elemento inverso para el $0 \in Z_3$, tal que $0 \times 0' = e$.

Por lo tanto, $(Z_3, \times)$ **no** es un grupo.

# 4. Sean $A_1 = \{ \overline 0, \overline 5 \}$ y $A_2 = \{ \overline 0, \overline 2, \overline 4, \overline 6, \overline 8 \}$ subconjuntos de $Z_{10}$:

## a. Probar que $A_1, A_2$ son subgrupos de $Z_{10}$

$Z_{10} = \{ \overline 0, \overline 1, \overline 2, \overline 3, \overline 4, \overline 5, \overline 6, \overline 7, \overline 8, \overline 9 \}$

$A_1 \subset Z_{10}, A_2 \subset Z_{10}$

Se quiere demostrar que $A_1, A_2$ son subgrupos de $Z_{10}$. Para esto, primero debe demostrarse que son grupos:
* La suma modular está bien definida para ambos, ya que $a + b = c \in A_1 \quad \forall a,b \in A_1, x + y = z \in A_2 \quad \forall x,y \in A_2$
* La suma modular es asociativa, ya que es asociativa en $Z_{10}$
* Tanto $A_1$ como $A_2$ tienen un único elemento neutro $e = 0$ para la operación, tal que $a + 0 = 0 + a = a$, para cualquier elemento de $A_1$ o $A_2$
* Cada elemento $\in A_1$ tiene un inverso tal que $a_1 + a_1' = 0$
    * $\overline 0: (0 + 0) \mod 10 = \overline 0$
    * $\overline 5: (5 + 5) \mod 10 = \overline 0$
* Cada elemento $\in A_2$ tiene un inverso $a_2' \in A_2$ tal que $a_2 + a_2' = 0$
    * $\overline 0: \overline 0 + \overline 0 = (0+0) \mod 10 = \overline 0$
    * $\overline 2: \overline 2 + \overline 8 = (2+8) \mod 10 = \overline 0$
    * $\overline 4: \overline 4 + \overline 6 = (4+6) \mod 10 = \overline 0$
    * $\overline 6: \overline 6 + \overline 4 = (6+4) \mod 10 = \overline 0$
    * $\overline 8: \overline 8 + \overline 2 = (8+2) \mod 10 = \overline 0$

Por lo tanto, $A_1$ y $A_2$ son grupos.

También se da que:
* El elemento neutro en $Z_{10}$ ($e$) está tanto en $A_1$ como $A_2$, y también es el neutro para la suma modular en dichos grupos.
* El inverso de cada elemento en $A_1$ también está en $A_1$. Lo mismo ocurre con $A_2$.
* La operación es cerrada.

Por lo tanto, $A_1$ y $A_2$ también son subgrupos de $Z_{10}$

## b. Mostrar que todo elemento de $Z_{10}$ puede escribirse como suma de elementos de $A_1$ y $A_2$ (es decir, para todo $x \in Z_{10}, x = x_1 + x_2$ con $x_1 \in A_1, x_2 \in A_2)$

$A_1$ está formado por los múltiplos de 5 en $Z_{10}$. Por otro lado, $A_2$ está formado por los múltiplos de 2.

Debido a esto, todos los números pares $\in Z_{10}$ se pueden escribir simplemente como la suma con el neutro, tal que $x = 0 + x : 0 \in A_1, x \in A_2$. El 5 puede escribirse de la misma manera a pesar de ser impar, ya que el neutro también está en $A_2$: $5 = 5 + 0 : 5 \in A_1, 0 \in A_2$

Los números restantes son los impares de $Z_{10}: \{ 1, 3, 9 \}$, para los cuales:
* $\overline 5 + \overline 6 = 11 \mod 10 = \overline 1 \quad \overline 5 \in A_1, \overline 6 \in A_2$
* $\overline 5 + \overline 8 = 13 \mod 10 = \overline 3 \quad \overline 5 \in A_1, \overline 8 \in A_2$
* $\overline 5 + \overline 4 = 9 \mod 10 = \overline 9 \quad \overline 5 \in A_1, \overline 4 \in A_2$

De esta manera se escribieron todos los elementos de $Z_10$ a partir de la suma de elementos de $A_1$ y $A_2$

# 5. Mostrar que $\overline 3$ es un generador del grupo cíclico $(Z_8, +)$.

$Z_8 = \{ \overline 0, \overline 1,\overline 2,\overline 3,\overline 4,\overline 5,\overline 6,\overline 7 \}$

Se quiere demostrar $Z_8 = <3>$. Para esto debe cumplirse $b = 3^k \quad \forall b \in Z_8$. Como la operación sobre el grupo es $+$, la potencia se ve como $3^k = 3k$. A partir de esto se puede obtener cada elemento de $Z_8$:
* $\overline 0 = 3 \times 0 = 0 \mod 8$
* $\overline 1 = 3 \times 3 = 9 \mod 8$
* $\overline 2 = 3 \times 6 = 18 \mod 8$
* $\overline 3 = 3 \times 1 = 3 \mod 8$
* $\overline 4 = 3 \times 4 = 12 \mod 8$
* $\overline 5 = 3 \times 7 = 21 \mod 8$
* $\overline 6 = 3 \times 2 = 6 \mod 8$
* $\overline 7 = 3 \times 5 = 15 \mod 8$

Se demostró que existe un entero $k$ para cada elemento $b \in Z_8$ tal que $b = 3^k$, por lo que 3 es un generador del grupo cíclico $Z_8$

## b. ¿Cuál es el orden del subgrupo cíclico generado por $\overline 2$?

El subgrupo $\overline 2$ se compone de todos los múltiplos de 2; escrito de otra manera, todos los elementos de $Z_8$ tales que $b = 2^k = 2k$:
* $\overline 2 \times 0 = \overline 0$
* $\overline 2 \times 1 = \overline 2$
* $\overline 2 \times 2 = \overline 4$
* $\overline 2 \times 3 = \overline 6$

Tal que $<2> = \{ \overline 0, \overline 2, \overline 4, \overline 6 \}$

Con $k = 4$ se da que $2^4 = 8 \mod 8 = \overline 0$. Como el 0 es el elemento neutro, se cumple $O(2) = 4$

> *Creo que otra manera de saber el orden es por la cantidad de elementos*