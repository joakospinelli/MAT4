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