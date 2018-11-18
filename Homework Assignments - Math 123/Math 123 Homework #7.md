Renee Senining

Math 123

### Homework #7

#### Chapter 17, exercises 3, 4, 8, 12, and 14.

##### Ex. 3:

Let 

$x' = y$ 

$y' = -x$ 

$X_0 = (x(0), y(0)) = (1, 0)$ 

We now have the system:

$X' = \begin{pmatrix} 0 & 1 \\ -1 & 0 \end{pmatrix}X$ , with $X_0 = \begin{pmatrix} 1 \\ 0 \end{pmatrix}$ 

We have $i$ as an eigenvalue, 

and so the general solution is

$X(t) = x_0\begin{pmatrix} \cos t \\ -\sin t \end{pmatrix} + y_0\begin{pmatrix} \sin t \\ \cos t \end{pmatrix}$

and using the initial condition, the solution to the initial value problem:

$(\cos t, -\sin t)$ 

Using the Picard Iteration:

$u_0(t) = (1,0)$ 

$u_1(t) = (1,0) + \int_0^t F(1,0) ds = (1,0) + \int_0^t (0, -1) ds = \begin{pmatrix} 1\\-t \end{pmatrix}$

$u_2(t) = (1,0) + \int_0^t (-s, -1) ds$ $= \begin{pmatrix} 1 - \frac{t^2}{2} \\ -t \end{pmatrix} $

$u_3(t) = (1,0) + \int_0^t (-s, -1 + s^2/2) ds = \begin{pmatrix} 1 -t^2/2 \\ -t + t^3/3!\end{pmatrix}$

$u_4(t) = (1,0) + \int_0^t (-s + s^3/3!, -1+s^2/2) ds$ $= \begin{pmatrix} 1 -t^2/2 + t^4/4! \\ -t + t^3/3! \end{pmatrix}$ 

I want to show $u_k = \begin{pmatrix} \sum_{i=0} ^{\lfloor k/2\rfloor} (-1)^i \frac{t^{2i}}{(2i)!} \\ \sum_{i=1}^{\lceil k/2 \rceil} (-1)^{i} \frac{t^{2i-1}}{(2i-1)!} \end{pmatrix}$ 

We know this is true for the case $k = 0$, $u_0(t) = (1, 0)$ 

so $u_{k+1}(t) = u_0(t) + \int_0^t F(u_{k}(s)) ds$

Using Inductive Step, we assume $u_k(t) = u_k = \begin{pmatrix} \sum_{i=0} ^{\lfloor k/2\rfloor} (-1)^i \frac{t^{2i}}{(2i)!} \\ \sum_{i=1}^{\lceil k/2 \rceil} (-1)^{i} \frac{t^{2i-1}}{(2i-1)!} \end{pmatrix}$ 

and we end up with $u_{k+1}(t) = u_0(t) + \int_0^t \begin{pmatrix}  \sum_{i=1}^{\lceil k/2 \rceil} (-1)^{i} \frac{s^{2i-1}}{(2i-1)!}\\  -\sum_{i=0} ^{\lfloor k/2\rfloor} (-1)^i \frac{s^{2i}}{(2i)!} \end{pmatrix} ds =\begin{pmatrix} 1 \\ 0 \end{pmatrix} + \begin{pmatrix}   \sum_{i=1}^{\lceil k/2 \rceil} (-1)^{i} \frac{t^{2i}}{(2i)!}\\ \sum_{i=0} ^{\lfloor k/2\rfloor} (-1)^{i+1} \frac{t^{2i+1}}{(2i+1)!} \end{pmatrix}$    

$=  u_{k+1}(t) =\begin{pmatrix}   \sum_{i=0}^{\lceil k/2 \rceil} (-1)^{i} \frac{t^{2i}}{(2i)!}\\ \sum_{i=1} ^{\lfloor k/2\rfloor + 1} (-1)^{i} \frac{t^{2i-1}}{(2i-1)!} \end{pmatrix}$

