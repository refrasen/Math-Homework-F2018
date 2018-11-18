Renee Senining

Math 123

### Homework #9

#### Chapter 8, exercise 3.

#### Chapter 9, exercises 6, 7(a, b), 8(b), 9, 10, 11, 16.

---

##### Chapter 8, exercise 3: Consider a first-order differential equation $x' = f_a(x)$ for which $f_a(x_0) = 0$ and $f_a'(x_0) \neq 0$. Prove that the differential equation $x' = f_{a+\epsilon}(x)$ has an equilibrium point $x_0(\epsilon)$ where $\epsilon \rightarrow x_0(\epsilon)$ is a smooth function satisfying $x_0(0) = x_0$ for $\epsilon$ sufficiently small

rewrite $f_a(x)$ as $f(a, x)$ 

we have $f(a, x_0) = 0$ and $\frac{\partial f}{\partial x}(a, x_0) \neq 0$ 

since $\frac{\partial f}{\partial x}(a, x_0) \neq 0$ (invertible)

Using Implicit Function Theorem:

There exists an open set $U$ of $\R$ containing $a$ such that there is a unique continuously differentiable function $g:U \rightarrow \R$ with $g(a) = x_0$ 

and $f(a, g(a)) = 0$ for all $a \in U$ 

so let $\epsilon > 0$ be sufficiently small so that $a + \epsilon \in U$  

we have that $f(a+\epsilon, g(a+\epsilon)) = 0$ 

so $x_0(\epsilon) = g(a+\epsilon)$ is a point such that $f_{a+\epsilon}(x_0(\epsilon)) = 0$ 

with $x_0(\epsilon) = g(a+\epsilon)$ being the smooth function (since $g$ is continuously differentiable)

satisfying $x_0(0) = g(a+0) = g(a) = x_0$ 

#### Chapter 9

##### 6: Find a strict Liapunov function for the equilibrium point $(0,0)$ of $x' = -2x - y^2 \\ y' = -y - x^2$. Find $\delta > 0$ as large as possible so that the open disk of radius $\delta$ and center $(0,0)$ is contained in the basin of $(0,0)$ 

$L(x,y) = ax^2 + by^2$ 

$\dot L = 2ax*x' + 2byy' = -4ax^2 - 2axy^2 -2by^2 - 2byx^2$

with $a = b= 1$ is a strict Lyapunov function:

$L(0,0) = 0$, $\dot L < 0$ when $(x,y)$ is near origin

$\dot L < 0$ when

$-4x^2 -2xy^2 -2y^2 -2yx^2 < 0$

$\equiv$

$2x^2 + xy^2 + y^2 + yx^2 > 0$ 

$\equiv$

$(2+y)x^2 + (x+1)y^2 > 0$

polar coordinates:

$(2+r\sin\theta)r^2\cos^2\theta + (r\cos\theta + 1)r^2\sin^2\theta > 0$

$2r^2\cos^2\theta + r^3\sin\theta\cos^2\theta + r^3\cos\theta\sin^2\theta + r^2\sin^2\theta > 0$

$r^2(1 + \cos^2\theta + r\sin\theta\cos\theta(\sin\theta + \cos\theta)) > 0$

$r^3(1+\cos^2\theta)(1/r + \frac{(\sin\theta\cos\theta(\sin\theta+\cos\theta))}{1+\cos^2\theta})$

since $r^3(1+\cos^2\theta) > 0$ for all $\theta > 0$

we turn our attention toa

$\frac{(\sin\theta\cos\theta(\sin\theta+\cos\theta))}{1+\cos^2\theta}$

$1 + \cos^2\theta \leq 2$

since $-\sin(\pi/4)\cos(\pi/4) <\sin\theta + \cos\theta < \sin(\pi/4)\cos(\pi/4) \approx 1.414$

and $|\sin(\theta)\cos(\theta)| < 0.5$

we have $\frac{(\sin\theta\cos\theta(\sin\theta+\cos\theta))}{1+\cos^2\theta} \geq -1/2$ 

$\implies$ $1/r > 1/2$ $\equiv r < 2$ 

so $\dot L < 0$ in the open disk with radius 2 centered at origin 

