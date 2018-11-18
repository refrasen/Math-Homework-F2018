Renee Senining

Math 123

### Homework #6

#### Chapter 7:  1(a), 2, 5, 6, and 8

##### Ex 1(a) Write out the first few terms of the Picard iteration scheme for each of the following initial value problems. Where possible, find explicit solutions and describe the domain of this solution.

$x' = x + 2$ , $x(0) = 2$ 

$F(x) = x + 2$ 

$u_0(t) = 2$ 

$u_1(t) = 2 + \int_0^t 2 + 2ds = 2 + 4t$ 

$u_2(t) = 2 + \int_0^t 4 + 4s \,ds = $ $2 + 4t + 2t^2 $ 

$u_3(t) = 2 + \int_0^t 4 + 4s + 2s^2\, ds = 2 + 4t + 2t^2 + \frac{2t^3}3$ 

$u_4(t) = 2 + \int_0^t 4 + 4s + 2s^2 + \frac{2s^3}{3} \, ds = $ $2 + 4t + 2t^2 + \frac{2t^3}{3} + \frac{2t^4}{4*3}$  

$ = 4-2 + 4t + \frac{4t}{2!} + \frac{4t^3}{3!} + \frac{4t^4}{4!}$ 

$u_{k}(t) =  4\sum_{i = 0}^{k} \frac{t^i}{i!} - 2$ 

as $k \rightarrow \infin$ $u_k(t) \rightarrow  4e^{t} - 2$ 

This is in fact the solution:

$\frac{dx}{dt} = x + 2$

$\int\frac{1}{x+2} dx = t$ 

$\ln(x+2) = t +C$

since $e^{t+C} = e^Ce^t$, we just let $C = e^C$ 

$Ce^t = x + 2$

$x(t) = Ce^t - 2$ 

and $x(0) = C - 2 = 2$ so $C = 4$ 

the domain is over all real numbers

##### **Ex. 2** Let $A$ be an $n\times n$ matrix. Show that the Picard method for solving $X' = AX$, $X(0) = X_0$ gives the solution $\exp(tA)X_0$ 

$u_0(t) = X_0$

$u_1(t) = X_0 + \int_0^t AX_0 \, ds = X_0 + tAX_0$, since $AX_0$ is a constant vector $\in \R^n$ 

$u_2(t) = X_0 + \int_0^t AX_0 + sA^2X_0 \,ds = $ $X_0 + tAX_0 + \frac{t^2}2 A^2X_0 $ 

$u_3(t) = X_0 + \int_0^t AX_0 + sA^2X_0 + \frac{s^2}{2}A^3X_0 \, ds =$$X_0 + tAX_0 + \frac{t^2}{2}A^2X_0 + \frac{t^3}{3*2}A^3X_0 $ 

so we have $u_k(t) = [\sum_{i= 0}^k \frac{(tA)^i}{i!}]X_0 $

and since $\exp(A) = \sum_{i=0}^\infin \frac{A^i}{i!}$ 

as $k \rightarrow \infin$ $u_k(t) \rightarrow \exp(tA)X_0$ 

##### **Ex. 5** Consider the first-order equation $x' = x/t$ What can you say about solutions that satisfy $x(0) = 0?$ $x(0) = a \neq 0$? 

$ \frac{1}{x}\, dx = \frac{1}{t} \, dt$ 

$\ln(x) = \ln(t) + C$ 

$x = Ce^{\ln(t)}$ 

$x(t) = Ct$  is the general solution

Suppose $y(t)$ is a solution..

let $w(t) = y(t)/t$  

$w' = \frac{y'(t)t - y(t)}{t^2} = \frac{y(t)- y(t)}{t^2} = 0$ 

so $w(t) = y(t)/t = C$, for some constant $C$ $\implies$ $y(t) = Ct$ 

Solutions are of the form: $x(t) = Ct$ and $x(0) = 0$ 

There are no unique solutions satisfying $x(0) = 0$ since for any $C \in \R$ , $x(0) = C*0 = 0$ 

There exist no solutions for $x(0)= a \neq 0$ since for all $C\in \R$, $x(0) = 0$ 

I think this is due to $x/t$ not being continuously differentiable in its derivative with respect to $t$ at $t = 0$ 

for any other $t_0 \neq 0$ 

$x(t_0) = a$ $\implies$ $Ct_0 = a$ $\implies C = \frac{a}{t_0}$ , so there exists unique solutions as long as $t_0 \neq 0$ 

##### **Ex. 6** Discuss the existence and uniqueness of solutions of the equation $x' = x^a$ where $a > 0$ and $x(0) = 0$ 

