# 1. Determinar cuáles de las siguientes operaciones están bien definidas sobre el conjunto A dado. Analizar las propiedades en los casos afirmativos.

## a. $A = N, a \ast b = 3ab$

Está bien definida ya que, por definición, la multiplicación es cerrada dentro de los naturales, y $\ast$ es simplemente el producto de tres términos entre $a, b, 3 \in N$.

* Es conmutativa, ya que:
    * $(a\ast b) = (b\ast a)$
    * $3ab = 3ba$
* Es asociativa, ya que:
    * $(a \ast b) \ast c = a \ast (b \ast c)$
    * $3(3ab)c = 3a(3bc)$
    * $9abc = 9abc$
* No existe el elemento neutro, ya que:
    * $a \ast e = 3ae = a$
    * $e = \frac 1 3$
    * $e \notin N$

## b. $A = Z, a \ast b = \dfrac {a+b} {3+ab}$

No es una operación válida, ya que no es cerrada en ciertos casos importantes:
* Cuando la división de los términos $(a+b), (3+ab)$ **no** sea exacta, ya que el resultado de una división inexacta $\notin Z$

$$a = 1 \qquad b=1$$

$$\dfrac {a+b} {3+ab} = \dfrac 2 3$$

$$\dfrac 2 3 \notin Z$$

* Cuando el divisor sea 0, ya que la división por 0 no está definida en ningún conjunto numérico.

$$a = -1 \qquad b=3$$

$$\dfrac {a+b} {3+ab} = \dfrac 2 {3-3} = \dfrac 2 0$$

$$\dfrac 2 0 \notin Z$$

## c. $A = R, x \ast y=x+y-xy$

Está bien definida, ya que tanto la suma, resta y multiplicación entre números reales da como resultado otro número real, por lo que la operación es cerrada.

* Es conmutativa, ya que:
    * $a \ast b = b \ast a$
    * $x+y - xy = y+x - yx$
* Es asociativa, ya que:
    * $(a \ast b) \ast c = a \ast (b \ast c)$
    * $(x+y-xy)+z - (x+y-xy)z = x+(y+z-yz)-x(y+z-yz)$
    * $x+y+z-xy-zx-zy+xyz = x+y+z-yz -xy -xz +xyz$
* Tiene un elemento neutro, ya que:
    * $a \ast e = a$
    * $a+e-ae = a$
    * $a+(e-ae)=a$
    * $a+(0-a0) = a$
    * $e=0$

## d. $A = \{ 0, 1, 2, 3 \}$

| * | 0 | 1 | 2 | 3 |
| - | - | - | - | - |
| 0 | 0 | 0 | 0 | 0 |
| 1 | 0 | 1 | 2 | 3 |
| 2 | 1 | 2 | 0 | 2 |
| 3 | 2 | 3 | 1 | 1 |

Está bien definida, ya que todos los resultados posibles están dentro de $A$, por lo que es una operación cerrada.

* No es conmutativa, ya que:
    * $\exists a,b \in A : a \ast b \ne b \ast a$
    * $2 \ast 0 = 1 \quad 0 \ast 2 = 0$
* No es asociativa, ya que:
    * $(2 \ast 2) \ast 0 = 0 \ast 0 = 0 \ast 0$
    * $2\ast (2\ast 0) = 2\ast 1 = 2$
    * $(a \ast b) \ast c \ne a \ast (b \ast c) \quad \forall a,b,c \in A$
* Tiene un elemento neutro, ya que:
    * $a \ast e = e \ast a = a$
    * $a \ast 1 = a \quad \forall a \in A$

# 2. Demostrar que:

## a. Dado $M=\{ m \in N : n > 0\}, (M,+)$ es un semigrupo pero no es un monoide.

Es un semigrupo ya que:
* La suma es una operación binaria bien definida para $M$, ya que $a \ast b=c : a,b,c \in M$
* La suma es asociativa en $M$, tal que $(a+b)+ c = a+(b+c) \quad \forall a,b,c \in M$.

