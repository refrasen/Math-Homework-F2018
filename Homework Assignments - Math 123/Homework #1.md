Renee Senining

Math 123 Fall 2018

## Homework #1

##### Ex. 5 Consider the family of differential equations

$x' = ax + \sin x$ 

where a is a parameter. 

a. Sketch the phase line when $a = 0$. 

$x' = \sin x$ 

Equilibrium points at $\pi k$ , where $k \in \Z$ 

$x'' = \cos x$ $= \begin{cases} 1 & x = 2k\pi  \\ -1 & x = (2k +1)\pi\end{cases}$

 So if $x = 2k\pi$ it is a source and if $x = (2k+1)\pi$ it is a sink

![1535505282417](C:\Users\Renee\AppData\Local\Temp\1535505282417.png)

b. as $a$ increases from $-1$ to $1$ 

When $a = -1$, we have 1 equilibrium point at x = 0, and it seems to be a sink.

![1535505416076](C:\Users\Renee\AppData\Local\Temp\1535505416076.png)

We keep gaining equilibrium points in quantities of 2 as $a$ increases towards $0$, since

1. For every $a = - (\frac{2}{(4m+1)\pi})$, with $m$ an integer $\geq 0$, we are "adding" one more equilibrium point at $x = \frac{(4m +1)\pi}{2}$, since $ax = -1$ and $\sin \frac{(4m +1)\pi}{2} = 1$

   1. Example: $a =-\frac{2}{5\pi}$ 

   ![1535511200281](C:\Users\Renee\AppData\Local\Temp\1535511200281.png)

2. for any additional equilibrium point x, with $ax + \sin x = 0$, we have $-x$ as an equilibrium point as well: $a(-x) + \sin (-x) = -ax - \sin x = - (ax + \sin x) = 0$, since $ax$ and $\sin x$ are both odd functions. 

   

3. Then once we have $a \in (-\frac{2}{(4m+1)\pi,} -\frac{2}{(4m+5)\pi})$, the equilibrium points at $x = \pm\frac{(4m+1)\pi}{2}$ each split into 2 more equilibrium points.

   Example: $a = -\frac{2}{5\pi} +.01$ ![1535512924376](C:\Users\Renee\AppData\Local\Temp\1535512924376.png)

   And so we keep gaining equilibrium points until we hit $a = 0$ , where we have infinitely many points, as can be seen from part (a).![1535505467376](C:\Users\Renee\AppData\Local\Temp\1535505467376.png)

As we go from $a = 0$ to $a = 1$, we observe a similar phenomenon as that of when $a$ increased from $-1$ to $0$, except that we lose equilibrium points as we $a$ increases, and whenever $a = \frac{2}{(4m+3)\pi}$, with $m$ a nonnegative integer, we have that $x = \pm\frac{(4m+3)\pi}{2}$ are equilibrium points: at these $x$, $ax = \pm 1$ and $\sin x = \mp 1$ so $ax + \sin x = 0$. 

Examples:

$ a = \frac{2}{3\pi}$![1535516036944](C:\Users\Renee\AppData\Local\Temp\1535516036944.png)

$a = \frac{2}{3\pi} +.01$ ![1535516120375](C:\Users\Renee\AppData\Local\Temp\1535516120375.png)

When $a = 1$ only 1 equilibrium point at $x = 0$ and is a source.![1535505505857](C:\Users\Renee\AppData\Local\Temp\1535505505857.png)

(c) The bifurcation diagram:

![1535516997064](C:\Users\Renee\AppData\Local\Temp\1535516997064.png)



##### Ex. 8 Consider a first-order linear equation of the form $x' = ax + f(t)$ where $a \in \R$. Let $y(t)$ be any solution of this equation. Prove that the general solution is $y(t) + c\exp(at)$ where $c \in \R$ is arbitrary. 

Let $w(t)$ be some solution to this equation. 

If we took $\frac{w(t)-y(t)}{e^{at}}$ and took the derivative w.r.t. $t$, since $(f\pm g)' = f' \pm g'$