and $\lfloor (k+1)/2 \rfloor  = \lceil k/2 \rceil$ , $\lceil (k+1)/2 \rceil = \lfloor k/2\rfloor+ 1$ 

so we have $u_{k+1}(t) = \begin{pmatrix}   \sum_{i=0}^{\lfloor (k+1)/2 \rfloor} (-1)^{i} \frac{t^{2i}}{(2i)!}\\ \sum_{i=1} ^{\lceil (k+1)/2\rceil } (-1)^{i} \frac{t^{2i-1}}{(2i-1)!} \end{pmatrix}$ 

so as $k \rightarrow \infin$, 

$u_k(t) \rightarrow (\cos t, - \sin t)$ , by the Existence and Uniqueness Theorem, since $F(x,y) = (-y, x)$ is $C^1$ 

so  $\begin{pmatrix}   \sum_{i=0}^{\infin} (-1)^{i} \frac{t^{2i}}{(2i)!}\\ \sum_{i=1} ^{\infin } (-1)^{i} \frac{t^{2i-1}}{(2i-1)!} \end{pmatrix} = \begin{pmatrix} \cos t \\ -\sin t \end{pmatrix}$ 

##### Ex 4: For each of the following functions, find a Lipschitz constant on the region indicated, or prove there is none:

To find a Lipschitz constant means to find a constant $K$ s.t.

$|F(Y) - F(X)| \leq K|Y-X|$ for all $X, Y $ in the region

this is equivalent to $|\frac{F(Y) - F(X)}{Y-X}| \leq K$ 

###### (a) $f(x) = |x|, -\infin < x < \infin$ 

Using the triangle inequality: 

$|(a-b) + b| \leq |a-b| + |b|$ $\implies$ $|a| - |b| \leq |a-b|$ 

$|(b-a) + a| \leq |b-a| + |a| \implies$ $|b| - |a| \leq |b-a|$ $\equiv |a| - |b| \geq -|a-b|$ 

so $| |a| - |b| | \leq |a-b|$ 

meaning: $| |y| - |x|| \leq |y - x|$  $\equiv$ $|F(y) - F(x)| \leq |y-x|$ , so $K = 1$ 

###### (b) $f(x) = x^{1/3}, -1 \leq x \leq 1$ 

Let $x = 0$, and $y \rightarrow 0$, 

 I will show: $|\frac{f(y) - f(0)}{y-0}|$ $\rightarrow \infin$ as $y \rightarrow 0$, which would mean there is no constant $K$

s.t. $|f(y) - f(0)| \leq K|y-0|$ , so there is no Lipschitz constant on the whole region.

 as $y \rightarrow 0$, $|\frac{f(y)-f(0)}{y-0}| \rightarrow $$\lim_{y \rightarrow 0} |\frac{y^{1/3} }{y}| = \lim_{y\rightarrow 0}\frac{1}{y^{2/3}} \rightarrow \infin$ 

###### (c) $f(x) = 1/x, 1 \leq x \leq \infin$ 

Need to find a constant $K$ s.t.

$|\frac{1}{y} - \frac{1}{x}| \leq K|y - x|$, for all $y, x$ $\in [1, \infin]$ 

$|\frac{1}{y} - \frac{1}{x}| = |\frac{x-y}{yx}|$ 

and since $y, x \geq 1$, $yx \geq 1$ , $|\frac{x-y}{yx}| = \frac{|x-y|}{xy}$

and $\frac{|x-y|}{yx} \leq |x-y|$, since $\frac{1}{xy} \leq 1$ 

###### (d) $f(x,y) = \begin{pmatrix} x+2y \\ -y \end{pmatrix}$, $(x,y) \in \R^2$ 

so let $X_1, X_2 \in \R^2$, 

$|f(X_2) - f(X_1)| = |\begin{pmatrix} x_2 + 2y_2 \\ -y_2 \end{pmatrix} - \begin{pmatrix} x_1 + 2y_1 \\ -y_1 \end{pmatrix}|$ 

$ = |(x_2, -y_2) + (2y_2, 0) - (x_1, -y_1) - (2y_1, 0)|$

