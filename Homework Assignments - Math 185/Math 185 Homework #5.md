Renee Senining

Math 185

### Homework #5

#### Section 3.1

##### Ex. 2: Evaluate $\int_\gamma xy\; dx$ both directly and using Green's theorem, where $\gamma$ is the boundary of the square with vertices at $(0,0), (1,0), (1,1),$ and $(0,1)$ 

Directly:

$\gamma_1(t) = (t, 0), 0 \leq t \leq 1$ $\gamma_2(t) = (1, t), 0 \leq t \leq 1$ $\gamma_3(t) = (1-t, 1), 0 \leq t \leq 1$ $\gamma_4(t) = (0, 1-t), 0 \leq t \leq 1$ 

$P(x,y) = xy$, $Q(x,y) = 0$ 

$\int_0^1(t)(0)dt + \int_0^1(1)(t)(0)dt + \int_0^1(1-t)(1)(-1)dt + \int_0^1(0)(1-t)dt$

$= \int_0^1(t-1)dt$ = $[\frac{t^2}{2} - t]_0^1 = -\frac{1}2$  

$\int_\gamma xy \;dx = \int_0^1\int_0^1-x\; dxdy = \int_0^1-\frac{1}{2}\;dx = -\frac{1}{2} $

##### Ex. 5: Show that $\int_{\partial D}x\; dy$ is the area of $D$, while $\int_{\partial D} y \; dx$ is minus the area of $D$ 

In multivariable calculus, ${\int\int}_D f(x,y) dA$ describes the volume of the solid that lies under the graph of $f$ and above the area of $D$. 

if $f(x,y) = 1$, this gives us the area

and $dxdy = dA$ 

so using Green's Theorem: $\int_{\partial D}x\; dy = \int\int_D 1 dx dy = A$

and $\int_{\partial D} y dx = \int\int_D -1 dxdy = -A$

##### Ex. 7: Show that the formula in Green's theorem is invariant under coordinate changes, in the sense that if the theorem holds for a bounded domain $U$ with piecewise smooth boundary, and if $F(x,y)$ is a smooth function that maps $U$ one-to-one onto another such domain $V$ and that maps the boundary of $U$ one-to-one smoothly onto the boundary of $V$, then Green's theorem holds for $V$. 

We want to show that $\int_{\partial V} P d\xi + Q d\eta = \int \int _D (\frac{\partial Q}{\partial \xi} - \frac{\partial P}{\partial \eta})d\xi\,d\mu$   

$\int_{\partial V} P d\xi = \int_{\partial U} (P\circ F)(\frac{\partial \xi}{\partial x}dx + \frac{\partial\xi}{\partial y}dy)$ 

$\int_{\partial V}Qd\eta = \int_{\partial U}(Q\circ F)(\frac{\partial \eta}{\partial x}dx + \frac{\partial\eta}{\partial y}dy)$ 

$\int_{\partial V} P(\xi, \eta) d\xi + Q(\xi, \eta) d\eta = \int_{\partial U}(P\circ F)(\frac{\partial \xi}{\partial x}dx + \frac{\partial\xi}{\partial y}dy) + (Q\circ F)(\frac{\partial \eta}{\partial x}dx + \frac{\partial\eta}{\partial y}dy) $

$= \int_{\partial U} ((P\circ F)\frac{\partial \xi}{\partial x} + (Q\circ F)\frac{\partial\eta}{\partial x})dx + ((P\circ F)\frac{\partial \xi}{\partial y} + (Q \circ F)\frac{\partial \eta}{\partial y})dy $  

using Green's Theorem

$= \int \int_U \frac{\partial ((P\circ F)\frac{\partial \xi}{\partial y} + (Q \circ F)\frac{\partial \eta}{\partial y})}{\partial x}-\frac{\partial((P\circ F)\frac{\partial \xi}{\partial x} + (Q\circ F)\frac{\partial\eta}{\partial x})}{\partial y}dx\,dy$   

and $P(F(x,y)) = P(\xi(x,y), \eta(x,y))$ and $Q(F(x,y)) = Q(\xi(x,y), \eta(x,y))$ so using chain rule:

