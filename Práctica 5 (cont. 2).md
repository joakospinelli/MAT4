# 1. Analizar si las siguientes funciones son homomorfismos entre las estructuras algebraicas indicadas. En caso afirmativo, hallar núcleo e imagen.

> *"Homomorfismo" es lo mismo que morfismo, no especifica nada en particular como mono, epi o isomorfismo.*

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

El complemento se define como todos los elementos del universo que no forman parte de $X$. La única parte de $A$ que cumple con esto es el conjunto vacío, tal que $\{ \emptyset \}^C = A$ (porque no tiene ningun elemento, entonces todo el universo **no** está en $X$).

Por lo tanto, $Nu(f) = \{ \emptyset \}$

### Imagen

$Im(f) = \{ X \in P(A) : \exists Y \in P(A), f(Y) = Y^C = X\}$

Como el dominio y el codominio trabajan con los mismos conjuntos, se da el caso de que el complemento de cualquier partición de $A$ es otra partición de $A$.

Dicho de otra manera, cualquier subconjunto $P \subset A$ puede escribirse como el complemento de otro subconjunto $S \subset A$. Por otro lado, $A$ puede escribirse como el complemento del conjunto vacío (y viceversa).

Por lo tanto, $Im(f) = P(A)$

# 2. Sea $f: G \to H$ un homomorfismo de grupos, demostrar que el núcleo y la imagen son subgrupos de $G$ y $H$ respectivamente.

El conjunto del grupo se define como

$$Nu(f) = \{ a \in G : f(a) = e_2 \}$$

A partir de las propiedades de morfismo se cumplen implícitamente algunas propiedades de los subgrupos:
* $f(e_1) = e_2$, por lo que el neutro de $G$ se encuentra en el núcleo.
* $f(a^{-1}) = f(a)^{-1}$, tal que $f(a^{-1}) = e_2^{-1} = e_2 \quad \forall a \in Nu(f)$ y, por lo tanto, $a^{-1} \in Nu(f)$

Por último, se debe probar que la operación es cerrada en $Nu(f)$. Dados $a, b \in Nu(f)$
* $f(a \ast b) = f(a) \ast f(b)$
* $f(a) \ast f(b) = e_2 \ast e_2 = e_2 \quad e_2 \in Nu(f)$
* $f(a \ast b) \in Nu(f) \quad \forall a,b \in Nu(f)$

Por lo tanto, el núcleo de $f: G \to H$ es un subgrupo del grupo $G$.

El conjunto de la imagen se define como

$$Im(f) = \{ h \in H : \exists g \in G, f(g) = h \}$$

A partir de las propiedades de morfismos se cumplen implícitamente algunas propiedades de los subgrupos:
* $f(e_1) = e_2$, por lo que el neutro se encuentra en la imagen.
* $f(a^{-1}) = f(a)^{-1}$, tal que $f(a) = h,\  \ f(a)^{-1} = h^{-1} = f(a^{-1})$, por lo que cada elemento $a \in Im(f)$ tiene a su inverso.

Por último, se quiere probar que la operación es cerrada en $Im(f)$. Dados $a,b \in Im(f), x,y \in G : f(x) = a, f(y) = b$

* $f(x \ast y) = f(x) \ast f(y)$
* $f(x) \ast f(y) = a \ast b$, siendo $a \ast b$ cerrada en $Im(f)$

Por lo tanto, la imagen generada a partir de $f: G \to H$ es un subgrupo de $H$.

# 3. Sea $(G, \ast)$ un grupo, demostrar que la función $f: G \to G$ definida por $f(a) = a^2$ es un homomorfismo si y sólo si $G$ es abeliano.

Un grupo es abeliano si la operación definida sobre él es conmutativa.

## Suponiendo que $G$ es abeliano

Se da que $(a \ast b) = (b \ast a)$ y, por lo tanto, $f(a \ast b) = (a \ast b)^2 = (b \ast a)^2 = f(b \ast a)$.

