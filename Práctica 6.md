# 1. Demostrar que los siguientes conjuntos son espacios vectoriales con las operaciones de suma y producto por escalar usuales correspondientes a cada espacio:

## a. $R^3$

La suma es cerrada en $R^3$:
* $v_1 = (a,b,c) \in R^3, v_2 = (d,e,f) \in R^3$

* $v_1 + v_2 = (a,b,c) + (d,e,f) = (a+d, b+e, c+f)$

* $a+d, b+e, c+f \in R$

* $(a+d, b+e, c+f) \in R^3$

El producto por escalar es cerrado en $R^3$:
* $v_1 = a,b,c \in R^3 \quad k \in K$

* $v_1.k = k(a,b,c) = (k.a, k.b, k.c)$

* $k.a, k.b, k.c \in R$

* $(k.a, k.b, k.c) \in R^3$

La suma es conmutativa en $R^3$:
* $v_1 = (a,b,c) \in R^3, v_2 = (d,e,f) \in R^3$

* $v_1 + v_2 = (a,b,c) + (d,e,f) = (a+d,\ b+e,\ c+f)$

* $v_2 + v_1 = (d,e,f) + (a,b,c) = (d+a,\ e+b,\ f+c)$

* $\forall x,y \in R : x+y = y+x \implies a+d = d+a, \quad b+e = e+b, \quad c+f = f+c$

* $(a+d,\ b+e,\ c+f) = (d+a,\ e+b,\ f+c)$

* $v_1 + v_2 = v_2 + v_1$

La suma es asociativa en $R^3$:
* $v_1 = (a,b,c) \in R^3, v_2 = (d,e,f) \in R^3, v_3 = (x,y,z) \in R^3$

* $v_1 + v_2 = (a + d,\ b+e,\ c+f)$

* $v_2 + v_3 = (d+x,\ e+y, f+z)$

* $v_1 + (v_2 + v_3) = (a,b,c) + (d+x,\ e+y,\ f+z) = (a+d+x,\ b+e+y,\ c+f+z)$

* $(v_1 + v_2) + v_3 = (a+d, \ b+e,\ c+f) + (x,y,z) = (a+d+x,\ b+e+y,\ c+f+z)$

* $v_1 + (v_2 + v_3) = (v_1 + v_2) + v_3$

Existe un elemento neutro $(0,0,0)$ para la suma tal que:
* $v_1 = (a,b,c) \in R^3 \quad e = (0,0,0) \in R^3$

* $v_1 + e = (a,b,c) + (0,0,0) = (a+0,\ b+0,\ c+0)$

* $\forall x \in R : x+0 = x \implies a+0 = a,\ b+0 = b,\ c+0 = c$

* $(a+0,\ b+0,\ c+0) = (a,b,c)$

* $v_1 + e = v_1$

Cada elemento $\in R^3$ tiene un inverso tal que:
* $v_1 = (a,b,c) \in R^3 \quad v_1^{-1} = (-a,-b,-c)$

* $v_1 + v_1^{-1} = (a + (-a),\ b + (-b),\ c+(-c))$

* $\forall x, x^{-1} \in R : x+(-x) = x-x = 0 \implies a+(-a) = 0,\ b+(-b) = 0, c+(-c) = 0$

* $(a + (-a),\ b + (-b),\ c+(-c)) = (0,0,0)$

* $v_1 + v_1^{-1} = e$

El producto por escalares es asociativo:
* $v_1 = (a,b,c) \in R^3 \quad \alpha, \beta \in K$

* $\beta.v_1= (\beta.a,\ \beta.b,\ \beta.c)$

* $\alpha(\beta.v_1) = \alpha(\beta.a,\ \beta.b,\ \beta.c) = (\alpha.\beta.a,\ \alpha.\beta.b,\ \alpha.\beta.c)$

* $\alpha.\beta(v_1) = \alpha\beta(a,b,c) =  (\alpha.\beta.a,\ \alpha.\beta.b,\ \alpha.\beta.c)$

* $\alpha(\beta.v_1) = \alpha.\beta(v_1)$

El producto por escalares es distributivo respecto a la suma de escalares:
* $v_1 = (a,b,c) \in R^3 \quad \alpha, \beta \in K$

* $(\alpha + \beta)v_1 = ((\alpha + \beta)a,\ (\alpha + \beta)b, (\alpha + \beta)c)$

* $\alpha.v_1 + \beta.v_1 = (\alpha.a,\ \alpha.b, \alpha.c) + (\beta.a,\ \beta.b, \beta.c) = (\alpha.a + \beta.a,\ \alpha.b + \beta.b, \alpha.c + \beta.c) = (a(\alpha + \beta),\ b(\alpha + \beta),\ c(\alpha + \beta))$

* $((\alpha + \beta)a,\ (\alpha + \beta)b, (\alpha + \beta)c) = (a(\alpha + \beta),\ b(\alpha + \beta),\ c(\alpha + \beta))$ // por conmutatividad del producto $\in R$

* $(\alpha + \beta)v_1 = \alpha.v_1 + \beta.v_1$

El producto por escalares es distributivo respecto a la suma de vectores:
* $v_1 = (a,b,c) \in R^3, v_2 = (d,e,f) \in R^3, \alpha \in K$

* $\alpha(v_1 + v_2) = \alpha(a+d,\ b+e,\ c+f) = (\alpha(a+d),\ \alpha(b+e), \alpha(c+f))$

* $\alpha.v_1 + \alpha.v_2 = (\alpha.a,\ \alpha.b,\ \alpha.c) + (\alpha.d,\ \alpha.e,\ \alpha.f) = (\alpha.a + \alpha.d,\ \alpha.b + \alpha.e,\ \alpha.c + \alpha.f) = (\alpha(a+d),\ \alpha(b+e),\ \alpha(d+f))$

* $\alpha(v_1+v_2) = \alpha.v_1 + \alpha.v_2$

Existe un neutro $1$ para el producto por escalares tal que:
* $v_1 = (a,b,c) \in R^3$
* $v_1.1 = (1.a, 1.b, 1.c)$
* $\forall x \in R: x.1 = x \implies 1.a = a,\ 1.b = b,\ 1.c = c$
* $(1.a, 1.b, 1.c) = (a,b,c)$
* $v_1.1 = v_1$

Se cumplen las 10 propiedades y axiomas, por lo que $R^3$ es un espacio vectorial válido respecto a la suma y producto por escalar.

## b. Matrices reales de $2 \times 2$

> no se va a ver nada porque github no entiende las matrices de LaTeX

La suma es cerrada en $R^{2 \times 2}$:
* $m_1 = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$

* $m_2 = \begin{pmatrix} w & x \\ y & z \end{pmatrix}$

* $m_1 + m_2 = \begin{pmatrix} a+w & b+x \\ c+y & d+z \end{pmatrix}$

* $\forall x,y \in R : x+y \in R \implies a+w, b+x, c+y, d+z \in R$

* $m_1 + m_2 \in R^{2 \times 2}$

El producto por escalar es cerrado en $R^{2 \times 2}$:
* $m_1 = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$

* $\alpha \in K$

* $\alpha.m_1 = \alpha \begin{pmatrix} a & b \\ c & d \end{pmatrix} = \begin{pmatrix} \alpha.a & \alpha.b \\ \alpha.c & \alpha.d \end{pmatrix}$

* $\forall x,y \in R : x.y \in R \implies \alpha.a, \alpha.b, \alpha.c, \alpha.d \in R$

* $\alpha.m_1 \in R^{2\times 2}$

La suma es conmutativa en $R^{2 \times 2}$:
* $m_1 = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$

* $m_2 = \begin{pmatrix} w & x \\ y & z \end{pmatrix}$

* $m_1 + m_2 = \begin{pmatrix} a+w & b+x \\ c+y & d+z \end{pmatrix}$

* $m_2 + m_1 = \begin{pmatrix} w+a & x+b \\ y+c & z+d \end{pmatrix}$

* $\forall x,y \in R : x+y = y+x \implies a+w = w+a,\ b+x = x+b,\ c+y = y+c,\ d+z = z+d$

* $m_1 + m_2 = m_2 + m_1$

La suma es asociativa en $R^{2\times 2}$:
* $m_1 = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$

* $m_2 = \begin{pmatrix} i & j \\ k & l \end{pmatrix}$

* $m_3 = \begin{pmatrix} w & x \\ y & z \end{pmatrix}$

* $m_1 + m_2 = \begin{pmatrix} a+i & b+j \\ c+k & d+l \end{pmatrix}$

* $m_2 + m_3 = \begin{pmatrix} i+w & j+x \\ k+y & l+z \end{pmatrix}$

* $m_1 + (m_2 + m_3) = \begin{pmatrix} a & b \\ c & d \end{pmatrix} + (\begin{pmatrix} i+w & j+x \\ k+y & l+z \end{pmatrix}) = \begin{pmatrix} a+i+w & b+j+x \\ c+k+y & d+l+z \end{pmatrix}$

* $(m_1 + m_2) + m_3 = (\begin{pmatrix} a+i & b+j \\ c+k & d+l \end{pmatrix}) + \begin{pmatrix} w & x \\ y & z \end{pmatrix} = \begin{pmatrix} a + i + w & b+j+w \\ c+k+y & d+l+z\end{pmatrix}$

* $m_1 + (m_2 + m_3) = (m_1 + m_2) + m_3$

Existe un elemento neutro $e = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix} \in R^{2 \times 2}$ tal que:
* $m_1 = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$

* $m_1 + e = \begin{pmatrix} a + 0 & b + 0 \\ c + 0 & d+0 \end{pmatrix}$

* $\forall x \in R : x+0 = x \implies a+0 = a,\ b + 0 = b,\ c + 0 = c,\ d + 0 = d$

* $m_1 + e = m_1$

Cada elemento $\in R^{2 \times 2}$ tiene un inverso tal que:
* $m_1 = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$

