# 1. Determinar el dominio de las siguientes funciones

## a. $f(x,y) = \dfrac {1} {x^2+y^2}$

$Dom(f) = R^2 - {\{(0;0)\}}$

## b. $f(x,y,z) = x^2+2y^2-z^2$

$Dom(f) = R^3$

## c. $f(x,y) = \dfrac {x} {x^2+y^2-9}$

1. $Dom(f) = \{ (x,y) ∈ R^2 : (x^2+y^2-9) \neq 0 \}$
2. $Dom(f) = \{(x,y) ∈ R^2 : (x^2+y^2) \neq 9\}$

## d. $f(x,y) = \dfrac {y} {x^2+y^2+1}$

1. $Dom(f) = \{ (x,y) ∈ R^2 : (x^2+y^2+1) \neq 0 \}$
2. $Dom(f) = \{(x,y) ∈ R^2 :(x^2+y^2) \neq -1\}$

## e. $f(x,y,z) = \dfrac {x^2} {y^2-z^2}$

1. $Dom(f) = \{ (x,y,z) ∈ R^3 : (y^2 - z^2) \neq 0 \}$
2. $Dom(f) = \{ (x,y,z) ∈ R^3 : y^2 \neq z^2 \}$
3. $Dom(f) = \{ (x,y,z) ∈ R^3 : \sqrt {y^2} \neq \sqrt {z^2} \}$
4. $Dom(f) = \{ (x,y,z) ∈ R^3 : |y| \neq |z| \}$

## f. $f(x,y) = \sqrt {9-x^2-y^2}$

1. $Dom(f) = \{ (x,y) ∈ R^2 : (9-x^2-y^2) \ge 0\}$
2. $Dom(f) = \{ (x,y) ∈ R^2 : (-x^2-y^2) \ge (-9)\}$
3. $Dom(f) = \{ (x,y) ∈ R^2 : (-x^2-y^2)(-1) \ge (-9)(-1) \}$
4. $Dom(f) = \{ (x,y) ∈ R^2 : (x^2+y^2) \le 9\}$

*// cuando multiplicás ambos lados por -1 el símbolo cambia de < a > y viceversa.*

## g. $f(x,y) = e^{-x^2+y^2}$

$Dom(f) = R^3$

## h. $f(x,y) = log(16-x^2-16y^2)$

1. $Dom(f) = \{ (x,y) ∈ R^2 : (16-x^2-16y^2) \gt 0\}$
2. $Dom(f) = \{ (x,y) ∈ R^2 : (-x^2-16y^2) \gt -16\}$
3. $Dom(f) = \{ (x,y) ∈ R^2 : (-x^2-16y^2)(-1) \gt (-16)(-1)\}$
4. $Dom(f) = \{ (x,y) ∈ R^2 : (x^2+16y^2) \lt 16\}$


# 2. Evaluar las siguientes funciones en los puntos dados (cuando los puntos pertenezcan al dominio)

## a. $f(x,y) = log(9-x^2-9y^2)$

### En $(1,0)$


$f(1,0) = log(9-1^2-9(0^2))$

$f(1,0) = log(9-1-0)$

$f(1,0) = log(8)$

*// en qué base es el logaritmo? 🤔*

Suponiendo $log _{10}$ $f(1,0) = 0,90308998699$

Suponiendo $log_e$ $f(1,0) = 2,07944154168$

### En $(1,1)$

$f(1,1) = log(9-1^2-9(1^2))$

$f(1,1) = log(9-1-9)$

$f(1,1) = log(-1)$

El logaritmo de un número negativo es indefinido en $R$, por lo que el punto $(1,1) ∉ Dom(f)$.

### En $(0,1)$

$f(0,1) = log(9-0^2-9(1^2))$

$f(0,1) = log(9-9)$

$f(0,1) = log(0)$

El logaritmo de 0 es indefinido en $R$, por lo que el punto $(0,1) ∉ Dom(f)$.