* $f(a \ast b) = (a \ast b)^2$
* $(a \ast b)^2 = (a \ast b) \ast (a \ast b)$
* $(a \ast b) \ast (a \ast b) = a \ast b \ast a \ast b$
* $a \ast b \ast a \ast b = a \ast a \ast b \ast b$ // Este reordenamiento sólo puede realizarse gracias a la conmutatividad de $G$.
* $a \ast a \ast b \ast b = (a \ast a) \ast (b \ast b)$
* $(a \ast a) \ast (b \ast b) = a^2 \ast b^2 = f(a) \ast f(b)$

Por lo tanto, la conmutatividad es necesaria para cumplir la propiedad del morfismo $f(a \ast b) = f(a) \ast f(b)$.

## Suponiendo que $f: G \to G$ es un morfismo

Se da $f(a \ast b) = f(a) \ast f(b)$. Esto implica $(a \ast b)^2 = a^2 \ast b^2$

* $f(a \ast b) = f(a) \ast f(b)$
* $(a \ast b)^2 = a^2 \ast b^2$
* $(a \ast b) \ast (a \ast b) = (a \ast a) \ast (b \ast b)$
* $a \ast b \ast a \ast b = a \ast a \ast b \ast b$
* $a \ast (b \ast a) \ast b = a \ast (a \ast b) \ast b$

El morfismo sólo es válido cuando $(a \ast b) = (b \ast a)$, por lo que $G$ debe ser un grupo abeliano.

# 4. Si $H_1, H_2$ son dos subgrupos de un grupo conmutativo $G$, probar que la aplicación $f: H_1 \times H_2 \to G$ dada por $f(a,b) = ab$ es un morfismo de grupos.

Como $H_1, H_2$ son subconjuntos de $G$, se sabe que todos los elementos de $H_1$ y $H_2$ también estarán en $G$.