and using the triangle inequality, ($\R^2$ is a metric space, metrics have the triangle inequality)

$\leq |(x_2, -y_2) - (x_1, -y_1)| + |(2y_2 - 2y_1, 0)|$  

Looking at each of the summands

1. $|(x_2, -y_2) - (x_1, -y_1)| = |(x_2 - x_1, y_1 - y_2)|$
   1. and since $(y_2 - y_1)^2 = (y_1 - y_2)^2$ we have $|(x_2 - x_1, y_1 - y_2)| = |X_2 - X_1|$  

2. $|(2(y_2 - y_1), 0)| = 2|(y_2 - y_1, 0)|$ 
   1.  $(y_2 - y_1)^2 \leq (y_2 - y_1)^2 + (x_2 - x_1)^2 $ $\equiv$ $|(y_2 - y_1, 0)| \leq |X_2 - X_1|$
   2. $2|(y_2 - y_1, 0)| \leq  2|X_2 - X_1|$  

So we have $|f(X_2) - f(X_1)| \leq 3|X_2 - X_1|$, $K = 3$ 

###### (e) $f(x,y) = \frac{xy}{1+x^2 +y^2}, x^2 + y^2 \leq 4$ 

I want to show $f$ is $C^1$, so I may use that an upper bound for $|Df_x| = |\nabla f|$ is a Lipchitz constant for $f(x,y)$ on $x^2 + y^2 \leq 4$, which is convex (it is a closed ball of radius 2)

$f(x,y)$ has both of its partial derivatives:

$f_x(x,y) = \frac{y-x^2y + y^3}{(1+x^2 +y^2)^2}$, and $f_y(x,y) = \frac{x - xy^2 + x^3}{(1+x^2+y^2)^2}$

sums, products, and quotients of continuous functions are continuous,

and $g(x,y) = x, h(x,y) = y, \text{and } k(x,y) = c$ are continuous 

polynomials are therefore continuous as they are sums and products of $f, g, h$ 

and $f_x, f_y$ are each a quotient of polynomials of two variables, so they are continuous  (and the denominator is never 0 on the region $x^2 + y^2 \leq 4$)

so $f$ is $C^1$ 

$|\nabla f| = \sqrt{f_x^2 + f_y^2}$ 

this is equal to the square root of

$\frac{x^2 + y^2 -x^4y^2-x^2y^4 +x^6 y^6 + 2(x^4+y^4)}{(1+x^2+y^2)^2}$ 

$|x|, |y| \leq 2$, so roughly, we have

$x^2 + y^2 - x^4y^2 - x^2y^4 + x^6 + y^6 + 2(x^4 + y^4) \leq 4 + 2^7 + 2^6 = 196$

and $1 \leq (1 + x^2 +y^2)^2  \leq 25$

so $|\nabla f|^2 \leq 196 \equiv $$|\nabla f| \leq 14$  , $K = 14$ is a Lipschitz Constant

##### Ex. 8 Let $A(t)$ be a continuous family of $n \times n$ matrices and let $P(t)$ be the matrix solution to the IVP $P' = A(t)P$, $P(0) = P_0$ Show that $\det P(t) = (\det P_0)\exp(\int_0^t \text{Tr }A(s) ds)$ 

$\frac{1}{h}(P(t+h) - P(t)) \rightarrow P'(t) = A(t)P$ as $ h \rightarrow 0$ 

$hA(t)P(t)- (P(t+h) - P(t)) = o(h)$,

​	since $\frac{A(t)P(t)h - P(t+h)+P(t)}{h} \rightarrow 0$ as $h \rightarrow 0$ 

$P(t+h) = hP'(t) + P(t) + o(h) = hA(t)P(t) + P(t) + o(h) = (I + hA(t))P(t) + o(h)$

$\det P(t+h) = \det(I + hA(t))\det P(t) + o(h)$

​	if $M = \begin{pmatrix} a + o(h) & b + o(h) \\ c + o(h) & d + o(h) \end{pmatrix}$, we have the determinant = $ad - bc + do(h) + ao(h) - bo(h) -co(h) \\= \det M+ o(h)$ 

