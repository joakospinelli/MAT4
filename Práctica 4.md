# 1. Sean los conjuntos $A = \{ 1, 0, -1 \}$ y $B = \{ 4, 3, 2, 1 \}$, decide si las siguientes corresponden a relaciones de A en B. Justifica.

## a. $R= \{ (1,1), (0,2)\}$

Sí, ya que sus elementos corresponden a un subconjunto de $A \times B$:

* $(1,1): 1 \in A;1 \in B$

* $(0,2): 0 \in A;2 \in B$

## b. $R = \{ (-1,1), (1,-1)\}$

No, ya que no existe en $A \times B$ el subconjunto $(1,-1)$:

* $(-1,1) : -1 \in A; 1 \in B$

* $(1,-1) : 1 \in A; -1 \notin B \to (1,-1) \not\subset A \times B$

## c. $R = \{(-1,1), (-1,2), (-1,3)\}$

Sí, ya que sus elementos corresponden a un subconjunto de $A \times B$:

* $(-1,1): -1 \in A; 1 \in B$

* $(-1,2): -1 \in A; 2 \in )$

* $(-1,3): -1 \in A; 3 \in B$

## d. $R = \{(4,1)\}$

No, ya que no existe en $A \times B$ el subconjunto $(4,1)$:

* $(4,1) : 4 \notin A; 1 \in B \to (4,1) \not\subset A \times B$

## e. $R = \{ \empty \}$

Sí, ya que aunque $R$ no tenga elementos igualmente puede obtenerse como un subconjunto de $A \times B$.

# 2. Sea $A = \{ -3, -2, -1, 0, 1, 2, 3\}$, $B = Z$ la una relación de $A$ con $B$ definida como: $xRy$ si y sólo si $y$ es el cuadrado de $x$.

## Escribir $R$ por extensión.

$R = \{(-3,9), (-2,4), (-1,1), (0,0), (1,1), (2,4), (3,9)\}$

## Definir $R^{-1}$ por comprensión y por extensión.

* **Comprensión:** $R^{-1} = \{ (y,x): x \in A; y \in B; x^2=y \}$

* **Extensión:** $R^{-1} = \{ (9,-3), (4,-2), (1,-1), (0,0), (1,1), (4,2), (9,3) \}$

# 3. Sean los conjuntos $A = \{a,b,c,d,e\}, V = \{vocales\}, B = \{1,2,3\}$. Decidir si las siguientes corresponden a relaciones válidas. Justificar:

## a. $R = \{(a,a,a);(a,b,c);(b,c,d)\}$ en $A\times A \times A$

Sí, ya que es un subconjunto del producto cartesiano:

* $\{ (a,a,a) \}: a \in A$
* $\{(a,b,c)\}: a \in A; b \in A; c \in A$
* $\{(b,c,d)\}: b \in A; c \in A; d \in A$

## b. $R=\{(a,a,a);(c,e,2);(a,b,1)\}$ en $A \times V \times B$

No, ya que el primer elemento no forma parte de ningún subconjunto posible para $A \times V \times B$:

* $\{ (a,a,a) \} : a \in A; a \in V; a \notin B \to R \not\subset A \times V \times B$

## c. $R = \{ (a,b,1); (e,c,2); (i,j,3)\}$ en $V \times A \times B$

No, ya que contiene elementos que no pertenecen a $V \times A \times B$, por lo tanto es un subconjunto inválido:

* $\{(a,b,1)\}: a \in V; b \in A; 1 \in B$

* $\{ (e,c,2) \}: e \in V; c \in A; 2 \in B$

* $\{ (i,j,3) \}: i \in V; j \notin A, 3 \in B \to R \not\subset V\times A \times B$

## d. $R = \{ (a,z,3); (b,i,2); (c,x,1) \}$ en $A \times V \times B$

No, ya que contienen elementos que no pertenecen a $A \times V \times B$, por lo que es un subconjunto inválido:

* $\{ (a,z,3)\}: a \in A; z \notin V; 3 \in B \to R \not\subset A \times V \times B$