$= \int \int_U \frac{\partial \xi}{\partial y}(\frac{\partial P}{\partial \xi}\frac{\partial \xi}{\partial x} + \frac{\partial P}{\partial \eta}\frac{\partial \eta}{\partial x}) + \frac{\partial \eta}{\partial y}(\frac{\partial Q}{\partial \xi}\frac{\partial \xi}{\partial x} + \frac{\partial Q}{\partial \eta}\frac{\partial \eta}{\partial x}) - \frac{\partial \xi}{\partial x}(\frac{\partial P}{\partial \xi}\frac{\partial \xi}{\partial y} + \frac{\partial P}{\partial \eta}\frac{\partial \eta}{\partial y}) - \frac{\partial \eta}{\partial x}(\frac{\partial Q}{\partial \xi}\frac{\partial \xi}{\partial y} + \frac{\partial Q}{\partial \eta}\frac{\partial \eta}{\partial y})$ 

$ = \int \int_U -\frac{\partial P}{\partial \eta}(\frac{\partial \xi}{\partial x}\frac{\partial \eta}{\partial y} -\frac{\partial \eta}{\partial x}\frac{\partial \xi}{\partial y}) + \frac{\partial P}{\partial \xi}(\frac{\partial \xi}{\partial y}\frac{\partial \xi}{\partial x} - \frac{\partial \xi}{\partial x}\frac{\partial \xi}{\partial y}) + \frac{\partial Q}{\partial \eta}(\frac{\partial \eta}{\partial x}\frac{\partial \eta}{\partial y} - \frac{\partial \eta}{\partial x}\frac{\partial \eta}{\partial y}) + \frac{\partial Q}{\partial \xi}(\frac{\partial \xi}{\partial x}\frac{\partial \eta}{\partial y} - \frac{\partial \xi}{\partial y}\frac{\partial \eta}{\partial x}) $ 

And since $\det J_F =\frac{\partial \xi}{\partial x}\frac{\partial \eta}{\partial y} -\frac{\partial \eta}{\partial x}\frac{\partial \xi}{\partial y}$   

$= \int \int_U [\frac{\partial Q}{\partial \xi}(\xi(x,y), \eta(x,y)) -\frac{\partial P}{\partial \eta}(\xi(x,y), \eta(x,y))]\det J_F \;dx\,dy$ 

Letting $R = \frac{\partial Q}{\partial \xi}(\xi, \eta) -\frac{\partial P}{\partial \eta}(\xi, \eta)$ 

and $R\circ F$  $\frac{\partial Q}{\partial \xi}(\xi(x,y), \eta(x,y)) -\frac{\partial P}{\partial \eta}(\xi(x,y), \eta(x,y))$

$ = \int \int_V \frac{\partial Q}{\partial \xi} -\frac{\partial P}{\partial \eta} \; d\xi\,d\eta$ 

So Green's theorem does hold for $V$ 

#### Section 3.2

##### Ex. 2: Show that the differential $\frac{-y dx + x dy}{x^2 + y^2}$, $(x,y) \neq (0,0)$ is closed. Show that it is not independent of path on any annulus centered at 0

$P(x,y) = \frac{-y}{x^2+y^2}$ and $Q(x,y) = \frac{x}{x^2+y^2}$ $P,Q$ not defined when $(x,y) = (0,0)$ 

$\frac{\partial P}{\partial y} = \frac{-(x^2+y^2) + y(2y)}{(x^2+y^2)^2} = \frac{y^2-x^2}{(x^2+y^2)^2}$ 

$\frac{\partial Q}{\partial x} = \frac{x^2+y^2 - 2x^2}{(x^2+y^2)^2} = \frac{y^2-x^2}{(x^2+y^2)^2}$ 

So, we have that the differential is closed.

Let $D$ be the region where $r_1 < x^2 + y^2 < r_2$ with $0 < r_1 < r_2$ 

let $A = (s, 0)$ where $ r_1 < s < r_2$ 

let $B = (0, s)$ 

so let $\gamma_1 = (s\cos \theta, s\sin\theta)$ with $0 \leq \theta \leq \pi/2$ 

let $-\gamma_2 = (s\cos \theta, s \sin \theta)$ with $\pi/2 \leq \theta \leq 2\pi$ 

So we have $\gamma_2$ moving from $A = (s, 0)$ to $B = (0, s)$ 

$\int_{\gamma_1} Pdx + Qdy = \int_0^{\pi/2}\frac{-s\sin\theta}{s^2} (-s\sin\theta) + \frac{s\cos\theta}{s^2}d\theta = \int_0^{\pi/2}\sin^2{\theta} + \cos^2{\theta} d\theta = \int_0^{\pi/2}1d\theta = \pi/2$ 