### En $(-1,1)$

$f(-1,1) = log(9-(-1)^2-9.1^2)$

$f(-1,1) = log(9-1-9)$

$f(-1,1) = log(-1)$

El logaritmo de un número negativo es indefinido en $R$, por lo que el punto $(1,1) ∉ Dom(f)$.

## b. $f(x,y) = \sqrt {4-x^2-4y^2}$

### En $(1,0)$

$f(1,0) = \sqrt {4-1^2-4.0^2}$

$f(1,0) = \sqrt {4-1}$

$f(1,0) = \sqrt 3$

$f(1,0) = 1.7320508075689$

### En $(1,1)$

$f(1,1) = \sqrt {4-1^2-4.1^2}$

$f(1,1) = \sqrt {4-1-4}$

$f(1,1) = \sqrt {-1}$

La raíz de un número negativo no está definida en $R$, por lo tanto el punto $(1,1) ∉ Dom(f)$.

### En $(0,1)$

$f(0,1) = \sqrt {4-0^2-4.1^2}$

$f(0,1) = \sqrt {4-0-4}$

$f(0,1) = \sqrt {0}$

$f(0,1) = 0$

### En $(-1,1)$

$f(-1,1) = \sqrt {4-(-1)^2-4.1^2}$

$f(-1,1) = \sqrt {4-1-4}$

$f(-1,1) = \sqrt {-1}$

La raíz de un número negativo no está definida en $R$, por lo tanto el punto $(-1,1) ∉ Dom(f)$.

### En $(2,2)$

$f(2,2) = \sqrt {4-2^2-4.2^2}$

$f(2,2) = \sqrt {4-4-16}$

$f(2,2) = \sqrt {-16}$

La raíz de un número negativo no está definida en $R$, por lo tanto el punto $(2,2) ∉ Dom(f)$.

## c. $f(x,y) = e^{x^2+y^2}$

### En $(1,0)$

$f(1,0) = e^{1^2+0^2}$

$f(1,0) = e^{1}$

$f(1,0) = 2,71828182846$

### En $(1,1)$

$f(1,1) = e^{1^2+1^2}$

$f(1,1) = e^{2}$

$f(1,1) = 7,38905609893$

### En $(0,1)$

$f(1,1) = e^{0^2+1^2}$

$f(1,1) = e^{1}$

$f(1,1) = 2,71828182846$

### En $(-1,1)$

$f(-1,1) = e^{(-1)^2+1^2}$

$f(-1,1) = e^{2}$

$f(-1,1) = 7,38905609893$

# 3. Calcular los siguientes límites o demostrar que no existen

## a. $\lim _{(x,y) \to (3,1)} 5x-x^2+3y^2$

$Dom(f) = R^2$

$(3,1) ∈ Dom(f)$, por lo que su límite se puede evaluar directamente.

1. $\lim_{(x,y) \to (3,1)} 5.3-3^2+3.1^2$

2. $15-9+3 = 9$

Se demostró que el límite para el punto $(3,1)$ existe y su valor es $9$.

## b. $\lim _{(x,y) \to (0,0)} (\dfrac {(7x^2-2y^2)} {x^2+y^2} + 1)$

$Dom(f) = R^2 - \{(0,0)\}$

$(0,0) ∉ Dom(f)$, por lo que su límite no se puede evaluar directamente.

### Límites iterados

A partir de $x$:

1. $\lim _{x \to 0} (\lim _{y \to 0} (\dfrac {7x^2-2y^2} {x^2+y^2} + 1))$

2. $\lim _{x \to 0} (\dfrac {7x^2-2.0^2} {x^2+0^2} + 1)$

3. $\lim _{x \to 0} (\dfrac {7x^2} {x^2} + 1)$

4. $\lim _{x \to 0} (7+ 1)$

5. $\lim _{x \to 0} = 8$

A partir de $y$:

1. $\lim _{y \to 0} (\lim _{x \to 0} (\dfrac {7x^2-2y^2} {x^2+y^2} + 1))$

2. $\lim _{y \to 0} (\dfrac {7.0^2-2y^2} {0^2+y^2} + 1)$

3. $\lim _{y \to 0} (\dfrac {-2y^2} {y^2} + 1)$

4. $\lim _{y \to 0} (-2 + 1)$

5. $\lim _{y \to 0} = -1$

Al acercarse al punto $(0,0)$ por dos caminos distintos se descubrió que los valores son distintos, por lo tanto el límite de $f$ no existe en $(0,0)$.

## c. $\lim _{(x,y,z) \to (1,1,0)} e^{x+y^2-z}$

$Dom(f) = R^3$

$(1,1,0) ∈ Dom(f)$, por lo que su límite se puede evaluar directamente.

1. $\lim _{(x,y,z) \to (1,1,0)} e^{x+y^2-z}$

2. $e^{1+1^2-0}$

3. $e^2$

Se demostró que el límite para el punto $(1,1,0)$ existe y su valor es $e^2$ (*no lo voy a calcular 👽*).

## d. $\lim _{(x,y,z) \to (0,0,0)} \sin(x+y+z)$

$Dom(f) = R^3$

$(0,0,0) ∈ Dom(f)$, por lo que su límite se puede evaluar directamente.

1. $\lim _{(x,y,z) \to (0,0,0)} \sin(x+y+z)$

2. $\sin(0+0+0)$

3. $\sin(0) = 0$

Se demostró que el límite para el punto $(0,0,0)$ existe y su valor es $0$.

## e. $\lim_{(x,y) \to (0,0)} \dfrac {x^4}{x^4+y^4}$

$Dom(f) = R^2 - \{(0,0)\}$

$(0,0) ∉ Dom(f)$, por lo que su límite no se puede evaluar directamente.

### Evaluación algebráica

1. $\lim_{(x,y) \to (0,0)} \dfrac {x^4}{x^4+y^4} = \dfrac {\lim _{(x,y) \to (0,0)} x^4} {\lim _{(x,y) \to (0,0)} x^4 + y^4}$

2. $\dfrac {0^4} {0^4 + 0^4}$

3. $\lim _{(x,y) \to (0,0)} x^4 = L = 0$

3. $\lim _{(x,y) \to (0,0)} x^4 + y^4 = M = 0$

No puede utilizarse la propiedad de límites $L/M$ ya que el denominador es 0; por lo tanto, aún no es suficiente para demostrar la existencia o no del límite.

### Límites iterados

A partir de $x$:

1. $\lim _{x \to 0} (\lim _{y \to 0} \dfrac {x^4}{x^4+y^4})$

2. $\lim _{x \to 0} (\dfrac {x^4} {x^4 + 0^4})$

3. $\lim _{x \to 0} (\dfrac {x^4} {x^4})$

3. $\lim _{x \to 0} = 1$

A partir de $y$:

1. $\lim_{y \to 0} (\lim _{x \to 0} \dfrac {x^4} {x^4+y^4})$

2. $\lim_{y \to 0} (\dfrac {0^4} {0^4+y^4})$

3. $\lim_{y \to 0} (\dfrac {0} {y^4})$

3. $\lim_{y \to 0} = 0$

Al acercarse al punto $(0,0)$ por dos caminos distintos se descubrió que los valores son distintos, por lo tanto el límite de $f$ no existe en $(0,0)$.

## f. $\lim _{(x,y) \to (0,0)} \dfrac {xy} {\sqrt {x^2+y^2} }$

$Dom(f) = R^2 - \{ (0,0) \}$

$(0,0) ∉ Dom(f)$, por lo que su límite no se puede evaluar directamente.

### Evaluación algebráica

