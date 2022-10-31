Tarea de Probabilidades y Estadística: Distribuciones
================
Marcelo J. Molinatti
2022-10-31



# 1 Problemas y Simulaciones.

1.  *(Problema 273)* Sea
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X") una variable aleatoria con distribución uniforme en el conjunto
    ![{1, \\ldots ,
    n}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%7B1%2C%20%5Cldots%20%2C%20n%7D
    "{1, \\ldots , n}") y sean
    ![x](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;x
    "x"),
    ![x\_1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;x_1
    "x_1"), y
    ![x\_2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;x_2
    "x_2") números dentro de este conjunto en donde ![x\_1 \<
    x\_2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;x_1%20%3C%20x_2
    "x_1 \< x_2"). Encuentre las siguientes probabilidades:

<!-- end list -->

  - ![P(X \\le
    x)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%5Cle%20x%29
    "P(X \\le x)")
  - ![P(X \\ge
    x)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%5Cge%20x%29
    "P(X \\ge x)")
  - ![P(x\_1 \\le X \\le
    x\_2)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28x_1%20%5Cle%20X%20%5Cle%20x_2%29
    "P(x_1 \\le X \\le x_2)")
  - ![P(x\_1 \< X \\le
    x\_2)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28x_1%20%3C%20X%20%5Cle%20x_2%29
    "P(x_1 \< X \\le x_2)")
  - ![P(x\_1 \\le X \<
    x\_2)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28x_1%20%5Cle%20X%20%3C%20x_2%29
    "P(x_1 \\le X \< x_2)")
  - ![P(x\_1 \< X \<
    x\_2)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28x_1%20%3C%20X%20%3C%20x_2%29
    "P(x_1 \< X \< x_2)")

Se tiene que la función de probabilidad es ![f(x)
= 1/n](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;f%28x%29%20%3D%201%2Fn
"f(x) = 1/n") por ser una distibución uniforme. Para la primera
probabilidad solo se calcula la funcion de distribucion acumulada para
valores menores que
![x](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;x
"x"):

  
![P(X \\le x) = \\sum\_{i=1}^x f(x) = \\sum\_{i=1}^x \\frac{1}{n} =
\\frac{1}{n}\\sum\_{i=1}^x1 =
\\frac{x}{n}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%5Cle%20x%29%20%3D%20%5Csum_%7Bi%3D1%7D%5Ex%20f%28x%29%20%3D%20%5Csum_%7Bi%3D1%7D%5Ex%20%5Cfrac%7B1%7D%7Bn%7D%20%3D%20%5Cfrac%7B1%7D%7Bn%7D%5Csum_%7Bi%3D1%7D%5Ex1%20%3D%20%5Cfrac%7Bx%7D%7Bn%7D
"P(X \\le x) = \\sum_{i=1}^x f(x) = \\sum_{i=1}^x \\frac{1}{n} = \\frac{1}{n}\\sum_{i=1}^x1 = \\frac{x}{n}")  

Para la siguiente probabilidad:

  
![P(X\\ge x) = 1-P(X \< x) = 1-\\sum\_{i=1}^{x - 1}f(x)
= 1-\\frac{1}{n}\\sum\_{i=1}^{x-1}1
= 1-\\frac{x-1}{n}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%5Cge%20x%29%20%3D%201-P%28X%20%3C%20x%29%20%3D%201-%5Csum_%7Bi%3D1%7D%5E%7Bx%20-%201%7Df%28x%29%20%3D%201-%5Cfrac%7B1%7D%7Bn%7D%5Csum_%7Bi%3D1%7D%5E%7Bx-1%7D1%20%3D%201-%5Cfrac%7Bx-1%7D%7Bn%7D
"P(X\\ge x) = 1-P(X \< x) = 1-\\sum_{i=1}^{x - 1}f(x) = 1-\\frac{1}{n}\\sum_{i=1}^{x-1}1 = 1-\\frac{x-1}{n}")  

Para las siguientes probabilidades:

  
![P(x\_1 \\le X \\le x\_2) = P(X \\le x\_2) - P(X \\le x\_1) =
\\frac{x\_2}{n} - \\frac{x\_1}{n} = \\frac{x\_2 -
x\_1}{n}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28x_1%20%5Cle%20X%20%5Cle%20x_2%29%20%3D%20P%28X%20%5Cle%20x_2%29%20-%20P%28X%20%5Cle%20x_1%29%20%3D%20%5Cfrac%7Bx_2%7D%7Bn%7D%20-%20%5Cfrac%7Bx_1%7D%7Bn%7D%20%3D%20%5Cfrac%7Bx_2%20-%20x_1%7D%7Bn%7D
"P(x_1 \\le X \\le x_2) = P(X \\le x_2) - P(X \\le x_1) = \\frac{x_2}{n} - \\frac{x_1}{n} = \\frac{x_2 - x_1}{n}")  

  
![P(x\_1 \< X \\le x\_2) = P(X \\le x\_2) - P(X \< x\_1) =
\\frac{x\_2}{n} - \\frac{x\_1 - 1}{n} = \\frac{x\_2 - x\_1
+ 1}{n}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28x_1%20%3C%20X%20%5Cle%20x_2%29%20%3D%20P%28X%20%5Cle%20x_2%29%20-%20P%28X%20%3C%20x_1%29%20%3D%20%5Cfrac%7Bx_2%7D%7Bn%7D%20-%20%5Cfrac%7Bx_1%20-%201%7D%7Bn%7D%20%3D%20%5Cfrac%7Bx_2%20-%20x_1%20%2B%201%7D%7Bn%7D
"P(x_1 \< X \\le x_2) = P(X \\le x_2) - P(X \< x_1) = \\frac{x_2}{n} - \\frac{x_1 - 1}{n} = \\frac{x_2 - x_1 + 1}{n}")  

  
![P(x\_1 \\le X \< x\_2) = P(X \< x\_2) - P(X \\le x\_1) = \\frac{x\_2
- 1}{n} - \\frac{x\_1}{n} = \\frac{x\_2 - x\_1
- 1}{n}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28x_1%20%5Cle%20X%20%3C%20x_2%29%20%3D%20P%28X%20%3C%20x_2%29%20-%20P%28X%20%5Cle%20x_1%29%20%3D%20%5Cfrac%7Bx_2%20-%201%7D%7Bn%7D%20-%20%5Cfrac%7Bx_1%7D%7Bn%7D%20%3D%20%5Cfrac%7Bx_2%20-%20x_1%20-%201%7D%7Bn%7D
"P(x_1 \\le X \< x_2) = P(X \< x_2) - P(X \\le x_1) = \\frac{x_2 - 1}{n} - \\frac{x_1}{n} = \\frac{x_2 - x_1 - 1}{n}")  

  
![P(x\_1 \< X \< x\_2) = P(X \< x\_2) - P(X \< x\_1) = \\frac{x\_2
- 1}{n} - \\frac{x\_1 - 1}{n} = \\frac{x\_2 -
x\_1}{n}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28x_1%20%3C%20X%20%3C%20x_2%29%20%3D%20P%28X%20%3C%20x_2%29%20-%20P%28X%20%3C%20x_1%29%20%3D%20%5Cfrac%7Bx_2%20-%201%7D%7Bn%7D%20-%20%5Cfrac%7Bx_1%20-%201%7D%7Bn%7D%20%3D%20%5Cfrac%7Bx_2%20-%20x_1%7D%7Bn%7D
"P(x_1 \< X \< x_2) = P(X \< x_2) - P(X \< x_1) = \\frac{x_2 - 1}{n} - \\frac{x_1 - 1}{n} = \\frac{x_2 - x_1}{n}")  

2.  *(Problema 274)* Sea
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X") una variable aleatoria con distribución uniforme en el conjunto
    ![\\{-1, 0, 1\\}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5C%7B-1%2C%200%2C%201%5C%7D
    "\\{-1, 0, 1\\}"). Demuestre que las variables aleatorias
    ![X^3](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%5E3
    "X^3") y
    ![-X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;-X
    "-X") tienen la misma distribución que
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X").

