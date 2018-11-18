Renee Senining

Math 123

### Homework #10

#### Chapter 10, 1 and 4

##### 1. For each of the following systems, identify all points that lie in either an $\omega$- or an $\alpha$- limit set

###### (a) $r' = r-r^2, \theta' = 1$ 

We have no equilibria except at origin

$r' = 0$ when $r = r^2$, 

so $r = 1$

The unit circle is a periodic solution

when $r > 1$:

$r^2 > r$ $\implies$ $r - r^2 < 0$, so $r' < 0$ 

which means solutions that begin outside the unit disk radially decrease until they get to $r = 1$,

when $r < 1$:

$r^2 < r$ $\implies$ $r - r^2 > 0$, so $r' > 0$ 

so solutions inside the unit disk radially increase until $r = 1$

so we have that all solutions tend towards the unit circle (periodic solution)

$\omega-$limit of all solutions is the periodic solution at the unit circle

if solutions start on the unit circle, their $\alpha$-limits are also the periodic solution on the unit circle

The $\alpha$ limit for solutions that start outside of the unit disk: $\infin$ since when moving backwards, $r' > 0$ 

the $\alpha$ limit for solutions that start inside of the unit disk: origin, since $r' < 0$ when $r < 1$ $\implies r \rightarrow 0$  

###### (b) $r' = r^3 - 3r^2 + 2r, \theta' = 1$ 

again, no equilibria except at origin

$r' = 0$ when $r^3 - 3r^2 + 2r = 0$

so $r(r^2 - 3r + 2) = 0$ $ \equiv$ $r(r-2)(r-1) = 0$

so at $r = 1, r= 2$ we have periodic solutions

for $\omega$-limits:

if $0<r < 1$: 

$(r-2)(r-1) > 0$, so $r' > 0$ 

so solutions that begin inside the unit circle tend towards the unit circle

if $1 < r < 2$

$r-2 < 0$, but $r-1 > 0$ 

so $r' < 0$, so all solutions that begin inside the circle of radius 2 tend towards the unit circle

if $r > 2$, $r' > 0$, so solutions tend towards infinity

When we go backwards in time:

solutions that begin inside the unit circle tend towards origin

solutions that begin outside the unit circle but inside the circle with radius 2 tend towards the circle of radius 2

solutions that begin outside the circle of radius 2 tend towards the circle of radius 2

###### (c) $r' = \sin r$, $\theta = -1$ 

$r' = 0$ whenever $r = \pi + 2\pi k$ or $r = 2\pi k$ for some nonnegative integer $k$ 

the only equilibrium solution is at origin

we have periodic solutions at $\pi + 2\pi k$ and $2\pi k$ for any nonnegative integer $k$ 

if $2\pi k < r < \pi + 2\pi k$, 

$r' > 0$

so solutions that start in this annulus all tend towards the circle with radius $\pi + 2\pi k$ 

if $\pi + 2\pi k < r < 2\pi(k+1)$ 

$r' < 0$ 

so solutions that begin in this annulus tend towards $\pi + 2\pi k$ 

$\omega$ limits are the circles of radius $\pi + 2\pi k$ 

going backwards in time

all solutions tend to some circle with radius $2\pi k$ 

$\alpha$ limits are the circles of radius $2\pi k$ and origin

###### (d) $x' = \sin x \sin y$, $y' = -\cos x \cos y$ 

$x' = 0$:

$x = 0$ mod $2\pi $ or $y = 0$ mod $2\pi$ or $x = \pi $ mod $2\pi$ of $y = \pi$ mod $2\pi$ 

likewise, $y' = 0$ whenever $x$ or $y$ equal $\pi/2$ mod $2\pi$ or $3\pi/2$ mod $2\pi$ 

we have equilibrium at

$(0, \pi /2)$, $(0, 3\pi/2)$, $(\pi, \pi/2)$, $(\pi, 3\pi/2)$ 

$(\pi/2, 0)$, $(\pi/2, \pi)$, $(3\pi/2, 0)$, $(3\pi/2, \pi)$ 

(adding $2\pi k$ for any $k \in \Z$ )

equilibrium points are their own $\omega, \alpha$ sets

$x' < 0$

$0 <x < \pi$ AND $\pi < y < 2\pi$  

Or

$\pi< x < 2\pi$ AND $0 < y < \pi$ 

----

$x' > 0$ 

$0 < x < \pi$  AND $\pi < y < 2\pi$ 

Or

$\pi < x < 2\pi$ AND $\pi < y < 2\pi$ 

(mod $2\pi$)

---

**$y' < 0$** 

$-\pi/2 < x < \pi/2$ AND $-\pi/2 < y < \pi/2$ 

OR

$\pi/2 < x < 3\pi/2$ AND $\pi/2 < y < 3\pi/2$ 

---

**$y' > 0$** 

$-\pi/2 < x < \pi/2$ AND $\pi/2 < y < 3\pi/2$ 

OR

$\pi/2 < x < 3\pi/2$ AND $-\pi/2 < y < \pi/2$ 

(mod $2\pi$)

$(0, \pi/2)$ is a source ($\alpha$)

$(0, 3\pi/2)$ is a sink ($\omega$)

$(\pi, \pi/2)$ is a sink $(\omega$)

$(\pi, 3\pi/2)$  is a source $(\alpha)$ 

$(\pi/2, 0)$ is a saddle ($\omega$ and $\alpha$ )

​	solutions tend towards it *from* the northwest or the southeast

$(\pi/2, \pi)$ is a saddle ($\omega$ and $\alpha$ )

​	solutions tend towards it from the northeast or the southwest

$(3\pi/2, 0)$ is a saddle ($\omega$ and $\alpha$)

​	solutions tend towards it from the northeast or the southwest

$(3\pi/2, \pi)$ is a saddle  ($\omega$ and $\alpha$)

​	solutions tend towards it *from* the northwest or the southeast