Sin embargo, no es un monoide ya que no existe un elemento neutro. El neutro para la suma de números naturales es 0; sin embargo, en la definición de $M$ se excluye dicho valor.

## b. El conjunto de un solo elemento $M = \{ e \}$ con la operación definida por $e \ast e = e$ es un monoide.

Es un monoide ya que:
* $ \ast $ es una operación binaria cerrada en $M$, por lo que está bien definida.
* Es asociativa, ya que:
    * $e \ast (e \ast e) = (e \ast e) \ast e$
    * $e=e$
* Existe un elemento neutro en $M$, el cual es el propio $e$:
    * $e \ast e = e$
    
## c. Dado un conjunto no vacío $A$, el conjunto de las partes $P(A)$ con la operación $\cap$ de conjuntos es un monoide conmutativo.

Es un monoide ya que:
* La intersección es una operación binaria bien definida para cualquier conjunto.
* La intersección entre dos partes de $A$ dará como resultado otra parte de $A$.
* La intersección de conjuntos es asociativa.
* El conjunto de partes siempre incluye al conjunto vacío, el cual es el elemento neutro para la intersección tal que $a \cap \empty = \empty \cap a = a \quad \forall a \in P(A)$

Por último, la intersección también es conmutativa, por lo que es un monoide conmutativo.

# 3. Demostrar que si para una operación asociativa $\ast $ en $A$ existe un elemento neutro $e$ y un elemento $a$ tiene inverso, entonces éste es único.

Se sabe que un elemento $e$ es neutro si se cumple $a\ast e = a$ para todo $a \in A$. Por otro lado, un elemento $a$ tiene un inverso $a'$ si se cumple $a\ast a' = e$.

Se quiere demostrar que dicho inverso es único para $a$, es decir, que $a$ sólo puede tener un inverso.

Supongamos que existen dos inversos de $a$, tales que:

$$a\ast b=e \qquad a\ast c=e \\ a\ast b = e = a\ast c$$

Como $\ast $ es asociativa, se puede escribir una operación tal que:
* $a \ast b = a \ast c$
* $b \ast (a \ast b) = b \ast (a \ast c)$
* $(b \ast a) \ast b = (b \ast a) \ast c$
* $e \ast b = e \ast c$
* $b = c$

Por lo tanto, el inverso de $a$ es único.

# 4. Sea $R$ una relación de congruencia sobre un semigrupo $(S,\ast)$, demostrar que $(S/R, \textcircled \ast)$ (el conjunto cociente y la operación inducida por $\ast$ sobre las clases de equivalencia) es un semigrupo llamado semigrupo cociente.

*// esto x ahora no lo voy a hacer*

# 5. Analizar si las siguientes son estructuras de grupo:

## a. $(Z,+)$

*Números enteros con la suma usual.*

* La suma es una operación válida para $Z$, ya que la suma de dos números enteros da como resultado otro entero.
* La suma entre enteros es asociativa.
* Existe un único neutro $e = 0 \in Z$ para la suma, tal que $a + e = a \quad \forall a \in Z$
* Cada elemento $a \in Z$ tiene un único inverso $a' = -a \in Z$ tal que $a + -a = e \quad \forall a \in Z$
* La suma es conmutativa, tal que $a+b = b+a \quad \forall a,b \in Z$

Por lo tanto, $(Z,+)$ tiene una estructura de grupo conmutativo.

## b. $(Z,.)$

*Números enteros con la multiplicación usual.*

* La multiplicación es una operación valida para $Z$, ya que el producto entre dos números enteros da como resultado otro entero.
* La multiplicación entre enteros es asociativa.
* Existe un único elemento neutro $e = 1 \in Z$ para la multiplicación, tal que $a.e = a \quad \forall a \in Z$
* No existe un inverso para cada elemento $a \in Z$, ya que el inverso para la multiplicación es $\frac 1 a$, pero éste no pertenece a $Z$.