we get, using product rule, 

 $(aw(t) + f(t) - ay(t) - f(t))(e^{-at}) -ae^{-at}(w(t)-y(t))\\= ae^{-at}(w(t)-y(t))-ae^{-at}(w(t)-y(t)) = 0$

Which means $\frac{w(t)-y(t)}{e^{at}}$ is equal to some constant $c \in \R$ 

so $\frac{w(t)-y(t)}{e^{at}} = c \implies w(t) = y(t) +ce^{at}$ 

##### Ex. 9 Consider a first-order, linear, nonautonomous equation of the form $x'(t) = a(t)x$ 

###### (a) Find a formula involving integrals for the solution of this system. 

$\frac{d x}{d t} = a(t)x \\ \frac{1}{x}d x = a(t)d t \\ \int \frac{1}{x}dx = \int a(t)dt\\$

 $\ln|x| = \int a(t)dt + c$

letting $\exp(c) = C$ 

$x = C\exp[\int a(t)dt]$ 

###### (b) Prove that your formula gives the general solution of this system. 

let $w(t)$ be a solution to this differential equation.

Finding the derivative w.r.t. t of $w(t)\exp[-\int a(t)dt]$:

Using chain rule and product rule, noting the derivative of $\int a(t)dt$ is $a(t)$ 

$ [w(t)\exp[-\int a(t)dt]]' = a(t)w(t)\exp[-\int a(t)dt] -a(t)\exp[-\int a(t)dt]w(t) = 0$ 

so $w(t)\exp[-\int a(t)dt] = C$, where $C$ is an arbitrary real constant, 

$\implies w(t) = C\exp[\int a(t)dt]$, which was my formula from (a).

##### Ex. 11 First-order differential equations need not have solutions that are defined for all times

###### (a) Find the general solution of the equation $x' = x^2$ 

$\frac{dx}{dt} = x^2 \equiv \frac{1}{x^2}dx = dt$ 

$\int \frac{1}{x^2}dx = t + C \\ -\frac{1}{x} = t +C \\ x = -\frac{1}{t+C}$

$x_0 = -\frac{1}{C} \equiv C = -\frac{1}{x_0}$ 

$x = -\frac{1}{t - \frac{1}{x_0}} = -\frac{x_0}{x_0t -1}$

###### (b) Discuss the domains over which each solution is defined

defined over $(-\infin, \frac{1}{x_0})\cup(\frac{1}{x_0}, \infin)$ 

###### (c) Give an example of a differential equation for which the solution satisfying x(0) = 0 is defined only for -1 < t < 1

$x' = -2t\exp[-x]$      $x(0) = 0$ 

A solution for this:

$\int \exp[x]dx = -\int 2t dt$

$\exp[x] = -t^2 + C$

$x(t) = \ln(-t^2+C)$

$x(0) = \ln(C) = 0 \equiv C = 1$

and so $x(t) = \ln(1 - t^2)$,  indeed, $\ln(1-t^2)$ is undefined when $1-t^2 < 0 \equiv t^2 > 1$

which happens when $t < -1$ or when $t > 1$ 

##### Ex. 12. First-order differential equations need not have unique solutions satisfying a given initial condition

###### (a) Prove that there are infinitely many different solutions of the differential equations $x' = x^{1/3}$ satisfying $x(0) = 0$ 

$\int x^{-1/3}dx = dt$

letting $u = x^{1/3}$ we get $\frac{du}{dx} = \frac{1}{3}x^{-2/3} = \frac{1}{3} u^{-2}$

so $dx = 3u^2du$

$3 \int u^{-1}u^2du = 3\int u \, du = \frac{3}{2}u^2 = \frac{3}{2}x^{2/3}$

$\frac{3}{2}x^{2/3} = t + C$

$x(t) = (\frac{2}{3}(t+C))^{3/2}$

Notice: not defined for $t < - C$ 

