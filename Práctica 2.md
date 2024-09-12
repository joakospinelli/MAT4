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

# 3. ?????????????????????????

# 4. Los siguientes datos corresponden a los tiempos relativos en segundos que tardaron en ejecutarse seis programas elegidos al azar en el entorno Windows y DOS:


| Windows | 2.5 | 7.1 | 5 | 8.5 | 7 | 8.1 |
| ------- | --- | --- | - | --- | - | --- |
|   DOS   | 2.3 | 7.1 | 4 | 8 | 6.6 | 5   |

## a. Realizar el gráfico de dispersión de los puntos

$x$: tiempo de ejecución en Windows.

$y$: tiempo de ejecución en DOS.

$n = 6$

```py
import matplotlib.pyplot as pyplot

x = [ 2.5, 7.1, 5, 8.5, 7, 8.1 ]
y = [ 2.3, 7.1, 4, 8, 6.6, 5 ]

pyplot.scatter(x, y)
pyplot.xlabel('Tiempo en Windows')
pyplot.ylabel('Tiempo en DOS')

pyplot.show()
```

## b. Si un programa tarda 6 segundos en ejecutarse en Windows, ¿cuánto tardará en ejecutarse en DOS?

### Cálculos previos

$\sum _{i=1}^n x_i = 38.2$

$\sum _{i=1}^n x_i^2 = 268.52$

$\overline x = 6.36$

$\sum_{i=1}^n y_i = 33$

$\overline y = 5.5$

$\sum _{i=1}^n x_iy_i = 230.86$

### Recta de ajuste

Para obtener el valor de $y$ para un valor determinado de $x$, se buscará obtener un estimador $\hat y$ usando el método de mínimos cuadrados.

Partiendo de la línea de regresión estimada $\hat y = \hat\beta_0 + \hat\beta_1 x$:

$\hat\beta_1 = \dfrac {\sum(x_i - \overline x)(y_i - \overline y)} {\sum (x_i - \overline x)^2} = \dfrac {S_{xy}} {S_{xx}}$

$S_{xy} = \sum _{i=1}^n x_iy_i - \dfrac {\sum {x_i} \sum {y_i}} {n}$

$S_{xy} = 230.86 - \dfrac {38.2 * 33} {6}$

$S_{xy} = 230.86 - \dfrac {1260.6} {6} = 20.76$

$S_{xx} = \sum_{i=1}^n x_i^2 - \dfrac {(\sum x_i)^2} {n}$

$S_{xx} = 268.52 - \dfrac {38.2^2} 6$

$S_{xx} = 268.52 - \dfrac {1459.24} 6 = 25.31$

$\hat\beta_1 = \dfrac {20.76} {25.31} = 0.8202$

$\hat\beta_0 = \overline y - \hat\beta_1 \overline x$

$\hat\beta_0 = 5.5 - 0.8202 * 6.36 = 0.283528$

Volviendo a la recta $\hat y = \hat\beta_0 + \hat\beta_1 x$:

$\hat y = 0.283528 + 0.8202*x$

```py
import matplotlib.pyplot as pyplot

x = [ 2.5, 7.1, 5, 8.5, 7, 8.1 ]
y = [ 2.3, 7.1, 4, 8, 6.6, 5 ]

pyplot.scatter(x, y)
pyplot.xlabel("Tiempo en Windows")
pyplot.ylabel("Tiempo en DOS")

x_recta = [i for i in range(0, 10)]
y_recta = [0.283528 + 0.8202*x for x in x_recta]

pyplot.plot(x_recta, y_recta, label="Recta de ajuste", color="red")

pyplot.show()
```

### Resolución del enunciado

A partir del estimador de $\hat y$ podemos deducir que cuando un programa tarde 6 segundos en Windows ($x = 6$), en DOS tardará:

$0.283528 + 0.8202*6 = 5.204$ segundos.

## c. Se estima que los tiempos de Windows mejorarán reduciéndose en un %10 en los próximos años, estime la recta de regresión considerando esta mejora. Suponga que los tiempos de DOS no se modifican.

Considerando la mejora, los valores de ejecución en Windows pasarían a ser el %90 de lo que eran antes.

### Cálculos previos

$\sum _{i=1}^n x_i = 34.38$

$\sum _{i=1}^n x_i^2 = 217.5012$

$\overline x = 5.73$

$\sum_{i=1}^n y_i = 33$

$\overline y = 5.5$

$\sum _{i=1}^n x_iy_i = 207.7773$

### Recta de ajuste

Partiendo de la línea de regresión estimada $\hat y = \hat\beta_0 + \hat\beta_1 x$:

$\hat\beta_1 = \dfrac {\sum(x_i - \overline x)(y_i - \overline y)} {\sum (x_i - \overline x)^2} = \dfrac {S_{xy}} {S_{xx}}$

$S_{xy} = \sum _{i=1}^n x_iy_i - \dfrac {\sum {x_i} \sum {y_i}} {n}$

$S_{xy} = 207.7773 - \dfrac {34.38 * 33} {6}$

$S_{xy} = 207.7773 - \dfrac {1134.54} {6} = 18.6873$

$S_{xx} = \sum_{i=1}^n x_i^2 - \dfrac {(\sum x_i)^2} {n}$