Por lo tanto, $(Z,.)$ no tiene estructura de grupo, sino que es un monoide.

## c. $(R^2, +)$

*Pares ordenados de reales con la suma usual.*

* La suma es una operación válida para $R^2$, ya que al sumar dos pares ordenados se obtiene un nuevo par ordenado $\in R^2$
* La suma entre pares ordenados es asociativa.
* Existe un único elemento neutro $e = (0,0) \in R^2$ para la suma, tal que $(a,b) + (0,0) = (a,b) \quad \forall (a,b) \in R^2$
* Cada par $(a,b) \in R^2$ tiene un elemento neutro $(-a, -b) \in R^2$ tal que $(a,b) + (-a, -b) = (0,0)$
* La suma es conmutativa, tal que $(a,b) + (c,d) = (c,d) + (a,b)$

Por lo tanto, $(R^2, +)$ tiene estructura de grupo conmutativo.

## d. $(M_{2 \times 2}, +)$

*Matrices de 2x2 con la suma usual de matrices.*

* La suma es una operación válida para $M_{2 \times 2}$, ya que al sumar dos matrices de $2 \times 2$ se obtiene una nueva matriz de $2 \times 2$
* La suma entre matrices es asociativa.
* Existe una única matriz neutra $0 = \begin{matrix} 0 & 0 \\ 0 & 0\end{matrix} \in M_{2 \times 2}$ tal que $A + 0 = A \quad \forall A \in M_{2 \times 2}$
* Para cada matriz $A \in M_{2 \times 2}$ existe un inverso $A' \in M_{2 \times 2}$ formada por los mismos elementos de $A$ pero negados, tal que $A + A' = 0$
* La suma de matrices es conmutativa, tal que $A+B = B+A$

Por lo tanto, $(M_{2 \times 2}, +)$ tiene estructura de grupo.

## e. $(P(A), \cup)$

*Conjunto de partes de $A$ con la unión de conjuntos.*

* La unión es una operación válida para $P(A)$, ya que al unir dos subconjuntos de $A$ se obtiene nuevamente un subconjunto de $A$.
    * En el mayor de los casos puede obtenerse $A$, el cual forma parte de $P(A)$.
* La unión de conjuntos es asociativa.
* Existe un subconjunto neutro $e = \empty \in P(A)$ tal que $B \cup \empty = B \quad \forall B \in P(A)$
* No existe un inverso $B'$ para cada elemento $B \in A$ que cumple $B \cup B' = \empty$

Por lo tanto, $(P(A), \cup)$ no tiene estructura de grupo. Es únicamente un monoide.

# 6. Probar que en todo grupo el único elemento idempotente es el neutro.

*// idempotencia es que, al realizar una acción N veces, se obtiene el mismo resultado que al realizarla una vez*

Un elemento $e$ es neutro en su grupo $(A, \ast)$, ya que $a \ast e = a \quad \forall a \in A$.

* Como $(A,\ast )$ es un grupo, entonces la operación $\ast $ está bien definida, es cerrada y el resultado de $a\ast b \in A \quad \forall a,b \in A$
* Como $e \in A$, se cumple que $e \ast e = e$
* Esto quiere decir que $e^n = e\ast e\ast ...\ast e \in A : e^n = e$

Por lo tanto, al operar sobre el elemento neutro $n$ veces el resultado va a seguir siendo el mismo, entonces $e$ es idempotente.