We extend $x(t)  = \begin{cases} (\frac{2}{3}(t+C))^{3/2} &t \geq -C \\ 0 &t < -C \end{cases}$

This extended function is a solution: if $t \geq -C , x'(t) = (\frac{2}{3}(t+C))^{1/2} = x(t)^{1/3} $

if $t < -C$ $x(t) =0, x'(t) = 0 = 0^{1/3}$ 

It is also differentiable: we know the derivative for $t > -C$ and $t < -C$, but need to make sure limit on the left matches limit on the right.

 $\lim_{h \rightarrow0} \frac{x(-C+h) - x(-C)}{h} $

if $h <0$, $\frac{0 - (\frac{2}{3}\times 0)^{3/2}}{h} = 0$ 

if $h > 0$ $\frac{(\frac{2}{3}h)^{3/2}}{h} = (2/3)^{3/2}\times h^{1/2} \rightarrow(2/3)^{3/2}\times0 = 0$ 

As long as $C < 0$, we have that $t = 0 < -C$, and so $x(0) = 0$ by definition. 

###### (b) Discuss the corresponding situation that occurs for $x' = x/t \;\;\;\;\;\;\;\; x(0) = x_0$ 

$\frac{dx}{dt} = \frac{x}{t}$

$\int x^{-1}dx = \int t^{-1}dt$ 

$\ln|x| = \ln|t| + c_1$

define $C = e^{c_1}$

$|x| = C|t|$

$x = Ct$ is the general solution. (if $x = C|t|$ $x$ is not differentiable at $t = 0$ )

$x(0) = C(0) = 0$, no matter what $C$ equals. so $\forall C, x = Ct $ is a solution. 

###### (c) Discuss the situation that occurs for $x' = x/t^2 \; \; x(0) = 0$ 

$\frac{dx}{dt} = x/t^2$

$\int x^{-1}dx = \int t^{-2} dt$

$\ln|x| = -1/t + c_1$

again $e^{c_1} = C$

$|x| = C\exp[-1/t]$

$x = C\exp[-1/t]$ 

As it is, the function is not continuous at $t = 0$ 

$\lim_{t\rightarrow 0^+} 1/t = \infin$ and so the limit of $\exp[-1/t]$ approaches 0 as $t \rightarrow 0^+$ 

However, as $t \rightarrow 0^-$, the limit of $\exp[-1/t]$ approaches positive infinity.

![1535529747211](C:\Users\Renee\AppData\Local\Temp\1535529747211.png)

We may be able to remedy this by setting $x(t) = 0$ whenever $t \leq 0$ , and when $t > 0$, $x(t) = C\exp[-1/t]$ , the function will be differentiable and a solution:

$t \leq 0$ $x'(t) = 0 = 0/t^2 $ $= x(t)/t^2$

$t > 0$ $x'(t) = (1/t^2)(C\exp[-1/t]) = x(t)/t^2$

So this new function is a solution and differentiable at $t < 0$ and $t > 0$ 

To show differentiability at $t = 0$: 

 $\lim_{h\rightarrow 0^-} \frac{x(h)-x(0)}{h} = \frac{0-0}{h} = 0$

$\lim_{h\rightarrow 0^+} \frac{x(h) -x(0)}{h} = \lim_{h\rightarrow 0^+} \frac{C\exp[-1/h]}{h} = \lim_{h \rightarrow 0^+ \frac{C}{h\exp[1/h]}}$

$\lim_{h\rightarrow 0^+} h\exp[1/h] = \exp[1/h]/(1/h) = \infin^+/\infin^+$

Using L'hospital's rule: $\lim_{h\rightarrow 0^+} \frac{(-1/h^2)\exp[1/h]}{(-1/h^2)} = \exp[1/h] \rightarrow \infin^+$ 

so $\lim_{h\rightarrow 0^+} C/(h\exp[1/h]) \rightarrow C/\infin^+ = 0$