* $m_1^{-1} = \begin{pmatrix} -a & -b \\ -c & -d \end{pmatrix}$

* $m_1 + m_1^{-1} = \begin{pmatrix} a+(-a) & b+(-b) \\ c+(-c) & d+(-d) \end{pmatrix}$

* $\forall x \in R : x + (-x) = x-x = 0 \implies a+(-a) = 0,\ b+(-b) = 0,\ c+(-c) = 0,\ d+(-d) = 0$

* $\begin{pmatrix} a+(-a) & b+(-b) \\ c+(-c) & d+(-d) \end{pmatrix} = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}$

* $m_1 + m_1^{-1} = e$

El producto por escalar es asociativo en $R^{2 \times 2}$:

* $m_1 = \begin{pmatrix} a & b \\c & d \end{pmatrix}$

* $\alpha, \beta \in K$

* $\beta.m_1 = \beta \begin{pmatrix} a & b \\ c & d \end{pmatrix} = \begin{pmatrix} \beta.a & \beta.b \\ \beta.c & \beta.d \end{pmatrix}$

* $\alpha(\beta.m_1) = \alpha.\begin{pmatrix} \beta.a & \beta.b \\ \beta.c & \beta.d \end{pmatrix} = \begin{pmatrix} \alpha.\beta.a & \alpha.\beta.b \\ \alpha.\beta.c & \alpha.\beta.d \end{pmatrix}$

* $(\alpha.\beta)m_1 = \alpha.\beta \begin{pmatrix} a & b \\c & d \end{pmatrix} = \begin{pmatrix} \alpha.\beta.a & \alpha.\beta.b \\ \alpha.\beta.c & \alpha.\beta.d \end{pmatrix}$

* $\alpha(\beta.m_1) = (\alpha.\beta)m_1$

El producto por escalar es distributivo respecto a la suma de escalares:

* $m_1 = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$

* $\alpha, \beta \in K$

* $(\alpha + \beta)m_1 = (\alpha + \beta)\begin{pmatrix} a & b \\ c & d \end{pmatrix} = \begin{pmatrix} (\alpha+\beta)a & (\alpha+\beta)b \\ (\alpha+\beta)c & (\alpha+\beta)d \end{pmatrix}$

* $\alpha.m_1 + \beta.m_1 = \begin{pmatrix} \alpha.a & \alpha.b \\ \alpha.c & \alpha.d \end{pmatrix} + \begin{pmatrix} \beta.a & \beta.b \\ \beta.c & \beta.d \end{pmatrix} = \begin{pmatrix} \alpha.a + \beta.a & \alpha.b + \beta.b \\ \alpha.c + \beta.c & \alpha.d + \beta.d \end{pmatrix} = \begin{pmatrix} (\alpha + \beta)a & (\alpha + \beta)b \\ (\alpha + \beta)c & (\alpha + \beta)d \end{pmatrix}$

* $(\alpha + \beta)m_1 = \alpha.m_1 + \beta.m_1$

El producto por escalar es distributivo a la suma de vectores:
* $m_1 = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$

* $m_2 = \begin{pmatrix} w & x \\ y & z \end{pmatrix}$

* $\alpha \in K$

* $m_1 + m_2 = \begin{pmatrix} a & b \\c & d\end{pmatrix} + \begin{pmatrix} w & x \\ y & z \end{pmatrix} = \begin{pmatrix} a+w & b+x \\ c+y & d+z\end{pmatrix}$

* $\alpha(m_1 + m_2) = \alpha\begin{pmatrix} a+w & b+x \\ c+y & d+z\end{pmatrix} = \begin{pmatrix} \alpha(a+w) & \alpha(b+x) \\ \alpha(c+y) & \alpha(d+z) \end{pmatrix}$

* $\alpha.m_1 + \alpha.m_2 = \alpha\begin{pmatrix} a & b \\ c & d \end{pmatrix} + \alpha\begin{pmatrix} w & x \\ y & z \end{pmatrix} = \begin{pmatrix} \alpha.a & \alpha.b \\ \alpha.c & \alpha.d \end{pmatrix} + \begin{pmatrix} \alpha.w & \alpha.x \\ \alpha.y & \alpha.z \end{pmatrix} = \begin{pmatrix} \alpha.a + \alpha.w & \alpha.b + \alpha.x \\ \alpha.c + \alpha.y & \alpha.d + \alpha.z \end{pmatrix} = \begin{pmatrix} \alpha(a+w) & \alpha(b+x) \\ \alpha(c+y) & \alpha(d+z) \end{pmatrix}$

* $\alpha(m_1 + m_2) = \alpha.m_1 + \alpha.m_2$

Existe un neutro $1 \in K$ para el producto por escalar tal que:

* $m_1 = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$

* $m_1.1 = 1\begin{pmatrix} 1.a & 1.b \\ 1.c & 1.d \end{pmatrix}$

* $\forall x \in R: x.1 = x \implies 1.a = a,\ 1.b = b,\ 1.c = c,\ 1.d = d$

* $m_1.1 = 1\begin{pmatrix} 1.a & 1.b \\ 1.c & 1.d \end{pmatrix} = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$

* $m_1.1 = m_1$

Se cumplen las 10 propiedades y axiomas, por lo que $R^{2\times 2}$ es un espacio vectorial válido respecto a la suma y producto por escalar.

## c. Los polinomios de grado menor o igual a 3 ($P(3)$). ¿El conjunto de los polinomios de grado 3 también es un espacio vectorial?

> e?

# 2. Sea $V$ un espacio vectorial, demostrar que si $\alpha.v = 0_V$ entonces $\alpha = 0$ ó $v = 0_V$ (o ambos son nulos).

$0$ es el valor nulo del escalar, mientras que $0_V$ es el valor nulo para $V$

Asumiendo $v \ne 0_V$:
* $a.v = 0_V \iff a = 0$

Asumiendo $a \ne 0$:
* $a.v = 0_V \iff v = 0_V$

Por definición, el valor nulo del producto se obtiene como resultado de operar cualquier elemento por él. El valor nulo es único.

Por lo tanto, el producto por escalar da como resultado al vector nulo $(0_V)$ sólo si el vector o el escalar son nulos (o ambos a la vez). En cualquier otro caso $a \ne 0 \land v \ne 0_V$ se da que $a.v \ne 0_V$.

Por lo tanto, $\alpha.v = 0_V \implies \alpha = 0\ \lor v = 0_V$

# 3. Decidir si los siguientes conjuntos son subespacios vectoriales:

## a. $S = \{ (x,0) : x \in R \}$

$R^2$ es un espacio vectorial y $S \subset R^2$. Se validarán las condiciones de subespacios en $S$:
* $0_{R^2} = (0,0) \in S$
    * $x = 0 : (0,0) \in S$
* $\forall s_1, s_2 \in S: (s_1 + s_2,0) \in S$
    * $x,y \in R : x+y \in R$
    * $x+y \in R \implies (x+y,0) \in S$
* $\forall s \in S: (k.s, 0) \in S$ para cualquier escalar $k \in K$
    * $x \in R : x.k \in R$
    * $k(x,0) = (x.k, 0.k)$
    * $(x.k, 0.k) = (x,0) \in S$
* $(0,0) \in S : x+0 = x \quad \forall x \in S$

Por lo tanto, $S$ es un subespacio vectorial de $R^2$.

## b. $S = \{ (1,y) : y \in R \}$

$R^2$ es un espacio vectorial y $S \subset R^2$. Se validarán las condiciones de subespacios en $S$:
* $0_{R^2} = (0,0) \notin S$

$S$ no cumple una de las condiciones, lo cual es suficiente para deducir que no es un subespacio vectorial de $R^2$.

## c. $S = \{ (x,y) \in R^2: x+y = 0 \}$

$R^2$ es un espacio vectorial y $S \subset R^2$. Se validarán las condiciones de subespacios en $S$:
* $0_{R^2} = (0,0) \in S$
    * $(0,0) : 0 + 0 = 0$
* $\forall s_1, s_2 \in S: s_1 + s_2 \in S$
    * $s_1 = (a,b) : a+b = 0$
    * $s_2 = (c,d) : c+d = 0$
    * $(a,b) + (c,d) = (a+c) + (b+d) = (a+b) + (c+d)$ // por conmutatividad de la suma de reales
    * $(a+b) + (c+d) = 0$
* $\forall s \in S: k.s \in S$ con cualquier escalar $k \in K$
    * $s = (a,b) : a+b = 0$
    * $k.s = k(a,b) = (k.a, k.b)$
    * $a + b = 0 \implies k.a + k.b = k(a+b) = k.0 = 0$

Por lo tanto, $S$ es un subespacio vectorial de $R^2$.

## d. $S = \{ (x,y) \in R^2: x+y = 1 \}$

$R^2$ es un espacio vectorial y $S \subset R^2$. Se validarán las condiciones de subespacios en $S$:
* $0_{R^2} = (0,0) \notin S$
    * $0 + 0 \ne 1$

$S$ no cumple una de las condiciones, lo cual es suficiente para deducir que no es un subespacio vectorial de $R^2$.

## e. $S= \{(x,y,z) \in R^3: z = x-y \}$

$R^3$ es un espacio vectorial y $S \subset R^2$. Se validarán las condiciones de subespacios en $S$:
* $0_{R^2} = (0,0,0) \in S$
    * $(0,0,0) : 0 = 0 - 0 = 0$
* $\forall s_1, s_2 : s_1 + s_2 \in S$
    * $s_1 = (a,b,c) : c = a-b$
    * $s_2 = (x,y,z) : z = x-y$
    * $s_1 + s_2 = (a,b,c) + (x,y,z) = (a+x,\ b+y,\ z+c)$
    * $(a+x,\ b+y,\ z+c) : (z+c) = (a+x) - (b+y)$
    * $(x-y) + (a-b) = a+x-b-y = (x-y) + (a-b)$ // por conmutatividad de la suma