1. $\lim _{(x,y) \to (0,0)} \dfrac {xy} {\sqrt {x^2+y^2} } = \dfrac {\lim _{(x,y) \to (0,0)} xy} {\lim _{(x,y) \to (0,0)} \sqrt {x^2+y^2}}$

2. $\dfrac {0.0} {\sqrt {0+0}}$

3. $\lim _{(x,y) \to (0,0)} xy = L = 0$

4. $\lim _{(x,y) \to (0,0)} \sqrt {x^2+y^2} = M = 0$

No puede utilizarse la propiedad de límites $L/M$ ya que el denominador es 0; por lo tanto, aún no es suficiente para demostrar la existencia o no del límite.

Como ambos límites tienden a 0, se puede usar la correspondencia con las coordenadas polares $r \to 0$.

### Coordenadas polares

1. $\lim _{(x,y) \to (0,0)} \dfrac {xy} {\sqrt {x^2+y^2} } = \lim _{r \to 0} \dfrac {r.\cos(\theta).r.\sin(\theta)} {\sqrt {(r.\cos(\theta))^2 + (r.\sin(\theta)^2)}}$

2. $\lim _{r \to 0} \dfrac {r^2.\cos(\theta).\sin(\theta)} {\sqrt {r^2(\cos(\theta)^2 + r^2.\sin(\theta)^2)}}$

3. $\lim _{r \to 0} \dfrac {r^2.\cos(\theta).\sin(\theta)} {\sqrt {r^2(1) }}$ *// acá usé una propiedad que dice que $\cos(\theta)^2 + \sin(\theta)^2 = 0$*

4. $\lim _{r \to 0} \dfrac {r^2.\cos(\theta).\sin(\theta)} {\sqrt {r^2 }}$

5. $\lim _{r \to 0} \dfrac {r^2.\cos(\theta).\sin(\theta)} {|r|}$

6. $\lim _{r \to 0} r.\cos(\theta).\sin(\theta)$

7. $0.\cos(\theta).\sin(\theta)$

8. $0$

Se demostró que el límite en el punto $(0,0)$ existe y su valor es $0$.

## g. $\lim _{(x,y) \to (2,2)} \dfrac {x^2-2xy+y^2} {x-y}$

$Dom(f) = (x,y) ∈ R^2 : (x - y) \neq 0$

$Dom(f) = \{ (x,y) ∈ R^2 : x \neq y \}$

$(2,2) ∉ Dom(f)$, por lo que el límite no puede evaluarse directamente.

### Evaluación algebráica

1. $\lim _{(x,y) \to (2,2)} \dfrac {x^2-2xy+y^2} {x-y} = \dfrac {(x-y)^2} {x-y}$

2. $\lim _{(x,y) \to (2,2)} x-y$

3. $2-2 = 0$

Se demostró que el límite en el punto $(2,2)$ existe y su valor es $0$.

# 4. Estudiar la continuidad de las siguientes funciones. En caso de no estar definida en todo $R^2$, redefinirla de manera que pueda extenderse su continuidad.

## a.

* $f(x,y) = {\dfrac {x^3} {\sqrt {x^2+y^2}}}$ si $(x,y) \neq (0,0)$
* $f(x,y) = 1$ si $(x,y) = (0,0)$

$Dom(f) = R^2$.

El punto que cuestiona la continuidad de $f$ es $(0,0)$. Para esto se buscará encontrar el límite de $f$ en dicho punto, y que éste coincida con el valor exacto en la coordenada.

1. $\lim _{(x,y) \to (0,0)} {\dfrac {x^3} {\sqrt {x^2+y^2}}} = \lim _{r \to 0} \dfrac {(r.\cos(\theta))^3} {\sqrt {(r.\cos(\theta))+(r.\sin(\theta))}}$

2. $\lim _{r \to 0} \dfrac {r^3\cos(\theta)^3} {\sqrt {r^2.\cos(\theta)^2+r^2.\sin(\theta)^2}}$

