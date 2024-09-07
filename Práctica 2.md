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

# 2.  Una cadena de supermercados financia un estudio sobre los gastos mensuales en alimentos, de familias de 4 miembros. La investigación se limitó a familias con ingresos netos entre \$688.000 y \$820.000, con lo cual se obtuvo la siguiente recta de estimación $\hat y = 0,85𝑥 − 18.000$.

## a. Estime los gastos en alimentos en un mes para una familia de 4 miembros con un ingreso de $700.000

* $y =$ gastos.
* $x =$ ingresos.

La recta dada para realizar la estimación de los gastos es $\hat y = 0.85x - 18000$.

Como en este caso se sabe que $x = 700000$, puede calcularse la estimación simplemente reemplazando dicha variable:

$\hat y = 0.85(700000) - 18000$

$\hat y = 595000 - 18000 = 577000$

## b. Uno de los directivos de la compañía se preocupa por el hecho de que la ecuación aparentemente indica que para una familia que tiene un ingreso de $12.000 no gastaría nada en alimentos ¿Cuál sería su respuesta?

Nuevamente, se sabe que $x = 12000$, por lo que puede obtenerse una estimación de los gastos alimenticios de la familia:

$\hat y = 0.85(12000) - 18000$

$\hat y = 10200 - 18000 = -7800$

Mi respuesta para el directivo sería que lamentablemente una familia con ese ingreso tendría que endeudarse para comer. Sin embargo, sabiendo que el análisis se realizó a partir de familias con ingresos entre \$688.000 - \$820.000, no sería coherente utilizar la misma estimación para una familia con un salario fuera de dicho rango, especialmente ya que se trata de un valor significativamente menor.