which means no solution (that enters the disk) exists such that $L$ is constant except for the equilibrium point at origin, since $L$ is strictly decreasing

so by Lasalle's Invariance Principle, the disk in contained in the basin of attraction of $(0,0)$

*since for any closed disk with radius $r < 2$, $L$ is strictly decreasing for any solution entering this closed disk

##### 7: For each of the following functions $V(X)$ sketch the phase portrait of the gradient flow $X' = -\text{grad }V(X)$. Sketch the level surfaces of $V$ on the same diagram. Find all of the equilibrium points and determine their type. 

###### (a) $x^2 + 2y^2$ 

$\text{grad }V(X) = (2x, 4y)$

$x' = -2x \\ y' = -4y$ 

![1540888759264](C:\Users\Renee\AppData\Roaming\Typora\typora-user-images\1540888759264.png)

The only equilibrium point: $(0,0)$, and it is a real sink

###### (b) $x^2 - y^2 - 2x + 4y + 5$ 

$\text{grad }V(X) = (2x -2, -2y + 4)$ 

$x' = -2x + 2 \\ y' = 2y - 4$ 

$\frac{1}{-2x+2} dx = dt$

$-\log|-2x+2|/2 = t +C$

$-2x + 2 = e^{-2t + C}$ 

$x = Ce^{-2t} +1$ $x' = -2Ce^{-2t} = -2Ce^{-2t} -2 + 2 = -2x + 2$ 

$y = Ce^{2t} + 2$, $y' = 2Ce^{2t} = 2Ce^{2t} +4 -4 = 2y - 4$

equilibrium points: $(1, 2)$ saddle

the line $y = 2$ is invariant, the line $x = 1$ is invariant

and solutions on $y = 2$ tend towards equilibrium

solutions on $x = 1$ tend away

![1541048964844](C:\Users\Renee\AppData\Roaming\Typora\typora-user-images\1541048964844.png)

##### 8: Sketch the phase portraits for the following systems. Determine if the system is Hamiltonian or gradient along the way. 

###### (b) $x' = y^2 + 2xy \\ y' = x^2 + 2xy$ 

$x' = 0$

$y^2 = -2xy \equiv -2x = y$ (if $y \neq 0$ )

or $y = 0$ 

$y' = 0$

$x^2 = -2xy \equiv -2y = x  $ (if $x\neq 0)$ 

or $x = 0$ 

the only point these two lines intersect at is $(0,0)$ 

8 basic regions: 1st quadrant

$-y/2 < x < 0$           $-x/2 < y < -2x$,           $0 < y < -x/2$ 

3rd quadrant, 
$0 < x < -y/2$           $-2x < y < -x/2$             $-x/2 < y < 0$ 

![1541049000712](C:\Users\Renee\AppData\Roaming\Typora\typora-user-images\1541049000712.png)

All solutions either tend towards infinity or towards $(0,0)$ 

If gradient then:

$\frac{\partial V}{\partial x} = -y^2 -2xy$ $\implies V(x,y) = -y^2x - x^2y +C(y)$

$\frac{\partial V}{\partial y} = -x^2 -2xy = -2xy -x^2 + C'(y)$

$\implies $$C(y) = $ real constant and $V(x,y) = -y^2x - x^2y + C$ 

and along the level curve $-y^2x - x^2y = 0$, which is the union of the $y-$axis, the $x$-axis, and $y = -x$ 

on $y = -x$, $x' = y^2 - 2y^2 = -y^2 \\ y' = y^2 - 2y^2 = -y^2$, so $x' = y'$ and we have the solutions on $y=-x$ going perpendicular to $y=-x$  

and similarly for other level curves:

![1540931902033](C:\Users\Renee\AppData\Roaming\Typora\typora-user-images\1540931902033.png)

If Hamiltonian

$\frac{\partial H}{\partial y} =  y^2 + 2xy$ $\implies$ $H(x,y) = \frac{y^3}{3}+xy^2 +C(x)$

$-y^2 -C'(x) = x^2 + 2xy$, which implies that $C(x)$ is a function of $x$ and $y$ 

so this is a gradient system with $V$ $= -y^2x - x^2y + C$ 