3. $\lim _{r \to 0} \dfrac {r^3\cos(\theta)^3} {\sqrt {r^2(\cos(\theta)+\sin(\theta))}}$

4. $\lim _{r \to 0} \dfrac {r^3\cos(\theta)^3} {\sqrt {r^2.1}}$

5. $\lim _{r \to 0} \dfrac {r^3\cos(\theta)^3} {r}$

6. $\lim _{r \to 0} r^2\cos(\theta)^3$

7. $0.\cos(\theta)^3$

8. $0$

Se demostró que el límite en el punto $(0,0)$ existe y su valor es $0$.

Para que $f$ sea continua en $(0,0)$ debe cumplirse que $\lim _{(x,y) \to (0,0)} =f(0,0)$. Sin embargo, el valor de $f(0,0) = 1$, por lo tanto $f$ no es continua en ese punto.

Para resolver la discontinuidad debe reformularse $f$ tal que:
* $f(x,y) = {\dfrac {x^3} {\sqrt {x^2+y^2}}}$ si $(x,y) \neq (0,0)$
* $f(x,y) = 0$ si $(x,y) = (0,0)$

## b.

* $f(x,y) = {\dfrac {x} {\sqrt {x^2+y^2}}}$ si $(x,y) \neq (0,0)$
* $f(x,y) = 0$ si $(x,y) = (0,0)$

$Dom(f) = R^2$.

El punto que cuestiona la continuidad de $f$ es $(0,0)$. Para esto se buscará encontrar el límite de $f$ en dicho punto, y que éste coincida con el valor exacto en la coordenada.

1. $\lim _{(x,y) \to (0,0)} {\dfrac {x} {\sqrt {x^2+y^2}}} = \lim _{r \to 0} \dfrac {r.\cos(\theta)} { \sqrt {(r.\cos(\theta))^2+(r.\sin(\theta))^2} }$

2. $\lim _{r \to 0} {\dfrac {r.\cos(\theta)} { \sqrt {r^2.\cos(\theta)^2+r^2.\sin(\theta)^2} }}$

3. $\lim _{r \to 0} {\dfrac {r.\cos(\theta)} { \sqrt {r^2(\cos(\theta)^2+.\sin(\theta)^2)} }}$

4. $\lim _{r \to 0} {\dfrac {r.\cos(\theta)} { \sqrt {r^2(1)} }}$

5. $\lim _{r \to 0} \dfrac {r.\cos(\theta)} {r}$

6. $\lim _{r \to 0} \cos(\theta)$

7. $\cos(\theta)$

Al calcular el límite en el punto $(0,0)$ se llegó a un resultado en el cual su valor depende de $\theta$, por lo tanto el límite no existe.

Como el límite de $f(0,0)$ no existe, se dice que $f$ no es continua en ese punto y no puede redefinirse.

## c.

* $f(x,y) = {\dfrac {x^2} {\sqrt {x^2+y^2}}}$ si $(x,y) \neq (0,0)$
* $f(x,y) = 0$ si $(x,y) = (0,0)$

$Dom(f) = R^2$

El punto que cuestiona la continuidad de $f$ es $(0,0)$. Para esto se buscará encontrar el límite de $f$ en dicho punto, y que éste coincida con el valor exacto en la coordenada.

1. $\lim _{(x,y) \to (0,0)} {\dfrac {x^2} {\sqrt {x^2+y^2}}} = \lim _{r \to 0} \dfrac {(r.\cos(\theta))^2} {\sqrt {(r.\cos(\theta))^2 + (r.\sin(\theta))^2}}$

2. $\lim _{r \to 0} \dfrac {(r.\cos(\theta))^2} {\sqrt {r^2.\cos(\theta)^2 + r^2.\sin(\theta)^2} }$

3. $\lim _{r \to 0} \dfrac {r^2.\cos(\theta)^2} {\sqrt {r^2(\cos(\theta)^2 + \sin(\theta)^2)} }$