* $\forall s \in S : k.s \in S$
    * $s = (a,b,c) : c = a -b$
    * $k.s = k(a,b,c) = (k.a,\ k.b,\ k.c)$
    * $k.c = k.a - k.b$
    * $k.c = k(a-b)$
    * $\dfrac {k.c} k = \dfrac {k(a-b)} k = c = a - b$

Por lo tanto, $S$ es un subespacio vectorial de $R^2$.

## f. $S= \{ (x,y,z,w) \in R^4: x+y+w = 1 \}$

$R^4$ es un espacio vectorial y $S \subset R^4$. Se validarán las condiciones de subespacios en $S$:
* $0_{R^4} = (0,0,0,0) \notin S$
    * $(0,0,0,0) : x+y+w = 0+0+0 \ne 1$

$S$ no cumple una de las condiciones, lo cual es suficiente para deducir que no es un subespacio vectorial de $R^2$.

## g. $S= \{ (x,y,z,w) \in R^4: x+y-w = 0, z+3y = 0 \}$

$R^4$ es un espacio vectorial y $S \subset R^4$. Se validarán las condiciones de subespacios en $S$:
* $0_{R^4} = (0,0,0,0) \in S$
    * $x+y-w = 0+0-0 = 0$
    * $z + 3y = 0 + 3.0 = 0$
* $\forall s_1, s_2 \in S : s_1 + s_2 \in S$
    * $s_1 = (a,b,c,d) : a+b-d = 0,\ c+3.b = 0$
    * $s_2 = (x,y,z,w) : x+y-w = 0,\ z+3y = 0$
    * $s_1 + s_2 = (a+x,\ b+y,\ c+z,\ d+w)$
    * $(a+x) + (b+y) - (d+w) = a+x+b+y-d-w = (a+b-d) + (x+y-w) = 0+0 = 0$ // por conmutatividad de la suma
    * $(c+z) + 3(b+y) = c+z + 3b + 3y = (c+3b) + (z+3y) = 0+0 = 0$

Por lo tanto, $S$ es un subespacio vectorial de $R^4$.

## h. $S= \{ \begin{pmatrix} a & b \\ a & c \end{pmatrix} : a,b,c\in R \}$

$R^{2 \times 2}$ es un espacio vectorial y $S \subset R^{2 \times 2}$. Se validarán las condiciones de subespacios en $S$:

* $0_{R^{2\times 2}} = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix} \in S$
    * $a = b = c = 0 \in R$

* $\forall s_1, s_2 \in S : s_1 + s_2 \in S$
    * $s_1 = \begin{pmatrix} a & b \\ a & c \end{pmatrix} : a,b,c \in R$
    * $s_2 = \begin{pmatrix} x & y \\ x & z \end{pmatrix} : x,y,z \in R$
    * $s_1 + s_2 = \begin{pmatrix} a+x & b+y \\ a+x & c+z \end{pmatrix}$
    * $\forall x,y \in R: x+y \in R \implies a+x,\ b+y, c+z \in R$
    * $s_1 + s_2 \in S$

* $\forall s \in S : k.s \in S$ siendo $k \in K$ un escalar cualquiera
    * $s = \begin{pmatrix} a & b \\ a & c \end{pmatrix} : a,b,c \in R$
    * $k.s = k\begin{pmatrix} k.a & k.b \\ k.a & k.c \end{pmatrix}$
    * $\forall x,y \in R : x.y \in R \implies k.a, k.b, k.c \in R$
    * $k.s \in S$

Por lo tanto, $S$ es un subespacio vectorial de $R^4$.

# 4. Decidir si los siguientes subconjuntos son generadores de $R^3$:

## a. $S = \{ (1,0,0); (0,1,0); (0,0,1); (1,2,3) \}$

Se quiere demostrar que se puede generar cualquier vector $(x,y,z) \in R^3$ a partir de $S$:

Primero se quiere demostrar que los elementos de $S$ sean linealmente independientes:
* $(0,0,0) = c_1(1,0,1) + c_2(0,1,0) + c_3(0,0,1) + c_4(1,2,3)$
* $= (c_1, 0, c_1) + (0, c_2, 0) + (0,0,c_3) + (c_4, 2.c_4, 3.c_4)$
* $= (c_1 + c_4,\ c_2 + 2.c_4,\ c_3 + 3.c_4)$
* Para igualar a $(0,0,0)$ debe darse:
    * $c_1 + c_4 = 0$
    * $c_2 + 2.c_4 = 0$
    * $c_3 + 3.c_4 = 0$
* Sin embargo, eso puede darse aún cuando un coeficiente no es nulo (por ejemplo: $a=1,\ b=2, c=3,\ d=-1$)
* Por lo tanto, los vectores no son linealmente independientes.

Debido a esto, $S$ no es un generador válido para $R^3$.
## b. $S = \{ (1,0,1); (1,1,1); (0,0,1) \}$

Se quiere demostrar que se puede generar cualquier vector $(x,y,z) \in R^3$ a partir de $S$.

Primero se quiere demostrar que los elementos de $S$ sean linealmente independientes:
* $(0,0,0) = c_1(1,0,1) + c_2(1,1,1) + c_3(0,0,1)$
* $= (c_1,0,c_1) + (c_2, c_2, c_2) + (0,0, c_3)$
* $= (c_1 + c_2,\ c_2, c_1 + c_2 + c_3)$
* Para igualar a $(0,0,0)$ debe darse:
    * $c_2 = 0$
    * $c_1 + c_2 = 0 \to c_1 = 0$
    * $c_1 + c_2 + c_3 \to c_3 = 0$
* Todos los coeficientes son nulos, por lo que $S$ es linealmente independiente.

Como $S$ es un espacio vectorial de dimensión 3 y sus vectores son linealmente independientes, se dice que $gen(S) = < R^3 >$

## c. $S = \{ (1,0,1); (0,1,0) \}$

Se quiere demostrar que se puede generar cualquier vector $(x,y,z) \in R^3$ a partir de $S$.

Primero se quiere demostrar que los elementos de $S$ sean linealmente independientes:
* $(0,0,0) = c_1(1,0,1) + c_2(0,1,0)$
* $= (c_1, 0, c_1) + (0, c_2, 0)$
* $= (c_1, c_2, c_1)$
* Para igualar a $(0,0,0)$ debe darse:
    * $c_1 = 0$
    * $c_2 = 0$
* Todos los coeficientes son nulos, por lo que $S$ es linealmente independiente.

Sin embargo, se obtuvo la forma $(c_1, c_2, c_1)$, tal que $(x,y,z) = (x,y,x)$. Esto implica que no podemos generar todos los elementos $\in R^3$ a partir de $S$.

# 5. Analizar si el siguiente conjunto puede generar el subespacio de matrices simétricas de $2 \times 2$: $S = \{ \begin{pmatrix} 1 & 0 \\ 0 & 0\end{pmatrix}, \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}, \begin{pmatrix} 0 & 0 \\ 0 & 1\end{pmatrix} \}$

Se quiere demostrar que se puede generar cualquier matriz simétrica de $2 \times 2$ a partir de $S$.

Primero se quiere demostrar que los elementos de $S$ son linealmente independientes:
* $\begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix} = c_1\begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix} + c_2\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} + c_3\begin{pmatrix} 0 & 0 \\ 0 & 1\end{pmatrix}$

* $= \begin{pmatrix} c_1 & 0 \\ 0 & 0 \end{pmatrix} + \begin{pmatrix} 0 & c_2 \\ c_2 & 0\end{pmatrix} + \begin{pmatrix} 0 & 0 \\ 0 & c_3\end{pmatrix}$
* $= \begin{pmatrix} c_1 & c_2 \\ c_3 & c_4 \end{pmatrix}$

* Para igualar a $\begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}$ debe darse:
    * $c_1 = 0$
    * $c_2 = 0$
    * $c_3 = 0$
    * $c_4 = 0$
* Todos los coeficientes son nulos, por lo que $S$ es linealmente independiente.

Una matriz simétrica $2 \times 2$ se define como cualquier matriz $\begin{pmatrix} a & b \\ c & d\end{pmatrix}$ tal que $a = d, b = c$; escrito de otra manera: $\begin{pmatrix} a & b \\ c & d \end{pmatrix} = \begin{pmatrix} a & b \\ b & a \end{pmatrix}$

Por lo tanto, cualquier matriz simétrica puede escribirse con los coeficientes:
* $\begin{pmatrix} a & b \\ b & a\end{pmatrix} = a\begin{pmatrix} 1 & 0 \\ 0 & 0\end{pmatrix} + b\begin{pmatrix} 0 & 1 \\ 1 & 0\end{pmatrix} + c\begin{pmatrix} 0 & 0 \\ 0 & 1\end{pmatrix}$

* $= \begin{pmatrix} a & 0 \\ 0 & 0\end{pmatrix} + \begin{pmatrix} 0 & b \\ b & 0\end{pmatrix} + \begin{pmatrix} 0 & 0 \\ 0 & d \end{pmatrix}$

* $= \begin{pmatrix} a & b \\ b & c\end{pmatrix}$

* Con $a = c$, tal que: $\begin{pmatrix} a & b \\ b & a \end{pmatrix}$

Por lo tanto, $gen(S) = <\{ \begin{pmatrix} a & b \\ c & d \end{pmatrix} \in M_{2\times2} : a = d, b = c \}>$

# 6. Dar el subespacio generado por los vectores $S=\{ (1,0,1); (1,1,0) \}$

Los vectores $v$ generados a partir de $S$ pueden escribirse como:
* $v = \alpha(1,0,1) + \beta(1,1,0)$
* $= (\alpha, 0, \alpha) + (\beta, \beta, 0)$
* $= (\alpha + \beta,\ \beta,\ \alpha + \beta)$

Por lo tanto, $S$ genera a los vectores de $R^3$ pertenecientes al conjunto $\{ (x,y,z) \in R^3 : x = z; x,y,z \in R \}$

