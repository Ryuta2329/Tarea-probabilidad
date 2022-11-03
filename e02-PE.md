---
title: "Ejercicio de Probabilidad y Estadística"
subtitle: "Ejercicios de Funciones de Distribución."
author: Marcelo J. Molinatti
date: "2022-11-02"
output:
 github_document:
  number_sections: yes
  html_preview: no
 html_document:
  number_sections: yes
  keep_md: yes
 pdf_document:
  keep_tex: yes
  number_sections: yes
 rdocx_document:
  base_format: bookdown::word_document2
  number_sections: yes
  plots:
   align: center
header-includes:
 - \usepackage{amsmath}
 - \usepackage{tikz}
 - \usepackage{pgfplots}
lang: es
---



1. **Ejercicio 2.10**. Considere una variable aleatoria discreta $X$ con función de probabilidad:

$$f(x) = 
    \begin{cases}
        1/3 & \text{si } x = 1, 2, 3; \\
        0   & \text{de otra forma} 
    \end{cases}
$$

Encuentra para los distintos valores para $x$, la función de distribución $F(x)$. Grafica $f(x)$ y  $F(x)$.

El valor de $F(x)$ corresponde a la probabilidad acumulada hasta $x$, de tal forma que se puede definir como:

$$F(x) = P(X\le x) = \sum_{u\le x} f(u) = 
    \begin{cases}
        0 & \text{si } x < 1; \\
        1/3 & \text{si } 1 \le x < 2; \\
        2/3 & \text{si } 2 \le x < 3; \\
        1 & \text{si } x \ge 3
    \end{cases}
$$


```tex
\begin{tikzpicture}
    \draw[step=2.5cm,gray,very thin] (0,0) grid (1,1);
    % Ejes
    \draw[thick,->] (0,0) -- (5,0) node[below, xshift=0pt]{$x$};
    \draw[thick,->, gray!60!white] (0,0) -- (5,0);
    \draw[thick] (0,0) -- (0,2) node[anchor=east] {$1/3$};
    \draw[thick] (0,0) -- (0,4) node[above, xshift=20pt, yshift=-25pt]{$f(x)$};
    \draw[thick,->, gray!60!white] (0,0) -- (0,4);
    % f(x)
    \draw[ultra thick] (0,0) -- (4,0);
    \foreach \x in {1,...,3}{
        \draw[fill=white] (\x,0) circle (0.1);
        \draw[dashed, gray!60!white] (\x,0) -- (\x,2);
        \draw[fill=black] (\x,2) circle (0.1);
    }
\end{tikzpicture}
%
\begin{tikzpicture}
    \draw[step=2.5cm,gray,very thin] (0,0) grid (1,1);
    % Ejes y Leyendas
    \draw[thick,->] (0,0) -- (4,0) node[below, xshift=0pt]{$x$};
    \draw[thick,->, gray!60!white] (0,0) -- (4,0);
    \draw[thick] (0,0) -- (0,3) node[anchor=east] {$1$};
    \draw[thick] (0,0) -- (0,2) node[anchor=east] {$2/3$};
    \draw[thick] (0,0) -- (0,1) node[anchor=east] {$1/3$};
    \draw[thick] (0,0) -- (0,4) node[above, xshift=20pt, yshift=-25pt]{$F(x)$};
    \draw[thick,->, gray!60!white] (0,0) -- (0,4);
    % F(x)
    \draw[ultra thick] (0,0) -- (1,0);
    \draw[ultra thick] (1,1) -- (2,1);
    \draw[ultra thick] (2,2) -- (3,2);
    \draw[ultra thick] (3,3) -- (4,3);
    \foreach \x in {1,...,3}{
        \draw[fill=black] (\x,\x) circle (0.1);
        \draw[fill=white] (\x,\x-1) circle (0.1);
    }
\end{tikzpicture}
```


![Funcion de densidad y de distribucion](e02-PE_files/figure-html/unnamed-chunk-1-1.png)


2. **Ejercicio 2.11.** Considere ahora la variable aleatoria continua $X$ con función de densidad:

$$f(x) = 
    \begin{cases}
        \vert x \vert & \text{si } -1 \le x \le 1; \\
        0   & \text{de otra forma}
    \end{cases}
$$

Encuentra la función de distribución $F(x)$. Grafica $f(x)$ y $F(x)$.

El valor de $F(x)$ corresponde a la probabilidad acumulada hasta $x$, de tal forma que se puede definir como:

$$F(x) = P(X\le x) = \int_{-\infty}^x f(u)du = 
    \begin{cases}
        0 & \text{si } x < -1; \\
        (1-x^2)/2 & \text{si } -1 \le x < 0; \\
        (1+x^2)/2 & \text{si } 0 \le x < 1; \\
        1 & \text{si } x \ge 1
    \end{cases}
$$


```pgfplots
\begin{tikzpicture}
    % F(x)
    \begin{axis}[axis lines = center, xlabel = $x$, ylabel = {$f(x)$},ymax=1.2,ytick={1},xtick={-1,1}]
        \addplot[domain=-1.5:-1, samples=10,color=black, ultra thick]{0};
        \addplot[domain=-1:0, samples=10,color=black, ultra thick]{-x};
        \addplot[domain=0:1, samples=10,color=black, ultra thick]{x};
        \addplot[domain=1:1.5, samples=10,color=black, ultra thick]{0};
        \addplot[color=gray!80!white, style=dashed] coordinates{(-1,0)(-1,1)(1,1)(1,0)};
        \addplot[fill=white,mark=o] coordinates{(1,0)};
        \addplot[fill=white,mark=o] coordinates{(-1,0)};
    \end{axis}
\end{tikzpicture}
%
\begin{tikzpicture}
    % F(x)
    \begin{axis}[axis lines = center, xlabel = $x$, ylabel = {$F(x)$},ymax=1.2,ytick={1},xtick={-1,1}]
        \addplot[domain=-1.5:-1, samples=100,color=black, ultra thick]{0};
        \addplot[domain=-1:0, samples=100,color=black, ultra thick]{(1-x^2)/2};
        \addplot[domain=0:1, samples=100,color=black, ultra thick]{(1+x^2)/2};
        \addplot[domain=1:1.5, samples=100,color=black, ultra thick]{1};
        \addplot[color=gray!80!white, style=dashed] coordinates{(1,0)(1,1)};
        \addplot[color=gray!80!white, style=dashed] coordinates{(0,1)(1,1)};
    \end{axis}
\end{tikzpicture}
```

**Proposición 2.1** Toda función de distribución $F(x)$ satisface las siguientes propiedades:

* $\lim\limits_{x \to \infty} F(x) = 1$

_Dm._: 

* $\lim\limits_{x \to -\infty} F(x) = 0$

_Dm._: 

* Si $x_1 \le x_2$, entonces $F(x_1) \le F(x_2)$

_Dm._: 

* $F(x) = F(x+)$.

_Dm._: 

3. **Ejercicio 2.14**. Sea $X$ una variaqble aleatoria con función de distribución 

$$F(x) = 
    \begin{cases}
        0 & \text{si } x < -1; \\
        1/3 & \text{si } -1 \le x < 0; \\
        2/3 & \text{si } 0 \le x < 1; \\
        1 & \text{si } x \ge 1
    \end{cases}
$$

Como un ejemplo del cálculo de probabilidades usando la función de distribución, verifique los siguientes resultados:

* $P(X \le 1) = 1$.
* $P(X > 0) = 1/3$.
* $P(0 < X \le 1) = 1/3$
* $P(X = 0) = 1/3$.