​	so with induction, it would be easy to set that this is the case for $\det P(t+h)$ 

and $I + hA(t) = \begin{pmatrix} 1+ha_{11}(t) & \cdots & ha_{1n}(t) \\ \vdots & \ddots & \vdots \\ ha_{n1}(t) & \cdots & 1 + ha_{nn}(t) \end{pmatrix}$

so the determinant will be $= $ $1 + ha_{11}(t) + ha_{22}(t) + . . .  + ha_{nn}(t) + O(h^2)$ 

$ = 1 + h\text{Trace }A + O(h^2)$ 

​	Proof:

​	Induction on size of square matrix, 

​	obvious for case $1\times 1$  , where the determinant is $1 + ha_{11}(t) + 0$ , 

​	and $ 0 \leq h^2$ whenever $0 \leq |h| < \delta$, for any $\delta > 0$ 

​	and the case $2\times2$ where the determinant is $(1 + ha_{11})(1+ha_{22})- h^2a_{12}a_{21}\\ = 1 + ha_{11}+ ha_{22} + h^2(a_{11}a_{22}-a_{12}a_{21})$ 

​	Suppose this is true for $k\times k$ matrices, and $(k-1)\times(k-1)$ matrices

​	let $B = I + hA$ be a $k+ 1 \times k +1$ matrix , 

​	and let $B_{ij}$ be the matrix without the $i$th row and $j$th column

​	then $\det B = (1+ha_{11}(t))\det B_{11} + \sum_{j=2}^{k+1}(-1)^{1+j}ha_{1j}\det B_{1j}$

​	$\det B_{11} = 1 + h\text{Trace }A_{11} + O(h^2)$ by inductive hypothesis

​	and each $\det B_{1j}$ is going to be a linear combination of the determinant of $(k-1)\times(k-1)$ matrices that have $k - 1$ diagonal entries of the form $1 + ha_{ii} (t)$, where $i \neq 1, i \neq j$ 

​	and all the other entries will be of the form $ha_{il}$, where $i \neq 1, l \neq 1, j$ , and using the inductive hypothesis again, the determinant of this matrix is $(1 + h\text{Trace }A_{12, jl} + O(h^2))$, where $l \neq j$ and these terms get multiplied by $h^2a_{1 j}a_{2 l}$,

​	so the sum will be $O(h^2)$, and we have altogether 

​	$1 + h\text{Trace }A_{11}  + ha_{11}(t) + O(h^2) = 1 + h\text{Trace }A + O(h^2)$ 

so $\det P(t+h) = (1 + h\text{Trace }A + O(h^2)\det P(t)) + o(h)$

and $\frac{d}{dt} \det P(t) = \lim_{h\rightarrow 0}\frac{\det P(t+h) - \det P(t)}{h} - \lim_{h\rightarrow0} \frac{h\text{Trace }A\cdot\det P(t) + O(h^2)\det P(t) + o(h)}{h}  $ 

which $ = \lim_{h\rightarrow 0} \text{Trace A}\cdot \det P(t) + O(h) + o(h)/h$, and $O(h), o(h)/h \rightarrow 0$ as $h \rightarrow 0$ 

so $\frac{d}{dt} \det P(t) = \text{Trace A}\cdot \det P(t)$ , so solving this differential equation, we get

$\det P(t) = C\exp(\int_0^t\text{Trace } A(s) ds)$ , and when $t = 0$, $C = \det P(0) = \det P_0$ , which proves the statement.

##### Ex. 12 Prove the following general fact: If $C \geq 0$ and $u,v:[0, \beta] \rightarrow \R$ are continuous and nonnegative, and $u(t) \leq C + \int_0^t u(s)v(s) ds$ for all $ t \in [0, \beta]$, then $u(t) \leq Ce^{V(t)}$ where $V(t) = \int_0^t v(s) \, ds$ 

Suppose $C > 0$, 

Let $U(t) =  C + \int_0^t u(s)v(s) ds$ , which is greater than $0$ since $u, v$ are nonnegative