Como $G$ es un grupo conmutativo, se sabe que:
* La operación entre sus elementos es cerrada.
* La operación es distributiva.
* Existe un elemento neutro $e$ tal que $ae = a$
* Cada elemento tiene un inverso tal que $a(a') = e$
* $ab = ba$

Por lo que dado el par $(a,b)$ resultante de $H_1 \times H_2$, se da que $a, b \in G,\ ab \in G,\ ab = ba$

Para probar que $f$ es un morfismo se verificará si las operaciones se respetan:
* $f((a,b) \ast (c,d)) = f(a,b) \ast f(c,d)$
* $f(ac, bd) = a \ast b \ast c \ast d$
* $a \ast c \ast b \ast d = a \ast b \ast c \ast d$ // Por conmutatividad

Existe un elemento neutro $(e, e) \in H_1 \times H_2$ tal que:
* $f((a,b) \ast (e,e)) = f(a,b) \ast f(e,e)$
* $f(ae, be) = a \ast b \ast e \ast e$
* $f(a,b) = a \ast b$

Por último, cada elemento $(a,b) \in H_1 \times H_2$ tiene un inverso $(a', b')$ tal que:
* $f(a,b)^{-1} = f((a,b)^{-1})$
* $(ab)^{-1} = f(a', b')$
* $a'b' = a'b'$

Por lo tanto, $f$ es un morfismo de grupos válido.

# 5. Si $f: G_1 \to G_2$ es un morfismo de grupos, entonces es monomorfismo si y sólo si $Nu(f) = \{ e_1 \}$

Un monomorfismo es un tipo de morfismo en el que no existen dos elementos del dominio con la misma imagen; es decir, a cada elemento del dominio le corresponde un único elemento y ese no se repite para ningún otro. Esto puede escribirse como $f(x) = f(y) \iff x = y$

## Suponiendo $Nu(f) = \{ e_1 \}$

Proposiciones:
1. $f(e_1) = e_2$
2. $Nu(f) = \{ e_1 \}$

Se partirá de un caso $f(x) = f(y)$; es decir, dos elementos con la misma imagen. Se buscará demostrar que esto sólo es posible si $x = y$ (es decir, $f$ es un monomorfismo) a partir de nuestras proposiciones.

* $f(x) = f(y) \implies f(x') = f(y')$

* $f(x') = f(y') \implies f(x) \ast f(y') = e_2$
* $f(x) \ast f(y') \implies f(x \ast y') = e_2$

Sabemos por la proposición 2 que $e_1$ es el único elemento de $G_1$ cuya imagen es el neutro de $G_2$. Por lo tanto, debe darse que $(x \ast y') = e_1$, lo cual es posible sólo cuando $y' = x'$, tal que $x = y$.

De esta manera, se demostró que $f$ es una función inyectiva y, por lo tanto, un monomorfismo.

## Suponiendo monomorfismo

Proposiciones:
1. $\forall x,y \in G_1: f(x) = f(y) \iff x = y$
2. $f(e_1) = e_2$

Debido a la proposición 1 (definición de monomorfismo), se da que $f(x) = e_2 \iff x = e_1$, por lo que $e_1$ es el único elemento de $G_1$ cuya imagen es el neutro de $G_2$

El núcleo se define como:

$$Nu(f) = \{ a \in G_1 : f(a) = e_2 \}$$

El único elemento que cumple esa condición es $e_1$, por lo que cuando $f$ es un monomorfismo, se da que $Nu(f) = \{ e_1 \}$

# 6. Sea $(G, \ast)$ un grupo, demostrar que la función $f: G \to G$ definida por $f(a) = a^{-1}$ es un isomorfismo si y sólo si $G$ es conmutativo.

## Si $G$ es conmutativo:

Se quiere demostrar que $f$ es un isomorfismo, por lo que debe ser tanto inyectiva como sobreyectiva.

$f$ es un homomorfismo válido, ya que:
* $f(a \ast b) = f(a) \ast f(b)$
* $(a \ast b)^{-1} = a^{-1} \ast b^{-1}$
* $b^{-1} \ast a^{-1} = a^{-1} \ast b^{-1}$ // iguales por conmutatividad de $G$

Existe un elemento neutro $e_1 \in G$ tal que $f(e_1) = e_1^{-1} = e_1$

Para cada elemento $a \in G$ se da que:
* $f(a^{-1}) = (f(a))^{-1}$
* $a = (a^{-1})^{-1}$
* $a = a$

Por lo que se respetan las operaciones.


Como $G$ es un grupo, podemos utilizar la propiedad de los inversos:
$$\forall a \in G \quad \exists a^{-1} : a \ast a^{-1} = e_1$$

Como el inverso es único para cada elemento, se da que $x^{-1} = y^{-1} \iff x = y$, tal que $f(x) = f(y) \iff x = y$, por lo que $f$ es **inyectiva**.

Como $G$ es un grupo, cada elemento tiene su inverso. De esto puede interpretarse al revés, diciendo que para cada inverso $g \in G$ existe otro elemento $a$ tal que $f(a) = g$, siendo $g = a^{-1}$, por lo que $f$ es **sobreyectiva**.

Como $f$ es inyectiva y sobreyectiva, se da que es un isomorfismo.

## Si $G$ es un isomorfismo:

Proposiciones:
* $\forall x,y \in G: f(x) = f(y) \iff x = y$
* $\forall g \in G: \exists x \in G: f(x) = g$

La operación puede escribirse como:
* $f(a \ast b) = f(a) \ast f(b)$
* $(a \ast b)^{-1} = a^{-1} \ast b^{-1}$
* $b^{-1} \ast a^{-1}= a^{-1} \ast b^{-1}$

$f$ es un morfismo válido sólo cuando se cumple la igualdad $a^{-1} \ast b^{-1} = b^{-1} \ast a^{-1}$, por lo que $G$ es un grupo conmutativo.