Esto no se cumple para ningún otro elemento de $A$. Se demostrará con un contraejemplo:
* $a \ast a = a \quad a \in A$
* $a' \ast  (a\ast a) = a'\ast a$
* $(a'\ast a)\ast a = a'\ast a$ // Se sabe que $\ast $ es asociativa, ya que $(A,\ast )$ es un grupo.
* $e\ast a = a'\ast a$
* $e\ast a=e$
* $e\ast a = e\ast e = e$
* Por lo tanto, $e=a$

Esto implica que el único caso en el que se cumple la idempotencia es cuando el elemento $a \in A$ es el neutro, el cual es único.

# 7. Mostrar que en todo grupo vale la propiedad cancelativa.

Un grupo $(A,\ast)$ tiene las siguientes propiedades:
* $\ast$ es una operación binaria bien definida sobre $A$.
* $\ast$ es asociativa.
* Existe un elemento neutro $e$ para $\ast$ en $A$.
* Existe un inverso $a'$ en la operación $*$ para cada elemento en $a \in A$.

Se quiere demostrar que se cumple la propiedad cancelativa, definida como $a\ast b = a\ast c \implies b=c$

* $a\ast b = a\ast c$
* $a'\ast (a\ast b) = a'\ast (a\ast c)$
* $(a'\ast a)\ast b = (a'\ast a)\ast c$
* $e\ast b = e\ast c$
* $\dfrac {e\ast b} e = \dfrac {e\ast c} e$
* $b=c$

# 8. Sea $(G,\ast)$ un grupo tal que todo elemento es su propio inverso, probar que $G$ es abeliano.

Un grupo tiene un elemento neutro $e$ tal que $a\ast e = a \quad \forall a \in G$

Un número tiene un inverso $a'$ tal que $a \ast  a' = e$

En este caso, se da que $a' = a \quad \forall a \in A$. Se quiere demostrar que, bajo estas condiciones, también se da que $G$ es abeliano, tal que $a\ast b = b\ast a \quad \forall a,b \in G$

* $a\ast a = e$
* $b\ast b = e$
* $(a\ast b) \ast  (a\ast b) = e \quad (a\ast b) \in G, (a\ast b)' = (a\ast b)$
* $a \ast  (b\ast a) \ast b = e$
* $(a\ast  (b\ast a) \ast  b) \ast b= e\ast b$ // Multiplico por $b$ ambos lados
* $a\ast (b\ast a)\ast (b\ast b)= b$
* $a\ast (b\ast a)\ast e = b$
* $a\ast (b\ast a) = b$ // Elimino el neutro ya que no influye en la operación
* $a\ast (a\ast (b\ast a)) = a\ast b$ // Multiplico por $a$ ambos lados
* $(a\ast a)\ast (b\ast a) = a\ast b$
* $e\ast (b\ast a) = a\ast b$
* $b\ast a = a\ast b$

Por lo tanto, se demostró que se cumpla la conmutatividad $a\ast b = b\ast a \quad \forall a,b \in G$ bajo la condición de que $a' = a$

# 9. Dado un grupo $(G,\ast)$, probar que $G$ es abeliano si y sólo si para cualquier $x,y$ en $G$ vale que $(x\ast y)^2 = x^2\ast y^2$

$(G,\ast)$ es un grupo, por lo que:
* $\ast$ es una operación binaria bien definida sobre $G$.
* $\ast$ es asociativa.
* Existe un elemento neutro $e$ para $\ast$ en $G$ tal que $a\ast e = a \quad \forall a \in G$
* Existe un inverso $a'$ en la operación $\ast$ para cada elemento en $a \in G$ tal que $a\ast a'=e$

Se quiere demostrar que, para que $(G,\ast)$ cumpla con la conmutatividad, necesariamente debe darse $(x\ast y)^2 = x^2 \ast y^2 \quad \forall x,y \in G$

Asumiendo que $(G,\ast)$ es abeliano:
* $(x\ast y)^2 = (y\ast x)^2$ // Por conmutatividad
* $(x\ast y)\ast (x\ast y) = (y\ast x)\ast (y\ast x)$ // Como es abeliano puedo conmutar y asociar como quiera
* $(x\ast x)\ast (y\ast y) = (x\ast x)\ast (y\ast y)$
* $x^2\ast y^2 = x^2\ast y^2$

Por lo tanto, cuando $\ast $ es conmutativa se cumple $(x\ast y)^2 = x^2\ast y^2$