$\int_{\gamma_2} Pdx + Qdy = \int_{2\pi}^{\pi/2}1d\theta = {-3\pi}/2$ $\neq \pi/2$ 

So even though $\gamma_1$ and $\gamma_2$ go from $A$ to $B$ the line integral along these two paths are not equal.

##### Ex. 5: Let $\gamma_0(t)$ and $\gamma_1(t)$, $0 \leq t \leq 1$ be paths in the slit annulus {$a < |z| < b$}$\setminus (-b, -a)$ from A to B. Write down explicitly a family of paths $\gamma_s(t)$ from $A$ to $B$ in the slit annulus that deforms $\gamma_0$ continuously to $\gamma_1$. 

We can use polar coordinates to describe any $\gamma(t)$ 

so $\gamma_0(t) =(r_0(t)\cos(\theta_0(t)), r_0(t)\sin(\theta_0(t)))$ and $\gamma_1(t) = (r_1(t)\cos(\theta_1(t)), r_1(t)\sin(\theta_1(t)))$ 

where $-\pi <\theta_{0,1}(t) < \pi$  and $a < r_{0,1}(t) < b$ (since the domain is the slit annulus) 

and $r_{0,1}(t), \theta_{0,1}(t)$ are continuous since the paths must be continuous

Define $\gamma_s(t) = (r_s(t)\cos(\theta_s(t)), r_s(t)\sin(\theta_s(t)))$  

In terms of polar coordinates, for any $t$ 

In the $\theta r-$plane, we can look at a line segment from $(\theta_0(t), r_0(t) )$ and $(\theta_1(t), r_1(t))$ 

so: $0 \leq s \leq 1$, $(\theta_0(t), r_0(t)) +s(\theta_1(t)-\theta_0(t), r_1(t)-r_0(t))$ 

$= ((1-s)\theta_0(t) +s\theta_1(t), (1-s)r_0(t)+ sr_1(t))$ 

So we  have at any point $t \in [0,1]$, for any $s \in [0,1]$ :

$(1-s)a + sa = a <(1-s)r_0(t) +sr_1(t) < (1-s)b + sb = b$ 

$\implies$ $a < (1-s)r_0(t) + sr_1(t) < b$

$-\pi = (s-1)\pi-s\pi <(1-s)\theta_0(t) + s\theta_1(t) < (1-s)\pi + s\pi = \pi$ 

$\implies -\pi < (1-s)\theta_0(t) + s\theta_1(t) < \pi$

setting $(\theta_s(t), r_s(t)) = ((1-s)\theta_0(t)+s\theta_1(t), (1-s)r_0(t)+sr_1(t))$ 

so we have $\gamma_s(t) = (r_s(t)\cos(\theta_s(t)), r_s(t)\sin(\theta_s(t)))$ is contained in the annulus for any $s, t \in [0,1]$ 

also when $t=0$ we have 

$(r_0(0)\cos(\theta_0(0)), r_0(0)\sin(\theta_0(0))) = (r_1(0)\cos(\theta_1(0)), r_1(0)\sin(\theta_1(0)))$ $= A$ 

so we have $r_0(0)^2 = r_1(0)^2$ so $r_0(0) = r_1(0)$ 

and $\theta_0(0) = \theta_1(0)$, since $\theta_{0,1}(t) \in (-\pi, \pi)$ 

so $r_s(t) = (1-s)r_0(0) +sr_1(0) = (1-s)r_0(0) +sr_0(0) = r_0(0) = r_1(0)$

and $\theta_s(t) = (1-s)\theta_0(0) +s\theta_1(0) = \theta_0(0) = \theta_1(0)$ 

(and similarly for $t=1$)

so $\gamma_s(t)$ is a path from $A$ to $B$, and since $r_s(t), \theta_s(t)$ are made of products and sums of continuous functions depending on $s$ or $t$ , we have that $\gamma_s(t)$ depends continuously on $s$ and $t$ for $0 \leq s \leq 1$ and $0 \leq t\leq 1$ 

##### Ex. 6: Show that any closed path $\gamma(t), 0 \leq t \leq 1$ in the annulus {$a < |z| < b$} can be deformed continuously to the circular path $\sigma(t) = \gamma(0)e^{2\pi i mt}$, $0 \leq t \leq 1$ for some integer $m$. 

