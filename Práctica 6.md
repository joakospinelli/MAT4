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