# GOAL: Solve Linear Differential Equations



## Basic Theory of LDE

A linear ODE of order $n$ in the dependent variable $y$ and independent variable $x$ is 
$$
a_0(x)\frac{\mathrm{d}^n y}{\mathrm{d}x^n} + ...+ a_{n-1}(x)\frac{\mathrm{d}y}{\mathrm{d}x} +a_n(x)y = F(x), a_0\neq0
$$
in Homogenous, $F(X)=0$

### Initial Value Problem

Solution of $y$ given values of $y^{(n-1)},..,y',y$ at $x_n,..,x_1, x_0 \in [a,b]$ when the differential eq. is valid in $[a,b]$

### Theorem on solutions

An order $n$ ODE has $n$ $LI$ solutions.

### Wronskian

### 

$$
{\displaystyle W(f_{1},\ldots ,f_{n})(x)={\begin{vmatrix}f_{1}(x)&f_{2}(x)&\cdots &f_{n}(x)\\f_{1}'(x)&f_{2}'(x)&\cdots &f_{n}'(x)\\\vdots &\vdots &\ddots &\vdots \\f_{1}^{(n-1)}(x)&f_{2}^{(n-1)}(x)&\cdots &f_{n}^{(n-1)}(x)\end{vmatrix}},\qquad x\in I.}
$$



$LD \iff W=0 \text{ identically}$