Let $\gamma(t)$ be a closed path, $0 \leq t \leq 1$ in the annulus

It can be continuously deformed to $\sigma(t) = \gamma(0)e^{2\pi i mt}$ if for $0 \leq s \leq1$ there exist paths $\gamma_s(t)$, $0 \leq t\leq1$ , such that $\gamma_s(t)$ depends continuously on $s$ and $t$ for $0 \leq s \leq 1$, $0 \leq t \leq1$ 

We reduce to the case where $|\gamma(t) \equiv |\gamma(0)|$ is constant: $\gamma(t) = |\gamma(0)|e^{i\theta(t)}$

Subdividing $[0,1]$ in such a way that each

$t_j$ denotes each time when the path crosses $\gamma(0)$, and $\theta_j(t)$ represents $\theta(t)$, when $t \in [t_{j-1}, t_j]$ 

so: $t_0 = 0, t_1, . . ., t_n = 1$ , and $\theta_1, . . ., \theta_n$ 

We should have $\theta_j(t_j) = \theta_{j+1}(t_j)$, since $\gamma(t)$ is continuous. 

And each $\theta_j(t_j) - \theta_j(t_{j-1})$ should be equal to $0$,  $2\pi$,  or $-2\pi$, since each $t_j$ represents every time $\gamma(t)$ is at point $\gamma(0)$.

The reason why it must be of multiples $2\pi k$ where $k = -1, 0, \text{or } 1$ is that if $|k| > 1$ , this would imply that $\gamma(t)$ managed to go around the annulus more than once from $t_{j-1}$ to $t_j$, meaning it was at the point $\gamma(0)$ at least once at some $t \in (t_{j-1}, t_j)$, which would contradict that we subdivided the interval $[0,1]$ at each point $t_j$ where $\gamma(t) = \gamma(0)$ 

Therefore, when we add all these $\theta_j(t_j) - \theta_j(t_{j-1})$ values, they should be equal to $2\pi m$ for some $m \in \Z$ 

So using that: 

1. the sum of these equals $2\pi m$, 
2. $\theta_j(t_j) = \theta_{j+1}(t_j)$ and  $t_n = 1, t_0 = 0$ 
3. and $\theta_n(t_n) = \theta(1)$ and $\theta_1(t_0) = \theta(0)$ 

$\theta_n(t_n) - \theta_n(t_{n-1}) + \theta_{n-1}(t_{n-1}) - \theta_{n-1}(t_{n-2}) + . . . , \theta_1(t_1)- \theta_1(t_0) = \\ \theta_n(t_n) - \theta_1(t_0) = \theta(1) - \theta(0) =  2\pi m$

Also we can deform the radius argument of $\gamma(t)$ to $\gamma(0)$ by thinking of $|\gamma(t)|$ and $|\gamma(0)|$ as being two points on the real number line in $(a, b)$ and defining a line segment from $|\gamma(t)|$ to $|\gamma(0)|$ at any $t$, so, $|\gamma(t)| +  s(|\gamma(0)|-\gamma(t)|) =(1-s)|\gamma(t)| + s|\gamma(0)|$ 

---

So we define:

$\gamma_s(t) = (|(1-s)\gamma(t)| + s|\gamma(0)|)e^{i[(1-s)\theta(t) + s(\theta(0) + 2\pi i mt  ])}$

$r_s(t) = |(1-s)\gamma(t)| + s|\gamma(0)|$

$a - sa <|(1-s)\gamma(t)| < b - sb$ , $sa < s|\gamma(0)| < sb$,

adding the two: $a <r_s(t) < b$ 

so, $\gamma_s(t)$ is contained in the annulus and:

$s = 0, \gamma_s(t) = |\gamma(t)|e^{i\theta(t)} = \gamma(t)$ 

$s = 1, \gamma_s(t) = |\gamma(0)|e^{i[\theta(0) + 2\pi mt]} =  \gamma(0)e^{i2\pi i mt} $ 

also for any $s \in [0,1]$, when $t = 0$ 

$\gamma_s(0) = ((1-s)|(\gamma(0))| + s|\gamma(0)|)e^{i[(1-s)\theta(0) + s\theta(0)]}$ $= |\gamma(0)|e^{i\theta(0)} = \gamma(0)$