Las variables aleatorias
![X^3](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%5E3
"X^3") y
![-X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;-X
"-X") toman los mismos valores que
![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
"X"), es decir, su valores estan contenidos en el conjunto
![\\{-1, 0, 1\\}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5C%7B-1%2C%200%2C%201%5C%7D
"\\{-1, 0, 1\\}") de forma que, para
![X^3](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%5E3
"X^3"):

  
![
\\begin{aligned} 
P(Y = 0) &= P(X^3 = 0) = P(X = 0) = 1/3 \\\\ 
P(Y = 1) &= P(X^3 = 1) = P(X = \\sqrt\[3\]{1}) = P(X = 1) = 1/3 \\\\
P(Y = -1) &= P(X^3 = -1) = P(X = \\sqrt\[3\]{-1}) = P(X = -1) = 1/3 
\\end{aligned}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Baligned%7D%20%0A%20%20%20%20P%28Y%20%3D%200%29%20%26%3D%20P%28X%5E3%20%3D%200%29%20%3D%20P%28X%20%3D%200%29%20%3D%201%2F3%20%5C%5C%20%0A%20%20%20%20P%28Y%20%3D%201%29%20%26%3D%20P%28X%5E3%20%3D%201%29%20%3D%20P%28X%20%3D%20%5Csqrt%5B3%5D%7B1%7D%29%20%3D%20P%28X%20%3D%201%29%20%3D%201%2F3%20%5C%5C%0A%20%20%20%20P%28Y%20%3D%20-1%29%20%26%3D%20P%28X%5E3%20%3D%20-1%29%20%3D%20P%28X%20%3D%20%5Csqrt%5B3%5D%7B-1%7D%29%20%3D%20P%28X%20%3D%20-1%29%20%3D%201%2F3%20%0A%5Cend%7Baligned%7D%0A
"
\\begin{aligned} 
    P(Y = 0) &= P(X^3 = 0) = P(X = 0) = 1/3 \\\\ 
    P(Y = 1) &= P(X^3 = 1) = P(X = \\sqrt[3]{1}) = P(X = 1) = 1/3 \\\\
    P(Y = -1) &= P(X^3 = -1) = P(X = \\sqrt[3]{-1}) = P(X = -1) = 1/3 
\\end{aligned}
")  

y para
![-X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;-X
"-X"):

  
![
\\begin{align\*} 
P(Y = 0) &= P(-X = 0) = P(X = 0) = 1/3 \\\\ 
P(Y = 1) &= P(-X = 1) = P(X = -1) = 1/3 \\\\
P(Y = -1) &= P(-X = -1) = P(X = 1) = 1/3 
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%20%0A%20%20%20%20P%28Y%20%3D%200%29%20%26%3D%20P%28-X%20%3D%200%29%20%3D%20P%28X%20%3D%200%29%20%3D%201%2F3%20%5C%5C%20%0A%20%20%20%20P%28Y%20%3D%201%29%20%26%3D%20P%28-X%20%3D%201%29%20%3D%20P%28X%20%3D%20-1%29%20%3D%201%2F3%20%5C%5C%0A%20%20%20%20P%28Y%20%3D%20-1%29%20%26%3D%20P%28-X%20%3D%20-1%29%20%3D%20P%28X%20%3D%201%29%20%3D%201%2F3%20%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*} 
    P(Y = 0) &= P(-X = 0) = P(X = 0) = 1/3 \\\\ 
    P(Y = 1) &= P(-X = 1) = P(X = -1) = 1/3 \\\\
    P(Y = -1) &= P(-X = -1) = P(X = 1) = 1/3 
\\end{align*}
")  

y se demuestra que las distribuciones son las mismas.

3.  *(Problema 275)* Sea
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X") una variable aleatoria con distribución uniforme en el conjunto
    ![\\{1, \\ldots ,
    n\\}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5C%7B1%2C%20%5Cldots%20%2C%20n%5C%7D
    "\\{1, \\ldots , n\\}"). Demuestre que:

<!-- end list -->

  - ![E(X) = (n + 1)
    / 2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;E%28X%29%20%3D%20%28n%20%2B%201%29%20%2F%202
    "E(X) = (n + 1) / 2")
  - ![E(X^2) = (n + 1)(2n + 1)
    / 6](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;E%28X%5E2%29%20%3D%20%28n%20%2B%201%29%282n%20%2B%201%29%20%2F%206
    "E(X^2) = (n + 1)(2n + 1) / 6")
  - ![Var(X) = (n^2 - 1)
    / 12](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Var%28X%29%20%3D%20%28n%5E2%20-%201%29%20%2F%2012
    "Var(X) = (n^2 - 1) / 12")

Para la esperanza de
![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
"X") se tiene:

  
![E(X) = \\sum\_{x=1}^n xf(x) = \\sum\_{x=1}^n x\\frac{1}{n} =
\\frac{1}{n}\\times(1 + 2 + 3 + \\ldots + n) =
\\frac{1}{n}\\frac{n(n+1)}{2} = \\frac{n
+ 1}{2}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;E%28X%29%20%3D%20%5Csum_%7Bx%3D1%7D%5En%20xf%28x%29%20%3D%20%5Csum_%7Bx%3D1%7D%5En%20x%5Cfrac%7B1%7D%7Bn%7D%20%3D%20%5Cfrac%7B1%7D%7Bn%7D%5Ctimes%281%20%2B%202%20%2B%203%20%2B%20%5Cldots%20%2B%20n%29%20%3D%20%5Cfrac%7B1%7D%7Bn%7D%5Cfrac%7Bn%28n%2B1%29%7D%7B2%7D%20%3D%20%5Cfrac%7Bn%20%2B%201%7D%7B2%7D
"E(X) = \\sum_{x=1}^n xf(x) = \\sum_{x=1}^n x\\frac{1}{n} = \\frac{1}{n}\\times(1 + 2 + 3 + \\ldots + n) = \\frac{1}{n}\\frac{n(n+1)}{2} = \\frac{n + 1}{2}")  

Para la esperanza de
![X^2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%5E2
"X^2") se tiene:

  
![E(X^2) = \\sum\_{x=1}^n x^2\\frac{1}{n} = \\frac{1}{n}\\times(1 + 4
+ 9 + 16 + \\ldots + n^2) = \\frac{1}{n}\\frac{n(n+1)(2n + 1)}{6} =
\\frac{(n + 1)(2n
+ 1)}{6}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;E%28X%5E2%29%20%3D%20%5Csum_%7Bx%3D1%7D%5En%20x%5E2%5Cfrac%7B1%7D%7Bn%7D%20%3D%20%5Cfrac%7B1%7D%7Bn%7D%5Ctimes%281%20%2B%204%20%2B%209%20%2B%2016%20%2B%20%5Cldots%20%2B%20n%5E2%29%20%3D%20%5Cfrac%7B1%7D%7Bn%7D%5Cfrac%7Bn%28n%2B1%29%282n%20%2B%201%29%7D%7B6%7D%20%3D%20%5Cfrac%7B%28n%20%2B%201%29%282n%20%2B%201%29%7D%7B6%7D
"E(X^2) = \\sum_{x=1}^n x^2\\frac{1}{n} = \\frac{1}{n}\\times(1 + 4 + 9 + 16 + \\ldots + n^2) = \\frac{1}{n}\\frac{n(n+1)(2n + 1)}{6} = \\frac{(n + 1)(2n + 1)}{6}")  

Oara la varianza se usa la ecuación ![Var(X) = E(X^2) -
(E(X))^2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Var%28X%29%20%3D%20E%28X%5E2%29%20-%20%28E%28X%29%29%5E2
"Var(X) = E(X^2) - (E(X))^2") por lo que:

  
![
\\begin{align\*} 
Var(X) &= \\frac{(n + 1)(2n + 1)}{6} - \\left(\\frac{n + 1}{2}\\right)^2
\\\\ 
&= \\frac{(n + 1)(2n + 1)}{6} - \\frac{(n+1)^2}{4} \\\\
&= \\frac{4(n + 1)(2n + 1) - 6(n^2 + 2n + 1)}{24} \\\\
&= \\frac{8n^2 + 12n + 4 - 6n^2 - 12n - 6}{24} \\\\
&= \\frac{2n^2 - 2}{24} \\\\
&= \\frac{n^2 - 1}{12}
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%20%0A%20%20%20%20Var%28X%29%20%26%3D%20%5Cfrac%7B%28n%20%2B%201%29%282n%20%2B%201%29%7D%7B6%7D%20-%20%5Cleft%28%5Cfrac%7Bn%20%2B%201%7D%7B2%7D%5Cright%29%5E2%20%5C%5C%20%0A%20%20%20%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7B%28n%20%2B%201%29%282n%20%2B%201%29%7D%7B6%7D%20-%20%5Cfrac%7B%28n%2B1%29%5E2%7D%7B4%7D%20%5C%5C%0A%20%20%20%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7B4%28n%20%2B%201%29%282n%20%2B%201%29%20-%206%28n%5E2%20%2B%202n%20%2B%201%29%7D%7B24%7D%20%5C%5C%0A%20%20%20%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7B8n%5E2%20%2B%2012n%20%2B%204%20-%206n%5E2%20-%2012n%20-%206%7D%7B24%7D%20%5C%5C%0A%20%20%20%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7B2n%5E2%20-%202%7D%7B24%7D%20%5C%5C%0A%20%20%20%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7Bn%5E2%20-%201%7D%7B12%7D%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*} 
    Var(X) &= \\frac{(n + 1)(2n + 1)}{6} - \\left(\\frac{n + 1}{2}\\right)^2 \\\\ 
           &= \\frac{(n + 1)(2n + 1)}{6} - \\frac{(n+1)^2}{4} \\\\
           &= \\frac{4(n + 1)(2n + 1) - 6(n^2 + 2n + 1)}{24} \\\\
           &= \\frac{8n^2 + 12n + 4 - 6n^2 - 12n - 6}{24} \\\\
           &= \\frac{2n^2 - 2}{24} \\\\
           &= \\frac{n^2 - 1}{12}
\\end{align*}
")  

4.  *(Problema 280)* Este es un mecanismo para generar valores al azar
    de una variable aleatoria con distribución ![\\text{unif}\\{x\_1,
    \\ldots ,
    x\_n\\}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bunif%7D%5C%7Bx_1%2C%20%5Cldots%20%2C%20x_n%5C%7D
    "\\text{unif}\\{x_1, \\ldots , x_n\\}") a partir de valores de una
    variable aleatoria con distribución
    ![\\text{unif}(0, 1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bunif%7D%280%2C%201%29
    "\\text{unif}(0, 1)"), la cual aparece definida más adelante. Sea
    ![u](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;u
    "u") un valor al azar con distribución
    ![\\text{unif}(0, 1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bunif%7D%280%2C%201%29
    "\\text{unif}(0, 1)"). Demuestre que la variable aleatoria
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X"), definida a continuación, tiene distribución
    ![\\text{unif}\\{x\_1, \\ldots ,
    x\_n\\}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bunif%7D%5C%7Bx_1%2C%20%5Cldots%20%2C%20x_n%5C%7D
    "\\text{unif}\\{x_1, \\ldots , x_n\\}").

  
![X = 
\\begin{cases}
x\_1 & \\text{si } 0 \< u \\le 1/n \\\\
x\_1 & \\text{si } 1/n \< u \\le 2/n \\\\
\\ldots & \\ldots \\\\
x\_{n-1} & \\text{si } (n-2)/n \< u \\le (n-1)/n \\\\
x\_{n} & \\text{si } (n-1)/n \< u \< 1 
\\end{cases}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%20%3D%20%0A%20%20%20%20%5Cbegin%7Bcases%7D%0A%20%20%20%20%20%20%20%20x_1%20%26%20%5Ctext%7Bsi%20%7D%200%20%3C%20u%20%5Cle%201%2Fn%20%5C%5C%0A%20%20%20%20%20%20%20%20x_1%20%26%20%5Ctext%7Bsi%20%7D%201%2Fn%20%3C%20u%20%5Cle%202%2Fn%20%5C%5C%0A%20%20%20%20%20%20%20%20%5Cldots%20%26%20%5Cldots%20%5C%5C%0A%20%20%20%20%20%20%20%20x_%7Bn-1%7D%20%26%20%5Ctext%7Bsi%20%7D%20%28n-2%29%2Fn%20%3C%20u%20%5Cle%20%28n-1%29%2Fn%20%5C%5C%0A%20%20%20%20%20%20%20%20x_%7Bn%7D%20%26%20%5Ctext%7Bsi%20%7D%20%28n-1%29%2Fn%20%3C%20u%20%3C%201%20%0A%20%20%20%20%5Cend%7Bcases%7D%0A
"X = 
    \\begin{cases}
        x_1 & \\text{si } 0 \< u \\le 1/n \\\\
        x_1 & \\text{si } 1/n \< u \\le 2/n \\\\
        \\ldots & \\ldots \\\\
        x_{n-1} & \\text{si } (n-2)/n \< u \\le (n-1)/n \\\\
        x_{n} & \\text{si } (n-1)/n \< u \< 1 
    \\end{cases}
")  

Simular en `R` una variable aleatoria utilizando este último ejercicio.

Desmotrar que
![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
"X") tiene distribución ![\\text{unif}\\{x\_1, \\ldots ,
x\_n\\}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bunif%7D%5C%7Bx_1%2C%20%5Cldots%20%2C%20x_n%5C%7D
"\\text{unif}\\{x_1, \\ldots , x_n\\}") es demostrar que la probabilidad
de cada
![X\_i](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X_i
"X_i") es la misma e igual a
![1/n](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;1%2Fn
"1/n"). Para ![i
= 1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;i%20%3D%201
"i = 1"), se tiene:

  
![P(X = x\_1) = P(0 \< u \\le 1/n) = P(u \\le 1/n) =
\\frac{1}{n}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3D%20x_1%29%20%3D%20P%280%20%3C%20u%20%5Cle%201%2Fn%29%20%3D%20P%28u%20%5Cle%201%2Fn%29%20%3D%20%5Cfrac%7B1%7D%7Bn%7D
"P(X = x_1) = P(0 \< u \\le 1/n) = P(u \\le 1/n) = \\frac{1}{n}")  

Para ![i = 2, \\ldots,
n-1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;i%20%3D%202%2C%20%5Cldots%2C%20n-1
"i = 2, \\ldots, n-1") se tiene:

  
![P(X = x\_i) = P((i-1)/n \< u \\le i/n) = P(u \\le i/n) - P(u \\le
(i-1)/n) = \\frac{i}{n} - \\frac{i-1}{n} =
\\frac{1}{n}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3D%20x_i%29%20%3D%20P%28%28i-1%29%2Fn%20%3C%20u%20%5Cle%20i%2Fn%29%20%3D%20P%28u%20%5Cle%20i%2Fn%29%20-%20P%28u%20%5Cle%20%28i-1%29%2Fn%29%20%3D%20%5Cfrac%7Bi%7D%7Bn%7D%20-%20%5Cfrac%7Bi-1%7D%7Bn%7D%20%3D%20%5Cfrac%7B1%7D%7Bn%7D
"P(X = x_i) = P((i-1)/n \< u \\le i/n) = P(u \\le i/n) - P(u \\le (i-1)/n) = \\frac{i}{n} - \\frac{i-1}{n} = \\frac{1}{n}")  

Finalmente, para
![i=n](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;i%3Dn
"i=n") se tiene:

  
![P(X = x\_n) = P((n-1)/n \< u \< 1) = P(u \< 1) - P(u \\le (n-1)/n) = 1
- \\frac{(n-1)}{n} =
\\frac{1}{n}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3D%20x_n%29%20%3D%20P%28%28n-1%29%2Fn%20%3C%20u%20%3C%201%29%20%3D%20P%28u%20%3C%201%29%20-%20P%28u%20%5Cle%20%28n-1%29%2Fn%29%20%3D%201%20-%20%5Cfrac%7B%28n-1%29%7D%7Bn%7D%20%3D%20%5Cfrac%7B1%7D%7Bn%7D
"P(X = x_n) = P((n-1)/n \< u \< 1) = P(u \< 1) - P(u \\le (n-1)/n) = 1 - \\frac{(n-1)}{n} = \\frac{1}{n}")  

Y queda demostrado.

Para la simulación, suponiendo ![n
= 20](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;n%20%3D%2020
"n = 20"), entonces

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-4-1.png" style="display: block; margin: auto;" />

5.  Correr en `R` la simulación 3.1 y hacer un histograma.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/sim-5-1-1.png" style="display: block; margin: auto;" />

Al considerar una muestra de mayor tamaño:

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/sim-5-2-1.png" style="display: block; margin: auto;" />

6.  *(Problema 292)* Este es un mecanismo para generar valores al azar
    si ![t \<
    \\lambda](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;t%20%3C%20%5Clambda
    "t \< \\lambda") de una variable aleatoria con distribución
    ![\\text{Ber}(p)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7BBer%7D%28p%29
    "\\text{Ber}(p)") a partir de valores de una variable aleatoria con
    distribución
    ![\\text{unif}(0, 1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bunif%7D%280%2C%201%29
    "\\text{unif}(0, 1)") definida más adelante. Sea
    ![u](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;u
    "u") un valor al azar con distribución
    ![\\text{unif}(0, 1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bunif%7D%280%2C%201%29
    "\\text{unif}(0, 1)"). Demuestre que la variable aleatoria
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X"), definida a continuación, tiene distribución
    ![\\text{Ber}(p)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7BBer%7D%28p%29
    "\\text{Ber}(p)")

  
![X = 
\\begin{cases}
0 & \\text{si } 0 \< u \\le 1-p \\\\
1 & \\text{si } 1-p \< u \< 1 
\\end{cases}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%20%3D%20%0A%20%20%20%20%5Cbegin%7Bcases%7D%0A%20%20%20%20%20%20%20%200%20%26%20%5Ctext%7Bsi%20%7D%200%20%3C%20u%20%5Cle%201-p%20%5C%5C%0A%20%20%20%20%20%20%20%201%20%26%20%5Ctext%7Bsi%20%7D%201-p%20%3C%20u%20%3C%201%20%0A%20%20%20%20%5Cend%7Bcases%7D%0A
"X = 
    \\begin{cases}
        0 & \\text{si } 0 \< u \\le 1-p \\\\
        1 & \\text{si } 1-p \< u \< 1 
    \\end{cases}
")  

Hacer una simulación utilizando este ejercicio

Se tiene que para ![X
= 0](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%20%3D%200
"X = 0"):

  
![P(X = 0) = P(0 \< u \\le 1-p) = P(u \\le 1-p) - P(u \\le 0)
= 1-p](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3D%200%29%20%3D%20P%280%20%3C%20u%20%5Cle%201-p%29%20%3D%20P%28u%20%5Cle%201-p%29%20-%20P%28u%20%5Cle%200%29%20%3D%201-p
"P(X = 0) = P(0 \< u \\le 1-p) = P(u \\le 1-p) - P(u \\le 0) = 1-p")  

y para ![X
= 1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%20%3D%201
"X = 1"):

  
![P(X = 1) = P(1 - p \< u \< 1) = 1 - P(0 \< u \\le 1-p) = 1 - 1 + p =
p](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3D%201%29%20%3D%20P%281%20-%20p%20%3C%20u%20%3C%201%29%20%3D%20%201%20-%20P%280%20%3C%20u%20%5Cle%201-p%29%20%3D%201%20-%201%20%2B%20p%20%3D%20p
"P(X = 1) = P(1 - p \< u \< 1) =  1 - P(0 \< u \\le 1-p) = 1 - 1 + p = p")  

y eso demuestra que ![X \\sim
\\text{Ber}(p)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%20%5Csim%20%5Ctext%7BBer%7D%28p%29
"X \\sim \\text{Ber}(p)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-6-1.png" style="display: block; margin: auto;" />

7.  Implemente la simulación 3.4 y genere una muestra aleatoria. Muestre
    el histograma. Coloque las leyendas.

Si se generan de manera independiente
![n](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;n
"n") valores al azar de la distribución
![\\text{Ber}(p)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7BBer%7D%28p%29
"\\text{Ber}(p)") y se suman estos valores, se obtiene un valor al azar
de la distribución ![\\text{bin}(n,
p)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bbin%7D%28n%2C%20p%29
"\\text{bin}(n, p)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-7-1.png" style="display: block; margin: auto;" />

8.  Genere una muestra aleatoria con 3.6 y muestre el histograma. Un
    examen tiene diez preguntas y cada una tiene tres opciones como
    respuesta, siendo solamente una de ellas la correcta. Si un
    estudiante contesta cada pregunta al azar, ¿cuál es la probabilidad
    de que apruebe el examen? Supponiendo que la nota mínima aprobatoria
    es 6.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-8-1.png" style="display: block; margin: auto;" />

La probabilidad de obtener la nota minima aprobatoria es ![P(X \\ge 6)
= 1 - P(X \< 6) = 1 - \\sum\_{k=0}^5 P(X = k)
=](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%5Cge%206%29%20%3D%201%20-%20P%28X%20%3C%206%29%20%3D%201%20-%20%5Csum_%7Bk%3D0%7D%5E5%20P%28X%20%3D%20k%29%20%3D
"P(X \\ge 6) = 1 - P(X \< 6) = 1 - \\sum_{k=0}^5 P(X = k) =") 0.213, la
cual es una probabilidad baja (solo hay un 21.3 % de probabilidad de que
el alumno apruebe al escoger respuestas al azar).

9.  *(Problema 314)* Sea ![X\_0, X\_1,
    \\ldots](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X_0%2C%20X_1%2C%20%5Cldots
    "X_0, X_1, \\ldots") una sucesión de variables aleatorias
    independientes con distribución
    ![\\text{Ber}(p)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7BBer%7D%28p%29
    "\\text{Ber}(p)"). Defina: ![X = \\text{min} \\{ n \\ge 0 : X\_n
    \\}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%20%3D%20%5Ctext%7Bmin%7D%20%5C%7B%20n%20%5Cge%200%20%3A%20X_n%20%5C%7D
    "X = \\text{min} \\{ n \\ge 0 : X_n \\}"). Demuestre que
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X") tiene distribución
    ![\\text{geo}(p)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bgeo%7D%28p%29
    "\\text{geo}(p)"). Esto permite encontrar valores al azar de la
    distribución geométrica a partir de una sucesión de valores al azar
    de la distribución Bernoulli. Implemente en `R`.

Se tiene que cada ensayo es independiente con distribución de Bernoulli,
con probabilidad de arrojar
![1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;1
"1") solo luego de que se han obtenido
![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
"X") ceros. Por lo tanto:

  
![P(X = \\text{min} \\{ n \\ge 0 : X\_n \\} ) = P(X = 0)P(X = 0)\\ldots
P(X = 1) = (1-p)^{n
- 1}p](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3D%20%5Ctext%7Bmin%7D%20%5C%7B%20n%20%5Cge%200%20%3A%20X_n%20%5C%7D%20%29%20%3D%20P%28X%20%3D%200%29P%28X%20%3D%200%29%5Cldots%20P%28X%20%3D%201%29%20%3D%20%281-p%29%5E%7Bn%20-%201%7Dp
"P(X = \\text{min} \\{ n \\ge 0 : X_n \\} ) = P(X = 0)P(X = 0)\\ldots P(X = 1) = (1-p)^{n - 1}p")  

Como ![n - 1 =
x](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;n%20-%201%20%3D%20x
"n - 1 = x") es el número de fracasos antes del primer éxito, entonces
se demuestra que la función de distribución es de una variable aleatoria
geométrica.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-9-1.png" style="display: block; margin: auto;" />

10. En Simulación 3.7, asigne valores a los parámetros de
    ![r](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;r
    "r") y
    ![p](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;p
    "p") y muestre los histogramas.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-10-1.png" style="display: block; margin: auto;" />

11. *(Problema 328)* Sea ![X\_1, X\_2,
    \\ldots](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X_1%2C%20X_2%2C%20%5Cldots
    "X_1, X_2, \\ldots") una sucesión de variables aleatorias
    independientes con distribución
    ![\\text{Ber}(p)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7BBer%7D%28p%29
    "\\text{Ber}(p)") y sea ![r
    \\ge 1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;r%20%5Cge%201
    "r \\ge 1") un entero. Defina ![X = \\text{min} \\{ n \\ge r :
    \\sum\_{k=1}^nX\_k = r \\} -
    r](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%20%3D%20%5Ctext%7Bmin%7D%20%5C%7B%20n%20%5Cge%20r%20%3A%20%5Csum_%7Bk%3D1%7D%5EnX_k%20%3D%20r%20%5C%7D%20-%20r
    "X = \\text{min} \\{ n \\ge r : \\sum_{k=1}^nX_k = r \\} - r").
    Demuestre que
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X") tiene distribución ![\\text{binNeg}(r,
    p)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7BbinNeg%7D%28r%2C%20p%29
    "\\text{binNeg}(r, p)"). Esto permite encontrar valores al azar de
    la distribución binomial negativa a partir de valores al azar de la
    distribución Bernoulli.

Se tiene que cada ensayo es independiente con distribución de Bernoulli,
y se repite hasta obtener
![r](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;r
"r") éxitos. Por lo tanto:

  
![P(X = \\text{min} \\{ n \\ge 0 : X\_n \\} ) =
\\left(\\prod\_{k=1}^xP(X = 0)\\right)\\left(\\prod\_{k=1}^rP(X
= 1)\\right) =
(1-p)^{x}p^r](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3D%20%5Ctext%7Bmin%7D%20%5C%7B%20n%20%5Cge%200%20%3A%20X_n%20%5C%7D%20%29%20%3D%20%5Cleft%28%5Cprod_%7Bk%3D1%7D%5ExP%28X%20%3D%200%29%5Cright%29%5Cleft%28%5Cprod_%7Bk%3D1%7D%5ErP%28X%20%3D%201%29%5Cright%29%20%3D%20%281-p%29%5E%7Bx%7Dp%5Er
"P(X = \\text{min} \\{ n \\ge 0 : X_n \\} ) = \\left(\\prod_{k=1}^xP(X = 0)\\right)\\left(\\prod_{k=1}^rP(X = 1)\\right) = (1-p)^{x}p^r")  

Como el número de fracasos y los ![r
- 1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;r%20-%201
"r - 1") pueden ocurrir en cualquier orden, se multiplica esta prob
abilidad por el ![\\binom{x + r
- 1}{x}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cbinom%7Bx%20%2B%20r%20-%201%7D%7Bx%7D
"\\binom{x + r - 1}{x}"); y se demuestra que la distribución es Binomial
Negativa. Implemente en `R`.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-11-1.png" style="display: block; margin: auto;" />

12. Simulación 3.8. Asigne usted valores a los parámetros
    ![N](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;N
    "N"),
    ![K](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;K
    "K") y
    ![n](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;n
    "n"), y genere tantos valores de esta distribución como desee
    modificando el valor de
    ![K](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;K
    "K"). Muestre el histograma.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-12-1.png" style="display: block; margin: auto;" />

13. Simulación 3.9. Especificando un valor para
    ![\\lambda](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Clambda
    "\\lambda"), genere tantos valores al azar como desee de una
    variable aleatoria con distribución
    ![\\text{Poisson}(\\lambda)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7BPoisson%7D%28%5Clambda%29
    "\\text{Poisson}(\\lambda)") y compare el promedio aritmético de
    estos valores con el valor de
    ![\\lambda](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Clambda
    "\\lambda"). ¿Son parecidos? Muestre los histogramas.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-13-1.png" style="display: block; margin: auto;" />

Los valores teóricos y los promedios calculados se muestran en la
siguiente tabla, donde se muestra que los valores calculados a partir de
los datos simulados y los teoricos es minima:

| Teorico | Calculado | Diferencia |
| ------: | --------: | ---------: |
|     0.5 |     0.473 |      0.027 |
|     5.0 |     5.002 |    \-0.002 |
|    25.0 |    25.012 |    \-0.012 |
|   100.0 |   100.485 |    \-0.485 |

14. Simulación 3.10 Asigne valores de su preferencia a los parámetros
    ![a](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;a
    "a") y
    ![b](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;b
    "b"), y genere valores al azar de esta distribución. Genere el
    histograma.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-14-1.png" style="display: block; margin: auto;" />

15. *(Problema 359)* Sea
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X") una variable aleatoria con distribución
    ![\\text{unif}(0, 4)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bunif%7D%280%2C%204%29
    "\\text{unif}(0, 4)") y denote por
    ![\\mu](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cmu
    "\\mu") a la media de esta distribución. Encuentre el valor de ![c
    \> 0](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;c%20%3E%200
    "c \> 0") tal que:

<!-- end list -->

  - ![P(X \\le c)
    = 1/8](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%5Cle%20c%29%20%3D%201%2F8
    "P(X \\le c) = 1/8")
  - ![P(X \> c + \\mu)
    = 1/4](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3E%20c%20%2B%20%5Cmu%29%20%3D%201%2F4
    "P(X \> c + \\mu) = 1/4")
  - ![P(\\vert X - \\mu\\vert \< c)
    = 1/2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28%5Cvert%20X%20-%20%5Cmu%5Cvert%20%3C%20c%29%20%3D%201%2F2
    "P(\\vert X - \\mu\\vert \< c) = 1/2")
  - ![P(\\vert X - 4\\vert \< c)
    = 3/4](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28%5Cvert%20X%20-%204%5Cvert%20%3C%20c%29%20%3D%203%2F4
    "P(\\vert X - 4\\vert \< c) = 3/4")

Para la primera probabilidad se tiene:

  
![P(X \\le c) = \\int\_{-infty}^c \\frac{1}{4-0}dx = \\int\_{0}^c
\\frac{1}{4}dx = \\frac{1}{4}(c - 0) = \\frac{c}{4} =
\\frac{1}{8}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%5Cle%20c%29%20%3D%20%5Cint_%7B-infty%7D%5Ec%20%5Cfrac%7B1%7D%7B4-0%7Ddx%20%3D%20%5Cint_%7B0%7D%5Ec%20%5Cfrac%7B1%7D%7B4%7Ddx%20%3D%20%5Cfrac%7B1%7D%7B4%7D%28c%20-%200%29%20%3D%20%5Cfrac%7Bc%7D%7B4%7D%20%3D%20%5Cfrac%7B1%7D%7B8%7D
"P(X \\le c) = \\int_{-infty}^c \\frac{1}{4-0}dx = \\int_{0}^c \\frac{1}{4}dx = \\frac{1}{4}(c - 0) = \\frac{c}{4} = \\frac{1}{8}")  

lo cual significa ![c
= 1/2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;c%20%3D%201%2F2
"c = 1/2"). Para la segunda probabilidad se tiene:

  
![P(X \> c + \\mu) = 1 - P(X \\le c + \\mu) = 1 - \\int\_{0}^{c+\\mu}
\\frac{1}{4}dx = 1 - \\frac{1}{4}(c + \\mu) =
\\frac{1}{4}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3E%20c%20%2B%20%5Cmu%29%20%3D%201%20-%20P%28X%20%5Cle%20c%20%2B%20%5Cmu%29%20%3D%201%20-%20%5Cint_%7B0%7D%5E%7Bc%2B%5Cmu%7D%20%5Cfrac%7B1%7D%7B4%7Ddx%20%3D%201%20-%20%5Cfrac%7B1%7D%7B4%7D%28c%20%2B%20%5Cmu%29%20%3D%20%5Cfrac%7B1%7D%7B4%7D
"P(X \> c + \\mu) = 1 - P(X \\le c + \\mu) = 1 - \\int_{0}^{c+\\mu} \\frac{1}{4}dx = 1 - \\frac{1}{4}(c + \\mu) = \\frac{1}{4}")  

De lo que se obtiene ![c = 3 -
\\mu](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;c%20%3D%203%20-%20%5Cmu
"c = 3 - \\mu"). Como la media de una distribución uniforme es el valor
medio entre los límites de la distribución, entonces ![\\mu
= 2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cmu%20%3D%202
"\\mu = 2") y ![c
= 1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;c%20%3D%201
"c = 1"). Para la siguiente probabilidad se tiene:

  
![
\\begin{align\*}
P(\\vert X - \\mu\\vert \< c) &= P(-c \< X - \\mu \< c) = P(-c + \\mu \<
X \< c + \\mu) = P(X \< c + \\mu) - P(X \< -c + \\mu)\\\\
&= P(X \\le c + \\mu) - P(X = c + \\mu) - (P(X \\le -c + \\mu) - P(X =
-c + \\mu)) \\\\
&= P(X \\le c + \\mu) - P(X \\le -c + \\mu) \\\\
&= \\int\_{0}^{c+\\mu}\\frac{1}{4}dx -
\\int\_{0}^{-c+\\mu}\\frac{1}{4}dx = \\frac{1}{4}(c + \\mu) -
\\frac{1}{4}(-c + \\mu) \\\\
&= \\frac{1}{4}2c = \\frac{1}{2}
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0A%20%20%20%20P%28%5Cvert%20X%20-%20%5Cmu%5Cvert%20%3C%20c%29%20%26%3D%20P%28-c%20%3C%20X%20-%20%5Cmu%20%3C%20c%29%20%3D%20P%28-c%20%2B%20%5Cmu%20%3C%20X%20%3C%20c%20%2B%20%5Cmu%29%20%3D%20P%28X%20%3C%20c%20%2B%20%5Cmu%29%20-%20P%28X%20%3C%20-c%20%2B%20%5Cmu%29%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20P%28X%20%5Cle%20c%20%2B%20%5Cmu%29%20-%20P%28X%20%3D%20c%20%2B%20%5Cmu%29%20-%20%28P%28X%20%5Cle%20-c%20%2B%20%5Cmu%29%20-%20P%28X%20%3D%20-c%20%2B%20%5Cmu%29%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20P%28X%20%5Cle%20c%20%2B%20%5Cmu%29%20-%20P%28X%20%5Cle%20-c%20%2B%20%5Cmu%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cint_%7B0%7D%5E%7Bc%2B%5Cmu%7D%5Cfrac%7B1%7D%7B4%7Ddx%20-%20%5Cint_%7B0%7D%5E%7B-c%2B%5Cmu%7D%5Cfrac%7B1%7D%7B4%7Ddx%20%3D%20%5Cfrac%7B1%7D%7B4%7D%28c%20%2B%20%5Cmu%29%20-%20%5Cfrac%7B1%7D%7B4%7D%28-c%20%2B%20%5Cmu%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7B1%7D%7B4%7D2c%20%3D%20%5Cfrac%7B1%7D%7B2%7D%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
    P(\\vert X - \\mu\\vert \< c) &= P(-c \< X - \\mu \< c) = P(-c + \\mu \< X \< c + \\mu) = P(X \< c + \\mu) - P(X \< -c + \\mu)\\\\
        &= P(X \\le c + \\mu) - P(X = c + \\mu) - (P(X \\le -c + \\mu) - P(X = -c + \\mu)) \\\\
        &= P(X \\le c + \\mu) - P(X \\le -c + \\mu) \\\\
        &= \\int_{0}^{c+\\mu}\\frac{1}{4}dx - \\int_{0}^{-c+\\mu}\\frac{1}{4}dx = \\frac{1}{4}(c + \\mu) - \\frac{1}{4}(-c + \\mu) \\\\
        &= \\frac{1}{4}2c = \\frac{1}{2}
\\end{align*}
")  

lo cual arroja ![c
= 1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;c%20%3D%201
"c = 1"). Al igual que antes, si reemplazamos
![\\mu](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cmu
"\\mu") por el valor
![4](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;4
"4"), se obtiene un resultado similar al anterior:

  
![
\\begin{align\*}
P(\\vert X - 4\\vert \< c) &= P(X \< c + 4) - P(X \< -c + 4)\\\\
&= P(X \\le c + 4) - P(X \\le -c + 4) \\\\
&= \\frac{1}{4}2c = \\frac{3}{4}
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0A%20%20%20%20P%28%5Cvert%20X%20-%204%5Cvert%20%3C%20c%29%20%26%3D%20P%28X%20%3C%20c%20%2B%204%29%20-%20P%28X%20%3C%20-c%20%2B%204%29%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20P%28X%20%5Cle%20c%20%2B%204%29%20-%20P%28X%20%5Cle%20-c%20%2B%204%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7B1%7D%7B4%7D2c%20%3D%20%5Cfrac%7B3%7D%7B4%7D%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
    P(\\vert X - 4\\vert \< c) &= P(X \< c + 4) - P(X \< -c + 4)\\\\
        &= P(X \\le c + 4) - P(X \\le -c + 4) \\\\
        &= \\frac{1}{4}2c = \\frac{3}{4}
\\end{align*}
")  

Entonces, ![c
= 3/2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;c%20%3D%203%2F2
"c = 3/2").

16. *(Problema 360)* Sea
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X") una variable aleatoria con distribución ![\\text{unif}(a,
    b)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bunif%7D%28a%2C%20b%29
    "\\text{unif}(a, b)"). Demuestre que:

<!-- end list -->

  - ![E(X) = (a + b)
    / 2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;E%28X%29%20%3D%20%28a%20%2B%20b%29%20%2F%202
    "E(X) = (a + b) / 2")
  - ![E(X^2) = (a^2 + ab + b^2)
    / 3](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;E%28X%5E2%29%20%3D%20%28a%5E2%20%2B%20ab%20%2B%20b%5E2%29%20%2F%203
    "E(X^2) = (a^2 + ab + b^2) / 3")
  - ![Var(X) = (b - a)^2
    / 12](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Var%28X%29%20%3D%20%28b%20-%20a%29%5E2%20%2F%2012
    "Var(X) = (b - a)^2 / 12")

Para la esperanza de
![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
"X") se tiene:

  
![E(X) = \\int\_{-\\infty}^{\\infty}xf(x)dx = \\int\_{a}^{b}xf(x)dx =
\\int\_{a}^{b}\\frac{1}{b-a}xdx = \\frac{1}{b-a}\\frac{(b^2 - a^2)}{2} =
\\frac{1}{b-a}\\frac{(b - a)(a + b)}{2} = \\frac{a +
b}{2}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;E%28X%29%20%3D%20%5Cint_%7B-%5Cinfty%7D%5E%7B%5Cinfty%7Dxf%28x%29dx%20%3D%20%5Cint_%7Ba%7D%5E%7Bb%7Dxf%28x%29dx%20%3D%20%5Cint_%7Ba%7D%5E%7Bb%7D%5Cfrac%7B1%7D%7Bb-a%7Dxdx%20%3D%20%5Cfrac%7B1%7D%7Bb-a%7D%5Cfrac%7B%28b%5E2%20-%20a%5E2%29%7D%7B2%7D%20%3D%20%5Cfrac%7B1%7D%7Bb-a%7D%5Cfrac%7B%28b%20-%20a%29%28a%20%2B%20b%29%7D%7B2%7D%20%3D%20%5Cfrac%7Ba%20%2B%20b%7D%7B2%7D
"E(X) = \\int_{-\\infty}^{\\infty}xf(x)dx = \\int_{a}^{b}xf(x)dx = \\int_{a}^{b}\\frac{1}{b-a}xdx = \\frac{1}{b-a}\\frac{(b^2 - a^2)}{2} = \\frac{1}{b-a}\\frac{(b - a)(a + b)}{2} = \\frac{a + b}{2}")  

Para la esperanza de
![X^2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%5E2
"X^2") se tiene:

  
![E(X^2) = \\int\_{-\\infty}^{\\infty}x^2f(x)dx =
\\int\_{a}^{b}x^2f(x)dx = \\int\_{a}^{b}\\frac{1}{b-a}x^2dx =
\\frac{1}{b-a}(\\frac{b^3}{3} -
\\frac{a^3}{3})](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;E%28X%5E2%29%20%3D%20%5Cint_%7B-%5Cinfty%7D%5E%7B%5Cinfty%7Dx%5E2f%28x%29dx%20%3D%20%5Cint_%7Ba%7D%5E%7Bb%7Dx%5E2f%28x%29dx%20%3D%20%5Cint_%7Ba%7D%5E%7Bb%7D%5Cfrac%7B1%7D%7Bb-a%7Dx%5E2dx%20%3D%20%5Cfrac%7B1%7D%7Bb-a%7D%28%5Cfrac%7Bb%5E3%7D%7B3%7D%20-%20%5Cfrac%7Ba%5E3%7D%7B3%7D%29
"E(X^2) = \\int_{-\\infty}^{\\infty}x^2f(x)dx = \\int_{a}^{b}x^2f(x)dx = \\int_{a}^{b}\\frac{1}{b-a}x^2dx = \\frac{1}{b-a}(\\frac{b^3}{3} - \\frac{a^3}{3})")  

Haciendo la división de polinomios ![(b^3 - a^3)/(b-a) = a^2 + ab +
b^2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%28b%5E3%20-%20a%5E3%29%2F%28b-a%29%20%3D%20a%5E2%20%2B%20ab%20%2B%20b%5E2
"(b^3 - a^3)/(b-a) = a^2 + ab + b^2") y se obtiene el resultado buscado.

Para la varianza, se pueden usar los resultados anteriores:

  
![
\\begin{align\*} 
Var(X) &= E(X^2) - (E(X))^2 \\\\
&= \\frac{a^2 + ab + b^2}{3} - \\left(\\frac{a + b}{2}\\right)^2 \\\\
&= \\frac{a^2 + ab + b^2}{3} - \\frac{a^2 + 2ab + b^2}{4} \\\\
&= \\frac{4a^2 + 4ab + 4b^2 - 3a^2 - 6ab - 3b^2}{12} \\\\
&= \\frac{a^2 - 2ab + b^2}{12} = \\frac{(b - a)^2}{12}
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%20%0A%20%20%20%20Var%28X%29%20%26%3D%20E%28X%5E2%29%20-%20%28E%28X%29%29%5E2%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7Ba%5E2%20%2B%20ab%20%2B%20b%5E2%7D%7B3%7D%20-%20%5Cleft%28%5Cfrac%7Ba%20%2B%20b%7D%7B2%7D%5Cright%29%5E2%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7Ba%5E2%20%2B%20ab%20%2B%20b%5E2%7D%7B3%7D%20-%20%5Cfrac%7Ba%5E2%20%2B%202ab%20%2B%20b%5E2%7D%7B4%7D%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7B4a%5E2%20%2B%204ab%20%2B%204b%5E2%20-%203a%5E2%20-%206ab%20-%203b%5E2%7D%7B12%7D%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7Ba%5E2%20-%202ab%20%2B%20b%5E2%7D%7B12%7D%20%3D%20%5Cfrac%7B%28b%20-%20a%29%5E2%7D%7B12%7D%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*} 
    Var(X) &= E(X^2) - (E(X))^2 \\\\
        &= \\frac{a^2 + ab + b^2}{3} - \\left(\\frac{a + b}{2}\\right)^2 \\\\
        &= \\frac{a^2 + ab + b^2}{3} - \\frac{a^2 + 2ab + b^2}{4} \\\\
        &= \\frac{4a^2 + 4ab + 4b^2 - 3a^2 - 6ab - 3b^2}{12} \\\\
        &= \\frac{a^2 - 2ab + b^2}{12} = \\frac{(b - a)^2}{12}
\\end{align*}
")  

17. Simulación 3.11 asigne un valor de su preferencia al parámetro
    ![\\lambda](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Clambda
    "\\lambda") y genere valores al azar de la distribución exponencial.
    Genere el histograma.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-17-1.png" style="display: block; margin: auto;" />

18. *(Problema 375)* Sea
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X") una variable aleatoria con distribución
    ![\\text{exp}(\\lambda)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bexp%7D%28%5Clambda%29
    "\\text{exp}(\\lambda)") con ![\\lambda
    = 2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Clambda%20%3D%202
    "\\lambda = 2"). Encuentre:

<!-- end list -->

  - ![P(X
    \< 1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3C%201%29
    "P(X \< 1)")
  - ![P(X
    \\ge 2)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%5Cge%202%29
    "P(X \\ge 2)")
  - ![P(X \< 1 \\vert X
    \< 2)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3C%201%20%5Cvert%20X%20%3C%202%29
    "P(X \< 1 \\vert X \< 2)")
  - ![P(1 \\le X \\le 2 \\vert X
    \> 0)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%281%20%5Cle%20X%20%5Cle%202%20%5Cvert%20X%20%3E%200%29
    "P(1 \\le X \\le 2 \\vert X \> 0)")

Para la primera probabilidad se tiene:

  
![P(X \< 1) = P(X \\le 1) - P(X = 1) = \\int\_0^1\\lambda e^{-\\lambda
x}dx = \\lambda(-\\frac{e^{-\\lambda}}{\\lambda} +
\\frac{e^{0}}{\\lambda}) = 1 - e^{-\\lambda}
= 0.8647](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3C%201%29%20%3D%20P%28X%20%5Cle%201%29%20-%20P%28X%20%3D%201%29%20%3D%20%5Cint_0%5E1%5Clambda%20e%5E%7B-%5Clambda%20x%7Ddx%20%3D%20%5Clambda%28-%5Cfrac%7Be%5E%7B-%5Clambda%7D%7D%7B%5Clambda%7D%20%2B%20%5Cfrac%7Be%5E%7B0%7D%7D%7B%5Clambda%7D%29%20%3D%201%20-%20e%5E%7B-%5Clambda%7D%20%3D%200.8647
"P(X \< 1) = P(X \\le 1) - P(X = 1) = \\int_0^1\\lambda e^{-\\lambda x}dx = \\lambda(-\\frac{e^{-\\lambda}}{\\lambda} + \\frac{e^{0}}{\\lambda}) = 1 - e^{-\\lambda} = 0.8647")  

Para la segunda probabilidad se tiene:

  
![P(X \\ge 2) = 1 - P(X \< 2) = 1 - \\int\_0^2\\lambda e^{-\\lambda x}dx
= 1 - (1 - e^{-2\\lambda}) = e^{-2\\lambda}
= 0.0183](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%5Cge%202%29%20%3D%201%20-%20P%28X%20%3C%202%29%20%3D%201%20-%20%20%5Cint_0%5E2%5Clambda%20e%5E%7B-%5Clambda%20x%7Ddx%20%3D%201%20-%20%281%20-%20e%5E%7B-2%5Clambda%7D%29%20%3D%20e%5E%7B-2%5Clambda%7D%20%3D%200.0183
"P(X \\ge 2) = 1 - P(X \< 2) = 1 -  \\int_0^2\\lambda e^{-\\lambda x}dx = 1 - (1 - e^{-2\\lambda}) = e^{-2\\lambda} = 0.0183")  

Para la siguiente probabilidad se utiliza la definición de probabilidad
condicional, de forma que:

  
![
\\begin{align\*}
P(X \< 1 \\vert X \< 2) &= \\frac{P(X \< 1 \\cap X \< 2)}{P(X \< 2)} =
\\frac{P(1 \\le X \< 2)}{P(X \< 2)} \\\\
&= \\frac{\\int\_1^2\\lambda e^{-\\lambda x}dx}{\\int\_0^2\\lambda
e^{-\\lambda x}dx} \\\\
&= \\frac{-e^{-2\\lambda} + e^{-\\lambda}}{-e^{-2\\lambda} + 1} =
\\frac{0.117}{0.9817} \\\\
&= 0.1192
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0A%20%20%20%20P%28X%20%3C%201%20%5Cvert%20X%20%3C%202%29%20%26%3D%20%5Cfrac%7BP%28X%20%3C%201%20%5Ccap%20X%20%3C%202%29%7D%7BP%28X%20%3C%202%29%7D%20%3D%20%5Cfrac%7BP%281%20%5Cle%20X%20%3C%202%29%7D%7BP%28X%20%3C%202%29%7D%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7B%5Cint_1%5E2%5Clambda%20e%5E%7B-%5Clambda%20x%7Ddx%7D%7B%5Cint_0%5E2%5Clambda%20e%5E%7B-%5Clambda%20x%7Ddx%7D%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7B-e%5E%7B-2%5Clambda%7D%20%2B%20e%5E%7B-%5Clambda%7D%7D%7B-e%5E%7B-2%5Clambda%7D%20%2B%201%7D%20%3D%20%5Cfrac%7B0.117%7D%7B0.9817%7D%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%200.1192%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
    P(X \< 1 \\vert X \< 2) &= \\frac{P(X \< 1 \\cap X \< 2)}{P(X \< 2)} = \\frac{P(1 \\le X \< 2)}{P(X \< 2)} \\\\
        &= \\frac{\\int_1^2\\lambda e^{-\\lambda x}dx}{\\int_0^2\\lambda e^{-\\lambda x}dx} \\\\
        &= \\frac{-e^{-2\\lambda} + e^{-\\lambda}}{-e^{-2\\lambda} + 1} = \\frac{0.117}{0.9817} \\\\
        &= 0.1192
\\end{align*}
")  

Para la cuarta probabilidad se usa la definición de probabilidad
condicional, notando que ![P(X \> 0) = P(\\Omega)
= 1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3E%200%29%20%3D%20P%28%5COmega%29%20%3D%201
"P(X \> 0) = P(\\Omega) = 1"), de forma que:

  
![
\\begin{align\*}
P(1 \\le X \\le 2 \\vert X \> 0) &= \\frac{P(1 \\le X \\le 2 \\cap X
\> 0)}{P(X \> 0)} = P(1 \\le X \\le 2) \\\\
&= \\int\_1^2\\lambda e^{-\\lambda x}dx = -e^{-2\\lambda} +
e^{-\\lambda} \\\\
&= 0.117
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0A%20%20%20%20P%281%20%5Cle%20X%20%5Cle%202%20%5Cvert%20X%20%3E%200%29%20%26%3D%20%5Cfrac%7BP%281%20%5Cle%20X%20%5Cle%202%20%5Ccap%20X%20%3E%200%29%7D%7BP%28X%20%3E%200%29%7D%20%3D%20P%281%20%5Cle%20X%20%5Cle%202%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cint_1%5E2%5Clambda%20e%5E%7B-%5Clambda%20x%7Ddx%20%3D%20-e%5E%7B-2%5Clambda%7D%20%2B%20e%5E%7B-%5Clambda%7D%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%200.117%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
    P(1 \\le X \\le 2 \\vert X \> 0) &= \\frac{P(1 \\le X \\le 2 \\cap X \> 0)}{P(X \> 0)} = P(1 \\le X \\le 2) \\\\
        &= \\int_1^2\\lambda e^{-\\lambda x}dx = -e^{-2\\lambda} + e^{-\\lambda} \\\\
        &= 0.117
\\end{align*}
")  

19. *(Problema 382)* **Propiedad de pérdida de memoria**. Sea
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X") una variable aleatoria con distribución exponencial de
    parámetro
    ![\\lambda](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Clambda
    "\\lambda"). Demuestre que, para cualesquiera valores ![x,y
    \\ge 0](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;x%2Cy%20%5Cge%200
    "x,y \\ge 0"),

  
![P(X \> x + y \\vert X \> y) = P(X \>
x)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3E%20x%20%2B%20y%20%5Cvert%20X%20%3E%20y%29%20%3D%20P%28X%20%3E%20x%29
"P(X \> x + y \\vert X \> y) = P(X \> x)")  

Usando la definción de probabilidad condicional se tiene:

  
![
\\begin{align\*}
P(X \> x + y \\vert X \> y) &= \\frac{P(X \> x + y \\cap X \> y)}{P(X \>
y)} = \\frac{P(X \\ge x + y)}{P(X \> y)} \\\\
&= \\frac{\\int\_{x + y}^\\infty\\lambda e^{-\\lambda
x}dx)}{\\int\_y^\\infty\\lambda e^{-\\lambda x}dx} = \\frac{e^{-\\lambda
(x + y)}}{e^{-\\lambda y}}\\\\
&= \\frac{e^{-\\lambda (x + y)}}{e^{-\\lambda y}} = e^{-\\lambda x} =
\\int\_x^\\infty \\lambda e^{-\\lambda x}dx\\\\
&= P(X \> x)
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0A%20%20%20%20P%28X%20%3E%20x%20%2B%20y%20%5Cvert%20X%20%3E%20y%29%20%26%3D%20%5Cfrac%7BP%28X%20%3E%20x%20%2B%20y%20%5Ccap%20%20X%20%3E%20y%29%7D%7BP%28X%20%3E%20y%29%7D%20%3D%20%5Cfrac%7BP%28X%20%5Cge%20x%20%2B%20y%29%7D%7BP%28X%20%3E%20y%29%7D%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7B%5Cint_%7Bx%20%2B%20y%7D%5E%5Cinfty%5Clambda%20e%5E%7B-%5Clambda%20x%7Ddx%29%7D%7B%5Cint_y%5E%5Cinfty%5Clambda%20e%5E%7B-%5Clambda%20x%7Ddx%7D%20%3D%20%5Cfrac%7Be%5E%7B-%5Clambda%20%28x%20%2B%20y%29%7D%7D%7Be%5E%7B-%5Clambda%20y%7D%7D%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cfrac%7Be%5E%7B-%5Clambda%20%28x%20%2B%20y%29%7D%7D%7Be%5E%7B-%5Clambda%20y%7D%7D%20%3D%20e%5E%7B-%5Clambda%20x%7D%20%3D%20%5Cint_x%5E%5Cinfty%20%5Clambda%20e%5E%7B-%5Clambda%20x%7Ddx%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20P%28X%20%3E%20x%29%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
    P(X \> x + y \\vert X \> y) &= \\frac{P(X \> x + y \\cap  X \> y)}{P(X \> y)} = \\frac{P(X \\ge x + y)}{P(X \> y)} \\\\
        &= \\frac{\\int_{x + y}^\\infty\\lambda e^{-\\lambda x}dx)}{\\int_y^\\infty\\lambda e^{-\\lambda x}dx} = \\frac{e^{-\\lambda (x + y)}}{e^{-\\lambda y}}\\\\
        &= \\frac{e^{-\\lambda (x + y)}}{e^{-\\lambda y}} = e^{-\\lambda x} = \\int_x^\\infty \\lambda e^{-\\lambda x}dx\\\\
        &= P(X \> x)
\\end{align*}
")  

20. *(Problema 384)* Sea
    ![U](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;U
    "U") una variable aleatoria con distribución
    ![\\text{unif}(0, 1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bunif%7D%280%2C%201%29
    "\\text{unif}(0, 1)") y sea ![\\lambda
    \> 0](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Clambda%20%3E%200
    "\\lambda \> 0") una constante. Demuestre que la variable aleatoria
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X"), definida a continuación, tiene distribución
    ![\\text{exp}(\\lambda)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bexp%7D%28%5Clambda%29
    "\\text{exp}(\\lambda)"). Este resultado permite obtener valores al
    azar de la distribución exponencial a partir de valores de la
    distribución uniforme continua. Muestre el histograma y compare con
    los resultados de Simulación 3.11.

  
![X = -\\frac{1}{\\lambda}\\text{ln}(1 -
U)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%20%3D%20-%5Cfrac%7B1%7D%7B%5Clambda%7D%5Ctext%7Bln%7D%281%20-%20U%29
"X = -\\frac{1}{\\lambda}\\text{ln}(1 - U)")  

Por teorema de cambio de variable se tiene que ![f\_X(x) = f\_U(u =
\\varphi^{-1}(x))\\vert
d\\varphi^{-1}(x)/dx\\vert](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;f_X%28x%29%20%3D%20f_U%28u%20%3D%20%5Cvarphi%5E%7B-1%7D%28x%29%29%5Cvert%20d%5Cvarphi%5E%7B-1%7D%28x%29%2Fdx%5Cvert
"f_X(x) = f_U(u = \\varphi^{-1}(x))\\vert d\\varphi^{-1}(x)/dx\\vert"),
dónde ![\\varphi^{-1}(x) = 1 - e^{-\\lambda
x}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cvarphi%5E%7B-1%7D%28x%29%20%3D%201%20-%20e%5E%7B-%5Clambda%20x%7D
"\\varphi^{-1}(x) = 1 - e^{-\\lambda x}"), y su derivada es
![d\\varphi^{-1}(x)/dx = \\lambda e^{-\\lambda
x}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;d%5Cvarphi%5E%7B-1%7D%28x%29%2Fdx%20%3D%20%5Clambda%20e%5E%7B-%5Clambda%20x%7D
"d\\varphi^{-1}(x)/dx = \\lambda e^{-\\lambda x}"). También, como
![f\_U(u)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;f_U%28u%29
"f_U(u)") es una distribución uniforme en el intervalo
![(0, 1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%280%2C%201%29
"(0, 1)"), entonces ![f\_U(u) = 1/(1-0)
= 1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;f_U%28u%29%20%3D%201%2F%281-0%29%20%3D%201
"f_U(u) = 1/(1-0) = 1") y entonces ![f\_X(x) = \\lambda e^{-\\lambda
x}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;f_X%28x%29%20%3D%20%5Clambda%20e%5E%7B-%5Clambda%20x%7D
"f_X(x) = \\lambda e^{-\\lambda x}"), la cual es la función de
probabilidad de la distribución exponencial.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-20-1.png" style="display: block; margin: auto;" />

21. Simulación 3.12. Asigne un valor de su preferencia a los parámetros
    ![\\alpha](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Calpha
    "\\alpha") y
    ![\\lambda](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Clambda
    "\\lambda") y genere valores al azar de esta distribución. Genere
    los histogramas.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-21-1.png" style="display: block; margin: auto;" />

22. *(Problema 398)* **Propiedades de la función beta**. Demuestre las
    siguientes propiedades de la función beta.

<!-- end list -->

  - ![B(a, b) = B(b,
    a)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;B%28a%2C%20b%29%20%3D%20B%28b%2C%20a%29
    "B(a, b) = B(b, a)")
  - ![B(a,1)
    = 1/a](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;B%28a%2C1%29%20%3D%201%2Fa
    "B(a,1) = 1/a")
  - ![B(1, b)
    = 1/b](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;B%281%2C%20b%29%20%3D%201%2Fb
    "B(1, b) = 1/b")
  - ![B(a+1,b) =
    \\frac{a}{b}B(a,b+1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;B%28a%2B1%2Cb%29%20%3D%20%5Cfrac%7Ba%7D%7Bb%7DB%28a%2Cb%2B1%29
    "B(a+1,b) = \\frac{a}{b}B(a,b+1)")
  - ![B(a+1,b) =
    \\frac{a}{a+b}B(a,b)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;B%28a%2B1%2Cb%29%20%3D%20%5Cfrac%7Ba%7D%7Ba%2Bb%7DB%28a%2Cb%29
    "B(a+1,b) = \\frac{a}{a+b}B(a,b)")
  - ![B(a,b+1) =
    \\frac{b}{a+b}B(a,b)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;B%28a%2Cb%2B1%29%20%3D%20%5Cfrac%7Bb%7D%7Ba%2Bb%7DB%28a%2Cb%29
    "B(a,b+1) = \\frac{b}{a+b}B(a,b)")
  - ![B(1/2,1/2) =
    \\pi](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;B%281%2F2%2C1%2F2%29%20%3D%20%5Cpi
    "B(1/2,1/2) = \\pi")

Para el primer inciso se escribe primero la función beta:

  
![B(a,b) = \\int\_0^1x^{a-1}(1 -
x)^{b-1}dx](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;B%28a%2Cb%29%20%3D%20%5Cint_0%5E1x%5E%7Ba-1%7D%281%20-%20x%29%5E%7Bb-1%7Ddx
"B(a,b) = \\int_0^1x^{a-1}(1 - x)^{b-1}dx")  

Usando el cambio de variable ![t = 1 -
x](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;t%20%3D%201%20-%20x
"t = 1 - x"), se tiene que:

  
![B(a,b) = -\\int\_1^0(1 - t)^{a-1}t^{b-1}dt = \\int\_0^1(1 -
t)^{a-1}t^{b-1}dt =
B(b,a)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;B%28a%2Cb%29%20%3D%20-%5Cint_1%5E0%281%20-%20t%29%5E%7Ba-1%7Dt%5E%7Bb-1%7Ddt%20%3D%20%5Cint_0%5E1%281%20-%20t%29%5E%7Ba-1%7Dt%5E%7Bb-1%7Ddt%20%3D%20B%28b%2Ca%29
"B(a,b) = -\\int_1^0(1 - t)^{a-1}t^{b-1}dt = \\int_0^1(1 - t)^{a-1}t^{b-1}dt = B(b,a)")  

Para los siguientes dos incisos, se tiene:

  
![
\\begin{align\*}
B(a\\text{,}1) &= \\int\_0^1x^{a-1}(1 - x)^{1-1}dx = \\int\_0^1x^{a-1}dx
= 1^{a}/a - 0^a/a = 1/a \\\\
B(1\\text{,}b) &= \\int\_0^1x^{1-1}(1 - x)^{b-1}dx = \\int\_0^1(1 -
x)^{b-1}dx = -(0^{b}/b - 1^b/b) = 1/b \\\\
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0A%20%20%20%20B%28a%5Ctext%7B%2C%7D1%29%20%26%3D%20%5Cint_0%5E1x%5E%7Ba-1%7D%281%20-%20x%29%5E%7B1-1%7Ddx%20%3D%20%5Cint_0%5E1x%5E%7Ba-1%7Ddx%20%3D%201%5E%7Ba%7D%2Fa%20-%200%5Ea%2Fa%20%3D%201%2Fa%20%5C%5C%0A%20%20%20%20B%281%5Ctext%7B%2C%7Db%29%20%26%3D%20%5Cint_0%5E1x%5E%7B1-1%7D%281%20-%20x%29%5E%7Bb-1%7Ddx%20%3D%20%5Cint_0%5E1%281%20-%20x%29%5E%7Bb-1%7Ddx%20%3D%20-%280%5E%7Bb%7D%2Fb%20-%201%5Eb%2Fb%29%20%3D%201%2Fb%20%5C%5C%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
    B(a\\text{,}1) &= \\int_0^1x^{a-1}(1 - x)^{1-1}dx = \\int_0^1x^{a-1}dx = 1^{a}/a - 0^a/a = 1/a \\\\
    B(1\\text{,}b) &= \\int_0^1x^{1-1}(1 - x)^{b-1}dx = \\int_0^1(1 - x)^{b-1}dx = -(0^{b}/b - 1^b/b) = 1/b \\\\
\\end{align*}
")  

Para los siguientes tres incisos se usa la definición de la función beta
en terminos de la función gamma:

  
![B(a, b) = \\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a +
b)}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;B%28a%2C%20b%29%20%3D%20%5Cfrac%7B%5CGamma%28a%29%5CGamma%28b%29%7D%7B%5CGamma%28a%20%2B%20b%29%7D
"B(a, b) = \\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b)}")  

y la propiedad ![\\Gamma(\\alpha + 1) =
\\alpha\\Gamma(\\alpha)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5CGamma%28%5Calpha%20%2B%201%29%20%3D%20%5Calpha%5CGamma%28%5Calpha%29
"\\Gamma(\\alpha + 1) = \\alpha\\Gamma(\\alpha)"). De esta forma, se
tiene:

  
![
\\begin{align\*}
B(a + 1\\text{,} b) &= \\frac{\\Gamma(a + 1)\\Gamma(b)}{\\Gamma(a + b
+ 1)} = a\\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b + 1)} =
\\frac{ab}{b}\\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b + 1)} =
\\frac{a}{b}\\frac{\\Gamma(a)\\Gamma(b + 1)}{\\Gamma(a + b + 1)} =
\\frac{a}{b}B(a\\text{,}b + 1) \\\\
B(a + 1\\text{,} b) &= \\frac{\\Gamma(a + 1)\\Gamma(b)}{\\Gamma(a + b
+ 1)} = a\\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b + 1)} = \\frac{a}{a
+ b}\\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b)} = \\frac{a}{a +
b}B(a\\text{,}b) \\\\
B(a\\text{,}b + 1) &= \\frac{\\Gamma(a)\\Gamma(b + 1)}{\\Gamma(a + b
+ 1)} = b\\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b + 1)} = \\frac{b}{a
+ b}\\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b)} = \\frac{b}{a +
b}B(a\\text{,}b) 
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0A%20%20%20%20B%28a%20%2B%201%5Ctext%7B%2C%7D%20b%29%20%26%3D%20%5Cfrac%7B%5CGamma%28a%20%2B%201%29%5CGamma%28b%29%7D%7B%5CGamma%28a%20%2B%20b%20%2B%201%29%7D%20%3D%20a%5Cfrac%7B%5CGamma%28a%29%5CGamma%28b%29%7D%7B%5CGamma%28a%20%2B%20b%20%2B%201%29%7D%20%3D%20%5Cfrac%7Bab%7D%7Bb%7D%5Cfrac%7B%5CGamma%28a%29%5CGamma%28b%29%7D%7B%5CGamma%28a%20%2B%20b%20%2B%201%29%7D%20%3D%20%5Cfrac%7Ba%7D%7Bb%7D%5Cfrac%7B%5CGamma%28a%29%5CGamma%28b%20%2B%201%29%7D%7B%5CGamma%28a%20%2B%20b%20%2B%201%29%7D%20%3D%20%5Cfrac%7Ba%7D%7Bb%7DB%28a%5Ctext%7B%2C%7Db%20%2B%201%29%20%5C%5C%0A%20%20%20%20B%28a%20%2B%201%5Ctext%7B%2C%7D%20b%29%20%26%3D%20%5Cfrac%7B%5CGamma%28a%20%2B%201%29%5CGamma%28b%29%7D%7B%5CGamma%28a%20%2B%20b%20%2B%201%29%7D%20%3D%20a%5Cfrac%7B%5CGamma%28a%29%5CGamma%28b%29%7D%7B%5CGamma%28a%20%2B%20b%20%2B%201%29%7D%20%3D%20%5Cfrac%7Ba%7D%7Ba%20%2B%20b%7D%5Cfrac%7B%5CGamma%28a%29%5CGamma%28b%29%7D%7B%5CGamma%28a%20%2B%20b%29%7D%20%3D%20%5Cfrac%7Ba%7D%7Ba%20%2B%20b%7DB%28a%5Ctext%7B%2C%7Db%29%20%5C%5C%0A%20%20%20%20B%28a%5Ctext%7B%2C%7Db%20%2B%201%29%20%26%3D%20%5Cfrac%7B%5CGamma%28a%29%5CGamma%28b%20%2B%201%29%7D%7B%5CGamma%28a%20%2B%20b%20%2B%201%29%7D%20%3D%20b%5Cfrac%7B%5CGamma%28a%29%5CGamma%28b%29%7D%7B%5CGamma%28a%20%2B%20b%20%2B%201%29%7D%20%3D%20%5Cfrac%7Bb%7D%7Ba%20%2B%20b%7D%5Cfrac%7B%5CGamma%28a%29%5CGamma%28b%29%7D%7B%5CGamma%28a%20%2B%20b%29%7D%20%3D%20%5Cfrac%7Bb%7D%7Ba%20%2B%20b%7DB%28a%5Ctext%7B%2C%7Db%29%20%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
    B(a + 1\\text{,} b) &= \\frac{\\Gamma(a + 1)\\Gamma(b)}{\\Gamma(a + b + 1)} = a\\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b + 1)} = \\frac{ab}{b}\\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b + 1)} = \\frac{a}{b}\\frac{\\Gamma(a)\\Gamma(b + 1)}{\\Gamma(a + b + 1)} = \\frac{a}{b}B(a\\text{,}b + 1) \\\\
    B(a + 1\\text{,} b) &= \\frac{\\Gamma(a + 1)\\Gamma(b)}{\\Gamma(a + b + 1)} = a\\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b + 1)} = \\frac{a}{a + b}\\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b)} = \\frac{a}{a + b}B(a\\text{,}b) \\\\
    B(a\\text{,}b + 1) &= \\frac{\\Gamma(a)\\Gamma(b + 1)}{\\Gamma(a + b + 1)} = b\\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b + 1)} = \\frac{b}{a + b}\\frac{\\Gamma(a)\\Gamma(b)}{\\Gamma(a + b)} = \\frac{b}{a + b}B(a\\text{,}b) 