# 4. Sea $A = \{ 1,2,3 \}$ y la relación $R$ en $A \times A \times A$ definida como: $(x,y,z) \in R$ si y sólo si $x < y; y < z$, siendo $<$ el "menor" usual entre números reales, escribir $R$ por extensión.

$R = \{ (1,2,3) \}$

# 5. Para cada una de las siguientes relaciones: dar tres pares que pertenezcan y tres pares que no. Indicar si son reflexivas, simétricas, antisimétricas y/o transitivas.

## a. En el conjunto de los números reales

### $xRy$ si y sólo si $x \ge 4; y \ge 5$

$(x,y) \in R$:
* $(4,5)$
* $(5,5)$
* $(6,5)$

$(x,y) \notin R$:
* $(0,0)$
* $(1,2)$
* $(4,4)$

$R$ no es reflexiva, ya que no se cumple $xRx$ para todos los elementos $x\in \real$.
* $0 \in \real; (0,0) \notin R$

$R$ no es simétrica, ya que que $(x,y)$ no implica $(y,x)$ para todos los elementos de la relación.
* $(4,5) \in R; (5,4) \notin R$

$R$ no es antisimétrica, ya que  en los casos que $(x,y) \to (y,x)$ no siempre se cumple que $x = y$
* $(8,9) \in R; (9,8) \in R; 8 \ne 9$

$R$ es transitiva, ya que $xRy$ y $yRz$ implican la existencia de $xRz$.
* $xRy = (4,5) \quad yRz=(5,6) \quad xRz = (4,6) \in R$

### $xRy$ si y sólo si $y \le x \le y+3$

$(x,y) \in R$
* $(1,1) = 1 \le 1 \le 4$
* $(2,1) = 1 \le 2 \le 4$
* $(2,2) = 2 \le 2 \le 5$

$(x,y) \notin R$
* $(1,2)$
* $(1,3)$
* $(1,4)$

$R$ es reflexiva, ya que se cumple $xRx$ para todos los elementos de $\real$:
* $xRx = (a,a) = a \le a \le a+3; a \in \real$

$R$ no es simétrica, ya que que $(x,y)$ no implica $(y,x)$ para todos los elementos de la relación.
* $(2,1) = 1 \le 2 \le 4; (2,1) \in R$
* $(1,2) = 2 \le 1 \le 5; (1,2) \notin R$ *// la condición de $R$ no se cumple*

$R$ es antisimétrica, ya que cuando se cumple $(x,y) \to (y,x)$ es porque se cumple que $x = y$

* $R$ no es simétrica, por lo que $(x,y) \not\to (y,x)$ para todos los pares $(x,y)$.
* $R$ es reflexiva, por lo que el par $(x,x) \in R$
    * $(a,a) = a \le a \le a+3; a \in \real$
    * Esto implica que $(x,y) \to (y,x)$ sí se cumple cuando $x=y$.

$R$ no es transitiva, ya que $xRy$ y $yRz$ no garantizan la existencia de $xRz$.
* $xRy = (5,4): 4 \le 5 \le 7$
* $yRz=(4,1): 1 \le 4 \le 4$
* $xRz: (5,1): 1 \le 5 \le 4; (5,1) \notin R$ *// la condición de $R$ no se cumple*

## b. Sean $A=\{ 1,2,3,4 \}$ y $P(A)$ el conjunto de partes de $A$

### En $P(A)$, $XRY$ si y sólo si $X \cap Y = \empty$

$(X,Y) \in X \cup Y = \empty$
* $\{ \{1\}, \{ 2,3,4 \} \}$
* $\{ \{2\}, \{ 1,3,4 \} \}$
* $\{ \{3\}, \{ 1,2,4 \} \}$

$(X,Y) \notin X \cup Y = \empty$
* $\{ \{1\}, \{ 1,2\} \}$
* $\{ \{2\}, \{ 2,4\} \}$
* $\{ \{3\}, \{ 3,4\} \}$