##### 9:  Let $X' = AX$ be a linear system where $A = \begin{pmatrix} a & b \\ c& d \end{pmatrix}$ 

###### (a) Determine conditions on $a, b, c$ and $d$ that guarantee that this system is a gradient system. Give a gradient function explicitly 

$x' = ax + by \\ y' = cx + dy$ 

$\frac{\partial V}{\partial x} = -ax - by $ $\frac{\partial V}{\partial y} = -cx - dy$ 

$V(x,y) = \frac{-ax^2}{2} - bxy +C(y)$

$-bx + C'(y) = -cx - dy$

so $b = c$, $C'(y) = -dy$, so $C(y) = -\frac{dy^2}{2}$ 

$V(x,y) = \frac{-ax^2}{2} -bxy - \frac{dy^2}{2} + C $ , with $b =c$, which makes sense since the linearized system needs to be a symmetric matrix

######  (b) Repeat the previous question for a Hamiltonian system

$\frac{\partial H}{\partial y} = ax + by, \frac{\partial H}{\partial x} = -cx - dy$ 

$H(x,y) = axy + \frac{by^2}{2} + C(x)$ 

$ay + C'(x) = -cx -dy$

$a = -d$, $C'(x) = -cx \implies C(x) = -cx^2/2$

$H(x,y) = axy + \frac{by^2}{2} -\frac{cx^2}{2}$ where $a = -d$ 

which makes sense since eigenvalues are of the form $\pm \lambda$ or $\pm \lambda i$ 

and for that to happen we'd need $a + d = 0$ 

##### 10. Consider the planar system $x' = f(x,y)  y' = g(x,y)$. 

Determine the explicit conditions on $f$ and $g$ that guarantee that this system is a gradient system or a Hamiltonian system.

###### Gradient System

There needs to be a function $V(x,y)$ s.t.

$\frac{\partial V}{\partial x} = -f(x,y)$ and $\frac{\partial V}{\partial y} = -g(x,y)$ 

For a gradient system, the mixed partial derivatives of $V(x,y)$ are equal (it is $C^\infin$) so:

$ \frac{\partial f}{\partial y} = -\frac{\partial^2 V}{\partial y \partial x} = -\frac{\partial ^2 V}{\partial x\partial y} = \frac{\partial g}{\partial x}$

$\frac{\partial f}{\partial y}(X^*) = \frac{\partial g}{\partial x}(X^*)$ 

So if $\frac{\partial f}{\partial y} = \frac{\partial g}{\partial x}$, we have a gradient system 

also: $f$ must be continuously differentiable and $g$ must be continuously differentiable (need to be $C^\infin$ since $V$ must be $C^\infin$)

if $\frac{\partial f}{\partial y} = \frac{\partial g}{\partial x} = 0$, then $f(x,y), g(x,y)$ are functions of $x$ and $y$ respectively and we rewrite

$f(x,y)$ as $f(x)$ and similarly for $g(x,y$ )

then we may set $C'(y) = g(y)$ and therefore: $C(y) = \int_0^y g(t)dt$

$V(x,y) = -\int_0^xf(t)dt - \int_0^yg(t)dt$ is a function whose associated gradient system is the above.

Otherwise,

we let $V(x,y) = -\int f(x,y)dx$ (negative the integral of f w.r.t. to x)

$\frac{\partial V}{\partial x} = -f(x,y)$ by FTC (the partial deriv. of V w.r.t. to x is -f)

and $\frac{\partial V}{\partial y} = -\frac{\partial}{\partial y}[\int f(x,y)dx]$ (the partial deriv. of V w.r.t. to y is negative the integral of f w.r.t. to x)

$\frac{\partial V}{\partial y} = -\int\frac{\partial f}{\partial y}(x,y)dx $ (can switch the order of differentiation and integration since $f$ is continuously differentiable)

$\frac{\partial V}{\partial y} = -\int \frac{\partial g}{\partial x}(x,y)dx$ (replacing partial deriv. f w.r.t. y with partial deriv. g w.r.t. to x from hypothesis)

$\frac{\partial V}{\partial y} = - g(x,y)$ (we obtain partial deriv. of V w.r.t. to y is -g)