4. $\lim _{r \to 0} \dfrac {r^2.\cos(\theta)^2} {\sqrt {r^2(1)} }$

5. $\lim _{r \to 0} \dfrac {r^2.\cos(\theta)^2} {r}$

6. $\lim _{r \to 0} r.\cos(\theta)^2$

7. $0.\cos(\theta)^2$

8. $0$

Se demostró que el límite en el punto $(0,0)$ existe y su valor es $0$.

Para que $f$ sea continua en $(0,0)$ debe cumplirse que $\lim _{(x,y) \to (0,0)} =f(0,0)$. En este caso, tanto el límite como el valor exacto en el punto son $0$, por lo que $f$ es continua en $(0,0)$.

## d.

$f(x,y) = \dfrac {xy} {x^2+y^2}$

$Dom(f) = R^2 -\{ (0,0) \}$

Como $(0,0)$ está fuera de $Dom(f)$, la función no es continua para todo $R^2$. A pesar de esto, se calculará su límite en dicho punto para ver si puede redefinirse $f$ de manera que sea continua para todo $R^2$.

1. $\lim _{(x,y) \to (0,0)} \dfrac {xy} {x^2+y^2} = \lim _{r \to 0} \dfrac {r.\cos(\theta).r.\sin(\theta)} {(r.\cos(\theta))^2+(r.\sin(\theta))^2}$

2. $\lim _{r \to 0} \dfrac {r^2.\cos(\theta).\sin(\theta)} {r^2.\cos(\theta)^2+r^2.\sin(\theta)^2}$

3. $\lim _{r \to 0} \dfrac {r^2.\cos(\theta).\sin(\theta)} {r^2(\cos(\theta)^2+\sin(\theta)^2)}$

4. $\lim _{r \to 0} \dfrac {r^2.\cos(\theta).\sin(\theta)} {r^2.1}$

4. $\lim _{r \to 0} \cos(\theta).\sin(\theta)$

4. $\cos(\theta).\sin(\theta)$

Al calcular el límite en $(0,0)$, se llegó a un resultado que depende totalmente del valor de $\theta$, por lo tanto el límite no existe y $f$ no puede redefinirse para ser continua en dicho punto.

## e.

$f(x,y) = \dfrac {xy^2} {x^2+y^2}$

$Dom(f) = R^2 -\{ (0,0) \}$

Como $(0,0)$ está fuera de $Dom(f)$, la función no es continua para todo $R^2$. A pesar de esto, se calculará su límite en dicho punto para ver si puede redefinirse $f$ de manera que sea continua para todo $R^2$.

1. $\lim _{(x,y) \to (0,0)} \dfrac {xy^2} {x^2+y^2} = \lim _{r \to 0} \dfrac {r.\cos(\theta)(r.\sin(\theta))^2} {(r.\cos(\theta))^2+(r.\sin(\theta))^2}$

2. $\lim _{r \to 0} \dfrac {r.\cos(\theta).r^2.\sin(\theta)^2} {r^2.\cos(\theta)^2+r^2.\sin(\theta)^2}$

3. $\lim _{r \to 0} \dfrac {r^3.\cos(\theta).\sin(\theta)^2} {r^2(\cos(\theta)^2+\sin(\theta)^2)}$

4. $\lim _{r \to 0} \dfrac {r^3.\cos(\theta).\sin(\theta)^2} {r^2(1)}$

5. $\lim _{r \to 0} r.\cos(\theta).\sin(\theta)^2$

6. $0.\cos(\theta).\sin(\theta)^2$

7. $0$

Se encontró que el límite de $f(0,0)$ existe y su valor es $0$. Por lo tanto, $f$ puede redefinirse para que sea continua en todo $R^2$ de la siguiente manera:

* $f(x,y) = {\dfrac {xy^2} {x^2+y^2}}$ si $(x,y) \neq (0,0)$
* $f(x,y) = 0$ si $(x,y) = (0,0)$