and when $t=1$ 

$\gamma_s(1) = ((1-s)|\gamma(1)| + s|\gamma(0)|)e^{i[\theta(1) +s(\theta(0)-\theta(1)+2\pi m)]}$

since $\gamma(1) = \gamma(0)$ we have

$r_s(1) = |\gamma(1)| +s (|\gamma(0)| - |\gamma(1)|) = |\gamma(1)|$ 

and $\theta(1) = \theta(0) + 2\pi m$ so $\theta(1) + s(\theta(0)-\theta(1)+2\pi m) = \theta(1)$ 

so $\gamma_s(1) = |\gamma(1)|e^{i\theta(1)} = \gamma(1)$ 

#### Extra Problems

https://math.berkeley.edu/~art/data/F18-185/HW5.pdf

##### 1. Let $P(x,y)dx + Q(x,y)dy$  be a closed differential in the annulus $\Omega =${$z, a < |z| < b$} $\sub \C$ 

###### Using Problem III.2.6 prove that for any closed path $\gamma$ in the annulus we have $\int_\gamma Pdx + Qdy = mI$, $I = \int_C Pdx + Qdy,$ $m \in \Z$ Where C is the circle of radius $\frac{|a| + |b|}2$ oriented counterclockwise 

$\gamma(0) = r(0)e^{i\theta(0)} \equiv (r(0)\cos\theta(0), r(0)\sin\theta(0))$

$\sigma(t) = r(0)e^{i\theta(0) + 2\pi i mt}$ $\equiv$ $(r(0)\cos(\theta(0)+2\pi mt ), r(0)\sin(\theta(0)+2\pi mt))$ 

The circle $C$ is parameterized by $Re^{2\pi i t}$, where $R = \frac{|a| + |b|}2$ 

$\sigma_{s}(t) = [(1-s)r(0) + sR]e^{(1-s)(i\theta(0) + 2\pi it) +s2\pi i t}$ continuously deforms $\sigma_1(t) = r(0)e^{i\theta(0) + 2\pi i t}$ to $C$ 

so $\int_{\sigma_1} Pdx + Qdy = \int_C Pdx + Qdy = I$

Since any closed path $\gamma$ can be deformed continuously to $\sigma(t) = \gamma(0)e^{2\pi i mt}$ 

We have $\int_\gamma Pdx + Qdy = $ $\int_\sigma Pdx + Qdy$ 

Since $\sigma(t) = \frac{m}{|m|}\sigma_1(t)\cup. . . \cup\frac{m}{|m|}\sigma_1(t)$ (|m| times) 

$\frac{m}{|m|}$ gives the sign for $m$ 

we have $\int_\sigma Pdx + Qdy = \frac{m}{|m|}\int_{\sigma_1}Pdx + Qdy + . . . + \frac{m}{|m|}\int_{\sigma_1}Pdx + Qdy$ = $mI$ 

###### Using Problem III.2.2 Show that differential $Pdx + Qdy - I\omega$, where $\omega = \frac{1}{2\pi}\frac{-y dx + x dy}{x^2 + y^2}$ is exact.

Let $\gamma$ be a closed path in the annulus

$\omega$ is a closed differential and using results from problem III.2.2

$\int_\gamma \omega = \int_{\sigma}\omega = \frac{1}{2\pi}\int_{\theta(0)}^{\theta(0)+2\pi m}d\theta = \frac{1}{2\pi}(2\pi m) = m$ 

so, we have for any closed path:

$\int_\gamma Pdx + Qdy - I\omega = 0$, so it is independent of path $\equiv$ exact

##### 2. Note that we have just shown that any closed differential in the annulus can be presented as $Pdx + Qdy = dh + m\omega$, for some $m \in \Z$ a sum of an exact differential and an integer multiple of $\omega$ The same will be true if instead of the annulus $\Omega$ we consider $\C\setminus${$0$}, the complex plane with one point removed.

###### What Will you expect for $\C\setminus{0,1}$, the complex plane with two points removed?

###### More generally, for $\C \setminus${$0, 1, 2, . . ., k$}, the complex plane with $k$ points removed?

For the statement to still be true... as long as it is finitely many points... for any curve, we could probably say it lies in some finite union of domains that are each an annulus, so we consider each subpath that lies in an annulus.