So we have that there exists a function $V(x,y)$ s.t. $\frac{\partial V}{\partial x}= -f(x,y)$, $\frac{\partial V}{\partial y} = -g(x,y)$ and the system above is a gradient system for $V$ 

###### For a Hamiltonian System 

The linearized system at an equilibrium point $X^*$ 

$\begin{pmatrix} \frac{\partial f}{\partial x}(X^*) & \frac{\partial f}{\partial y}(X^*) \\ \frac{\partial g}{\partial x}(X^*) & \frac{\partial g}{\partial y}(X^*) \end{pmatrix}$ 

Since Hamiltonian systems have eigenvalues of $\pm \lambda$ or $\pm i\lambda$ 

we need $\frac{\partial f}{\partial x}(X^*) + \frac{\partial g}{\partial y}(X^*) = 0$  

so $\frac{\partial f}{\partial x} = -\frac{\partial g}{\partial y}$ 

$f(x,y) = -\int_0^x \frac{\partial g}{\partial y}(t, y)dt$ 

$g(x,y) = -\int_0^y \frac{\partial f}{\partial x}(x,t)dt$ 

So we have a Hamiltonian system if $f, g$ are $C^\infin$ and $\frac{\partial f}{\partial x} = -\frac{\partial g}{\partial y}$ 

To see this let: $H(x,y) = \int f(x,y) dy$

$\frac{\partial H}{\partial x} = \frac{\partial}{\partial x}[\int f(x,y)dy] = \int \frac{\partial f}{\partial x}(x,y)dy$ since $f$ is $C^\infin$ 

$= \int -\frac{\partial g}{\partial y}(x,y)dy$ $= -g(x,y)$ 

which means $x' = \frac{\partial H}{\partial y}, y' = -\frac{\partial H}{\partial x}$ , the definition of a Hamiltonian system  

##### 11. Prove that the linearization at an equilibrium point of a planar Hamiltonian system has eigenvalues that are either $\pm \lambda$ or $\pm i\lambda$ where $\lambda \in \R$ 

the linearization:

$\begin{pmatrix} \frac{\partial ^2 H}{\partial x \partial y}(X^*) & \frac{\partial ^2 H}{\partial y^2}(X^*) \\ -\frac{\partial^2 H}{\partial x^2}(X^*) & -\frac{\partial^2 H}{\partial y \partial x}(X^*) \end{pmatrix}$  

and since $\frac{\partial^2 H}{\partial x \partial y} = \frac{\partial^2 H}{\partial y \partial x}$ 

so $T = \frac{\partial^2 H}{\partial x \partial y} - \frac{\partial ^2 H}{\partial y \partial x} = 0$ 

so $\implies$ the eigenvalues $\lambda_{1, 2} = \frac{T \pm \sqrt{T^2 -4D}}2$

so $\lambda_{1,2} = \pm \frac{\sqrt{-4D}}{2}$ , where if $D < 0$, $\lambda$'s are real otherwise pure imaginary  

##### 16. A solution $X(t)$ of a system is called recurrent if $X(t_n) \rightarrow X(0)$ for some sequence $t_n \rightarrow \infin$. Prove that a gradient dynamical system has no nonconstant recurrent solutions.

So need to show if $X(t)$ is recurrent, it must be constant

so let $X(t)$ be a solution such that

$\lim_{n \rightarrow \infin} X(t_n) = X(0) = X_0$ for some sequence $t_n \rightarrow \infin$ 

Using the definition:  $\omega$-limit points of a given solutions are points $Z$ such that 

$\lim_{n\rightarrow \infin} X(t_n) = Z$  for some sequence $t_n \rightarrow \infin$ 

so $X_0$ is an $\omega$-limit point

and from the proposition at the bottom page 204, $X_0$ is an equilibrium point

and since the $\omega$-set is invariant

$\phi_t(X_0)$ remains in $\omega$-set for all $t$, which means $\phi_t(X_0)$ is an equilibrium point for all $t$ since $\omega$-limits in gradient systems are equilibrium points

which means $\phi_t(X_0)$ is constant for all $t$ 