$x \equiv 0$ will always be a solution.

if $ a = 1$, then we have $x(t) = x_0e^t$ and $x(0) = 0 \implies$  $x_0 = 0$ so $x(0) \equiv 0$ is the only solution

For other values of $a:$ 

$\frac{dx}{dt} = x^a$

$\frac{1}{x^a} dx= dt$ ,  

$-\frac{1}{(a-1)x^{a-1}} = t + C$ 

$-\frac{1}{(a-1)(t+C)} = x^{a-1}$

$x(t) = (-\frac{1}{(a-1)(t+C)})^{\frac{1}{a-1}}$

If $a > 1$ ,  We have that the only solution is $x \equiv 0$ since

​	$x(0) = (-\frac{1}{C(a-1)})^{\frac{1}{a-1}} \neq 0$ , and $C(a-1)$ must "remain" in the denominator due to $1/(a-1) > 0$ and $x(t)$ wouldn't be defined for $C = 0$ or $t = -C$ 

if $ 0 < a < 1$ , $\frac{1}{a-1} < 0$ and moreover, $|a-1| < 1$ , so $|\frac{1}{a-1}| > 1$ 

so we have $x(t) = (-(a-1)(t+C))^{-\frac{1}{a-1}}$ , 

where $-\frac{1}{a-1} > 1$  

and $x(0) = $$(C(1-a))^{-\frac{1}{a-1}}$ 

so if we let $C = 0$, we get another solution: $x(t) = [(1-a)(t)]^{-\frac{1}{a-1}}$ satisfying $x(0) = 0$ 

so only when $a \geq 1$ , i.e, $x^a$ is $C^1$ so we have unique solutions.

##### Ex. 8 Construct an example of a first-order differential equation on $\R$ for which there are no solutions to any initial value problem

$x' = F(x) = \begin{cases} 1 & \text{if } x \in \Q \\ -1 & \text{if } x \in \R\setminus \Q\end{cases}$ , which is not continuous anywhere:

for $0<\epsilon < 1$, and for any $\delta > 0$ 

if $x_0 \in \Q$: $F(x_0) = 1$ and there always exist both rational and irrational numbers $\in (x_0 - \delta, x_0 + \delta)$ 

so there will always exist an $x \in (x_0 - \delta, x_0 + \delta)$ for any $\delta > 0$ s.t. $F(x) = -1 \notin (1 - \epsilon, 1+\epsilon)$ 

For $x_0 \in \R \setminus \Q$ a similar situation occurs

so $F(x)$ is not continuous anywhere, which means, from page 143, 

at any point in the vector field, nearby vectors point in opposing directions.

---

Using Darboux's Theorem:

Let $I$ be a closed interval and $f: I \rightarrow \R$ is differentiable then $f'$ has the intermediate value property

Suppose we have the initial value problem $x' = F(x), x(t_0) = x_0$ where $t_0, x_0 \in \R$ 

Suppose $x(t)$ is a solution to this initial value problem

this means $x(t)$ is differentiable at $t_0$ and depending on $x_0$ has a derivative of $-1$ or $1$ 

let $[a,b]$ with $t_0 \in [a,b]$ be the largest interval $x(t)$ is differentiable over

1. suppose $a = b$ , and since $t_0 \in [a,b]$, $t_0 = a$ so the domain for $x(t)$ is a singleton {$t_0$}

   The derivative of $x(t)$ at $t_0$ does not exist since the limit, $\lim_{t \rightarrow t_0} \frac{f(t) - f(t_0)}{t-t_0}$ , does not exist

   so, we have a contradiction since $x'(t_0) = 1$ or $-1$  depending on $x_0 \in \Q \text{ or }\R\setminus \Q$  

   there is no solution.

2. Otherwise, $a < b$, and we can use the theorem here:

   we can find an interval $[a, c]$ where $a <c \leq b$ and $c \in \Q$ if $a \in \R\setminus\Q$ or $c \in \R\setminus\Q$ if $a \in \Q$ 

​	since irrational and rational numbers are dense in $\R$ 

​	so $x'(a) = -1 < x'(c) = 1$ or $x'(c) = -1 < x'(a) = 1$ 

​	and since $x(t)$ is differentiable over $[a,c]$, according to Darboux's Thm:

​	for any $\lambda \in (-1, 1)$, $\exists d$  $\in (a,c)$ s.t. $x'(d) = \lambda$ 

​	but since $x(t)$ satisfies $x'(t) = F(x)$ for all of $[a,c]$ , we must have 

​	for all $t \in [a,c]$ $x'(t) = 1$ or $x'(t) = -1$ , so we have a contradiction

So there are no solutions.