# 7. Dar el subespacio generado por los vectores $S=\{ (1,1,1); (1,-1,0) \}$

Los vectores $v$ generador a partir de $S$ pueden escribirse como:
* $v = \alpha(1,1,1) + \beta(1,-1,0)$
* $= (\alpha, \alpha, \alpha) + (\beta, -\beta, 0)$
* $= (\alpha + \beta, \alpha - \beta,\ \alpha)$

Despejando a partir de $v = (x,y,z)$:
* $x = z + \beta$

* $y = z - \beta$

* $x + y = (z+ \beta) + (z - \beta) = z + z + \beta - \beta = 2z$

Por lo tanto, $S$ describe al conjunto $\{ (x,y,z) \in R^3 : x + y = 2z \}$

# 8. Decidir si los vectores de los siguientes conjuntos son linealmente independientes:

## a. $S = \{ (1,0,0); (0,1,0); (0,0,1); (1,2,3)\}$

> *Este ya lo resolví en el 4.a, pero en realidad en ese querían que lo resolvamos sin independencia jej*

## b. $S = \{ (1,0,0); (0,1,0); (0,0,1) \}$

* $(0,0,0) = c_1(1,0,0) + c_2(0,1,0) + c_3(0,0,1)$
* $= (c_1,0,0) + (0,c_2,0) + (0,0,c_3)$
* $= (c_1, c_2, c_3)$
* Para igualar a $(0,0,0)$ debe cumplirse:
    * $c_1 = 0$
    * $c_2 = 0$
    * $c_3 = 0$
* Todos los coeficientes son nulos, por lo que $S$ es linealmente independiente.

## c. $S = \{ (1,0); (0,1); (2,3) \}$

* $(0,0) = c_1(1,0) + c_2(0,1) + c_3(2,3)$
* $= (c_1,0) + (0,c_2) + (c_3.2, c_3.3)$
* $= (c_1 + c_3.2, c_2 + c_3.3)$
* Para igualar a $(0,0)$ debe cumplirse:
    * $c_1 = -(c_3.2)$
    * $c_2 = -(c_3.3)$
* $c_3$ puede tomar cualquier valor, por lo que no todos los coeficientes son necesariamente nulos para cumplir $(0,0)$.
* Por lo tanto, $S$ no es linealmente independiente.

## d. $S = \{ (1, -3); (1,-1) \}$

* $(0,0) = c_1(1, -3) + c_2(1, -1)$
* $= (c_1, -3.c_1) + (c_2, -c_2)$
* $= (c_1 + c_2, -3.c_1 - c_2)$
* Para igualar a $(0,0)$ debe cumplirse:
    * $c_1 + c_2 = 0$
    * $-3.c_1 = c_2$
    * $c_1 -3.c_1 = 0$
    * $c_1 = 3.c_1 \implies c_1 = 0 :\ 0 = 0.3$
    * $0 + c_2 = 0 \implies c_2 = 0$
* Para obtener el vector nulo todos los coeficientes deben ser nulos, por lo que $S$ es linealmente independiente.

## e. $S = \{ (0,2,-1); (1,7,1); (1,3,-1); (0,0,0) \}$

* $(0,0,0) = c_1(0,2,-1) + c_2(1,7,1) + c_3(1,3,-1) + c_4(0,0,0)$
* $= (0,2.c_1,\ -c_1) + (c_2,\ 7.c_2,\ c_2) + (c_3,\ 3.c_3,\ -c_3) + (0,0,0)$
* $= (c_2 + c_3,\ 2.c_1 + 7.c_2 + 3.c_3,\ -c_1 + c_2 - c_3)$
* Para igualar a $(0,0,0)$ debe cumplirse:
    * $c_2 + c_3 = 0$
    * $c_2 = -c_3$
    * $-c_1 + c_2 - c_3 = 0$
    * $c_1 - c_2 = c_3$
    * $c_2 + (c_1 - c_2) = c_2 - c_2 + c_1 = c_1 = 0$
    * $2.c_1 + 7.c_2 + 3.c_3 = 0$
    * $2.0 + 7(-c_3) + 3.c_3 = c_3(-7 + 3) = c_3(-4) = 0 \iff c_3 = 0$
    * $c_2 = -c_3 = -0 = 0$
* Sin embargo, esto es válido para cualquier valor de $c_4$, por lo que no todos los coeficientes deben ser nulos para igualar a $(0,0,0)$.
* Por lo tanto, $S$ no es linealmente independiente.

## f. $S = \{ (4,1,0,0); (-3,0,1,0); (1,0,0,1) \}$

* $(0,0,0,0) = c_1(4,1,0,0) + c_2(-3,0,1,0) + c_3(1,0,0,1)$
* $= (4.c_1, c_1, 0, 0) + (-3.c_2, 0, c_2, 0) + (c_3, 0, 0, c_3)$
* $= (4.c_1 -3.c_2 + c_3,\ c_1,\ 4.c_1 + c_3)$
* Para igualar a $(0,0,0,0)$ debe darse:
    * $c_1 = 0$
    * $4.0 + c_3 = 0 + c_3 = 0 \implies c_3 = 0$
    * $4.0 - 3.c_2 + 0 = -3.c_2 = 0 \implies c_2 = 0$
* Todos los coeficientes son nulos, por lo tanto $S$ es linealmente independiente.

## g. $S = \{\begin{pmatrix} 1 & 0 \\ 1 & 1 \end{pmatrix}; \begin{pmatrix} 0 & 2 \\ 0 & 1 \end{pmatrix} \}$

* $\begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix} = c_1\begin{pmatrix} 1 & 0 \\ 1 & 1\end{pmatrix} + c_2\begin{pmatrix} 0 & 2 \\ 0 & 1\end{pmatrix}$

* $= \begin{pmatrix} c_1 & 0 \\ c_1 & c_1 \end{pmatrix} + \begin{pmatrix} 0 & 2.c_2 \\ 0 & c_2\end{pmatrix}$

* $= \begin{pmatrix} c_1 & 2.c_2 \\ c_1 & c_1 + c_2\end{pmatrix}$

* Para igualar a $\begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}$ debe cumplirse:
    * $c_1 = 0$
    * $c_1 + c_2 = 0 + c_2 = 0 \implies c_2 = 0$
    * $2.c_2 = 2.0 = 0$
* Todos los coeficientes son nulos, por lo tanto $S$ es linealmente independiente.

## h. $S = \{ \begin{pmatrix} 1 & 1 \\ 1 & 1 \end{pmatrix}; \begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}; \begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix} \}$

* $\begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix} = c_1\begin{pmatrix} 1 & 1 \\ 1 & 1 \end{pmatrix} + c_2\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix} + c_3\begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix}$

* $= \begin{pmatrix} c_1 & c_1 \\ c_1 & c_1 \end{pmatrix} + \begin{pmatrix} 0 & c_2 \\ c_2 & 0 \end{pmatrix} + \begin{pmatrix} 0 & 0 \\ 0 & c_3 \end{pmatrix}$

* $= \begin{pmatrix} c_1 & c_1 + c_2 \\ c_1+c_2 & c_1 + c_3 \end{pmatrix}$

* Para igualar a $\begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}$ debe cumplirse:

    * $c_1 = 0$
    * $c_1 + c_2 = 0 + c_2 \implies c_2 = 0$
    * $c_1 + c_3 = 0 + c_3 \implies c_3 = 0$

* Todos los coeficientes son nulos, por lo que $S$ es linealmente independiente.

# 9. Analizar si un conjunto de vectores que contiene al vector nulo puede ser linealmente independiente. Justificar.

Un vector nulo $0_V \in R^n$ puede escribirse como el producto por escalar de cualquier número real $k: k.0_V$, y su resultado seguirá siendo el vector nulo debido a la propiedad del producto de reales con el elemento nulo.

Por lo tanto, al describir la combinación lineal del vector nulo en un conjunto de vectores que lo incluya se llega a la forma:

$$0_V = c_1v_1 + c_2v_2 + ... + c_n0_V$$

En este caso, el valor de $c_n$ puede ser cualquier número real, ya que su producto por escalar siempre dará como resultado el vector nulo. Esto implica que, en un conjunto de vectores que incluya a $0_V$, siempre habrá un coeficiente que podría no ser nulo y aún así obtener una combinación lineal válida para el vector nulo.

# 10. Si el conjunto de vectores $M = \{ u, v, w \}$ de $V$ es linealmente independiente, mostrar que el conjunto $\{ u, u+2v, u+2v+3w \}$ es linealmente independiente.

Se sabe que $M$ es linealmente independiente, tal que existe una combinación lineal para $0_V$ en la cual:
* $c_1u + c_2v + c_3w = (0,0,0)$
* $c_1, c_2, c_3 = 0$

El nuevo conjunto puede expresarse a partir de los elementos de $M$. Quiere demostrarse que, si $M$ es independiente, este nuevo conjunto también lo es:

* $(0,0,0) = c_1.u + c_2(u+2v) + c_3(2v+3w)$

* $= (c_1.u) + (c_2.u + c_2.2v) + (c_3.u + c_3.2v + c_3.3w)$

* Esto puede reescribirse como una combinación lineal para $M$:

* $= u(c_1 + c_2 + c_3) + v(2.c_2 + 2.c_3) + w(3.c_3)$

* Como $M$ es linealmente independiente, sus coeficientes deben ser nulos:
    * $3.c_3 = 0 \implies c_3 = 0$
    * $2.c_2 + 2.c_3 = 2.c_2 + 0 \implies c_2 = 0$
    * $c_1 + c_2 + c_3 = c_1 + 0 + 0 \implies c_1 = 0$

* Por lo tanto, si $M$ es linealmente independiente, entonces $\{ u, u+2v, u+2v+3w \}$ también.

# 11. Analizar si los siguientes conjuntos de vectores pueden ser base de $R^2$

## a. $\{ (2,-1); (1,3) \}$

