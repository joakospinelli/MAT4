# Estructuras algebraicas

Son conjuntos no vacíos en los que se definen una o más operaciones, las cuales deben ser **cerradas**.

> una operación es cerrada en un conjunto si da como resultado un elemento del mismo conjunto: por ejemplo, la división de enteros no es cerrada porque $\frac 2 3 \notin Z$
## Propieades

Dada una estructura algebraica $(A,\ast)$:
* $\ast$ es conmutativa si $\forall a,b \in A : a \ast b = b \ast a$
* $\ast$ es asociativa si $\forall a,b,c \in A : a \ast (b \ast c) = (a \ast b) \ast c$
* $(A,\ast)$ tiene neutro si existe un elemento $e \in A : a \ast e = e \ast a = a \quad \forall a \in A$
* Cada elemento $a \in A$ tiene un inverso $a' \in A$ si se cumple $a' \ast a = a \ast a' = e$
* Si existe un neutro, este es único.
* Si para una operación asociativa existe un neutro $e$, para todo elemento $a$ existe un inverso $a'$ que es único para cada elemento.
* Si una operación tiene neutro y cada elemento tiene inverso, se cumple la propiedad cancelativa: $a \ast b = a \ast c \implies b = c$. Esto se demuestra:
    * $a \ast b = a \ast c \implies a' \ast (a \ast b) = a' \ast (a \ast c)$
    * $(a' \ast a) \ast b = (a' \ast a) \ast c$ // por asociatividad
    * $\implies e \ast b = e \ast c$
    * $\implies b = c$

## Tipos de estructuras

Cada tipo de estructura es igual al anterior + algo nuevo:
1. $(A, \ast)$ es un grupoide si $\ast$ es una operación binaria válida.
1. $(A, \ast)$ es un semigrupo si es un grupoide y $\ast$ es asociativa.
    * Si además es conmutativa, es un **semigrupo conmutativo**.
1. $(A, \ast)$ es un monoide si es un semigrupo y existe un neutro para $\ast$
    * Si además es conmutativa, es un **monoide conmutativo**.
1. $(a, \ast)$ es un grupo si es un monoide y cada elemento tiene un inverso.
    * Si además es conmutativa, es un **grupo conmutativo** o **abeliano**.

Algunos ejemplos:
* $(N,+)$ es un semigrupo conmutativo (si se considera $0 \notin N$ ):
    * No existe un neutro para la suma.
    * No existe un inverso $-a$ para los elementos de $A$.
* $(Z,.)$ es un monoide conmutativo:
    * Existe un neutro $1$
    * No existe un inverso para cada elemento en $Z$
* $(Q,.)$ es un grupo conmutativo:
    * Existe un neutro $0$
    * Cada elemento tiene un inverso $\frac 1 a$

### Anillos

Tipo especial de estructura formada a partir de dos operaciones binarias, con la forma $(A,+,.)$. Debe cumplir:
* $(A,+)$ es un grupo conmutativo.
* $(A,.)$ es asociativa.
* Las operaciones son distributivas:
    * Por izquierda: $a(b+c) = ab + ac$
    * Por derecha: $(a+b)c = (ac + bc)$
* Si el producto es conmutativo, $(A,+,.)$ es un **anillo conmutativo**.
* Si existe un neutro para el producto diferente al de la suma, $(A,+,.)$ tiene un **elemento unitario**.
* Si en un anillo conmutativo con elemento unitario, ocurre que $a.b = \implies a=0 \lor b = 0$, entonces es un **dominio de integridad**.

**Ejemplo:** $(Z,+,.)$, enteros con la suma y el producto, es un anillo conmutativo:
* $(Z,+)$ es un grupo conmutativo.
* $(Z,.)$ es asociativa.
* La suma es distributiva respecto al producto.
* $(Z,.)$ es conmutativa.
* Tiene un elemento unitario $1 \ne 0$
* Es un dominio de integridad.

# Propiedades de grupos

> yo creo que podrían tomar las demostraciones de las propiedades

Para trabajar con grupos se suele usar la notación multiplicativa, aunque no haga referencia a los símbolos de la multiplicación exactamente.

Dado un grupo $(G,.)$:
* El neutro es único.
* Todo elemento tiene un único inverso.
* $\forall a \in G : (a^{-1})^{-1} = a$
    * $a^{-1}. (a^{-1})^{-1} = e$
    * $\implies (a^{-1})^{-1} = a$
* $\forall a,b \in G: (ab)^{-1} = b^{-1}a^{-1}$ // EL ORDEN ES IMPORTANTE CUANDO NO ES UN GRUPO CONMUTATIVO
    * $(ab)^{-1}.(ab) = e$
    * $(ab).(b^{-1}a^{-1}) = e$
    * $(ab).(b^{-1}a^{-1}) = a(b.b^{-1})a^{-1} = a.e.a^{-1} = e$

Dados los grupos $(G_1, \ast_1), (G_2, \ast_2), ... , (G_n, \ast_n)$, entonces existe un nuevo grupo $G = G_1 \times G_2 \times ... \times G_n$ con la operación $\ast$ definida como:

$$(a_1, ..., a_m) \ast (b_1, ..., b_m) = (a_1 \ast_1 b_1, ..., a_m \ast_m b_m)$$

Una potencia $a^k$ (siendo $k$ un entero) definida sobre un elemento $a \in G$ implica realizar la operación $\ast$ $k$ veces sobre $a$. La operación **no siempre** es la multiplicación, así que se tiene que hacer la cuenta "a mano".

## Grupos cíclicos

Un grupo es cíclico si tiene un elemento $a \in G$ tal que para todo otro elemento $b \in G$ existe un número $k \in Z: b = a^k$

$a$ es un generador de $G$ y se escribe $G = <a>$

> esto de generadores se usa mas en aritmética modular, así que lo voy a explicar después

Todo grupo cíclico es abeliano. se puede desmostrar a partir del generador $a$:
* $x = a^k,\ y = a^j$
* $x \ast y = a^k \ast a^j$
* $= a^{k+j}$ // por propiedades de la potencia
* $= a^{j+k}$ // por conmutatividad en la suma de enteros
* $= a^j \ast a^k$
* $= y \ast x = x \ast y$

### Orden finito

A partir del generador $a \in G$, se dice que $a$ es de orden finito $m$ cuando $a^m = e$.

Si $G$ es un grupo cíclico de orden $m$, entonces se da que $G = \{ e, a, a^2, ..., a^{m-1} \}$

Un buen ejemplo de un orden finito es la hora del reloj (o los enteros módulo 12 con la suma):
* $Z_{12} = \{ 0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11\}$
* $1  \in Z_{12} : b = 1^k \quad \forall b \in Z_{12}$
* $Z_{12} = <1>$
* $1^{12} = 12 \implies 12 \mod 12 = 0 = e$
* $1^{m-1} = 1^{11} = 11$ // siendo 11 el último elemento de $Z_{12}$

## Subgrupos

A partir de un grupo $(G,\ast)$ y $H \subset G$, si $(H,\ast)$ es un grupo entonces se dice que es un subgrupo de $G$ con la misma operación.

El subgrupo hereda todas las propiedades del grupo original, por lo que se le considera un grupo sin demostración. Sin embargo, para que sea un subgrupo de $G$ debe cumplir:
* $e \in H$ (existencia del neutro en $H$)
* $a,b \in H \implies a \ast b \in H$ (operación cerrada en $H$)
* $a \in H \implies a^{-1} \in H$ (existencia del inverso en $H$)
    * $e \in H, a \ast b \in H \implies a \ast a^{-1} = e \in H$

> si $G$ es cíclico, $H$ también