\\end{align*}
")  

Para el ultimo inciso se utiliza la misma definición de la función beta
en terminos de la función gamma, y la propiedad ![\\Gamma(1/2) =
\\sqrt{\\pi}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5CGamma%281%2F2%29%20%3D%20%5Csqrt%7B%5Cpi%7D
"\\Gamma(1/2) = \\sqrt{\\pi}") y ![\\Gamma(1)
= 1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5CGamma%281%29%20%3D%201
"\\Gamma(1) = 1"), de forma que:

  
![
\\begin{align\*}
B(1/2\\text{,}1/2) &= \\frac{\\Gamma(1/2)\\Gamma(1/2)}{\\Gamma(1)} =
(\\Gamma(1/2))^2 = \\pi
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0A%20%20%20%20B%281%2F2%5Ctext%7B%2C%7D1%2F2%29%20%26%3D%20%5Cfrac%7B%5CGamma%281%2F2%29%5CGamma%281%2F2%29%7D%7B%5CGamma%281%29%7D%20%3D%20%28%5CGamma%281%2F2%29%29%5E2%20%3D%20%5Cpi%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
    B(1/2\\text{,}1/2) &= \\frac{\\Gamma(1/2)\\Gamma(1/2)}{\\Gamma(1)} = (\\Gamma(1/2))^2 = \\pi
\\end{align*}
")  

23. *(Problema 410)*. Sea
    ![U](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;U
    "U") una variable aleatoria con distribución
    ![\\text{unif}(0, 1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7Bunif%7D%280%2C%201%29
    "\\text{unif}(0, 1)") y sean ![\\alpha
    \> 0](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Calpha%20%3E%200
    "\\alpha \> 0") y ![\\lambda
    \< 0](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Clambda%20%3C%200
    "\\lambda \< 0") dos constantes. Demuestre que:

  
![\\frac{1}{\\lambda}(-\\text{ln}(1 - U))^{1/\\alpha} \\sim
\\text{Weibull}(\\alpha,
\\lambda)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cfrac%7B1%7D%7B%5Clambda%7D%28-%5Ctext%7Bln%7D%281%20-%20U%29%29%5E%7B1%2F%5Calpha%7D%20%5Csim%20%5Ctext%7BWeibull%7D%28%5Calpha%2C%20%5Clambda%29
"\\frac{1}{\\lambda}(-\\text{ln}(1 - U))^{1/\\alpha} \\sim \\text{Weibull}(\\alpha, \\lambda)")  

Este resultado permite obtener valores al azar de la distribución
Weibull a partir de valores al azar de la distribución uniforme. Genere
una muestra aleatoria usando este ejercicio y directamente en `R`.
Compare.

Sea ![X = \\frac{1}{\\lambda}(-\\text{ln}(1 -
U))^{1/\\alpha}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%20%3D%20%5Cfrac%7B1%7D%7B%5Clambda%7D%28-%5Ctext%7Bln%7D%281%20-%20U%29%29%5E%7B1%2F%5Calpha%7D
"X = \\frac{1}{\\lambda}(-\\text{ln}(1 - U))^{1/\\alpha}") una variable
aleatoria. Por teorema de cambio de variable se tiene que ![f\_X(x) =
f\_U(u = \\varphi^{-1}(x))\\vert
d\\varphi^{-1}(x)/dx\\vert](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;f_X%28x%29%20%3D%20f_U%28u%20%3D%20%5Cvarphi%5E%7B-1%7D%28x%29%29%5Cvert%20d%5Cvarphi%5E%7B-1%7D%28x%29%2Fdx%5Cvert
"f_X(x) = f_U(u = \\varphi^{-1}(x))\\vert d\\varphi^{-1}(x)/dx\\vert"),
dónde:

  
![\\varphi^{-1}(x) = 1 - e^{-(\\lambda
x)^\\alpha}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cvarphi%5E%7B-1%7D%28x%29%20%3D%201%20-%20e%5E%7B-%28%5Clambda%20x%29%5E%5Calpha%7D
"\\varphi^{-1}(x) = 1 - e^{-(\\lambda x)^\\alpha}")  

Su derivada es:

  
![\\frac{d\\varphi^{-1}(x)}{dx} = \\alpha\\lambda(\\lambda x)^{\\alpha
- 1} e^{-(\\lambda
x)^\\alpha}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cfrac%7Bd%5Cvarphi%5E%7B-1%7D%28x%29%7D%7Bdx%7D%20%3D%20%5Calpha%5Clambda%28%5Clambda%20x%29%5E%7B%5Calpha%20-%201%7D%20e%5E%7B-%28%5Clambda%20x%29%5E%5Calpha%7D
"\\frac{d\\varphi^{-1}(x)}{dx} = \\alpha\\lambda(\\lambda x)^{\\alpha - 1} e^{-(\\lambda x)^\\alpha}")  

También, como
![f\_U(u)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;f_U%28u%29
"f_U(u)") es una distribución uniforme en el intervalo
![(0, 1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%280%2C%201%29
"(0, 1)"), entonces ![f\_U(u) = 1/(1-0)
= 1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;f_U%28u%29%20%3D%201%2F%281-0%29%20%3D%201
"f_U(u) = 1/(1-0) = 1") y entonces:

  
![f\_X(x) = \\alpha\\lambda(\\lambda x)^{\\alpha - 1} e^{-(\\lambda
x)^\\alpha}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;f_X%28x%29%20%3D%20%5Calpha%5Clambda%28%5Clambda%20x%29%5E%7B%5Calpha%20-%201%7D%20e%5E%7B-%28%5Clambda%20x%29%5E%5Calpha%7D
"f_X(x) = \\alpha\\lambda(\\lambda x)^{\\alpha - 1} e^{-(\\lambda x)^\\alpha}")  

la cual es la función de probabilidad de la distribución Weibull.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-23-1.png" style="display: block; margin: auto;" />

24. *(Problema 421)* Sean
    ![a](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;a
    "a") y
    ![b](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;b
    "b") dos constantes positivas, con ![a \<
    b](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;a%20%3C%20b
    "a \< b"), y sea
    ![Z](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Z
    "Z") una variable aleatoria con distribución normal estándar.
    Demuestre que:

  
![P(a \< Z^2 \< b) = 2(\\Phi(\\sqrt{b}) -
\\Phi(\\sqrt{a}))](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28a%20%3C%20Z%5E2%20%3C%20b%29%20%3D%202%28%5CPhi%28%5Csqrt%7Bb%7D%29%20-%20%5CPhi%28%5Csqrt%7Ba%7D%29%29
"P(a \< Z^2 \< b) = 2(\\Phi(\\sqrt{b}) - \\Phi(\\sqrt{a}))")  

Para desmostrar esta igualdad se sigue:

  
![
\\begin{align\*}
P(a \< Z^2 \< b) &= P(\\sqrt{a} \< Z \< \\sqrt{b}) + P(-\\sqrt{b} \< Z
\< -\\sqrt{a}) \\\\ 
&= P(Z \\le \\sqrt{b}) - P(Z \\le \\sqrt{a}) + P(Z \\le -\\sqrt{a}) -
P(Z \\le -\\sqrt{b}) \\\\
&= P(Z \\le \\sqrt{b}) - P(Z \\le \\sqrt{a}) + 1 - P(Z \\le \\sqrt{a}) -
(1 - P(Z \\le \\sqrt{b})) \\\\
&= P(Z \\le \\sqrt{b}) - P(Z \\le \\sqrt{a}) + P(Z \\le \\sqrt{b}) - P(Z
\\le \\sqrt{a}) \\\\
&= 2(P(Z \\le \\sqrt{b}) - P(Z \\le \\sqrt{a})) \\\\
&= 2(\\Phi(\\sqrt{b}) - \\Phi(\\sqrt{a}))
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0A%20%20%20%20P%28a%20%3C%20Z%5E2%20%3C%20b%29%20%26%3D%20P%28%5Csqrt%7Ba%7D%20%3C%20Z%20%3C%20%5Csqrt%7Bb%7D%29%20%2B%20P%28-%5Csqrt%7Bb%7D%20%3C%20Z%20%3C%20-%5Csqrt%7Ba%7D%29%20%5C%5C%20%0A%20%20%20%20%20%20%20%20%26%3D%20P%28Z%20%5Cle%20%5Csqrt%7Bb%7D%29%20-%20P%28Z%20%5Cle%20%5Csqrt%7Ba%7D%29%20%2B%20P%28Z%20%5Cle%20-%5Csqrt%7Ba%7D%29%20-%20P%28Z%20%5Cle%20-%5Csqrt%7Bb%7D%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20P%28Z%20%5Cle%20%5Csqrt%7Bb%7D%29%20-%20P%28Z%20%5Cle%20%5Csqrt%7Ba%7D%29%20%2B%201%20-%20P%28Z%20%5Cle%20%5Csqrt%7Ba%7D%29%20-%20%281%20-%20P%28Z%20%5Cle%20%5Csqrt%7Bb%7D%29%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20P%28Z%20%5Cle%20%5Csqrt%7Bb%7D%29%20-%20P%28Z%20%5Cle%20%5Csqrt%7Ba%7D%29%20%2B%20P%28Z%20%5Cle%20%5Csqrt%7Bb%7D%29%20-%20P%28Z%20%5Cle%20%5Csqrt%7Ba%7D%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%202%28P%28Z%20%5Cle%20%5Csqrt%7Bb%7D%29%20-%20P%28Z%20%5Cle%20%5Csqrt%7Ba%7D%29%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%202%28%5CPhi%28%5Csqrt%7Bb%7D%29%20-%20%5CPhi%28%5Csqrt%7Ba%7D%29%29%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
    P(a \< Z^2 \< b) &= P(\\sqrt{a} \< Z \< \\sqrt{b}) + P(-\\sqrt{b} \< Z \< -\\sqrt{a}) \\\\ 
        &= P(Z \\le \\sqrt{b}) - P(Z \\le \\sqrt{a}) + P(Z \\le -\\sqrt{a}) - P(Z \\le -\\sqrt{b}) \\\\
        &= P(Z \\le \\sqrt{b}) - P(Z \\le \\sqrt{a}) + 1 - P(Z \\le \\sqrt{a}) - (1 - P(Z \\le \\sqrt{b})) \\\\
        &= P(Z \\le \\sqrt{b}) - P(Z \\le \\sqrt{a}) + P(Z \\le \\sqrt{b}) - P(Z \\le \\sqrt{a}) \\\\
        &= 2(P(Z \\le \\sqrt{b}) - P(Z \\le \\sqrt{a})) \\\\
        &= 2(\\Phi(\\sqrt{b}) - \\Phi(\\sqrt{a}))
\\end{align*}
")  

25. *(Problema 422)* Sea
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X") una variable aleatoria con distribución
    ![\\text{N}(10, 36)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Ctext%7BN%7D%2810%2C%2036%29
    "\\text{N}(10, 36)"). Calcule:

<!-- end list -->

  - ![P(X
    \> 5)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%3E%205%29
    "P(X \> 5)")
  - ![P(4 \< X
    \< 16)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%284%20%3C%20X%20%3C%2016%29
    "P(4 \< X \< 16)")
  - ![P(X
    \\le 8)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%5Cle%208%29
    "P(X \\le 8)")
  - ![P(X
    \\ge 16)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28X%20%5Cge%2016%29
    "P(X \\ge 16)")
  - ![P(\\vert X - 4\\vert
    \\le 6)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28%5Cvert%20X%20-%204%5Cvert%20%5Cle%206%29
    "P(\\vert X - 4\\vert \\le 6)")
  - ![P(\\vert X - 6\\vert
    \> 3)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;P%28%5Cvert%20X%20-%206%5Cvert%20%3E%203%29
    "P(\\vert X - 6\\vert \> 3)")

En todos los casos se estandariza
![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
"X") como ![Z=(X -
\\mu)/\\sigma](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Z%3D%28X%20-%20%5Cmu%29%2F%5Csigma
"Z=(X - \\mu)/\\sigma"), y se busca la probabilidad:

  
![
\\begin{align\*}
P(X \> 5) &= P(X - \\mu \> 5 - 10) \\\\
&= P(X - \\mu \> -5) \\\\
&= P(\\frac{X - \\mu}{\\sigma} \> -\\frac{5}{6}) \\\\
&= P(Z \> -\\frac{5}{6}) \\\\
&= 1 - P(Z \\le -\\frac{5}{6}) \\\\
&= 0.7977 \\\\
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0AP%28X%20%3E%205%29%20%26%3D%20P%28X%20-%20%5Cmu%20%3E%205%20-%2010%29%20%5C%5C%0A%20%20%20%20%26%3D%20P%28X%20-%20%5Cmu%20%3E%20-5%29%20%5C%5C%0A%20%20%20%20%26%3D%20P%28%5Cfrac%7BX%20-%20%5Cmu%7D%7B%5Csigma%7D%20%3E%20-%5Cfrac%7B5%7D%7B6%7D%29%20%5C%5C%0A%20%20%20%20%26%3D%20P%28Z%20%3E%20-%5Cfrac%7B5%7D%7B6%7D%29%20%5C%5C%0A%20%20%20%20%26%3D%201%20-%20P%28Z%20%5Cle%20-%5Cfrac%7B5%7D%7B6%7D%29%20%5C%5C%0A%20%20%20%20%26%3D%200.7977%20%5C%5C%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
P(X \> 5) &= P(X - \\mu \> 5 - 10) \\\\
    &= P(X - \\mu \> -5) \\\\
    &= P(\\frac{X - \\mu}{\\sigma} \> -\\frac{5}{6}) \\\\
    &= P(Z \> -\\frac{5}{6}) \\\\
    &= 1 - P(Z \\le -\\frac{5}{6}) \\\\
    &= 0.7977 \\\\
\\end{align*}
")  
  
![
\\begin{align\*}
P(4 \< X \< 16) &= P(-1 \< Z \< 1) \\\\
&= P(Z \\le 1) - P(Z \\le -1) \\\\
&= 0.8413 - 0.1587 \\\\
&= 0.6826 \\\\
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0AP%284%20%3C%20X%20%3C%2016%29%20%26%3D%20P%28-1%20%3C%20Z%20%3C%201%29%20%5C%5C%0A%20%20%20%20%26%3D%20P%28Z%20%5Cle%201%29%20-%20P%28Z%20%5Cle%20-1%29%20%5C%5C%0A%20%20%20%20%26%3D%200.8413%20-%200.1587%20%5C%5C%0A%20%20%20%20%26%3D%200.6826%20%5C%5C%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
P(4 \< X \< 16) &= P(-1 \< Z \< 1) \\\\
    &= P(Z \\le 1) - P(Z \\le -1) \\\\
    &= 0.8413 - 0.1587 \\\\
    &= 0.6826 \\\\
\\end{align*}
")  
  
![
\\begin{align\*}
P(X \\le 8) &= P(Z \\le -1/3) \\\\
&= 0.3694 \\\\
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0AP%28X%20%5Cle%208%29%20%26%3D%20P%28Z%20%5Cle%20-1%2F3%29%20%5C%5C%0A%20%20%20%20%26%3D%200.3694%20%5C%5C%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
P(X \\le 8) &= P(Z \\le -1/3) \\\\
    &= 0.3694 \\\\
\\end{align*}
")  
  
![
\\begin{align\*}
P(X \\ge 16) &= 1 - P(X \\le 16) \\\\
&= 1 - P(Z \\le 1) \\\\
&= 0.1587 \\\\
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0AP%28X%20%5Cge%2016%29%20%26%3D%201%20-%20P%28X%20%5Cle%2016%29%20%5C%5C%0A%20%20%20%20%26%3D%201%20-%20P%28Z%20%5Cle%201%29%20%5C%5C%0A%20%20%20%20%26%3D%200.1587%20%5C%5C%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
P(X \\ge 16) &= 1 - P(X \\le 16) \\\\
    &= 1 - P(Z \\le 1) \\\\
    &= 0.1587 \\\\
\\end{align*}
")  
  
![
\\begin{align\*}
P(\\vert X - 4\\vert \\le 6) &= P(-6 \\le X - 4 \\le 6) \\\\
&= P(-2 \\le X \\le 10) \\\\
&= P(-2 \\le Z \\le 0) \\\\
&= P(Z \\le 0) - P(Z \\le -2) \\\\
&= 0.5 - 0.0228 \\\\
&= 0.4772 \\\\
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0AP%28%5Cvert%20X%20-%204%5Cvert%20%5Cle%206%29%20%26%3D%20P%28-6%20%5Cle%20X%20-%204%20%5Cle%206%29%20%5C%5C%0A%20%20%20%20%26%3D%20P%28-2%20%5Cle%20X%20%5Cle%2010%29%20%5C%5C%0A%20%20%20%20%26%3D%20P%28-2%20%5Cle%20Z%20%5Cle%200%29%20%5C%5C%0A%20%20%20%20%26%3D%20P%28Z%20%5Cle%200%29%20-%20%20P%28Z%20%5Cle%20-2%29%20%5C%5C%0A%20%20%20%20%26%3D%200.5%20-%200.0228%20%5C%5C%0A%20%20%20%20%26%3D%200.4772%20%5C%5C%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
P(\\vert X - 4\\vert \\le 6) &= P(-6 \\le X - 4 \\le 6) \\\\
    &= P(-2 \\le X \\le 10) \\\\
    &= P(-2 \\le Z \\le 0) \\\\
    &= P(Z \\le 0) -  P(Z \\le -2) \\\\
    &= 0.5 - 0.0228 \\\\
    &= 0.4772 \\\\
\\end{align*}
")  
  
![
\\begin{align\*}
P(\\vert X - 6\\vert \> 3) &= P(X - 6 \< -3 \\cup X - 6 \> 3 ) \\\\
&= P(X - 6 \< -3) + P(X - 6 \> 3) \\\\
&= P(X \< 3) + P(X \> 9) \\\\
&= P(Z \< -7/6) + P(Z \> -1/6) \\\\
&= P(Z \\le -7/6) + 1 - P(Z \\le -1/6) \\\\
&= 0.6879 
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0AP%28%5Cvert%20X%20-%206%5Cvert%20%3E%203%29%20%26%3D%20P%28X%20-%206%20%3C%20-3%20%5Ccup%20X%20-%206%20%3E%203%20%29%20%5C%5C%0A%20%20%20%20%26%3D%20P%28X%20-%206%20%3C%20-3%29%20%2B%20P%28X%20-%206%20%3E%203%29%20%5C%5C%0A%20%20%20%20%26%3D%20P%28X%20%3C%203%29%20%2B%20P%28X%20%3E%209%29%20%5C%5C%0A%20%20%20%20%26%3D%20P%28Z%20%3C%20-7%2F6%29%20%2B%20P%28Z%20%3E%20-1%2F6%29%20%5C%5C%0A%20%20%20%20%26%3D%20P%28Z%20%5Cle%20-7%2F6%29%20%2B%201%20-%20P%28Z%20%5Cle%20-1%2F6%29%20%5C%5C%0A%20%20%20%20%26%3D%200.6879%20%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
P(\\vert X - 6\\vert \> 3) &= P(X - 6 \< -3 \\cup X - 6 \> 3 ) \\\\
    &= P(X - 6 \< -3) + P(X - 6 \> 3) \\\\
    &= P(X \< 3) + P(X \> 9) \\\\
    &= P(Z \< -7/6) + P(Z \> -1/6) \\\\
    &= P(Z \\le -7/6) + 1 - P(Z \\le -1/6) \\\\
    &= 0.6879 
\\end{align*}
")  

26. Genere en `R` una muestra aleatoria de una ditribución normal con
    los parámetros de su preferencia y muestre el histograma.

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-26-1.png" style="display: block; margin: auto;" />

27. *(Problema 428)* Sea
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X") una variable aleatoria continua. Demuestre que:

<!-- end list -->

  - ![F\_{X^2}(x) = F\_X(\\sqrt{x}) -
    F\_X(-\\sqrt{x})](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;F_%7BX%5E2%7D%28x%29%20%3D%20F_X%28%5Csqrt%7Bx%7D%29%20-%20F_X%28-%5Csqrt%7Bx%7D%29
    "F_{X^2}(x) = F_X(\\sqrt{x}) - F_X(-\\sqrt{x})"), para ![x
    \> 0](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;x%20%3E%200
    "x \> 0").
  - Si ![X \\sim
    \\text{N}(0, 1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%20%5Csim%20%5Ctext%7BN%7D%280%2C%201%29
    "X \\sim \\text{N}(0, 1)") entonces ![X^2 \\sim
    \\chi^2(1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%5E2%20%5Csim%20%5Cchi%5E2%281%29
    "X^2 \\sim \\chi^2(1)")

Para ![x
\> 0](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;x%20%3E%200
"x \> 0"):

  
![
\\begin{align\*}
F\_{X^2}(x) &= P(X^2 \\le x) \\\\
&= P(\\vert X\\vert \\le \\sqrt{x}) \\\\
&= P(\\vert X\\vert \\le \\sqrt{x}) \\\\
&= P(-\\sqrt{x} \\le X \\le \\sqrt{x}) \\\\
&= P(X \\le \\sqrt{x}) - P(X \\le -\\sqrt{x}) \\\\
&= F\_X(\\sqrt{x}) - F\_X(-\\sqrt{x})
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0A%20%20%20%20F_%7BX%5E2%7D%28x%29%20%26%3D%20P%28X%5E2%20%5Cle%20x%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20P%28%5Cvert%20X%5Cvert%20%5Cle%20%5Csqrt%7Bx%7D%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20P%28%5Cvert%20X%5Cvert%20%5Cle%20%5Csqrt%7Bx%7D%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20P%28-%5Csqrt%7Bx%7D%20%5Cle%20X%20%5Cle%20%5Csqrt%7Bx%7D%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20P%28X%20%5Cle%20%5Csqrt%7Bx%7D%29%20-%20P%28X%20%5Cle%20-%5Csqrt%7Bx%7D%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20F_X%28%5Csqrt%7Bx%7D%29%20-%20F_X%28-%5Csqrt%7Bx%7D%29%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
    F_{X^2}(x) &= P(X^2 \\le x) \\\\
        &= P(\\vert X\\vert \\le \\sqrt{x}) \\\\
        &= P(\\vert X\\vert \\le \\sqrt{x}) \\\\
        &= P(-\\sqrt{x} \\le X \\le \\sqrt{x}) \\\\
        &= P(X \\le \\sqrt{x}) - P(X \\le -\\sqrt{x}) \\\\
        &= F_X(\\sqrt{x}) - F_X(-\\sqrt{x})
\\end{align*}
")  

Usando el resultado anterior, y tomando en cuenta que ![F\_X(\\sqrt{x})
=
\\Phi(\\sqrt{x})](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;F_X%28%5Csqrt%7Bx%7D%29%20%3D%20%5CPhi%28%5Csqrt%7Bx%7D%29
"F_X(\\sqrt{x}) = \\Phi(\\sqrt{x})") y que ![\\Phi(-\\sqrt{x}) = 1 -
\\Phi(\\sqrt{x})](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5CPhi%28-%5Csqrt%7Bx%7D%29%20%3D%201%20-%20%5CPhi%28%5Csqrt%7Bx%7D%29
"\\Phi(-\\sqrt{x}) = 1 - \\Phi(\\sqrt{x})"), entonces:

  
![F\_{X^2}(x) = F\_X(\\sqrt{x}) - F\_X(-\\sqrt{x}) = \\Phi(\\sqrt{x}) -
\\Phi(-\\sqrt{x}) = 2\\Phi(\\sqrt{x})
- 1](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;F_%7BX%5E2%7D%28x%29%20%3D%20F_X%28%5Csqrt%7Bx%7D%29%20-%20F_X%28-%5Csqrt%7Bx%7D%29%20%3D%20%5CPhi%28%5Csqrt%7Bx%7D%29%20-%20%5CPhi%28-%5Csqrt%7Bx%7D%29%20%3D%202%5CPhi%28%5Csqrt%7Bx%7D%29%20-%201
"F_{X^2}(x) = F_X(\\sqrt{x}) - F_X(-\\sqrt{x}) = \\Phi(\\sqrt{x}) - \\Phi(-\\sqrt{x}) = 2\\Phi(\\sqrt{x}) - 1")  

Derivando ambos lados:

  
![\\frac{dF\_{X^2}(x)}{dx} = 2\\frac{d\\Phi(\\sqrt{x})}{dx}
= 2\\frac{d}{dx}\\left(
\\int\_{-\\infty}^{\\sqrt{x}}\\frac{1}{\\sqrt{2\\pi}}e^{-u^2/2}du
\\right)
= 2\\frac{1}{\\sqrt{2\\pi}}e^{-(\\sqrt{x})^2/2}\\frac{d\\sqrt{x}}{dx} =
\\frac{1}{\\sqrt{2\\pi}}e^{-x/2}\\frac{1}{\\sqrt{x}}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cfrac%7BdF_%7BX%5E2%7D%28x%29%7D%7Bdx%7D%20%3D%202%5Cfrac%7Bd%5CPhi%28%5Csqrt%7Bx%7D%29%7D%7Bdx%7D%20%3D%202%5Cfrac%7Bd%7D%7Bdx%7D%5Cleft%28%20%5Cint_%7B-%5Cinfty%7D%5E%7B%5Csqrt%7Bx%7D%7D%5Cfrac%7B1%7D%7B%5Csqrt%7B2%5Cpi%7D%7De%5E%7B-u%5E2%2F2%7Ddu%20%5Cright%29%20%3D%202%5Cfrac%7B1%7D%7B%5Csqrt%7B2%5Cpi%7D%7De%5E%7B-%28%5Csqrt%7Bx%7D%29%5E2%2F2%7D%5Cfrac%7Bd%5Csqrt%7Bx%7D%7D%7Bdx%7D%20%3D%20%5Cfrac%7B1%7D%7B%5Csqrt%7B2%5Cpi%7D%7De%5E%7B-x%2F2%7D%5Cfrac%7B1%7D%7B%5Csqrt%7Bx%7D%7D
"\\frac{dF_{X^2}(x)}{dx} = 2\\frac{d\\Phi(\\sqrt{x})}{dx} = 2\\frac{d}{dx}\\left( \\int_{-\\infty}^{\\sqrt{x}}\\frac{1}{\\sqrt{2\\pi}}e^{-u^2/2}du \\right) = 2\\frac{1}{\\sqrt{2\\pi}}e^{-(\\sqrt{x})^2/2}\\frac{d\\sqrt{x}}{dx} = \\frac{1}{\\sqrt{2\\pi}}e^{-x/2}\\frac{1}{\\sqrt{x}}")  

Esta es la función de probabilidad de
![X^2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X%5E2
"X^2") la cual conincide con la función de probabilidad
![\\chi^2(1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cchi%5E2%281%29
"\\chi^2(1)"). Integrando a ambos lados de
![-\\infty](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;-%5Cinfty
"-\\infty") a
![x](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;x
"x") se obtiene que ![\\int\_{-\\infty}^x(dF\_{X^2}(x)/dx) dx =
\\int\_{0}^x(dF\_{X^2}(x)/dx) dx =
F\_{X^2}(x)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cint_%7B-%5Cinfty%7D%5Ex%28dF_%7BX%5E2%7D%28x%29%2Fdx%29%20dx%20%3D%20%5Cint_%7B0%7D%5Ex%28dF_%7BX%5E2%7D%28x%29%2Fdx%29%20dx%20%3D%20F_%7BX%5E2%7D%28x%29
"\\int_{-\\infty}^x(dF_{X^2}(x)/dx) dx = \\int_{0}^x(dF_{X^2}(x)/dx) dx = F_{X^2}(x)")
y:

  
![F\_{X^2}(x) =
\\int\_{0}^{x}\\frac{1}{\\sqrt{2\\pi}}\\frac{1}{\\sqrt{u}}e^{-u/2}du](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;F_%7BX%5E2%7D%28x%29%20%3D%20%5Cint_%7B0%7D%5E%7Bx%7D%5Cfrac%7B1%7D%7B%5Csqrt%7B2%5Cpi%7D%7D%5Cfrac%7B1%7D%7B%5Csqrt%7Bu%7D%7De%5E%7B-u%2F2%7Ddu
"F_{X^2}(x) = \\int_{0}^{x}\\frac{1}{\\sqrt{2\\pi}}\\frac{1}{\\sqrt{u}}e^{-u/2}du")  

la cual coincide con la función de distribución de
![\\chi^2(1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cchi%5E2%281%29
"\\chi^2(1)").

28. *(Problema 429)*. Sea
    ![X](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;X
    "X") una variable aleatoria con distribución
    ![\\chi^2(n)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cchi%5E2%28n%29
    "\\chi^2(n)") y sea ![c
    \> 0](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;c%20%3E%200
    "c \> 0") una constante. Defina los parámetros ![\\alpha =
    n/2](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Calpha%20%3D%20n%2F2
    "\\alpha = n/2") y ![\\lambda
    = 1/(2c)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Clambda%20%3D%201%2F%282c%29
    "\\lambda = 1/(2c)"). Demuestre que: ![cX \\sim gamma(\\alpha,
    \\lambda)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;cX%20%5Csim%20gamma%28%5Calpha%2C%20%5Clambda%29
    "cX \\sim gamma(\\alpha, \\lambda)"). Genere en `R` una muestra
    aleatoria con los parámetros de su preferencia y muestre el
    histograma.

Se tiene que ![F\_X(x) \\sim
\\chi^2(n)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;F_X%28x%29%20%5Csim%20%5Cchi%5E2%28n%29
"F_X(x) \\sim \\chi^2(n)"). Ahora:

  
![
\\begin{align\*}
F\_{cX}(x) &= P(cX \\le x) = P(X \\le x/c) \\\\
&=
\\int\_{0}^{x/c}\\frac{1}{\\Gamma(n/2)}\\left(\\frac{1}{2}\\right)^{n/2}u^{n/2
- 1}e^{-u/2}du \\\\
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0A%20%20%20%20F_%7BcX%7D%28x%29%20%26%3D%20P%28cX%20%5Cle%20x%29%20%3D%20P%28X%20%5Cle%20x%2Fc%29%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cint_%7B0%7D%5E%7Bx%2Fc%7D%5Cfrac%7B1%7D%7B%5CGamma%28n%2F2%29%7D%5Cleft%28%5Cfrac%7B1%7D%7B2%7D%5Cright%29%5E%7Bn%2F2%7Du%5E%7Bn%2F2%20-%201%7De%5E%7B-u%2F2%7Ddu%20%5C%5C%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
    F_{cX}(x) &= P(cX \\le x) = P(X \\le x/c) \\\\
        &= \\int_{0}^{x/c}\\frac{1}{\\Gamma(n/2)}\\left(\\frac{1}{2}\\right)^{n/2}u^{n/2 - 1}e^{-u/2}du \\\\
\\end{align*}
")  

Derivando con respecto a
![x](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;x
"x"), y luego integrando de
![-\\infty](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;-%5Cinfty
"-\\infty") a
![x](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;x
"x") queda:

  
![
\\begin{align\*}
F\_{cX}(x) &=
\\int\_{0}^{x}\\frac{1}{\\Gamma(n/2)}\\left(\\frac{1}{2}\\right)^{n/2}\\frac{1}{c}\\left(\\frac{u}{c}\\right)^{n/2
- 1}e^{-u/2c}du \\\\
&=
\\int\_{0}^{x}\\frac{1}{\\Gamma(n/2)}\\left(\\frac{1}{2c}\\right)^{n/2
- 1}\\left(\\frac{1}{2c}\\right)u^{n/2 - 1}e^{-u/2c}du \\\\
&=
\\int\_{0}^{x}\\frac{1}{\\Gamma(n/2)}\\left(\\frac{u}{2c}\\right)^{n/2
- 1}\\left(\\frac{1}{2c}\\right)e^{-u/2c}du \\\\
&= \\int\_{0}^{x}\\frac{1}{\\Gamma(\\alpha)}(\\lambda u)^{n/2
- 1}\\lambda e^{-\\lambda u}du
\\end{align\*}
](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%0A%5Cbegin%7Balign%2A%7D%0A%20%20%20%20F_%7BcX%7D%28x%29%20%26%3D%20%5Cint_%7B0%7D%5E%7Bx%7D%5Cfrac%7B1%7D%7B%5CGamma%28n%2F2%29%7D%5Cleft%28%5Cfrac%7B1%7D%7B2%7D%5Cright%29%5E%7Bn%2F2%7D%5Cfrac%7B1%7D%7Bc%7D%5Cleft%28%5Cfrac%7Bu%7D%7Bc%7D%5Cright%29%5E%7Bn%2F2%20-%201%7De%5E%7B-u%2F2c%7Ddu%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cint_%7B0%7D%5E%7Bx%7D%5Cfrac%7B1%7D%7B%5CGamma%28n%2F2%29%7D%5Cleft%28%5Cfrac%7B1%7D%7B2c%7D%5Cright%29%5E%7Bn%2F2%20-%201%7D%5Cleft%28%5Cfrac%7B1%7D%7B2c%7D%5Cright%29u%5E%7Bn%2F2%20-%201%7De%5E%7B-u%2F2c%7Ddu%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cint_%7B0%7D%5E%7Bx%7D%5Cfrac%7B1%7D%7B%5CGamma%28n%2F2%29%7D%5Cleft%28%5Cfrac%7Bu%7D%7B2c%7D%5Cright%29%5E%7Bn%2F2%20-%201%7D%5Cleft%28%5Cfrac%7B1%7D%7B2c%7D%5Cright%29e%5E%7B-u%2F2c%7Ddu%20%5C%5C%0A%20%20%20%20%20%20%20%20%26%3D%20%5Cint_%7B0%7D%5E%7Bx%7D%5Cfrac%7B1%7D%7B%5CGamma%28%5Calpha%29%7D%28%5Clambda%20u%29%5E%7Bn%2F2%20-%201%7D%5Clambda%20e%5E%7B-%5Clambda%20u%7Ddu%0A%5Cend%7Balign%2A%7D%0A
"
\\begin{align*}
    F_{cX}(x) &= \\int_{0}^{x}\\frac{1}{\\Gamma(n/2)}\\left(\\frac{1}{2}\\right)^{n/2}\\frac{1}{c}\\left(\\frac{u}{c}\\right)^{n/2 - 1}e^{-u/2c}du \\\\
        &= \\int_{0}^{x}\\frac{1}{\\Gamma(n/2)}\\left(\\frac{1}{2c}\\right)^{n/2 - 1}\\left(\\frac{1}{2c}\\right)u^{n/2 - 1}e^{-u/2c}du \\\\
        &= \\int_{0}^{x}\\frac{1}{\\Gamma(n/2)}\\left(\\frac{u}{2c}\\right)^{n/2 - 1}\\left(\\frac{1}{2c}\\right)e^{-u/2c}du \\\\
        &= \\int_{0}^{x}\\frac{1}{\\Gamma(\\alpha)}(\\lambda u)^{n/2 - 1}\\lambda e^{-\\lambda u}du
\\end{align*}
")  

Este ultimo resultado corresponde a la función de distribución
![Gamma(\\alpha,
\\lambda)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Gamma%28%5Calpha%2C%20%5Clambda%29
"Gamma(\\alpha, \\lambda)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-28-1.png" style="display: block; margin: auto;" />

29. Para las distribuciones
    ![t](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;t
    "t") y
    ![F](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;F
    "F") genere muestras aleatorias y los histogramas.

Para la dsitribución
![t](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;t
"t") con 12 grados de libertad:

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-29-1-1.png" style="display: block; margin: auto;" />

Para la dsitribución
![F](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;F
"F") con 3 y 14 grados de libertad:

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/prob-29-2-1.png" style="display: block; margin: auto;" />

# 2 Gráficos de densidad para las distribuciones de probabilidad.

30. Para todas las distribuciones grafique sus densidades. Mostrar estos
    cómputos para todas las distribuciones. Incluyan un *q-q plot* de
    todas las distribuciones y los diagramas de cajas.

Digamos que de cada distribución tomamos ![n
= 500](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;n%20%3D%20500
"n = 500") muestras.

## 2.1 Distribución Uniforme Discreta.

Se simula una Distribución uniforme discreta entre 0 y 10, ![Unif\\{0,
\\ldots, 10\\}](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Unif%5C%7B0%2C%20%5Cldots%2C%2010%5C%7D
"Unif\\{0, \\ldots, 10\\}").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/dicrete-uniform-1.png" style="display: block; margin: auto;" />

## 2.2 Distribución de Bernoulli.

Se simula una Distribución de Bernoulli con probabilidad de éxito de
![0{,}7](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;0%7B%2C%7D7
"0{,}7"),
![Ber(p=.7)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Ber%28p%3D.7%29
"Ber(p=.7)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/bernoulli-1.png" style="display: block; margin: auto;" />

## 2.3 Distribución Binomial.

Se simula una Distribución de Binomial con probabilidad de éxito de
![0{,}7](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;0%7B%2C%7D7
"0{,}7") y tamaño
![13](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;13
"13"), ![Bin(n=13,
p=.7)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Bin%28n%3D13%2C%20p%3D.7%29
"Bin(n=13, p=.7)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/binomial-1.png" style="display: block; margin: auto;" />

## 2.4 Distribución Geométrica.

Se simula una Distribución Geométrica con probabilidad de éxito de
![0{,}4](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;0%7B%2C%7D4
"0{,}4"),
![Geo(p=.4)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Geo%28p%3D.4%29
"Geo(p=.4)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/geometrica-1.png" style="display: block; margin: auto;" />

## 2.5 Distribución Binomial Negativa.

Se simula una Distribución de Binomial con probabilidad de éxito de
![0{,}5](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;0%7B%2C%7D5
"0{,}5") y numero de éxitos igual a
![5](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;5
"5"), ![BinNeg(r=5,
p=.5)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;BinNeg%28r%3D5%2C%20p%3D.5%29
"BinNeg(r=5, p=.5)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/binomial-negativa-1.png" style="display: block; margin: auto;" />

## 2.6 Distribución Hipergeométrica.

Se simula una Distribución de Hipergeométrica con tamaño de muestra 5, y
en la que se tienen 8 elementos de un tipo y 13 del otro tipo,
![Hypergeo(k=8, m=13,
n=5)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Hypergeo%28k%3D8%2C%20m%3D13%2C%20n%3D5%29
"Hypergeo(k=8, m=13, n=5)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/hipergeometrica-1.png" style="display: block; margin: auto;" />

## 2.7 Distribución de Poisson.

Se simula una Distribución de Poisson con parámetro de escala igual a 5,
![Pois(\\lambda=5)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Pois%28%5Clambda%3D5%29
"Pois(\\lambda=5)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/poisson-1.png" style="display: block; margin: auto;" />

## 2.8 Distribución uniforme continua.

En este caso se simula una Distribución uniforme continua entre 0 y 1,
![Unif(0, 1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Unif%280%2C%201%29
"Unif(0, 1)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/uniforme-continua-1.png" style="display: block; margin: auto;" />

## 2.9 Distribución Exponencial.

Se simula una Distribución Exponencial con parámetro igual a 2,
![exp(\\lambda=2)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;exp%28%5Clambda%3D2%29
"exp(\\lambda=2)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/exponencial-1.png" style="display: block; margin: auto;" />

## 2.10 Distribución Gamma.

Se simula una Distribución Gamma con parámetro de forma igual a 5 y
parámetro de escala igual a 3, ![Gamma(\\alpha=5,
\\lambda=3)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Gamma%28%5Calpha%3D5%2C%20%5Clambda%3D3%29
"Gamma(\\alpha=5, \\lambda=3)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/gamma-1.png" style="display: block; margin: auto;" />

## 2.11 Distribución Beta.

Se simula una Distribución Beta con parámetro de forma igual a 6 y 2,
![Beta(a=6,
b=2)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Beta%28a%3D6%2C%20b%3D2%29
"Beta(a=6, b=2)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/beta-1.png" style="display: block; margin: auto;" />

## 2.12 Distribución de Weibull.

Se simula una Distribución Weibull con parámetro de forma igual a 2 y
parámetro de escala igual a 1, ![Weibull(\\alpha=2,
\\lambda=1)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;Weibull%28%5Calpha%3D2%2C%20%5Clambda%3D1%29
"Weibull(\\alpha=2, \\lambda=1)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/weibull-1.png" style="display: block; margin: auto;" />

## 2.13 Distribución Normal.

Se simula una Distribución Normal con media 5 y varianza
![0{,}64](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;0%7B%2C%7D64
"0{,}64"), ![N(\\mu=5,
\\sigma^2=.64)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;N%28%5Cmu%3D5%2C%20%5Csigma%5E2%3D.64%29
"N(\\mu=5, \\sigma^2=.64)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/normal-1.png" style="display: block; margin: auto;" />

## 2.14 Distribución Chi-Cuadrado.

Se simula una Distribución Chi-Cuadrado con 3 grados de libertad,
![\\chi^2(\\gamma=3)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;%5Cchi%5E2%28%5Cgamma%3D3%29
"\\chi^2(\\gamma=3)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/chi-cuadrado-1.png" style="display: block; margin: auto;" />

## 2.15 Distribución ![t](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;t "t")-Student.

Se simula una Distribución
![t](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;t
"t")-Student con 4 grados de libertad,
![t(\\gamma=4)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;t%28%5Cgamma%3D4%29
"t(\\gamma=4)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/t-student-1.png" style="display: block; margin: auto;" />

## 2.16 Distribución ![F](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;F "F").

Se simula una Distribución
![F](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;F
"F") con 4 y 10 grados de libertad, ![F(\\gamma\_1=4,
\\gamma\_2=10)](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;F%28%5Cgamma_1%3D4%2C%20%5Cgamma_2%3D10%29
"F(\\gamma_1=4, \\gamma_2=10)").

<img src="Tarea-1-Prob-Stat-2022_files/figure-gfm/f-1.png" style="display: block; margin: auto;" />

31. También calculen los coeficientes de Asimetría y kurtosis para todas
    las muestras de las distribuciones y explique.

Los coeficientes de asimetría y kurtosis para cada una de las
distribuciones se muestran en la siguiente tabla:

| Distribución      | Kurtosis | Sesgo o Asimetría |
| :---------------- | -------: | ----------------: |
| Uniforme Discreta |    1.813 |             0.066 |
| Bernoulli         |    1.753 |           \-0.868 |
| Binomial          |    2.865 |           \-0.251 |
| Geometrica        |    8.958 |             2.087 |
| Binomial Negativa |    4.136 |             0.961 |
| Hipergeometrica   |    2.690 |             0.048 |
| Poisson           |    3.093 |             0.483 |
| Uniforme Continua |    1.725 |             0.013 |
| Exponencial       |    9.255 |             2.047 |
| Gamma             |    3.548 |             0.714 |
| Beta              |    2.959 |           \-0.650 |
| Weibull           |    3.189 |             0.596 |
| Normal            |    2.954 |             0.058 |
| Chi-Cuadrado      |    5.692 |             1.493 |
| t-Student         |    7.189 |             0.024 |
| F                 |   27.353 |             3.835 |

El coeficiente de asimetría es aproximadamente cero para la distribución
normal y
![t](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;t
"t")-Student, lo cual se espera dado que estas son simétricas. Las
distribuciones normales también tiene asimetría nula, y la
hipergeométrica, lo cual indica que con los parámetros usados la
distribución es bastante simétrica con respecto a la media. La kurtosis
para estas distribuciones muestran que para la normal e hipergeométrica,
las distribuciones son mesokurticas (kurtosis cercana a 3), la
![t](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;t
"t")-Student es leptokurtica (kurtosis mayor a 3) lo cual indica un pico
agudo para esta distribución, y las uniformes son platikurticas
(kurtosis menor a 3).

Los mayores valores de asimetría se obtuvieron para la distribución
![F](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;F
"F"), seguido de la exponencial y geométrica (aproximadamente 2), y la
Chi-Cuadrado (aproximadamente
![1{,}5](https://latex.codecogs.com/png.image?%5Cdpi%7B110%7D&space;%5Cbg_white&space;1%7B%2C%7D5
"1{,}5")). Estas son las que muestran el mayor sesgo, con las
observaciones acumulándose a la izquierda, por debajo de la media. Al
igual que antes, la kurtosis es variable al igual que antes, pero en
todos los casos es mucho mayor a 3, indicando que todas estas
distribuciones tienen un pico agudo.

Para los parámetros usados, las distribuciones Gamma, Weibull y Poisson
son mesokurticas (kurtosis aproximadamente 3), y tienen coeficientes de
asimetría similares también: positivos y menores a 1, lo cual indica que
el sesgo es pequeño. La binomial negativa tiene una kurtosis un poco
mayor 3 indicando que su pico no es tan pronunciado, y su sesgo es
también positivo y similar al de las distribuciones Gamma, Poisson y
Weibull.

Finalmente, las únicas distribuciones que muestran sesgo negativo son la
beta, la binomial y la de Bernoulli, las primeras dos con kurtosis
cercana a 3, y la de Bernoulli con una kurtosis mas cercana a una
platikurtica.

<!---rmarkdown::render("Tarea-1-Prob-Stat-2022.Rmd", "rdocx_document")--->

<!---rmarkdown::render("Tarea-1-Prob-Stat-2022.Rmd", "pdf_document")--->