Se buscará demostrar que los vectores son independientes:
* $(0,0) = c_1(2,-1) + c_2(1,3)$
* $= (2.c_1, -c_1) + (c_2, 3.c_2)$
* $= (2.c_1 + c_2,\ -c_1 + 3.c_2)$
* Para igualar a $(0,0)$ debe cumplirse:
    * $2.c_1 + c_2 = 0$
    * $-c1 + 3.c_2 = 0$
    * $3.c_2 = c_1$
    * $2.3.c_2 + c_2 = 6.c_2 + c_2 = 7.c_2 = 0 \implies c_2 = 0$
    * $c_1 = 3.0 \implies c_1 = 0$
* Los coeficientes son nulos, por lo que el conjunto es linealmente independiente.

Siendo $R^2$ un espacio vectorial de 2 dimensiones, se da que $\{ (2,-1); (1,3) \}$ son 2 vectores linealmente independientes, por lo tanto el conjunto genera $R^2$.

Como $\{ (2,-1); (1,3) \}$ es linealmente independiente y genera a $R^2$, se dice que es una base.

## b. $\{ (2,1); (1,1); (3,2) \}$

La dimensión de $\{ (2,1); (1,1); (3,2) \}$ es mayor a la de $R^2$, por lo que es linealmente dependiente.

Por lo tanto, no puede ser una base para $R^2$.

## c. $\{ (1, -1); (1,0) \}$

Se buscará demostrar que son independientes:
* $(0,0) = c_1(1, -1) + c_2(1,0)$
* $= (c_1, -c_1) + (c_2, 0)$
* $= (c_1 + c_2, -c_1)$
* Para igualar a $(0,0)$ debe cumplirse:
    * $-c_1 = 0 \implies c_1 = 0$
    * $c_1 + c_2 = 0 + c_2 \implies c_2 = 0$
* Los coeficientes son nulos, por lo que el conjunto es linealmente independiente.

Siendo $R^2$ un espacio vectorial de 2 dimensiones, se da que $\{ (1,-1); (1,0) \}$ son 2 vectores linealmente independientes, por lo tanto el conjunto genera $R^2$.

Como $\{ (1,-1); (1,0) \}$ es linealmente independiente y genera a $R^2$, se dice que es una base.

## d. $\{ (1,2); (2,4) \}$

> *con verlo ya te das cuenta que no son independiente porque $2(1,2) = (2,4)$ pero no creo que les guste esa respuesta en un parcial*

Se buscará demostrar que son independientes:
* $(0,0) = c_1(1,2) + c_2(2,4)$
* $= (c_1,\ 2.c_1) + (2.c_2,\ 4.c_2)$
* $= (c_1 + 2.c_2,\ 2.c_1 + 4.c_2)$
* Para igualar a $(0,0)$ debe cumplirse:
    * $c_1 + 2.c_2 = 0$
    * $2.c_1 + 4.c_2 = 0$
    * $2(c_1 + 2.c_2) = 2.c_1 + 4.c_2 = 0$
* Puede obtenerse $(0,0)$ a partir de varios valores no nulos para los coeficientes (por ejemplo, $c_1 = 2,\ c_2 = -1$)

Por lo tanto, $\{(1,2); (2,4) \}$ es linealmente dependiente y no puede ser una base para $R^2$.

# 12. Dar las coordenadas de $v = (1,2)$ en los conjuntos del ejercicio anterior que resultaron ser bases.

## a. $\{ (2,-1); (1,3) \}$

* $v = (1,2) = \alpha(2, -1) + \beta(1,3)$
* $= (2\alpha, -\alpha) + (\beta, 3\beta)$
* $= (2\alpha + \beta, -\alpha + 3\beta)$
* Para llegar a $v = (1,2)$ los coeficientes deben cumplir:
    * $2\alpha + \beta = 1$

    * $-\alpha + 3\beta = 2$

    * $\beta = 1 - 2\alpha$

    * $-\alpha + 3(1-2\alpha) = 2$

    * $-\alpha + 3 - 6\alpha = 2$

    * $-\alpha - 6\alpha = -1$

    * $-7\alpha = -1$

    * $\alpha = \dfrac 1 7$

    * $\beta = 1 - 2.\dfrac 1 7 = 1 - \dfrac 2 7 = \dfrac 5 7$

Por lo tanto, las coordenadas de $v = (1,2)$ en la base $\{ (2,-1); (1,3) \}$ son $(\dfrac 1 7,\ \dfrac 5 7)$.

## b. $\{ (1,-1); (1,0) \}$

* $v = (1,2) = \alpha(1, -1) + \beta(1,0)$
* $= (\alpha, -\alpha) + (\beta,0)$
* $= (\alpha + \beta, -\alpha)$
* Para llegar a $v = (1,2)$ los coeficientes deben cumplir:
    * $-\alpha = 2 \implies \alpha = -2$
    * $\alpha + \beta = -2 + \beta = 1$
    * $-2-1 = -\beta$
    * $\beta = 3$

Por lo tanto, las coordenadas de $v=(1,2)$ en la base $\{ (1,-1); (1,0) \}$ son $(-2,\ 3)$.

# 13. Hallar la base para cada conjunto del ejercicio 3 que sea un subespacio.

## a. $S = \{ (x,0): x \in R \}$

Cualquier vector en $S$ puede escribirse como una combinación lineal:

* $(x,0) = x(1,0)$

Por lo que $(1,0)$ es la base de $S$.

## b. $S = \{ (x,y) \in R^2 : x + y = 0 \}$

* $x + y = 0$

* $x = -y \implies y = -x$

Cualquier vector $\in S$ cumple con la forma $(x,-x)$. Esto puede generarse con una combinación lineal:
* $(x,-x) = x(1,-1)$

Por lo que $(1,-1)$ es la base de $S$.

## c. $\{ (x,y,z) \in R^3 : z = x-y \}$

* $z = x-y$

Se quiere hallar una base $B = \{ v_1, v_2 \}$ a partir de la cual se pueda obtener cualquier vector tal que:

$$\alpha\begin{pmatrix} v_{11} \\ v_{12} \\ v_{13} \end{pmatrix} + \beta\begin{pmatrix} v_{21} \\ v_{22} \\ v_{23} \end{pmatrix} = \begin{pmatrix} \alpha \\ \beta \\ \alpha - \beta \end{pmatrix}$$

> *cuando un subespacio tiene N restricciones, se le quitan N vectores a la base del conjunto (en este caso $R^3$ tiene 3 vectores, se quita 1)*

* $= \alpha(v_{11}, v_{12}, v_{13}) + \beta(v_{21}, v_{22}, v_{23})$
* $= (\alpha.v_{11} + \beta.v_{21}, \alpha.v_{12} + \beta.v_{22}, \alpha.v_{13} + \beta.v_{13})$
* $\alpha.v_{13} + \beta.v_{23} = (\alpha.v_{11} + \beta.v_{21}) - (\alpha.v_{12} + \beta.v_{22})$
* $= \alpha.v_{11} + \beta.v_{21} - \alpha.v_{12} - \beta.v_{12} = \alpha.v_{11} - \alpha.v_{12} + \beta.v_{21} - \beta.v_{22}$
* $= \alpha(v_{11} - v_{12}) + \beta(v_{21} - v_{22})$
    * $v_{13} = v_{11} - v_{12}$
    * $v_{23} = v_{21} - v_{22}$

Algunas posibles bases que cumplan con esta condición son:
* $(1,0,1); (0,1,-1)$
    * $(x,y,z) = (1,0,1): x-y = 1-0 = 1$
    * $(x,y,z) = (0,1,-1): x-y = 0-1 = -1$
* $(1,0,1); (1,1,0)$
    * $(x,y,z) = (1,0,1): x-y = 1-0 = 1$
    * $(x,y,z) = (1,1,0): x-y = 1-1 = 0$

## d. $\{ (x,y,z,w) \in R^4 : x + y - w = 0, z + 3y = 0 \}$

* $x+y-w = 0$
* $w = x+y$
* $z+3y = 0$
* $z = -3y$

Se quiere hallar una base $B = \{ v_1, v_2 \}$ a partir de la cual se pueda obtener cualquier vector tal que:

$$\alpha\begin{pmatrix} v_{11} \\ v_{12} \\ v_{13} \\ v_{14}\end{pmatrix} + \beta\begin{pmatrix} v_{21} \\ v_{22} \\ v_{23} \\ v_{24}\end{pmatrix} = \begin{pmatrix} x \\ y \\ -3y \\ x+y \end{pmatrix}$$

* $\alpha.v_{11} + \beta.v_{21} = x$
* $\alpha.v_{12} + \beta.v_{22} = y$
* $\alpha.v_{13} + \beta.v_{13} = -3y = -3(\alpha.v_{12} + \beta.v_{22}) = -3\alpha.v_{12} -3\beta.v_{22}$
* $\alpha.v_{14} + \beta.v_{24} = z = x+y = (\alpha.v_{11} + \beta.v_{21}) + (\alpha.v_{12} + \beta.v_{12}) = \alpha(v_{11} + v_{12}) + \beta(v_{21} + v_{22})$

Una posible base para $S$ sería:
* $(1,1, -3, 2); (1,0,0,1)$
    * $(\alpha, \alpha, -3\alpha, 2\alpha) + (\beta, 0, 0, \beta)$
    * $(\alpha + \beta, \alpha, -3\alpha, 2\alpha + \beta)$
    * $x = \alpha + \beta$
    * $y = \alpha$
    * $z = -3\alpha = -3y$
    * $w = 2\alpha + \beta = \alpha + (\alpha + \beta) = x+y$

# 14. Analizar si las siguientes aplicaciones entre espacios vectoriales son transformaciones lineales:

## a. $L: R^2 \to R^3$ definida por $L(x,y) = (x,y,x+y)$

