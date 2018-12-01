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

# Math 123 Chapter 13 problem 3

What does a particle moving away from origin at $t=0$ tell us about how the particle is moving in accordance with this central force system?

What are the initial conditions we want to consider?

- is it position and velocity?

This system is conservative and a central force field.

The system without polar coordinates:

$X' = V$ 

$V' = -\frac{X}{|X|^3}$ 

The system with polar coordinates: (when we have the system as above)

$r' = v_r$

$\theta' = v_\theta/r$

$v'_r = -\frac{1}{r^2} + v_\theta^2/r$ 

$v_\theta' = -v_rv_\theta/r$ 

---

$X' = V$

$m_p V' = -gm_sm_p \frac{X}{|X|^3}$ 

so $V' = -gm_s \frac{X}{|X|^3}$, where $m_s = $ $\text{mass of the sun}$

Things to consider as well:

- restrict attention to particles moving in the plane $\R^2$
- Configuration space: $C = \R^2 - \{0\}$ 
- Phase space: $P = (\R^2 - \{0\}\times \R^2)$ 
  - the collection of all tangent vectors at each point $X \in C$ 
- $T_X = \{(X, V)| V \in \R^2\}$ : the tangent plane to the configuration at $X$
- $P = \cup_{X \in C}T_X$

So at each point in the plane $X$, we associate a plane of tangent vectors with it.

Why can we do this again?

-  How does total energy and angular momentum play into this?

Describing each solution curve $(r(t), v(t))$ with $v = r'$ i.e. $(r, v_r)$ 

$r(v)$ (the graph of)

$r' = v_r$

$\frac{dr}{dt} = v_r$

$\frac{d v_r}{dt} = -\frac{1}{r^2} + \frac{v_\theta^2}{r}$ 

$v_\theta' = -\frac{v_rv_\theta}{r}$