$S_{xx} = 217.5012 - \dfrac {34.38^2} 6$

$S_{xx} = 217.5012 - \dfrac {1181.98} 6 = 20.5038$

$\hat\beta_1 = \dfrac {18.6873} {20.5038} = 0.9114$

$\hat\beta_0 = \overline y - \hat\beta_1 \overline x$

$\hat\beta_0 = 5.5 - 0.9114 * 5.73 = 0.27763$

### Resolución del enunciado

Volviendo a la recta $\hat y = \hat\beta_0 + \hat\beta_1 x$, asumiendo la mejora del 10% esta pasaría a ser:

$\hat y = 0.27763 + 0.9114*x$

*// es la manera más correcta calcular todos los estimadores de nuevo?*

# 5. En la tabla siguiente se muestra la variable $y$ (el rendimiento de un sistema informático) respecto a la variable $x$ (número de buffers). Se quiere asjutar la variable $y$ como función de $x$:

| $x$ | 5 | 10 | 15 | 20 | 25 | 5 | 10 | 15 | 20 | 25 | 5 | 10 | 15 | 20 | 25 |
| --- | - | -- | -- | -- | -- | - | -- | -- | -- | -- | - | -- | -- | -- | -- |
| $y$ | 9.6 | 20.1 | 29.9 | 39.1 | 50.0 | 9.6 | 19.4 | 29.7 | 40.3 | 49.9 | 10.7 | 21.3 | 30.7 | 41.8 | 51.2 |

## a. Realizar el análisis de regresión de datos (estimación de recta, test de hipótesis, indicadores).

$n = 15$

$x =$ cantidad de buffers.

$y =$ rendimiento de un sistema informático.

*// no termino de entender a qué se refiere con "rendimiento". es tiempo de ejecución? uso de memoria? de cpu?*

### Estimación de la recta

$\hat y = \hat\beta_0 + \hat\beta_1 x$

$\hat\beta_1 = \dfrac {S_{xy}} {S_{xx}}$

$S_{xy} = \sum_{i=1}^n x_iy_i - \dfrac {\sum x_i \sum y_i} n$

$S_{xy} = 8313.5 - \dfrac {225*453.3} {15}$

$S_{xy} = 8313.5 - 6799.5 = 1514$

$S_{xx} = \sum_{i=1}^n x_i^2 - \dfrac {(\sum x_i)^2} n$

$S_{xx} = 4125 - \dfrac {225^2} {15}$

$S_{xx} = 4125 - 3375 = 750$

$\hat\beta_1 = \dfrac {1514} {750} = 2.0186$

$\hat\beta_0 = \overline y - \hat\beta_1 \overline x$

$\hat\beta_0 = 30.219 - 2.0186 * 15 = -0.06$

$\hat y = -0.06 + 2.0186*x$

*// no le tenía nada de fe pero la recta quedó bastante bien*

```py
import matplotlib.pyplot as pyplot

x = [ 5, 10, 15, 20, 25, 5, 10, 15, 20, 25, 5, 10, 15, 20, 25 ]
y = [ 9.6, 20.1, 29.9, 39.1, 50.0, 9.6, 19.4, 29.7, 40.3, 49.9, 10.7, 21.3, 30.7, 41.8, 51.2 ]

x_recta = [i for i in range(0,30)]
y_recta = [-0.06 + 2.0186*el for el in x_recta]

pyplot.scatter(x, y)
pyplot.xlabel("Cantidad de buffers")
pyplot.ylabel("Rendimiento del SI")

pyplot.plot(x_recta, y_recta, label="Recta de ajuste", color="red")

pyplot.show()
```

*// no entiendo cómo tendría que hacer los test de hipótesis 👽 cuál sería la constante para hacer las hipótesis?*

## b. Comentar los siguientes resultados:

### Recta de regresión del rendimiento del SI frente al número de buffers e interpretación de los coeficientes.

La recta de regresión $\hat y = -0.06 + 2.0186*x$ está muy buena porque tiene muy poca variación. Esto puede calcularse con el estimador de variabilidad:

$\hat\sigma^2 = \dfrac {SCE} {n-2}$

$SCE = S_{yy} - \dfrac {(S_{xy})^2} {S_{xx}}$ 

$SCE = 3064.324 - \dfrac {(1514^2)} {750}$

$\hat\sigma^2 = \dfrac {8.0626} {13}$

$\hat\sigma^2 = 0.6202$

### Contraste de hipótesis sobre la pendiente de la pendiente de la recta.

*// ni hice hipótesis je*

### Coeficiente de determinación y correlación lineal.

$R^2 = 1 - \dfrac {SCE} {STC}$

$STC = S_{yy} = 3064.324$

$R^2 = 1 - \dfrac {8.0626} {3064.324}$

$R^2 = 1 - 0.00263$

$R^2 = 0.99736$

El coeficiente de determinación es muy cercano a 1, por lo que es muy preciso para explicar la variación de la variable $y$.

$r = \sqrt {R^2}$

$r = \sqrt {0.99736} =  \pm 0.99868$

$\hat\beta_1$ es un valor positivo, por lo que $r = 0.99868$. Esto implica que hay una relación directa entre $x$ e $y$, en la que $y$ aumenta con el valor de $x$.