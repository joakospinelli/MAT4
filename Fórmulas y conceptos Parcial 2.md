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

Cada tipo de estructura es igual al anterior más algo nuevo:
1. $(A, \ast)$ es un grupoide si $\ast$ es una operación binaria válida.
1. $(A, \ast)$ es un semigrupo si es un grupoide y $\ast$ es asociativa.
    * Si además es conmutativa, es un **semigrupo conmutativo**.
1. $(A, \ast)$ es un monoide si es un semigrupo y existe un neutro para $\ast$
    * Si además es conmutativa, es un **monoide conmutativo**.
1. $(a, \ast)$ es un grupo si es un monoide y cada elemento tiene un inverso.
    * Si además es conmutativa, es un **grupo conmutativo** o **abeliano**.

| Estructura | Propiedades |
| ---------- | ----------- |
| Grupoide | Operación binaria válida |
| Semigrupo | Grupoide + asociativa |
| Monoide | Semigrupo + neutro |
| Grupo | Monoide + inverso |

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

# Aritmética modular

Forma de representar números sin que superen un valor máximo (denominado **módulo**).

Un valor pertenece a la clase de congruencia módulo $m$ según su valor bajo ese módulo. Por ejemplo: $18$ pertenece a la clase de congruencia $6\mod 12$, ya que $18 = 12\times 1 + 6, \quad r=6$

## Propiedades

* $\overline x + \overline y = \overline {x + y}$
    * Es asociativa.
    * Es conmutativa.
    * Existe un elemento neutro 0.
    * Todo elemento tiene un inverso $a' = -a$
* $\overline x \times \overline y = \overline {x \times y}$
    * Es asociativa.
    * Es conmutativa.
    * Existe un elemento neutro 1.
    * El producto es distributivo en la suma.
* $(Z_m,+)$ es un grupo conmutativo para todo $m \in Z$
* $(Z_m,.)$ es un monoide conmutativo para todo $m \in Z$ (salvo $m = 1$ que es un grupo).
* Un número $x \in Z_m$ es generador de $(Z_m,+)$ sólo si $(x,m)=1$ (es decir, son coprimos).

## Tablas

Las tablas se obtienen al realizar una operación módulo $m$ sobre todos los elementos de $Z_m$. Tomando como ejemplo a $Z_4$:

| + | 0 | 1 | 2 | 3 |
| - | - | - | - | - |
| 0 | 0 | 1 | 2 | 3 |
| 1 | 0 | 2 | 3 | 0 |
| 2 | 2 | 3 | 0 | 1 |
| 3 | 3 | 0 | 1 | 2 |

El resultado de cada celda se calcula como $(i + j) \mod m$

## Invertibles

Un elemento $a$ en un anillo $Z_m$ es invertible si existe otro elemento $x \in Z_m$ tal que $a.x = 1$.

Otra definición es que $a$ es invertible si es coprimo con $m$ (es decir, $(a,m) = 1$ ). Para encontrar a los elementos invertibles $\in Z_m$, se tiene que buscar el MCD con $m$.

Como su nombre indica los invertibles tienen inverso con el producto, tal que para todo $a$ invertible existe un entero $k \in Z_m: a.k = 1$

### Divisores de 0

Un número $a$ es divisor de 0 si existe un entero $b \ne 0 \in Z_m : a.b = 0$

Un elemento invertible en $Z_m$ nunca va a ser divisor de 0.

# Morfismos

Dados dos grupos $(G,\ast), (G, \circ)$, la función $f: G_1 \to G_2$ es un morfismo si se respetan las operaciones:

$$f(a\ast b) = f(a) \circ f(b) \quad \forall a,b \in G_1$$

Otras cosas que se respetan:
* $f(e_1) = e_2$ // el neutro de un grupo es el neutro en el otro
* $f(a^{-1}) = (f(a))^{-1} \quad \forall a \in G_1$ // el morfismo del inverso es lo mismo que el morfismo del elemento, invertido.
## Tipos

Dada una función $f: G \to H$
* **Monomorfismo:** cuando no existen dos elementos del $G_1$ con la misma imagen. Es inyectiva.

    * $\forall g_1, g_2 \in G: f(g_1) = f(g_2) \iff g_1 = g_2$

* **Epimorfismo:** cuando todo elemento de $H$ es imagen de al menos un elemento de $G$. Es sobreyectiva.

    * $\forall h \in H: \exists g \in G : f(g) = h$

* **Epimorfismo:** tanto inyectiva como sobreyectiva, también llamada biyectiva.

## Núcleo e imagen

El núcleo está formado por todos los elementos del dominio cuya imagen es el elemento neutro del codominio.

$$Nu(f) = \{ a \in G_1 : f(a) = e_2 \}$$

La imagen está compuesta por todos los elementos del codominio que tienen al menos una preimagen en el dominio.

$$Im(f) = \{ a \in G_2 : \exists x \in G_1, f(x) = a \}$$

El núcleo es un subgrupo del dominio $G_1$, mientras que la imagen es un subgrupo del codominio $G_2$.