So the limit for $\frac{x(h) -x(0)}{h}$ as $h$ approaches 0 is 0. 

Also, $x(0) = 0$ by definition, so $x(t) = \begin{cases} 0 & t \leq 0 \\ C\exp[-1/t] & t >0\end{cases}]$ a solution for any $C \in \R$, so we have infinitely many solutions for this IVP. 

##### Ex. 13.

###### (a) Suppose $f'(x_0) = 0$. What can you say about the behavior of solutions near $x_0$? Give examples. 

Can't say anything: 

$x = 0$ is an equilibrium point or which $f'(0) = 0$ for each of the following

$x' = -x^3$, $x_0$ is a sink/stable

$x' = x^3$, $x_0$ is a source/unstable

$x' = x^2$, solutions to the left of $x_0$ tend towards $x_0$ and solutions to the right tend away

$x' = 0$ solutions neither tend towards, nor away from $x_0$ 

###### (b) Suppose $f'(x_0)$ and $f''(x_0) \neq 0$, what can you say now?

Rules out $x' = 0$ and $x' = x^3$ 

if the slope is negative to the left of $x_0$ then the slope needs to increase for $f'(x_0)$ to become 0 at $x_0$, so we have $f''(x) > 0$ to the left of $x_0$ . But if we try to make $f'(x)$ negative again when $x$ is to the the right, we need $f''(x) < 0$ when $x$ is to the right of $x_0$ so this means at $x_0$, $f''(x_0) = 0$, a contradiction. So we must have $f'(x)$ go from negative to 0 at $x_0$ to positive, or positive to 0 at $x_0$ to negative using the same logic as before. In other words, as $x$ passes through $x_0$, $f'(x)$ must change signs as it goes through $x_0$ 

so $x_0$ will be an equilibrium point that looks like the case for $x' = x^2$ i.e, it attracts on the left, repels on the right or vice versa. 

###### (c) Suppose $f'(x_0) = f''(x_0) = 0$ but $f'''(x_0) \neq 0$ 

If $f'''(x_0) \neq 0$, then as $f''(x)$ passes through $x_0$, it is going from negative to positive or positive to negative. 

Suppose $f''(x)$ is going from negative to positive ($f'''(x_0) > 0$)

This means for $f'(x_0) = 0$, $f'(x)$ must be decreasing from a positive number at the left of $x_0$ then  hits 0 at $x_0$, but since $f''(x)$ is positive on the right of $x_0$, $f'(x)$ increases on the right of  $x_0$ to become positive again. 

meaning, $f(x)$ must be increasing from a negative number at the left of $x_0$ to hit 0 at $x_0$ then it continues to increase. //looks more like a source