$U'(t) = u(t)v(t)$ 

$\frac{U'(t)}{U(t)} = \frac{u(t)v(t)}{U(t)} \leq v(t)$ since $u(t) \leq U(t)$ 

and $\frac{d}{dt} \log U(t) = (1/U(t))U'(t)$ so

$\frac{d}{dt}(\log U(t)) \leq v(t)$ 

$\implies$ $\int_0^t \frac{d}{dt} \log U(s) ds = \log U(t) - \log U(0) \leq \int_0^t v(s) ds$

$\log U(t) \leq \log U(0) + \int_0^t v(s) ds$ 

and $U(0) = C + \int_0^0 u(s)v(s)ds$ $= C$ 

$U(t) \leq \exp(\log C + \int_0^t v(s)ds)$ $= C\exp(\int_0^t v(s)ds)$  

and $u(t) \leq C\exp(\int_0^t v(s)ds)$ 

For the case of $C = 0$

We can construct a sequence of positive real numbers $c_n \rightarrow 0$ as $n \rightarrow \infin$, like $c_n = 1/n$ 

this gives us a sequence $u(t) \leq u_n(t) = c_n + \int_0^t u(s)v(s)ds$, 

and since $c_n > 0$ , using the argument above, this means each $u_n(t) \leq c_ne^{V(t)}$ for each $n \in \N$, 

and as $n \rightarrow \infin$, we have $c_n e^{V(t)} \rightarrow 0$, and so $u_n(t) \leq 0$, meaning $u(t) \leq 0$ 

##### Ex. 14 Let $A(t)$ be a continuous family of $n\times n$ matrices. Let $(t_0, X_0) \in J \times \R^n$ . Then the initial value problem $X' = A(t)X, X(t_0) = X_0$ has a unique solution on all of $J$

This the Corollary of the Theorem on page 399:

Let $ \mathcal{O} \sub \R \times \R^n$ be open and $F: \mathcal{O} \rightarrow \R^n$ a function that is $C^1$ in $X$ and continuous in $t$. If $(t_0, X_0) \in \mathcal{O}$, there is an open interval $J$ containing $t_0$ and a unique solution of $X' = F(t,X)$ defined on $J$ and satisfying $X(t_0) = X_0$ 

The function $F(t, X)$ $ = A(t)X$ is a function that takes $\R \times \R^n \rightarrow \R^n$ 

$F$ is continuous in $t$, since $A(t)$ is continuous

Showing $F$ is $C^1$ in $X$: 

$A(t) = \begin{pmatrix} a_{11}(t) & \cdots & a_{1n}(t) \\ \vdots & \cdots & \vdots \\ a_{n1}(t) & \cdots & a_{nn}(t) \end{pmatrix}$

$A(t)X =  \begin{pmatrix} \sum_{k = 1}^n a_{1k}(t)x_k(t) \\ \vdots \\ \sum_{k=1}^n a_{nk}(t)x_k(t) \end{pmatrix}$  

$DF_X = (\frac{\partial f_i}{\partial x_j}) = \frac{\partial }{\partial x_j}(\sum_{k=1}^n a_{ik}(t)x_k)$ $ = \sum_{k=1}^n \frac{\partial}{\partial x_j}(a_{ik}(t)x_k)$  

the last equality coming from the definition of a derivative being a limit, and the limit of a sum is the sum of the limits.

$= a_{ij}(t)$ 

$DF_X = A(t)$  

and $A(t)​$ is continuous, so $DF_X​$ is continuous.

$A(t)$ is continuous everywhere, and so $DF_X = A(t)$ is continuous everywhere, 

so on any $\mathcal{O}$ $\sub \R\times\R^n$, $F(t,X) = A(t)X$ is $C^1$ in $X$ and continuous in $t$. 

$J$ is an open interval containing $t_0$, and so, if we define $\mathcal{O}$ to be an open set in $\R \times \R^n$ containing $J$, then using the theorem, we have a unique solution for $X' = A(t)X$ defined on $J$ satisfying $X(t_0) = X_0​$ 



 











