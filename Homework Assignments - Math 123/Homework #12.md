Renee Senining

Math 123

### Homework #12

#### Chapter 13: Exercises 1, 2, 3, 5, 8, 9, and 10

---

##### 1. Which of the following force fields on $\R^2$ are conservative?

###### (a) $F(x, y) = (-x^2, -2y^2)$ 

**conservative**: there is a function $U$ s.t. $F(x,y) = -\text{grad }U(x,y)$ 

$U = \frac{x^3}{3} + \frac{2y^3}{3}$ 

$\frac{\partial U}{\partial x} = x^2$, $\frac{\partial U}{\partial y} = 2y^2$

###### (b) $F(x,y) = (x^2 - y^2, 2xy)$ 

need $\frac{\partial U}{\partial x} = -(x^2 - y^2)$, $\frac{\partial U}{\partial y} = -2xy$ 

$\frac{\partial U}{\partial x} =- x^2 + y^2$ $\implies$ $U(x,y) = -\frac{x^3}{3} + xy^2 + C(y)$

$\frac{\partial U}{\partial y} = 2xy + C'(y)$, 

but we need $\frac{\partial U}{\partial y} = -2xy$, and no choice of $C(y)$ makes this happen as it only depends on $y$ so 

**not conservative** 

###### (c) $F(x,y) = (x,0)$   

$\frac{\partial U}{\partial x} = -x$, $\frac{\partial U}{\partial y} = 0$

$\implies$ $U = -\frac{x^2}{2} + C(y)$

$\frac{\partial U}{\partial y} = C'(y) = 0$

so $U = -\frac{x^2}{2}$ is a function s.t. $F(x,y) = -\text{grad }U(x,y)$ 

**conservative** 

##### 2. Prove that the equation $\frac{1}{r} = \frac{1}{h}(1 + \epsilon \cos \theta)$ determines a hyperbola, parabola, and ellipse when $\epsilon > 1, \epsilon = 1$, and $\epsilon < 1$ respectively$r = \frac{h}{1 + \epsilon \cos \theta}$

$h$ is the latus rectum, which $ = p\epsilon$, where $p$ is the distance from the focus to the directrix

let the focus be origin, and the directrix be $x = d$, for some $d \in \R^+$ , so $p = d$ 

so $r + r\epsilon \cos\theta = h$ $\equiv$ $r = h - r\epsilon \cos \theta = \epsilon (d - r\cos\theta)$ 

squaring both sides: $r^2 = \epsilon^2(d-r\cos\theta)^2$

subbing $x^2 + y^2$ for $r^2$ and $x$ for $r\cos\theta$: $x^2 + y^2 = \epsilon^2(d-x)^2 = \epsilon^2(d^2 - 2dx +x^2)$

$\equiv$ $x^2 + y^2 +2\epsilon^2dx -\epsilon^2x^2 = \epsilon^2d^2$

if **$\epsilon = 1$: $x^2 + y^2 + 2dx - x^2 = d^2 \equiv y^2 +2dx = d^2 $, which is an equation for a parabola.**

However, if $\epsilon \neq 1$, we keep going:

$(1-\epsilon^2)x^2 +2\epsilon^2dx + y^2 = \epsilon^2d^2$ 

$x^2 + \frac{2\epsilon^2d}{1-\epsilon^2}x + \frac{y^2}{1-\epsilon^2} = \frac{\epsilon^2d^2}{1-\epsilon^2}$ $\implies$ 

$(x + \frac{\epsilon^2d}{1-\epsilon^2})^2 - \frac{\epsilon^4d^2}{(1-\epsilon^2)^2} + \frac{y^2}{1-\epsilon^2} = \frac{\epsilon^2d^2}{1-\epsilon^2}$ $\implies$ 

$(x+\frac{\epsilon^2d}{1-\epsilon^2})^2 + \frac{y^2}{1-\epsilon^2} = \frac{\epsilon^2d^2}{(1-\epsilon^2)^2}$ $\implies$ 

if $\epsilon < 1$ $\implies 1 - \epsilon^2 > 0$ 

and with $h = -\frac{\epsilon^2d}{1-\epsilon^2}$, $a^2 = \frac{\epsilon^2d^2}{(1-\epsilon^2)^2}$, $b^2 = \frac{\epsilon^2d^2}{1-\epsilon^2}$  

we have $\frac{(x-h)^2}{a^2} + \frac{y^2}{b^2} = 1$ , an ellipse

if $\epsilon  > 1$, $1 - \epsilon^2 < 0$ 

we have $h$ the same, $a^2$ the same, but $b^2 = -\frac{\epsilon^2d^2}{1-\epsilon^2}$ 

and we obtain $\frac{(x-h)^2}{a^2} - \frac{y^2}{b^2} = 1$, a hyperbola

##### 3. Consider the case of a particle moving directly away from the origin at time $t= 0$ in the Newtonian central force system. Find a specific formula for this solution and discuss the corresponding motion of the particle. For which initial conditions does the particle eventually reverse direction?

