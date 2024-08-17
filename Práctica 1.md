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

## $f(x,y) = e^{x^2+y^2}$

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