Para que $L$ sea una transformación lineal válida deben cumplirse las propiedades:
* $L(v_1 + v_2) = L(v_1) + L(v_2) \quad \forall v_1, v_2 \in R^2$
    * $L((x,y) + (w,z)) = L(x,y) + L(w,z)$
    * $L(x+w, y+z) = (x,y,x+y) + (w,z, w+z)$
    * $(x+w, y+z, x+w+y+z) = (x+w, y+z, x+y+w+z)$ // válido por conmutatividad de la suma en $R$

* $L(\alpha.v) = \alpha.L(v) \quad \forall v \in R^2,\ \forall \alpha \in K$
    * $L(\alpha(x,y)) = \alpha.L(x,y)$
    * $L(\alpha.x, \alpha.y) = \alpha.(x,y,x+y)$
    * $(\alpha.x, \alpha.y, \alpha.x + \alpha.y) = \alpha.x, \alpha.y, \alpha(x+y)$
    * $(\alpha.x, \alpha.y, \alpha.x + \alpha.y) = (\alpha.x, \alpha.y, \alpha.x + \alpha.y)$

$L$ cumple con las dos propiedades, por lo que es una transformación lineal válida de $R^2$ hacia $R^3$.

> también se podría resolver con una sola propiedad $L(\alpha.v_1 + \alpha.v_2) = \alpha.L(v_1) + \alpha.L(v_2)$, pero por separado se entiende más

## b. $L: R^3 \to R^2$ definida por $L(x,y,z) = (x+z, y+z)$

* $L(v_1 + v_2) = L(v_1) + L(v_2) \forall v_1, v_2 \in R^3$
    * $L((x,y,z) + (a,b,c)) = L(x,y,z) + L(a,b,c)$
    * $L(x+a,\ y+b,\ z+c) = (x+z,\ y+z) + (a+c,\ b+c)$
    * $(x+a+z+c, \ y+b+z+c) = (x+z+a+c,\ y+z+b+c)$ // válido por conmutatividad de la suma en $R$
* $L(\alpha.v) = \alpha.L(v) \quad \forall v \in R^3,\ \alpha \in K$
    * $L(\alpha(x,y,z)) = \alpha.L(x,y,z)$
    * $L(\alpha.x,\ \alpha.y,\ \alpha.z) = \alpha(x+z, y+z)$
    * $(\alpha.x + \alpha.z,\ \alpha.y + \alpha.z) = (\alpha(x+z),\ \alpha(y+z))$
    * $(\alpha.x + \alpha.z,\ \alpha.y + \alpha.z) = (\alpha.x + \alpha.z,\ \alpha.y + \alpha.z)$

$L$ cumple con las dos propiedades, por lo que es una transformación lineal válida de $R^3$ hacia $R^2$.

## c. $L: R^3 \to R^3$ definida por $L(x,y,z) = (x-2, y+3x, 1)$

* $L(v_1 + v_2) = L(v_1) + L(v_2)$
    * $L((x,y,z) + (a,b,c)) = L(x,y,z) + L(a,b,c)$
    * $L(x+a,\ y+b,\ z+c) = (x-2,\ y+3x,\ 1) + (a-2,\ b+3a,\ 1)$
    * $(x+a-2,\ y+b+3(x+a),\ 1) = (x-2+a-2,\ y+3x+b+3a,\ 1+1)$
    * $(x+a-2,\ y+b+3x+3a,\ 1) = (x-4+a,\ y+3x+b+3a,\ 2)$ // **NO** se cumple la igualdad

$L$ no cumple con una de las propiedades de las transformaciones lineales, lo cual es evidencia suficiente para asumir que no lo es.

## d. $L: R^{2\times 2} \to R^{2\times 2}$ definida por $L\begin{pmatrix} x & y \\ z & w\end{pmatrix} = \begin{pmatrix} z & -x \\ y & -w \end{pmatrix}$

* $L(v_1 + v_2) = L(v_1) + L(v_1) \quad \forall v_1, v_2 \in R^{2\times2}$

    * $L(\begin{pmatrix} x & y \\ z & w\end{pmatrix} + \begin{pmatrix} a & b \\ c & d \end{pmatrix}) = L\begin{pmatrix} x & y \\ z & w\end{pmatrix} + L\begin{pmatrix} a & b \\ c & d\end{pmatrix}$

    * $L\begin{pmatrix} x+a & y+b \\ z+c & w+d\end{pmatrix} = \begin{pmatrix} z & -x \\ y & -w\end{pmatrix} + \begin{pmatrix} c & -a \\ b & -d\end{pmatrix}$

    * $\begin{pmatrix} z+c & -(x+a) \\ y+b & -(w+d) \end{pmatrix} = \begin{pmatrix} z+c & -x-a \\ y+b & -w-d \end{pmatrix}$

    * $\begin{pmatrix} z+c & -x-a \\ y+b & -w-d \end{pmatrix} = \begin{pmatrix} z+c & -x-a \\ y+b & -w-d \end{pmatrix}$

* $L(\alpha.v) = \alpha.L(v) \quad \forall v \in R^{2\times2},\ \forall \alpha \in K$

    * $L(\alpha\begin{pmatrix} x & y \\ z & w \end{pmatrix}) = \alpha.L\begin{pmatrix} x & y \\ z & w\end{pmatrix}$

    * $L\begin{pmatrix} \alpha.x & \alpha.y \\ \alpha.z & \alpha.w\end{pmatrix} = \alpha\begin{pmatrix} z & -x \\ y & -w\end{pmatrix}$

    * $\begin{pmatrix} \alpha.z  & -(\alpha.x) \\ (\alpha.y) & -(\alpha.w) \end{pmatrix} = \begin{pmatrix} \alpha.z & -x.\alpha \\ (\alpha.y) & -w.\alpha \end{pmatrix}$

$L$ cumple con las dos propiedades, por lo que es una transformación lineal válida en $R^{2\times2}$.

## e. $L: R^{2\times 2} \to R^{2\times 2}$ definida por $L\begin{pmatrix} x & y \\ z & w\end{pmatrix} = \begin{pmatrix} x & -x \\ y & 1\end{pmatrix}$

> *BASTA DE MATRICES NO VOY A HACER MÁS ODIO ESCRIBIR MATRICES*

## f. $L: R^{2\times 2} \to R^2$ definida por $L\begin{pmatrix} x & y \\ z & w\end{pmatrix} = (x+z, y+w)$

☝

## g. $L: R^3 \to R^2$ definida por $L(x,y,z) = (0,0)$

> *la transformación nula ya está definida dentro de los mismos conjuntos, no sé qué pasa cuando pasás de uno a otro así que lo tengo que demostrar igual 😴*

* $L(v_1 + v_2) = L(v_1) + L(v_2) \quad \forall v_1, v_2 \in R^3$
    * $L((x,y,z) + (a,b,c)) = L(x,y,z) + L(a,b,c)$
    * $L(x+a,\ y+b,\ z+c) = (0,0) + (0,0)$
    * $(0,0) = (0,0)$
* $L(\alpha.v) = \alpha.L(v) \quad \forall v \in R^3,\ \forall \alpha \in K$
    * $L(\alpha(x,y,z)) = \alpha.L(x,y,z)$
    * $L(\alpha.x,\ \alpha.y,\ \alpha.z) = \alpha(0,0)$
    * $(0,0) = (0,0)$

$L$ cumple con las dos propiedades, por lo que es una transformación lineal válida de $R^3$ hacia $R^2$.

# 15. Hallar el núcleo e imagen de cada una de las transformaciones lineales del punto anterior y las dimensiones de cada uno de esos subespacios.

## a. $L: R^2 \to R^3$ definida por $L(x,y) = (x,y,x+y)$

El núcleo de $L$ está formado por todos aquellos elementos de $R^2$ que al ser transformados por $L$ dan como resultado el vector nulo de $R^3: (0,0,0)$.

$L$ está definida como $L(x,y) = (x,y,x+y)$, tal que la única forma de obtener el vector nulo es:
* $x = 0$
* $y = 0$
* $x+y = 0$
* $(x,y,x+y) = \alpha(0,0) = (0,0)$

Por lo cual, el núcleo está formado únicamente por el vector nulo de $R^2: (0,0)$. La base para este conjunto contiene únicamente al vector nulo, por lo que tiene dimensión 0.

> *🤓 aunque la base tenga un elemento, si justo es un valor nulo se dice que tiene dimensión 0*

La imagen de $L$ está formada por los elementos de $R^3$ que tienen una preimagen en $R^2$. A partir de la definición de $L$, la imagen contendrá a los vectores de $(x,y,z) \in R^3 : z = x+y$.

* $Im(L) = \{ (x,y,z) \in R^3 : z = x+y \}$
* $(x,y,x+y) = x(1,0,1) + y(0,1,1) = (x,0,x) + (0,y,y) = (x,y,x+y)$

La base para $Im(L)$ está dada por $\{ (1,0,1); (0,1,1) \}$, por lo que la imagen tiene dimensión 2.

## b. $L: R^3 \to R^2$ definida por $L(x,y,z) = (x+z, y+z)$

Para obtener el vector nulo a partir de $L$ debe darse:
* $x+z = 0$
* $y+z = 0$
* $x = y = -z$
* $(x,y,z) \in Nu(f) \iff (x,x, -x)$
* $(x,x,-x) = x(-1, -1, 1) = (-x, -x, x) \to (-x + x, -x + x) = (0,0)$

La base para el núcleo está dada por $\{ (-1, -1, 1) \}$, por lo que tiene dimensión 1.

La imagen de $L$ contiene a los elementos tales que:
* $Im(L) = \{ (x+y,y+z) \in R^2 : (x,y,z) \in R^3 \}$
* $(x+z, y+z) = x(1,0) + y(0,1) + z(1,1) = (x,0) + (0,y) + (z,z) = (x+z, y+z)$

$\{ (1,1) \}$ es redundante en la base, por lo que puede eliminarse.

La base de la imagen está dada por $\{ (1,0); (0,1) \}$, por lo que tiene dimensión 2.