# Espacios vectoriales

Un espacio vectorial es una estructura algebraica $(V,+,.)$ definida sobre un cuerpo $K$ (generalmente los reales) que tiene muchas propiedades.

El producto es una operación externa definida entre $V$ y el cuerpo $K$. Por lo general es el producto por escalar.

## Axiomas

Según el apunte, para que una estructura sea un espacio vectorial tiene que cumplir 8 axiomas o propiedades, pero a eso se le suma que las operaciones tienen que ser cerradas así que son 10.

* $+$ debe ser cerrada en $V$. $\forall a,b \in V : a+b \in V$
* $.$ debe ser cerrada en $V$. $\forall a,b \in V, \forall k \in K: k.a \in V$
* $+$ debe ser conmutativa. $\forall a,b \in V : a+b = b+a$
* $+$ debe ser asociativa. $\forall a,b,c \in V: (a+b)+c = a+(b+c)$
* Debe existir un elemento neutro para $+$. $\exists e \in V : \forall a \in V: a + e = a$
* Cada elemento debe tener un inverso para $+$. $\forall a \in V, \exists a' \in V : a+a' = e$
* $.$ debe ser asociativa. $\forall \alpha, \beta \in K : (\alpha\beta)v = \alpha(\beta.v) \quad \forall v \in V$
* $.$ debe ser distributiva a la suma de escalares. $\forall \alpha, \beta\in K : (\alpha+\beta)v = \alpha.v + \beta.v \quad \forall v \in V$
* $.$ debe ser distributiva a la suma de vectores. $\forall \alpha \in K : (v_1 + v_2)\alpha = v_1.\alpha + v_2.\alpha \quad \forall v_1,v_2 \in V$
* Existe un elemento neutro para $.$ $\exists 1 \in K: 1.v = v \quad \forall v \in V$

Esto nos da algunas cositas importantes:
* Para todo escalar $\alpha$ se cumple $\alpha.0 = 0$ (valor *nulo*).
* Para todo $v \in V$ se cumple $0.v = 0$
* Si $\alpha.v = 0$, entonces $\alpha = 0 \lor v = 0$

## Subespacios vectoriales

Sea $(V,+,.)$ un espacio vectorial, $(S,+,.)$ es un subespacio si $S \subset V$ es un conjunto no vacío y es en sí mismo un espacio vectorial, bajo las mismas operaciones que $V$.

Como $S \subset V$, casi todos los axiomas se cumplen automáticamente. Sólo hay que demostrar:

* $0_V \in S$ // EN EL APUNTE PRIMERO DICE QUE NO TIENE QUE SER VACÍO PERO DESPUÉS DICE QUE TIENE QUE TENER SÍ O SÍ A $0_V$, ADEMÁS SI TIENE A $0_V$ YA SE CUMPLE QUE NO SEA VACÍO
* $\forall s_1, s_2 \in S: s_1 + s_2 \in S$ // cerrado respecto a la suma
* $\forall s \in S: k.s \in S, k \in K$ // cerrado respecto al producto por escalar

## Combinaciones lineales

Un conjunto de vectores $S$ dentro de un espacio vectorial $V$ pueden escribirse a partir de una combinación de lineal de vectores tales que:

$$v = c_1v_1 + c_2v_2 + ... + c_rv_r$$

## Independencia lineal

Un conjunto de vectores $v_1, v_2, ... , v_r$ son linealmente independientes si al escribirlos como una combinación lineal igualada a 0:

$$c_1v_1 + c_2v_2 + ... + c_rv_r = 0$$

Implica que todos los coeficientes $c_i$ son nulos. En caso contrario, son dependientes.

Si dentro de un conjunto de vectores son todos linealmente independientes, existe una combinación lineal única para expresarlo. Por contraposición, el conjunto no es linealmente independiente si cualquier vector se puede escribir de varias formas.

## Generadores

Un conjunto de generadores es aquel a partir del cual se puede escribir cualquier vector $v \in V$ mediante una combinación lineal.

Por ejemplo, $(1,0); (0,1)$ es el generador de $R^2$:
* $(23,99) = 23(1,0) + 99(0,1)$
* $= (23,0) + (0,99)$
* $= (23+0, 0+99)$
* $= (23,99)$

Un generador es minimal si todos sus elementos son independientes.

### Bases

Un conjunto de vectores $v_1, v_2, ..., v_r$ forma una base de $V$ si y sólo si:
* Son todos linealmente independientes.
* Generan todo $V$.

Esto implica que no puede haber bases con vectores redundantes, y son siempre minimales.
> esto le pifié en un ej de la práctica y puse que no puede ser un GENERADOR porque tenía vectores redundantes. en realidad sí puede ser un generador pero nunca una base

## Teoremas

