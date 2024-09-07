# 1. Suponga que $(x_1, y_1), ... , (x_n, y_n)$ son pares observados generados por los siguientes modelos. Deduzca los estimadores de mínimos cuadrados de $\beta_1$ y $\beta_0$.

## a. $Y = \beta_1 x + \epsilon$

$\beta_0 = 0$ a partir de la definición del modelo de regresión $Y = \beta_0 + \beta_1x + \epsilon$, por lo que no es necesaria su estimación.

Se quiere saber el valor de la recta de regresión verdadera en el punto $x=0$, a partir de la deducción de que la ordenada al origen es 0:

* $Y = \beta_1 0 + 0$ // *$\epsilon = 0$ porque es la recta de regresión verdadera*
* $Y = 0$

Por lo tanto, la recta pasa por el punto $(0,0)$.

### Cálculo de desviación vertical

$Altura Punto - Altura Línea = y_i - (\beta_0 + \beta_1 x)$

En este caso, al ser una recta con ordenada al origen en 0, la altura de un punto $(x_i, y_i)$ está dada por $y_i$. La altura de la línea, por otro lado, está definida por el modelo; en este caso, por $\beta_1x$.

$y_i - \beta_1x_i = y_i-(\beta_0 + \beta_1x_i)$

$y_i - \beta_1x_i = y_i - (\beta_1x_i)$

Por lo tanto, la desviación vertical está dada por:

$y_i - \beta_1x_i$

### Cálculo de estimadores

A partir de la desviación vertical puede definirse una función $f$ para calcular la sumatoria de desviaciones al cuadrado:

$f(b_0,b_1) = \sum_{i=1}^n[y_i - (b_0 + b_1x_i)]^2$

$f(b_0,b_1) = \sum_{i=1}^n(y_i - b_0 - b_1x_i)^2$

Nuevamente, como se sabe que $\beta_0 = 0$, la función puede reducirse a:

$f(0,b_1) = \sum_{i=1}^n(y_i - b_1x_i)^2$

### Cálculo de derivadas parciales

$\dfrac {df(0,b_1)} {db_1} = \dfrac {d(\sum_{i=1}^n {(y_i - b_1x_i)}^2)} {db_1}$

$\dfrac {df(b_0,b_1)} {db_1} = -2 \sum _{i=1} ^n x_i(y_i-b_1x_i)$

A partir de esto, se buscará obtener un estimador puntual $\hat\beta_1$:

$\hat\beta_1 = -2 \sum _{i=1} ^n x_i(y_i-b_1x_i) = 0$

$\sum _{i=1} ^n x_i(y_i-b_1x_i) = 0$

$\sum _{i=1}^n (x_i.y_i) - \sum_{i=1}^n x_i.b_1.x_i = 0$

$\sum _{i=1}^n (x_i.y_i) = \sum_{i=1}^n x_i^2.b_1$

$\sum _{i=1}^n (x_i.y_i) = b_1 \sum_{i=1}^n x_i^2$

$\hat\beta_1 = \dfrac {\sum _{i=1}^n (x_i.y_i)} {b_1 \sum_{i=1}^n x_i^2}$

## b. $Y = \beta_1(ax+c) + \beta_0 + \epsilon$

A partir del modelo de regresión $Y = \beta_0 + \beta_1x + \epsilon$ se puede reformular $Y$:

$Y = \beta_1(ax) + \beta_1c + \beta_0 + \epsilon$

Donde la ordenada al origen está dada por $\beta_1c + \beta_0$.

### Cálculo de desviación vertical

$AlturaPunto - AlturaLinea = y_i -(\beta_1(ax_i) + \beta_1c + \beta_0)$

En este caso, la altura en un punto está dada por $y_i$, mientras que la altura de la línea está dada por $\beta_1(ax_i) + \beta_1c + \beta_0$.

$DV = y_i - (\beta_1ax_i + \beta_1c + \beta_0)$

### Cálculo de estimadores

A partir del cálculo de la desviación vertical puede definirse una función $f$ para calcular la sumatoria de desviaciones al cuadrado:

$f(b_0, b_1) = \sum _{i=1}^n { [y_i - (\beta_1ax_i + \beta_1c + \beta_0)] }^2$

A continuación se realizará el cálculo de las derivadas parciales:

$\dfrac {df(b_0,b_1)} {db_0} = \dfrac {d(\sum _{i=1}^n [y_i - (\beta_1ax_i + \beta_1c + \beta_0)]^2)} {db_0}$

$df(b_0, b_1) = -2 \sum_{i=1}^n (y_i - (b_1ax_i + b_1c + b_0))$

$\dfrac {df(b_0,b_1)} {db_1} = \dfrac {d(\sum _{i=1}^n [y_i - (\beta_1ax_i + \beta_1c + \beta_0)]^2)} {db_1}$

$\dfrac {df(b_0,b_1)} {db_1} = $ *// esta estaba complicada de resolver así que va a quedar acá*

### Estimador puntual $\hat\beta_0$

$\hat\beta_0 = -2\sum_{i=1}^n(y_i - (b_1ax_i + b_1c + b_0)) = 0$

$\sum_{i=1}^n(y_i - (b_1ax_i + b_1c + b_0)) = 0$

$\sum_{i=1}^n(y_i - b_1x_i - b_1c -b_0) = 0$

$\sum_{i=1}^ny_i - b_1\sum_{i=1}^nx_i - n.b_1.c - n.b_0 = 0$

$n.b_0 = \sum_{i=1}^ny_i - b_1\sum_{i=1}^nx_i - n.b_1.c$

$\hat\beta_0 = \dfrac {\sum_{i=1}^ny_i - b_1\sum_{i=1}^nx_i - n.b_1.c} {n}$

$\hat\beta_0 = \dfrac 1 n \sum_{i=1}^n y_i - \dfrac {b_1} n \sum_{i=1}^nx_i - b_1.c$