## c. $L: R^3 \to R^2$ definida por $L(x,y,z) = (0,0)$

Como $L$ es una transformación nula (que da como resultado al vector nulo), el núcleo contendrá a todos los elementos de $R^3$, ya que serán convertidos a $(0,0)$ independientemente de su valor.

Como la base de $R^3$ es de dimensión 3, el núcleo también lo será.

La imagen, por otro lado, contendrá únicamente a $(0,0)$, ya que es el único elemento $\in R^2$ con preimagen en $R^3$. Por lo tanto, la base de la imagen será $\{(0,0)\}$ y tendrá dimensión 0.

# 16. Mostrar que la composición de transformaciones lineales es una transformación lineal

?

# 17.

## a. ¿Es la aplicación identidad una transformación lineal? En caso de serlo, hallar núcleo e imagen.

> *sí porque lo dice el apunte de la teoría*

La aplicación identidad es una transformación lineal $L: V \to V$ definida por $L(v) = v$.

Se demostrará que cumple con las propiedades de transformaciones lineales:
* $L(v_1 + v_2) = L(v_1) + L(v_2) \quad \forall v_1,v_2 \in V$
    * $v_1 + v_2 = v_1 + v_2$

* $L(\alpha.v) = \alpha.L(v) \quad \forall v \in V,\ \alpha \in K$
    * $\alpha.v = \alpha.v$

$L$ cumple con ambas propiedades, por lo que es una transformación lineal.

El núcleo de $L$ contiene sólo al vector nulo, ya que es el único caso en el que $L(0_V) = 0_V$, por lo que tiene dimensión 0.

La imagen contiene a todos los elementos de $V$, ya que cualquier elemento $\in V$ es su "propia" preimagen. Debido a esto, la imagen tendrá la misma dimensión que $V$.
## b. ¿Es la aplicación nula una transformación lineal? En caso de serlo, hallar núcleo e imagen.

> *sí porque lo dice el apunte de la teoría*

La aplicación nula es una transformación lineal $L: V \to V$ definida por $L(v) = 0_V$

Se demostrará que cumple con las propiedades de transformaciones lineales:
* $L(v_1 + v_2) = L(v_1) + L(v_2) \quad \forall v_1, v_2 \in V$
    * $0_V = 0_V + 0_V = 0_V$

* $L(\alpha.v) = \alpha.L(v) \quad \forall v \in V,\ \alpha \in K$
    * $0_V = \alpha.0_V = 0_V$

$L$ cumple con ambas propiedades, por lo que es una transformación lineal.

El núcleo de $L$ contiene a todos los elementos de $V$, ya que todos se transforman en $0_V$ al aplicar $L$. Debido a esto, su dimensión será la misma que la de $V$.

La imagen sólo contiene a $0_V$, ya que es el único elemento de $V$ con preimagen (en este caso, todos los elementos de $V$ serían preimágenes de $0_V$). Debido a esto, la imagen tiene dimensión 0.

# 18. Sean $C = C[a,b]$  el espacio vectorial de las funciones de $[a,b] $ en $R$ y $L:C \to R$ definida por $L(f) = \int_{a}^b f(x)dx$. Mostrar que $L$ es una transformación lineal.

Para que $L$ sea una transformación lineal debe cumplir las propiedades:
* $L(f_1 + f_2) = L(f_1) + L(f_2) \quad \forall f_1, f_2 \in C$

    * $\int_{a}^b ((f_1(x) + f_2(x)) dx) = \int_{a}^b f_1(x)dx + \int_{a}^b f_2(x)dx$

    * $\int_{a}^b ((f_1(x) + f_2(x)) dx) = \int_{a}^b ((f_1(x) + f_2(x)) dx)$

* $L(\alpha.f) = \alpha.L(f) \quad \forall f \in C,\ \forall \alpha \in K$

    * $\int_{a}^b \alpha.f(x)dx = \alpha\int_a^b f(x)dx$

    * $\alpha\int_a^b f(x)dx = \alpha\int_a^b f(x)dx = \alpha.L(f)$

$L$ cumple ambas propiedades, por lo que es una transformación lineal válida de $C$ a $R$.

# 19. Sean $C = C[a,b] $ el espacio vectorial de funciones definidas en $R$ y sea $D: C \to C$ dado por $D(f) = f'$ (esto es, para cada función $f \in C$ el operador Derivación, D, devuelve la derivada $f'$ de $f$ ). Mostrar que $D$ es una transformación lineal.

?????????????????

Para que $D$ sea una transformación lineal debe cumplir las propiedades:
* $D(f_1 + f_2) = D(f_1) + D(f_2) \quad \forall f_1, f_2 \in C$
    * $D(f_1 + f_2) = (f_1 + f_2)'$
    * $= f_1' + f_2' = D(f_1) + D(f_2)$ // por propiedades de derivadas con la suma