* Si $B = \{ v_1, ..., v_n \}$ es una base vectorial de $V$, todo conjunto con más vectores que $V$ es linealmente **de**pendiente.
* Si $B = \{v_1,...,v_n \}, B' = \{ u_1, ..., u_m \}$ son dos bases de $V$, entonces $m=n$. Todas las bases de un espacio vectorial tienen el mismo número de elementos.
* Si una base de $V$ tiene $n$ vectores, entonces $V$ tiene dimensión $n$.
    * Por ejemplo: la base de $R^2$ es $(0,1);(1,0)$, entonces $R^2$ es de base 2.
    * Si se genera sólo con el vector nulo, se dice que tiene dimensión 0.
* Si $V$ es un espacio vectorial con dimensión $n > 0$:
    * Cualquier conjunto de $n$ vectores linealmente independiente lo generan.
    * Todo conjunto de $n$ vectores que lo generan son linealmente independiente, por lo tanto son una base.

# Transformaciones lineales

> *es como morfismos pero para espacios vectoriales.*

Una transformación lineal es una alpicación de un espacio $V$ a otro $W$, definida como $L: V \to W$. Debe cumplir las propiedades:

* $\forall v_1, v_2 : L(v_1 + v_2) = L(v_1) + L(v_2)$
* $\forall v \in V, \forall \alpha \in K : L(\alpha.v) = \alpha.L(v)$

## Núcleo e imagen

El núcleo está formado por todos los elementos $\in V$ que son transformados al vector nulo de $W$.

$$Nu(L) = \{ v \in V : L(v) = 0_W \}$$

La imagen está formada por todos los vectores $w \in W$ que tienen al menos una preimagen en $V$.

$$Im(L) = \{ w \in W: \exists v \in V, L(v) = w \}$$

* Una transformación inyectiva conserva la independencia lineal.
* Una transformación sobreyectiva cubre todo el codominio.

## Cómo hallar una transformación lineal + matrices asociadas

Se puede buscar la forma de $L$ si sabés el valor de una aplicación específica aún sin saber la forma exacta.

Si te dan los valores en la base canónica es re fácil. Tenés que escribir una combinación lineal con la base y usar las propiedades de las transformaciones. Un ejemplo con el ejercicio 21.a:

$L(1,0) = (1,-2);\ L(0,1) = (1,-1)$

* $L(x,y) = L(x(1,0) + y(0,1))$
* $= L(x(1,0)) + L(y(0,1))$ // propiedad 1 de transformaciones
* $= x.L(1,0) + y.L(0,1)$ // propiedad 2
* $= x(1,-2) + y(1,-1)$ reemplazo por las aplicaciones del enunciado. acá llegué a la forma "estándar" de las combinaciones lineales
* $= (x, -2x) + (y,-y)$
* $= (x+y, -2x-y)$ // este ese el resultado de aplicar $L$ sobre cualquier $(x,y)$

$L: R^2 \to R^2 : L(x,y) = (x+y,-2x-y)$

Pero si los valores no son de la base canónica es más difícil porque no sabés exactamente con qué vectores se hace la combinación lineal. Tenés que hacer la combinación lineal con la matriz asociada a la transformación. Un ejemplo con el ejercicio 21.c

* $L(x,y) = (a_{11}.x + a_{12}.y, a_{21}.x + a_{22}.y)$ // $a$ sería la matriz asociada a la transformación lineal. Yo odio las matrices pero se puede escribir como:
    $$L(x,y) = \begin{pmatrix} a_{11} & a_{12} \\ a_{21} & a_{22}\end{pmatrix} \begin{bmatrix} x \\ y \end{bmatrix}$$
* $L(1,1) = (4,2)$
    * $L(a_{11}.1 + a_{12}.1, a_{21}.1 + a_{22}.1) = L(a_{11} + a_{12}, a_{21} + a_{22}) = (4,2)$
* $L(0,3) = (1,0)$
    * $L(a_{11}.0 + a_{12}.3, a_{21}.0 + a_{22}.3)$
    * $= L(3a_{12}, 3a_{22}) = (1,0)$

A partir de esto podés despejar los valores de la matriz

* $3a_{22} = 0 \implies a_{22} = 0$
* $3a_{12} = 1 \implies a_{12} = \frac 1 3$
* $a_{11} + a_{12} = a_{11} + \frac 1 3 = 4 \implies a_{11} = \frac {11} 3$
* $a_{21} + a_{22} = a_{21} + 0 = 2 \implies a_{21} = 2$

Entonces reemplazamos en la maravillosa matriz asociada:

$$A = \begin{pmatrix} \frac {11} 3 & \frac 1 3 \\ 2 & 0 \end{pmatrix}$$

Después para calcular la transformación lineal hacemos:

$$L(x,y) = \begin{pmatrix} \frac {11} 3 & \frac 1 3 \\ 2 & 0\end{pmatrix} \begin{bmatrix} x \\ y\end{bmatrix}$$

$$= \begin{pmatrix} \frac {11} 3 x & \frac 1 3 y \\ 2x & 0\end{pmatrix}$$

Porque cuando multiplicás una matriz por un vector tenés que hacer $fila[i] \times vector[i]$ para cada fila de la matriz.

Y de acá sacamos que $L(x,y) = (\frac {11} 3x + \frac 1 3y, 2x)$