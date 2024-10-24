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

# 10. Dados los grupos $(G, \ast)$ y $(F, \diamond)$, se define en el conjunto $G \times F$ la ley $\bullet$ tal que $(x,y) \bullet (z,t) = (x \ast z, y \diamond t)$. Probar que $(G \times F, \bullet)$ es un grupo.

*Esta estructura se denomina Grupo Producto*

Como $(G, \ast)$ y $(F, \diamond)$ son grupos, se saben las siguientes propiedades de $\ast, \diamond$:
* Son operaciones binarias bien definidas sobre sus respectivos conjuntos.
* Son asociativas.
* Existe un elemento neutro para la operación en un respectivo conjunto.
* Cada elemento tiene un inverso.

A partir de esto, se quiere demostrar que la operación $\bullet$ definida sobre $G \times F$ cumple estas mismas propiedades.

$(x,y) \bullet (z,t) = (x \ast z, y\diamond t)$

Operación bien definida:
* Se sabe que $x,z \in G, y, t \in F$
* Por lo tanto, $x \ast z$ es una operación cerrada en $G$ y $y \diamond t$ es cerrada en $F$.
* Por lo tanto, el resultado de operar entre dos pares de $G \times F$ dará otro par del mismo conjunto.

Asociativa:
* $(a,b) \bullet((x,y) \bullet (z,t)) = ((a,b) \bullet (x,y)) \bullet (z,t)$
* $(a,b) \bullet (x \ast z, y\diamond t) = (a \ast x, b\diamond y) \bullet (z,t)$
* $((x \ast z) \ast a, (y\diamond t) * b) = ((a \ast x) \ast z, (b\diamond y) \diamond t)$
* Ya se sabe que $\ast$ y $\diamond$ son asociativas, por lo que se cumple la asociatividad.

Existencia de neutro:
* Existe un neutro $e \in G$ tal que $a \ast e = a \quad \forall a \in G$
* Existe un neutro $d \in F$ tal que $b \diamond f = d \quad \forall b \in F$
* Por lo tanto, existe un par $(e,d) \in G \times F$ tal que:
    * $(a,b) \bullet (e,d) = (a \ast e, b \diamond d) = (a,b)$
    * Por lo que $(e,d)$ es el neutro para la operación $\bullet$

Existencia del inverso:
* Para todo elemento $a \in G$ existe un inverso tal que $a \ast a' = e$
* Para todo elemento $b \in F$ existe un inverso tal que $b \ast b' = d$
* Por lo tanto, existe un par $(a', b') \in G \times F$ tal que:
    * $(a,b) \bullet (a', b') = (a \ast a', b \diamond b') = (e,d)$
    * Siendo $(e,d)$ el neutro de $\bullet$, por lo que existe un inverso $(a',b')$ para todo $(a,b) \in G\times F$

# 11. Estudiar si son subgrupos de los grupos indicados:

## a. Los enteros pares de $(Z, +)$

Para que el conjunto de los pares sea un subgrupo de $(Z,+)$ debe cumplirse:
* $Pares \subset Z$
* $e \in H : a + e = a \quad \forall a \in Pares$
* $a,b \in Pares \implies a+b \in Pares$
* $a \in Pares \implies a' \in Pares : a + a' = e$

Los números pares son un subconjunto de los números enteros, por lo que dicha propiedad se cumple.

Existe el elemento neutro $e = 0$, el cual siempre se debate si es par o no pero definiendo a los pares como $x = 2k$ sí lo es.

La suma de números pares siempre da otro número par. Esto se puede demostrar como:
* $a = 2k, b = 2m \quad k,m \in Z$
* $a+b = c$
* $2k + 2m = c$
* $c = 2(k+m) \quad (k+m) \in Z$

Sigue existiendo el inverso $a' = -a$ para todos los números enteros pares, tales que $a + a' = a-a = 0 \quad \forall a \in Pares$

Por lo tanto, los enteros pares son un subgrupo de $(Z,+)$.

## b. Las matrices simétricas de $2 \times 2$

*// no entendí el enunciado directamente*

# 12. Demostrar que si $H$ y $K$ son subgrupos de $(G, \ast)$, entonces $H \cap K$ es un subgrupo de $(G, \ast)$.