$dv_\theta/v_\theta = -\frac{v_r(t)}{r(t)}dt = -\frac{r'(t)}{r(t)}dt$

$\int \frac{1}{v_\theta} dv_\theta = -\int\frac{r'(t)}{r(t)}dt$

$\ln(v_\theta) = -\ln(r) + C$

$v_\theta = Ce^{-\ln(r)} = \frac{C}{r}$, $C = rv_{\theta, 0}$ ?????

$v_\theta^2 = C^2/r^2$, for some constant $C$

 $\frac{dv_r}{dt} = -\frac{1}{r^2} + \frac{C^2}{r^3}$ 

$\frac{dv_r}{dt} = -\frac{r + C^2}{r^3}$

$\frac{dt}{dv_r} = \frac{r^3}{r+C^2}$ 

$\frac{dr}{dt}\frac{dt}{dv_r} = \frac{v_r r^3}{r + C^2}$ 

$\frac{dr}{dv_r} = \frac{v_r r^3}{r + C^2}$  

$x_1' = v_1 \\ x_2'  = v_2 \\ v_1' = -x_1/(x_1^2 + x_2^2)^{3/2} \\ v_2' = -x_2/(x_1^2 + x_2^2)^{3/2}$

$v_1' = -r \cos\theta/r$

$v_2' = -r\sin\theta/r$ 

$(r_0, v_0)$, $r_0 > 0, v_0 > 0$ 

"each solution curve"... so do I try out different $h, l$?

##### 5. Let $F(X)$ be a force field on $\R^3$. Let $X_0, X_1$ be points in $\R^3$ and let $Y(s)$ be a path in $\R^3$ with $s_0 \leq s \leq s_1$, parametrized by arc length $s$, from $X_0$ to $X_1$. The *work* done in moving a particle along this path is defined to be the integral $\int_{s_0}^{s_1} F(y(s))\cdot y'(s)ds$, where $Y'(s)$ is the unit tangent vector to the path. Prove that the force field is conservative if and only if the work is independent of path. In fact, if $F = -\text{grad V}$, then the work done is $V(X_1) -V(X_0)$ 

Assume the force field is conservative:

then there exists a smooth function $U: \R^n \rightarrow \R$ such that 

$F(X) = -\text{grad }U(X) =- (\frac{\partial U}{\partial x_1}(X), \frac{\partial U}{\partial x_2}(X) , \frac{\partial U}{\partial x_3}(X))$ 

$F(y(s))\cdot y'(s) = -\text{grad } U(y(s))\cdot y'(s)$  

$= -\frac{d }{d s}U(y(s))$

$\int_{s_0}^{s_1} F(y(s))\cdot y'(s)ds = \int_{s_0}^{s_1} -\frac{d }{d s}U(y(s))ds$ 

$ = \int_{s_0}^{s_1} - d U(y(s))$ = $\int_{X_0}^{X_1}-dU$  $= -[U(X_1) - U(X_0)]$ , so independent of path, as it doesn't matter which path we take from $X_0$ to $X_1$ since the integral is the same for any path from $X_0$ to $X_1$

Assuming independence of path

$\int_{s_0}^{s_1}F(y(s))\cdot y'(s)ds$, as long as $X_0$ and $X_1$ are the initial and terminal points of any path $y(s)$, the integral is the same

so $\int_{s_0}^{s_1} F(y(s))\cdot y'(s) = \int_{X_0}^{X_1} F(X) dX$

fixing $X_0$, define a function $h(X_1)  = \int_{X_0}^{X_1}F(X)dX$ 

we fix a path $\gamma(s)$ from $X_0$ to $(a, b, c)$ $y(s) = (s, b, c)$, where $s_0 = a$, $s_1 = x_1$ ,for $x_1$  near $a$ 

we have then $h(x_1, b, c) = \int_{\gamma} F(X)dX + \int_{a}^{x_1} F_1(s, b, c)ds$ 

the first integral on the right is a constant, since we fixed $\gamma$, so

$h(x_1, b, c) = \int_a^{x_1}F_1(s, b, c)ds + C$, and by FTC, $\frac{\partial h}{\partial x_1}(a, b, c) = F_1(a, b, c)$

and similarly for the other coordinates

so $\text{grad }h = (F_1, F_2, F_3) = F$ and we let $U = -h$, so $-\text{grad }U = \text{grad }h = F$  

##### 8. The following three problems deal with the two-body problem. Let the potential energy be $U = \frac{gm_1m_2}{|X_2 - X_1|}$ and $\text{grad}_j(U) = (\frac{\partial U}{\partial x_1^j}, \frac{\partial U}{\partial x_2^j}, \frac{\partial U}{\partial x_3^j})$ . Show that the equations for the two-body problem may be written $m_j X_j'' = -\text{grad}_j(U)$  

For the two -body problem, the equations of motion are

$m_1X_1'' = gm_1m_2 \frac{X_2 - X_1}{|X_2-X_1|^3}$ 

$m_2X_2'' = gm_1m_2 \frac{X_1 - X_2}{|X_1-X_2|^3}$ 

We have $ |X_2 - X_1|$ = $\sqrt{\sum_{i = 1}^3(x_i^2- x_i^1)^2}$   

and $|X_1 - X_2|  = \sqrt{\sum_{i=1}^3(x_i^1 - x_i^2)^2}$

so $U = \frac{gm_1m_2}{\sqrt{(x_1^2 - x_1^1)^2 + (x_2^2 - x_2^1)^2 + (x_3^2 - x_3^1)^2}}$ 

and $\frac{\partial U}{\partial x_i^1}= $ $gm_1gm_2 (-\frac{1}{2|X_2 - X_1|^3})(2(x_i^2 - x_i^1))(-1)$ $ = gm_1m_2\large \frac{x_i^2 - x_i^1}{|X_2 - X_1|^3}$ 

and $\frac{\partial U}{\partial x_i^2} = -gm_1m_2\frac{x_i^2 - x_i^1}{|X_2 - X_1|^3}$ $ = gm_1m_2 \large \frac{x_i^1 - x_i^2}{|X_1 - X_2|^3}$  (because $|X_1 - X_2| = |X_2 - X_1|$ )

I think either $U = \frac{gm_1m_2}{|X_1 - X_2|}$ so that the signs are switched. If we do that, then we have the proof. 

##### 9. Show that the total energy $K + U$ of the system is a constant of motion, where $K = \frac{1}{2}(m_1|V_1|^2 + m_2|V_2|^2)$ 

so $E = K + U = \frac{1}{2}(m_1|V_1|^2  + m_2|V_2|^2) + \frac{gm_1m_2}{|X_2-X_1|}$ 

$\dot E = m_1V_1\cdot V_1' + m_2V_2 \cdot V_2'$ $+ \text{grad}_1U\cdot X_1'$ $+ \text{grad}_2U\cdot X_2'$ 

$ = V_1\cdot(-\text{grad}_1U)$ $+ V_2 \cdot (-\text{grad}_2U)$ $+ \text{grad}_1U\cdot V_1$ $+ + \text{grad}_2U\cdot V_2 $

$ = 0$ 

so $E$ is constant

##### 10. Define the angular momentum of the system by $l = m_1(X_1 \times V_1) + m_2(X_2 \times V_2)$ and show that $l$ is also a first integral

$l' = m_1(X_1' \times V_1 + X_1 \times V_1') + m_2(X_2' \times V_2 + X_2 \times V_2')$ 

so $X_i' = V_i$, so $X_i' \times V_i = 0$ 

$l' = m_1(X_1 \times X_1'') + m_2(X_2 \times X_2'')$ 

$X_i''$ are scalar multiples of $X_2 - X_1$  if $i = 1$, $X_1 - X_2$ , if $i = 2$ 

$X_1 \times (X_2 - X_1) = (x_2^1(x_3^2 - x_3^1) - x_3^1(x_2^2- x_2^1), x_3^1(x_1^2 - x_1^1) - x_1^1(x_3^2 - x_3^1), x_1^1(x_2^2 - x_2^1) - x_2^1(x_1^2 - x_1^1))$ $= X_1 \times X_2 + X_1 \times (-X_1)$ = $X_1 \times X_2 - X_1 \times X_1$ $= X_1 \times X_2$ 

and similalry, $X_2 \times (X_1 - X_2) = X_2 \times X_1 = - X_1 \times X_2$ 

and we have

$l' = \frac{gm_1m_2}{|X_2 - X_1|^3}(X_1 \times X_2 - X_1 \times X_2)$ $= 0$ 

so since $l' = 0$, $l$ is constant and thus a first integral