And if $f''(x)$ is going from positive to negative ($f'''(x_0)<0$), using the same logic as earlier, $f(x)$ must b decreasing from the left of $x_0$ and decreasing to the right of $x_0$ //looks more like a sink

##### Ex. 14. Consider the first-order nonautonomous equation $x' = p(t)x$, where $p(t)$ is differentiable and periodic with period $T$. Prove that all solutions of this equation are periodic with period $T$ $\iff$ $\int_0^Tp(s)ds = 0$

In general: 

$dx/dt = p(t)x$

$\int x^{-1}dx = \int p(t) dt$ 

$\ln|x| = \int p(t) dt +c_1$

$|x| = \exp[c_1] \exp[\int p(t)]dt$

with $c_2 = \exp[c_1]$ 

$x(t) = \pm C\exp[\int p(t)]$ , since $C$ is any constant, we can include $\pm$ in it.

Define $P(t) = \int p(t)$ then  $P(t) = \int_0^t p(s)ds + P(0)$

$x(t) =  C\exp[P(0)]\exp[\int_0^t p(s) ds]$

and $x(0) = C\exp[P(0)]$ , so $x(t) = x_0\exp[\int_0^tp(s)ds]$ 

From exercise 9, this is the general solution.

1. Proving $\rightarrow$ 

   Suppose all solution $x(t)$ that satisfy $x' = p(t)x$ also satisfies $x(t+T) = x(t)$ 

   then: $x(T) = x(0)$ 

   $x(T) - x(0) = 0 =  x_0(\exp[\int_0^Tp(s)ds ] - \exp[\int _0^0p(s)ds]) =\\  x_0(\exp[\int_0^Tp(s)ds] -1)$

   so $\exp[\int_0^Tp(s)ds] = 1 \implies \int_0^Tp(s)ds = 0$

2. Proving $\leftarrow$

   Since $p(t)$ is periodic: $\int_t^{t+T}p(s)ds = \int_0^Tp(s)ds$ for all $t$ 

   ​	b/c: $P'(t+T)- P'(t) = p(t+T) - p(t) = 0$

   so: $P(t+T)-P(t)$ is a constant.  And we're assuming $P(T) - P(0) = \int_0^Tp(s)ds = 0$ 

   So $P(t+T) - P(t) = 0$ 

   also from the general solution of the equation, we have that $x(T) = x(0)$ 

   so if we multiply by $x(t)$ on both sides we get:

   $x(t)x(T) = x(0)x(t)$

   $x_0^2\exp[\int_0^tp(s)ds + \int_0^Tp(s)ds] = x_0x(t)]$

   since $\int_t^{t+T}p(s)ds = \int_0^Tp(s)ds$ for all $t$ and cancelling out $x_0$ The right side becomes $x(t)$, and the left side:

   $x_0\exp[\int_0^tp(s)ds+\int_t^{t+T}p(s)ds  ] = x_0\exp[\int_0^{t+T}p(s)ds] = x(t+T)  \implies x(t+T) = x(t)$ 

   ##### Ex. 15: Consider the differential equation $x' = f(t,x)$, where $f(t,x)$ is continuously differentiable in $t$ and $x$. Suppose that $f(t+T,x) = f(t,x)$ for all $t$. Suppose there are constants $p, q$ such that $f(t,p) > 0, f(t,q) <0$ for all $t$. Prove that there is a periodic solution $x(t)$ for this equation with $p < x(0) < q$ 

   I want to prove that the Poincare map is continuous, maps $[p,q]$ to itself, and therefore has a fixed-point, which means there exists a periodic solution with $x(0) \in (p,q)$ 

   Poincare map $P(x_0)$ $= \phi(T, x_0)$ and from section 1.5, we have:

   $P'(x_0) = \exp[\int_0^T\frac{\partial f}{\partial x_0}(s, \phi(s, x_0))ds]$, and since $f$ is continuously differentiable in $x$, $P'$ is defined for all $x_0$, meaning $P$ is differentiable and therefore continuous.

   To show $P$ maps $[p,q]$ to itself, I will need to show $\forall x_0 \in [p, q], P(x_0) \in [p, q]$

   since the derivative of $P'(x_0)$is positive ($\exp$ takes positive values), and $f(t,p) > 0$  and $f(t,q) < q$ for all $t$ 

   we must have not only that $P(p) > p$ and $P(q) < q$, $P(p) <q$ and $P(q) > p$ since $P'(x_0)$ is positive, $P$ is increasing: so $P(q)- P(p) > 0$ AND for $x_0 \in (p,q)$ $p < P(p) < P(x_0) < P(q) < q$

   Therefore, $P$ maps $[p,q]$ to itself. 

   Taking the function $Q(x_0) = P(x_0) - x_0$, 

   $Q(p) = P(p) - p > 0$

   $Q(q) = P(q) - q < 0$ 

   Since the endpoint have different signs, using intermediate value theorem,

   there exists an $x_0 \in (p,q)$ s.t. $Q(x_0) = 0 = P(x_0) - x_0$ $\equiv$ $\exist x_0 \in (p,q)$ s.t. $P(x_0) = x_0$ 

   Thus, there exists a fixed point, and therefore a periodic solution $x(t)$ with $p <x(0) < q$.

   