Se sabe que tanto $(H, \ast)$ como $(K, \ast)$ cumplen con las condiciones para ser subgrupos de $(G, \ast)$. A partir de esto se examinará el comportamiento de su intersección.

Operación cerrada:
* Sea $a,b \in H \cap K$ se sabe que $a,b \in H \quad a,b \in K$
* Esto implica que $a*b$ es cerrada tanto en $H$ como en $K$.
* Su resultado también estará dentro de la intersección, por lo que la operación es cerrada.

Existencia del neutro:
* Para que $H$ y $K$ sean subgrupos de $(G,\ast)$ debe cumplirse para el elemento neutro, de forma independiente, que $e \in H$ y $e \in K$.
* Como $e$ se encuentra en ambos conjuntos, necesariamente estará en su intersección.
* Por lo tanto, el elemento neutro de la operación se encuentra en $H \cap K$.

Existencia de inversos:
* Sea $a$ un elemento tal que $a \in H$ y $a \in  K$, existe un inverso $a'$ tal que $a \ast a' = e$
* Como $H$ es un subgrupo de $(G,\ast)$, el inverso $a'$ también se encuentra en el conjunto. Lo mismo ocurre con $K$.
* Por lo tanto, el inverso también existe dentro de la intersección.

A partir de la premisa de que $(H, \ast)$ y $(K, \ast)$ sean subgrupos de $(G, \ast)$, se demostró que en $H \cap K$ la operación $\ast$ es cerrada, existe el elemento neutro $e$ y cada elemento $a$ tiene su inverso $a'$. Por lo tanto, $H \cap K$ es un subgrupo de $G(\ast)$.

# 13. Sea $(G, \ast)$ un grupo, sea $a \in G$ y $H$ un subgrupo de $G$, demostrar que el conjunto $aHa^{+1} = \{ a \ast h \ast a^{-1} : h \in H \}$ es un subgrupo de $G$.


# 14. Probar que todo grupo cíclico es abeliano.

Un grupo es cíclico si existe un elemento $a \in G$ tal que para otro elemento $b$ existe un entero $k$ tal que $b = a^k$.

Por definición de la potencia, sabemos que $a^k = a \ast a \ast ... \ast a$ ($k$ veces).

A partir de esto, se quiere demostrar que $a \ast b = b \ast a$:
* Dado $a,b \in G$, existen dos enteros $k, j$ tales que $a  = g^k, b = g^j$
* $a \ast b = g^k \ast g^j$
* $a \ast b = g^{(k + j)}$
* $a \ast b = g^{(j + k)}$ // Por conmutatividad de la suma de enteros
* $a \ast b = g^j \ast g^k$
* $a \ast b = b \ast a$

Por lo tanto, para todo grupo cíclico se cumple la propiedad de conmutatividad.

# 15. Sea $G$ un grupo cíclico de orden $n$, si $m$ es divisor de $n$ entonces el elemento $a^m$ y sus potencias generan un subgrupo.

*// qué este enunciado? una afirmación? lo tengo que demostrar?*

$G = \{ e, a, a^2, ... , a^{n-1} \}$

$G^m = \{ e, a^m, a^{m2}, ... , a^{m(k-1)} \}$

$m|n : n = m \times g$

$G^m$ es de orden $g$, ya que $(a^m)^g = a^n =e$. Como $g = \frac n m$, también puede escribirse el orden de esa forma.

A partir de esto se demostrarán las propiedades de grupo de $G^m$:
* Es un conjunto no vacío, ya que contiene las potencias de $a$ hasta $a^m(k-1)$
* Es una operación cerrada, ya que $a^{hm} \ast a^{km} = a^{(h+k)m} \in G^m$
* Tiene al elemento neutro, ya que como se demostró antes, existe un entero $g : (a^m)^g = a^n = e$, siendo $e$ el neutro para la operación $\ast$.
* Cada elemento tiene a su inverso, tal que:
    * $a^{mi} \ast (a^{mi})^{-1} = e$
    * $a^{mi} \ast a^{-mi} = e, a^{-mi} \in G^m$

# 16. Sea $(G, \ast)$ un grupo, sea $a \in G$ y $H$ un subgrupo de $G$. Si $a,b \in G$, probar que la relación dada por $a \equiv b \pmod H$ si $a \ast b^{-1} \in H$ es una relación de equivalencia.