* $D(\alpha.f) = \alpha.D(f) \quad \forall f \in C,\ \alpha \in K$
    * $D(\alpha.f) = (\alpha.f)'$
    * $= \alpha(f') = \alpha.D(f)$ // por propiedades de derivadas con el producto por constantes

$D$ cumple con ambas propiedades, por lo que es una transformación lineal válida en $C$.

# 20. Demostrar que dada cualquier transformación lineal $L: V \to W$ (con $V,W$ espacios vectoriales) el núcleo y la imagen de $L$ forman un subespacio $V$ y $W$ respectivamente.

## Demostración del núcleo

$Nu(f)$ está formado por todos los elementos $v \in V$ tales que $L(v) = 0_W$.

Por definición de transformaciones lineales se sabe que $L(0_V) = 0_W$, por lo que se cumple la primera propiedad de un subespacio: $Nu(L) \subset V: (0_V) \in Nu(L) \implies Nu(L) \ne \emptyset$.

Sean dos elementos $v_1, v_2 \in Nu(L)$, se sabe que $L(v_1) = L(v_2) = 0_V$. A partir de esto se quiere demostrar que $L(v_1 + v_2) = 0$ y, por lo tanto, la suma pertenece al núcleo:
* $L(v_1 + v_2) = L(v_1) + L(v_2)$
* $= 0_V + 0_V = 0_v \implies L(v_1 + v_2) \in Nu(f)$

Por último, se debe probar que el producto por escalar también pertenece al núcleo.
* $L(\alpha.v) = \alpha.L(v)$
* $=\alpha.0_V = 0_V \implies L(\alpha.v) \in Nu(L)$ // por definición del valor nulo

Entonces, el núcleo de $L: V \to W$ cumple todas las propiedades necesarias para considerarse un subespacio de $V$.

## Demostración de la imagen

$Im(f)$ está formado por todos los elementos $w \in W$ tales que $\exists v \in V : L(v) = w$

Nuevamente, se sabe que $L(0_V) = 0_W$, por lo tanto existe una preimagen para el vector nulo de $W$. Esto implica que $Im(L) \ne \emptyset$.

Sean dos elementos $w_1, w_2 \in Im(L)$, se sabe que existen dos elementos $v_1, v_2 \in V : L(v_1) = w_1, L(v_2) = w_2$. A partir de esto se quiere demostrar que la suma de $w_1 + w_2$ también pertenece a la imagen:
* $w_1 + w_2 = L(v_1 + v_2)$
* $= L(v_1) + L(v_2)$
* $= w_1 + w_2 \implies (w_1 + w_2) \in Im(L)$

Por último, se debe probar que el producto por escalar de cualquier elemento $w \in Im(L)$ también pertenece a la imagen:
* $w = L(v)
* $\alpha.w = \alpha.L(v)$
* $= L(\alpha.v) \implies (\alpha.v) \in Im(L)$

Entonces, la imagen de $L: V \to W$ cumple todas las propiedades necesarias para considerarse un subespacio de $W$.

# 21.

## a. Hallar $L: R^2 \to R^2$ sabiendo $L(1,0) = (1,-2); \ L(0,1) = (1,-1)$

Como sabemos los valores de $L$ en la base canónica de $R^2$, podemos describir cualquier $(x,y)$ resultante como:

$$(x,y) = x(1,0) + y (0,1)$$

Podemos aplica la transformación lineal en ese vector para obtener el vlaor de $L$:

* $L(x,y) = L(x(1,0) + y(0,1))$

* $= L(x(1,0)) + L(y(0,1))$

* $= x.L(1,0) + y.L(0,1)$

* $= x(1,-2) + y(1,-1)$

* $= (x,\ -2x) + (y,\ -y)$

* $= (x+y, -2x-y)$

Por lo tanto, la transformación $L: R^2 \to R^2$ se define como $L(x,y) = (x+y,\ -2x-y)$

## b. Hallar $L: R^3 \to R^2$ sabiendo que $L(1,0,0) = (1,0);\ L(0,1,0) = (-1,-6);\ L(0,0,1) = (0,4)$

Como sabemos los valores de $L$ en los vectores de la base de $R^3$, podemos describir cualquier $(x,y,z)$ resultante como:

$$(x,y,z) = x(1,0,0) + y(0,1,0) + z(0,0,1)$$

Podemos aplicar la transformación lineal en ese vector para obtener el valor de $L$:

* $L(x,y,z) = L(x(1,0,0) + y(0,1,0) + z(0,0,1))$

* $= L(x(1,0,0)) + L(y(0,1,0)) + L(z(0,0,1))$

* $= x.L(1,0,0) + y.L(0,1,0) + z.L(0,0,1)$

* $= x(1,\ 0) + y(-1,\ -6) + z(0,\ 4)$

* $= (x,\ 0) + (-y,\  -6y) + (0,\ 4z)$

* $= (x-y, -6y + 4z)$

Por lo tanto, la transformación $L: R^3 \to R^2$ se define como $L(x,y,z) = (x-y, -6y + 4z)$

## c. Hallar $L: R^2 \to R^2$ sabiendo que $L(1,1) = (4,2);\ L(0,3) = (1,0)$

Cualquier vector $(z,w) \in R^2$ puede escribirse como una combinación lineal tal que:

* $(w,z) = (a_{11}.x + a_{12}.y,\ a_{21}x + a_{22}.y)$

Sabiendo $L(1,1) = (4,2)$ se puede despejar:
* $(4,2) = (a_{11} + a_{12},\ a_{21} + a_{22})$

Por otro lado, sabeindo $L(0,3) = (1,0)$ se obtiene:
* $(1,0) = (a_{11}.0 + a_{12}.3,\ a_{21}.0 + a_{22}.3)$
* $= (a_{12}.3, a_{22}.3)$

De los cuales se obtienen las ecuaciones:
* $4 = a_{11} + a_{12}$
* $2 = a_{21} + a_{22}$
* $1 = a_{12}.3$
* $0 = a_{22}.3$

A partir de lo que se pueden obtener los valores:
* $0 = a_{22}.3 \implies a_{22} = 0$

* $1 = a_{12}.3 \implies a_{12} = \dfrac 1 3$

* $2 = a_{21} + a_{22} = a_{21} + 0 \implies a_{21} = 2$

* $4 = a_{11} + \dfrac 1 3 = 4 - \dfrac 1 3 = a_{11} \implies a_{11} = \dfrac {11} 3$

Por lo que la transformación lineal se define como:

$$L(x,y) = (\dfrac {11} 3x + \dfrac 1 3 y,\ 2x)$$

## d. Hallar $L: R^3 \to R^3$ sabiendo que $L(1,1,1) = (1,2,3);\ L(0,1,0) = (1,-1,0);\ L = (-1,1,1) = (5,4,3)$

Un vector $(a,b,c) \in R^3$ puede escribirse como una combinación lineal tal que:

* $(a,b,c) = (a_{11}.x + a_{12}.y + a_{13}.z,\ a_{21}.x + a_{22}.y + a_{23}.z, a_{31}.x + a_{32}.y + a_{33}.z)$

Sabiendo $L(1,1,1) = (1,2,3)$ se puede despejar:

* $(1,2,3) = (a_{11} + a_{12} + a_{13}, \ a_{21} + a_{22} + a_{23},\ a_{31} + a_{32} + a_{33})$

Sabiendo $L(0,1,0) = (1,-1,0)$:

* $(1,-1,0) = (a_{12},\ a_{22}, a_{32})$

Sabiendo $L(-1,1,1) = (5,4,3)$:

* $(5,4,3) = (-a_{11} + a_{12} + a_{13}, -a_{21} + a_{22} + a_{23}, -a_{31} + a_{32} + a_{33})$

A partir de lo que se pueden obtener los valores:

* $a_{12} = 1$
* $a_{22} = -1$
* $a_{32} = 0$
* $a_{11} + a_{12} + a_{13} = a_{11} + 1 + a_{13} = 1 \implies a_{11} = -a_{13}$
* $-a_{11} + a_{12} + a_{13} = a_{13} + 1 + a_{13} = 2.a_{13} + 1 = 5 \implies a_{13} = 2,\ a_{11} = -2$
* $a_{21} + a_{22} + a_{23} = a_{21} -1 + a_{23} = 2 \implies a_{21} + a_{23} = 3$
* $-a_{21} + a_{22} + a_{23} = -a_{21} -1 + a_{23} = 4 \implies -a_{21} + a_{23} = 5$
* $a_{23} = 3-a_{21}$
* $-a_{21} + 3 - a_{21} = 5$
    * $-2a_{21} = 2$
    * $a_{21} = -1$
* $a_{21} + a_{23} = -1 + a_{23} = 3 \implies a_{23} = 4$
* $a_{31} + a_{32} + a_{33} = a_{31} + 0 + a_{33} = 3 \implies a_{31} + a_{33} = 3$
* $-a_{31} + a_{32} + a_{33} = -a_{31} + 0 + a_{33} = 3 \implies -a_{31} + a_{33} = 3$
* $a_{31} = -a_{31} \implies a_{31} = 0$
* $a_{31} + a_{33} = 0 + a_{33} = 3 \implies a_{33} = 3$

Por lo que la transformación lineal $L: R^3 \to R^3$ se define como:

$$L(x,y,z) = (-2x + y + 2z,\ -x -y + 4z,\ 3z)$$

Esto se puede comprobar a partir de los casos conocidos:
* $L(1,1,1) = (1,2,3)$
    * $-2x + y + 2z = -2 + 1 + 2 = 1$
    * $-x -y + 4z = -1-1+4 = 2$
    * $3z = 3.1 = 3$
* $L(0,1,0) = (1,-1,0)$
    * $-2x + y + 2z = 0 + 1 + 0 = 1$
    * $-x-y + 4z = 0 -1 - 4.0 = -1$
    * $3z = 3.0 = 0$
* $L(-1,1,1) = (5,4,3)$
    * $-2x+y+2z = -2(-1) + 1 + 2.1 = 2 + 1 + 2 = 5$
    * $-x-y+4z = -(-1) -1 + 4 =0+4 = 4$
    * $3z = 3.1 = 3$

# 22. Hallar las matrices asociadas a las siguientes transformaciones lineales en las bases indicadas

## a. $L: R^3 \to R^2$ definida como $L(x,y,z) = (z-y, z-x)$ con las bases canónicas de $R^3$ y $R^2$

$B_{R^3} = B_1 = \{ (1,0,0); (0,1,0); (0,0,1) \}$

$B_{R^2} = B_2 = \{ (1,0); (0,1) \}$

Primero se aplica $L$ sobre los vectores de la base de $R^3$:
* $L(1,0,0) = (0-0, 0-1) = (0,-1)$
* $L(0,1,0) = (0-1, 0-0) = (-1,0)$
* $L(0,0,1) = (1-0, 1-0) = (1,1)$

> *🤓 en este caso no es necesario convertir las coordenadas a otra base porque son las 2 canónicas*

Por lo tanto, la matriz asociada a $L$ en las bases $B_1$ y $B_2$ es:

$$[L]_{B_1,\ B_2} = \begin{pmatrix} 0 & -1 & 1 \\ -1 & 0 & 1 \end{pmatrix}$$

## b. $L: R^3 \to R^3$ definida como $L(x,y,z) = (3x+z, y-x, 2z+2y)$ con la base canónica de $R^3$.

$B_{R^3} = B = \{ (1,0,0);\ (0,1,0);\ (0,0,1) \}$

Primero se aplica $L$ sobre los vectores de la base:
* $L(1,\ 0,\ 0) = (3.1+0,\ 0-1,\ 0) = (3,\ -1,\ 0)$
* $L(0,\ 1,\ 0) = (0,\ 1-0,\ 0 + 2.1) = (0,\ 1,\ 2)$
* $L(0,\ 0,\ 1) = (3.0 + 1,\ 0,\ 2.1 + 2.0) = (1,\ 0,\ 2)$

Por lo tanto, la matriz asociada $L$ en la base canónica de $R^3$ es:

$$[L]_B = \begin{pmatrix} 3 & 0 & 1 \\ -1 & 1 & 0 \\ 0 & 2 & 2\end{pmatrix}$$

## c. $L: R^{2\times2} \to R^2$ definida como $L\begin{pmatrix} x & y \\ z & w\end{pmatrix} = (x+y, z+w)$ con $B$ siendo la base canónica de $R^{2\times2}$ y $B_1 = \{ (1,1); (-1,5) \}$ una base de $R^3$.

$B_{R^2} = B_1 = \{ (1,0);\ (0,1) \}$

$B_{R^{2\times2}} = B_2 = \{ \begin{pmatrix} 1 & 0 \\ 0 & 0 \end{pmatrix};\ \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix};\ \begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix};\ \begin{pmatrix} 0 & 0 \\ 0 & 1 \end{pmatrix} \}$


Primero se aplica $L$ sobre los vectores de la base de $R^{2\times2}$:

* $L\begin{pmatrix} 1 & 0 \\ 0 & 0\end{pmatrix} = (1+0, 0+0) = (1,0)$

* $L\begin{pmatrix} 0 & 1 \\ 0 & 0\end{pmatrix} = (0+1, 0+0) = (1,0)$

* $L\begin{pmatrix} 0 & 0 \\ 1 & 0\end{pmatrix} = (0+0, 1+0) = (0,1)$

* $L\begin{pmatrix} 0 & 0 \\ 0 & 1\end{pmatrix} = (0+0, 0+1) = (0,1)$

Al estar trabajando sobre la base $B_1$, que no es canónica, deben convertirse las coordenadas:
* $(1,0) = \alpha(1,1) + \beta(-1,5)$
    * $=(\alpha, \alpha) + (-\beta, 5\beta)$
    * $= (\alpha - \beta,\ \alpha + 5\beta)$
    * $\alpha - \beta = 1$
    * $\alpha + 5\beta = 0 \implies \alpha = -5\beta$
    * $-5\beta - \beta = 1$
    * $-6\beta = 1 \implies \beta = -\dfrac 1 6$
    * $\alpha - \beta = \alpha + \dfrac 1 6 = 1 \implies \alpha = \dfrac 5 6$
* $(0,1) = \alpha(1,1) + \beta(-1,5)$
    * $=(\alpha, \alpha) + (-\beta, 5\beta)$
    * $= (\alpha - \beta,\ \alpha + 5\beta)$
    * $\alpha - \beta = 0$
    * $\alpha + 5\beta = 1$
    * $\alpha = \beta$
    * $\alpha + 5\alpha = 6\alpha = 1 \implies \alpha = \dfrac 1 6,\ b = \dfrac 1 6$

Por lo tanto, la matriz asociada para las bases $B_1, B_2$ será:

$$[L]_{B_1, B_2} = \begin{pmatrix} \dfrac 5 6 & \dfrac 5 6 & \dfrac 1 6 & \dfrac 1 6 \\\\ -\dfrac 1 6 & - \dfrac 1 6 & \dfrac 1 6 & \dfrac 1 6 \end{pmatrix}$$