# 1. Analizar si las siguientes funciones son homomorfismos entre las estructuras algebraicas indicadas. En caso afirmativo, hallar núcleo e imagen.

> *"Homomorfismo" es lo mismo que morfismo, no especifica nada específico como mono, epi o isomorfismo.*

## a. $f: G \to F$ dada por $f(x) = 2^x$, siendo los grupos $G = (R,+)$ y $F = (R_0, .)$

$f(x) = 2^x$

$2^x \ne 0 \quad \forall x \in R$

Por lo tanto, existe una correspondencia válida entre $F$ y $G$.

A continuación se evaluará si las operaciones se respetan:

* $f(x+y) = 2^{x+y}$
* $2^{x+y} = 2^x \times 2^y = f(x)f(y) \quad \forall x,y \in R$

Por lo tanto, $f(x) = 2^x$ es un homomorfismo válido entre $G$ y $F$.

## Núcleo

$e_2 = 1 \in R_0 : x \times 1 = x \quad \forall x \in G$

Se quiere hallar $Nu(f) = \{ a \in F : f(a) = e_2 \}$, es decir, los elementos de $F$ cuya imagen corresponde al neutro de $G$.

Por definición de potencia, se sabe que $x^0 = 1 \quad \forall x \in R$, por lo que $2^0 = e_2$

En conclusión, $Nu(f) = \{ 0 \}$

## Imagen

Se quiere hallar $Im(f) = \{ m \in R_0 : \exists x \in R, f(x) = m \}$

$f(x) = 2^x$ es una función exponencial, por lo que:
* Su valor siempre estará dentro de los reales positivos
* Es una función continua que crece infinitamente
* Nunca se dará $f(x) = 0$

En conclusión, $Im(f) = (0, \infty)$

## b. $f: G \to F$ dada por $f(x) = -x$, siendo los grupos $G = (Z, \ast)$ y $F=(Z, \circ)$

$a \ast b = a + b + ab$

$a \circ b = a + b - ab$

$f(x) = -x$

Se evaluará si las operaciones se respetan:

* $f(a \ast b) = f(a) \circ f(b)$
* $-(a \ast b) = (-a) \circ (-b)$
* $-(a+b+ab) = (-a) + (-b) - (-a)(-b)$
* $-a-b-ab = (-a) + (-b) - ab$
* $-a-b-ab = -a-b-ab$

Las operaciones en $G$ se corresponden en $F$, por lo que la función $f$ es un morfismo válido.

### Núcleo

Primero debe encontrarse el neutro de $F$, tal que $a\circ e_2 = a + e_2 - a \times e_2 = a$
* $a \circ 0 = a + 0 - a \times 0$
* $a - 0 = a \quad \forall a \in Z$
* $e_2 = 0$

$Nu(f) = \{ a \in G : f(a) = e_2 \}$

* $f(a) = -a$
* $f(0) = 0$

Siendo $a=0 \in G$ el único caso en el que se cumple $f(a) = 0$.

En conclusión, $Nu(f) = \{ 0 \}$

### Imagen

$Im(f) = \{ x \in F : \exists m \in G, f(x) = m \}$

Sea $x \in F$ un entero cualquiera, pueden darse tres casos:
* $x$ es un entero positivo, tal que $f(x) = -x$
* $-x$ es un entero negativo, tal que $f(-x) = x$
* $x = 0$, tal que $f(x) = 0$

Por lo tanto, $Im(f) = Z$

## c. $f: (P(A), \cup) \to (P(A), \cap)$, dada por $f(X) = X^C$

Se evaluará si las operaciones se respetan:

* $f(P_1 \cup P_2) = f(P_1) \cap f(P_2)$
* $(P_1 \cup P_2)^C = {P_1}^C \cap {P_2}^C$ // esto se cumple x propiedades de complementos

Por lo tanto, $f$ es un morfismo válido.

### Núcleo

El neutro de la intersección es $e_2 = \{ A \}$, tal que $P(A) \cap A = P(A)$ para cualquier partición de $A$.

$Nu(f) = \{ X \in P(A) : f(X) = X^C = A \}$

El complemento se define como todos los elementos del universo que no forman parte de $X$. La única parte de $A$ que cumple con esto es el conjunto vacío, tal que $\{ \empty \}^C = A$ (porque no tiene ningun elemento, entonces todo el universo **no** está en $X$).

Por lo tanto, $Nu(f) = \{ \empty \}$

### Imagen

$Im(f) = \{ X \in P(A) : \exists Y \in P(A), f(Y) = Y^C = X\}$

Como el dominio y el codominio trabajan con los mismos conjuntos, se da el caso de que el complemento de cualquier partición de $A$ es otra partición de $A$.

Dicho de otra manera, cualquier subconjunto $P \subset A$ puede escribirse como el complemento de otro subconjunto $S \subset A$. Por otro lado, $A$ puede escribirse como el complemento del conjunto vacío (y viceversa).

Por lo tanto, $Im(f) = P(A)$