$R$ no es reflexiva, ya que no se cumple $XRX$ para ninguna partición de $P(A)$.
* $XRX =( \{ {a} , {b} \}, \{ {a} , {b} \}); \{ a,b\} \in P(A): X \cap X = \{ a,b\}$ *// siendo $a,b$ valores cualquiera $\in P(A)$*
* $X \cap X = \empty$ no se cumple para ninguna partición de $A$, a excepción del conjunto vacío.

$R$ es simétrica, ya que $XRY$ implica $YRX$ para todas las particiones de $A$.
* $XRY =  (\{ 1,2\}, \{ 3,4\}) : X \cap Y = \empty$
* $YRX =  (\{ 3,4\}, \{ 1,2\}) : Y \cap X = \empty$
* La intersección de conjuntos es una operación conmutativa, por lo que $X \cap Y = Y \cap X$. Esto quiere decir que, cuando la intersección es vacía, lo será independientemente del orden de la relación.

$R$ no es antisimétrica, ya que se cumple $XRY \to YRX$ incluso cuando $X \ne Y$.
* *// esto es lo mismo que el ejemplo anterior con $\{1,2\}, \{3,4\}$.*

$R$ no es transitiva, ya que $XRY$ y $YRZ$ no implican $XRZ$.
* $XRY = (\{ 1\}, \{ 2,3\}) \in R$
* $YRZ = (\{ 2,3\}, \{ 1,4\}) \in R$
* $XRZ = (\{1 \}, \{1,4\}) \notin R: X \cap Z = \{ 1\}$

### En $P(A)$, $XRY$ si y sólo si $X \subset Y$

$(X,Y) \in X \subset Y$
* $\{ \{ 1\}, \{ 1,2\} \}$
* $\{ \{ 1\}, \{ 1,2,3\} \}$
* $\{ \{ 1\}, \{ 1,2,3,4\} \}$

$(X,Y) \notin X \subset Y$
* $\{ \{ 1\}, \{ 1\} \}$
* $\{ \{ 1\}, \{ 2,3\} \}$
* $\{ \{ 1\}, \{ 3,4\} \}$

$R$ no es reflexiva, ya que no se cumple $XRX$ para ninguna partición de $P(A)$.
* La operación $\subset$ es estricta, por lo que no permite igualdad entre conjuntos.
* $XRX$ implica siempre que $X = X$, por lo cual nunca cumplirá la condición de $R$.

$R$ no es simétrica, ya que $XRY$ no implica $YRX$ para ninguna partición de $P(A)$.
* $XRY=\{ \{ 1\}, \{ 1,2\} \}: X \subset Y$
* $YRX = \{ \{ 1,2\}, \{ 1\} \}: Y \not\subset X$
* La operación $\subset$ implica que $X$ está contenido en $Y$, por lo tanto si se cumple $X \subset Y$ es imposible que, al mismo tiempo $Y$ sea un subconjunto de $X$.

$R$ no es antisimétrica, ya que $XRY \to YRX$ no se cumple aún cuando $X=Y$.

* $R$ no es reflexiva para ningún par $X,Y$, ya que la operación $\subset$ es estricta y no acepta igualdades.
* $R$ no es simétrica, ya que no se cumple $XRY \to YRX$ para ningún valor de $X,Y$.
* Por lo tanto, tampoco se cumple cuando $X=Y$. Esto no pasaría si en vez de $\subset$ fuese $\subseteq$.

$R$ es transitiva, ya que $XRY$ y $YRZ$ implican $XRZ$.

* $XRY = \{ \{ 1\}, \{ 1,2\} \} : X \subset Y$
* $YRZ = \{ \{ 1,2 \}, \{ 1,2,3 \} \}: Y \subset Z$
* $XRZ = \{ \{ 1\}, \{ 1,2,3 \} \}: X \subset Z$
* La operación $\subset$ en conjuntos en transitiva, indicando que el subconjunto de un subconjunto también pertenece a un conjunto original (👈 trabalenguas). Por lo tanto, la relación $R$ definida por esta operación también será transitiva.