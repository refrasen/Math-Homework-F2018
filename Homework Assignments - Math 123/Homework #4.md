Renee Senining

Math 185

### Homework #4

#### Chapter 2, Sec. 5

##### Ex. 2 Show that if $v$ is a harmonic conjugate for $u$, then $-u$ is a harmonic conjugate for $v$ 

Suppose $v$ is a harmonic conjugate for $u$. 

This means that $u$ is harmonic and $v$ is harmonic such that $u+iv$ is analytic.

so: $\frac{\partial ^2 u}{\partial x^2} = -\frac{\partial^2 u}{\partial y^2}$ and $\frac{\partial ^2 v}{\partial x^2} = -\frac{\partial }{\partial x}\frac{\partial u }{\partial y} = -\frac{\partial }{\partial y}\frac{\partial u}{\partial x} = - \frac{\partial^2 v}{\partial y^2}$ 

We need to show that $-u$ is harmonic and $v - iu$ is analytic

and since $\frac{\partial u}{\partial x} = \frac{\partial v}{\partial y}$ , $\frac{\partial u}{\partial y} = -\frac{\partial v}{\partial x}$and $\lim_{\Delta x \rightarrow 0} \frac{(-u)(x + \Delta x, y) - (-u)(x, y)}{\Delta x} = -\frac{\partial u}{\partial x}$ 

and $\lim_{\Delta y \rightarrow 0} \frac{(-u)(x, y+\Delta y) - (-u)(x, y)}{\Delta y} = -\frac{\partial u}{\partial y}$ 

and the partial derivatives of $u$ are continuous, so are the ones for $-u$.

So we have:

$\frac{\partial (-u)}{\partial x} = - \frac{\partial v}{\partial y}$ and $\frac{\partial (-u)}{\partial{y}} = \frac{\partial v}{\partial x}$, this shows $v - iu$ is analytic.

And: $\frac{\partial ^2 (-u)}{\partial x^2} = \frac{\partial }{\partial x}\frac{ \partial (-u)}{\partial x} = -\frac{\partial }{\partial x}\frac{\partial v}{\partial y} = -\frac{\partial }{\partial y}\frac{\partial v}{\partial x} = -\frac{\partial ^2(-u)}{\partial y^2}$ , this shows $-u$ is harmonic

##### Ex. 7 Show that $\log|z|$ has no conjugate harmonic function on the punctured plane $\C$$\setminus${$0$}, though it does have a conjugate harmonic function on the slit plane $\C \setminus(-\infin, 0]$  

Over $D = \C \setminus (-\infin, 0]$ 

letting $u = \log|z|$ so $\frac{\partial u}{\partial x} = \frac{x}{x^2+y^2}$ and $\frac{\partial u}{\partial y} = \frac{y}{x^2+y^2}$ 

and $\frac{\partial ^2 u}{\partial x} = \frac{y^2-x^2}{(x^2+y^2)^2}$ and $\frac{\partial^2 u}{\partial y} = \frac{x^2 - y^2}{(x^2+y^2)^2}$ , so $u = \log|z|$ is harmonic

Taking the integral of $\frac{x}{x^2+y^2}$ w.r.t. to $y$, 

we get $\arctan(y/x) + C(x)$ and then taking the derivative of this with respect to $x$ it can be easily shown that $C'(x) = 0$ if $v$ is a harmonic conjugate to $u$ 

it must be equal to $\arctan(y/x) + C$ where $C$ is a constant $\in \R$ 

and $\arctan(y/x) = Arg(z)$

so $u+iv = Log(z) +iC$   

If we were to extend $u$ to $D = \C \setminus$ {$0$}

$u$ is still continuous, since $|z|$ is continuous over all points in $\C$ and $\log(x)$ is continuous over all $x \in $ $\R$ s.t. $x > 0$  and therefore harmonic.

however, $Arg(z)$ = $\arctan(y/x)$ is not continuous over $\C\setminus${$0$} since

for $x < 0$:

$\lim_{y\rightarrow 0^+}Arg(x+iy) = \pi $

$\lim_{y\rightarrow 0^-}Arg(x+iy) = -\pi $

#### Chapter 2, Sec. 6

##### Ex. 1 Sketch the families of level curves of $u$ and $v$ for the following functions $f = u+iv$ 

###### (a) $f(z) = 1/z$

$f(x+iy) = \frac{1}{x+iy} \times\frac{x-iy}{x-iy} = \frac{x}{x^2+y^2} +i\frac{-y}{x^2+y^2}$ 

$u(x,y) = \frac{x}{x^2 +y^2}$ , $v(x,y) = \frac{-y}{x^2+y^2}$ 

$u(x^2+y^2) = x \\ x^2-\frac{x}{u} + y^2 = 0 \\ (x - \frac{1}{2u})^2 - \frac{1}{4u^2} + y^2= 0 \\ (x-\frac{1}{2u})^2 +y^2 = \frac{1}{4u^2}$ and $v = \frac{-y}{x^2+y^2} \\ x^2+y^2 +\frac{y}{v} = 0 \\ x^2 +(y+\frac{1}{2v})^2 =\frac{1}{4v^2}  $

So the families of level curves of $u$ are going to be circles centered at $(\frac{1}{2u}, 0)$ with radius $|\frac{1}{2u}|$ 

and families of level curves of $v$ are going to be circles centered at $(0, -\frac{1}{2v})$ with radius $|\frac{1}{2v}|$ 

Except at $u = 0, v = 0$, $u = 0$ represents the line $x=0$ and $v = 0$ represents the line $y = 0$ 

![1537073633968](C:\Users\Renee\AppData\Local\Temp\1537073633968.png)

red curves represent $u$ level curves, from $-5 \leq u \leq 5$ increasing by 1

blue curves represent $v$ level curves from $-5 \leq v \leq 5$ increasing by 1

and when $u < 0$ they are circles in the left plane, and when $u > 0$ they are circles in the right plane

when $v < 0$ they are circles in the upper plane and when $v > 0$ they are circles in the lower plane

also smaller magnitudes of $u, v$ correspond to larger circles

So $f$ is conformal whenever $z \neq 0$, since $1/z$ is not defined at $z = 0$ and $f'(z) = -\frac{1}{z^2}$ 

###### (b) $f(z) = 1/z^2$

$f(x+iy) = \frac{1}{(x+iy)^2} = \frac{1}{x^2-y^2+i2xy} = \frac{x^2-y^2}{(x^2-y^2)^2 +(2xy)^2} +i \frac{-2xy}{(x^2-y^2)^2+(2xy)^2}$ 

In terms of $|z|$ and $\arg z = \theta$ , and $(x^2-y^2)^2 +(2xy)^2 = (x^2+y^2)^2 = |z|^4$

$u = \frac{|z|^2(\cos^2\theta - \sin^2\theta)}{|z|^4} = \frac{\cos2\theta}{|z|^2}$

$v = \frac{-2|z|^2\sin\theta\cos\theta}{|z|^4} = -\frac{\sin2\theta}{|z|^2}$ 

$u = c$, $\cos2\theta = c|z|^2 \equiv|z| = \sqrt{\frac{1}{c}\cos2\theta}$ , if $c > 0$ not defined for $\frac{\pi}{4}<\theta<\frac{3\pi}{4}$ and $-\frac{3\pi}{4}<\theta <-\frac{\pi}{4}$  

if $c<0$ not defined for $-\frac{\pi}4 < \theta < \frac{\pi}4$ and $\frac{3\pi}4 < \theta <\frac{5\pi}{4}$ 

$v = c, |z|^2 = -\frac{1}{c}\sin2\theta$, if $c>0$ not defined for $0 < \theta <\frac{\pi}{2} $ and $ -\pi<\theta<- \frac{\pi}2$   

if $c<0$ not defined for $\frac{\pi}{2} < \theta <\pi$ and $-\frac{\pi}2 < \theta < 0$ 

![1537073578236](C:\Users\Renee\AppData\Local\Temp\1537073578236.png)

red curves correspond to $u$, blue curves correspond to $v$ 

and each curve represents an integer from $-3$ to $3$ 

When $u = 0$, we must have $x^2 = y^2$, so the lines $y = x$ and $y=-x$ 

When $v =0$ we must have either $x = 0$ or $y=0$, so the lines $y = 0$ and $x=0$  ($f(z)$ not defined at $(0,0)$)

Conformal everywhere except $z = 0$ 

###### (c) $f(z) = z^6$ 

$f(|z|e^{i\theta}) = |z|^6e^{i6\theta}$ 

$u= |z|^6\cos(6\theta)\\u = c  \implies\\ |z|^6\cos(6\theta) = c \\ |z| = (\frac{c}{\cos(6\theta)})^{1/6}$ 

$v = |z|^6\sin(6\theta) \\ v = c \implies |z|^6\sin(6\theta) = c \\ |z| = (\frac{c}{\sin(6\theta)})^{1/6} $ 

![1537076235153](C:\Users\Renee\AppData\Local\Temp\1537076235153.png)

Red, $u$ curves. Blue, $v$ curves

The radius of the circle at which 6 curves (corresponding to the same $u$ or $v$  value) intersects only once = the value of $u^{1/6}$ or $v^{1/6}$  

and the points $(x,y)$ at which these curves intersect the circle represent a 6th root of $u$ or $iv$ 

The black lines represent the angles $k\frac{\pi}{3}$ where $k \in Z$ 

​	and where it intersects with the curves for $v$ as $v \rightarrow 0$, 

The purple lines represent the angles $\frac{\pi}{12} + k\frac{pi}3$ where $k \in \Z$  

​	and the curves for $u$ as $u \rightarrow 0$ 

and where the black lines intersect with the circle of radius $1$ represents 6th roots of 1

​	the second set of red curves these black lines intersect with represent 6th roots of 2

​	the third set of red curves these black lines intersect with represent 6th roots of 3

and similarly for the purple lines and 6th roots of $ki$ where $k = 1, 2$ or $3$ 

 $f(z) = z^6$ is conformal everywhere except for when $f'(z) = 0$ @ $z=0$ 

##### Ex. 7 For the function $f(z) = z+1/z = u+iv$ sketch the families of level curves of $u$ and $v$ Determine the images under $f(z)$ of 

so $f(z) = (x + \frac{x}{x^2+y^2}) +i(y-\frac{y}{x^2+y^2})$ 

and $u = 0$ $\implies x = 0$ 

If we have $y^2+x^2 = 1-\epsilon$, for some $0 \leq \epsilon \leq 1$ (meaning, (x,y) are on or inside the unit circle)

$u(x,y) = x + \frac{x}{x^2+y^2} = x + \frac{x}{1-\epsilon}$ 

and as $\epsilon \rightarrow 0^+$, we get $u \rightarrow 2x$, so $x = \frac{u}{2}$ 

so for any $|c| \leq 2$ , we can find points $(x,y)$ within or on the unit circle that satisfy $u(x,y) = c$ 

if we restrict $x^2 +y^2 = 1/(c-1)$ , with $c > 2$, we will always have points $(x,y)$ in the unit disk

and $u(x,y) = x + (c-1)x = cx$ 	

$x = u/c$ , if $u > 0$, $x> 0$ 

$y = \pm \sqrt{\frac{1}{c-1} - \frac{u^2}{c^2}}$

and $y = 0$ when $\frac{1}{c-1}-\frac{u^2}{c^2} = 0$

$c^2 -u^2c+u^2$ 

so when $c = \frac{u^2 \pm \sqrt{u^4 - 4u^2}}2$ real when $u^2 \geq 4$

![1537083595070](C:\Users\Renee\AppData\Local\Temp\1537083595070.png)

orange lines correspond to positive $u$ values

​	not pictured: for large $u$ values, we have lines looking like $x = u$  corresponding to this $u$ value

​	because as $x$ grows larger, $\frac{x}{x^2+y^2} \rightarrow 0$ 

red lines correspond to negative $u$ values

and $x=0$ is the line corresponding to $u=0$ 

purples lines correspond to positive $v$ values

blue lines correspond to negative $v$ values

the green line corresponds to $v = 0$ 

As can be seen in the image, for any $u = c$ curve, it will intersect any curve $v$ in and out of the unit circle.

###### the top half of the unit disk $(x^2+y^2 \leq1), y \geq0$

Corresponds to $v \leq 0$ 

and $u \in (-\infin, +\infin)$ 

so the lower plane

###### the bottom half of the unit disk 

Corresponds to $v \geq 0$ 

$u \in (-\infin, +\infin)$ 

the upper plane

###### the part of the upper half plane outside the unit disk

$v > 0$, and $u \in (-\infin, +\infin)$

the upper plane

###### the part of the lower half-plane outside the unit disk

$v<0$, and $u\in(-\infin, +\infin)$ 

the lower plane

#### Chapter 2, Sec. 7                                                                                       

##### Ex. 2 Consider the fractional linear transformation $(1+i, 2, 0) \mapsto (0, \infin, i-1)$. Without referring to an explicit formula, determine the image of the circle ${|z-1| = 1}$, the image of the disk ${|z-1|<1}$ and the image of the real axis

$1+i, 2, 0$ all lie on the circle $|z - 1|=1$ 

so this fractional linear transformation maps the circle to the line passing through origin and $(i-1)$ $(y = -x)$

Since orientation is preserved, all points within the circle are mapped under the line $y=-x$ 

The real line is a circle containing $0$, $2$ and is orthogonal to the circle $|z-1| = 1$ 

Its image will be the circle that contains the points $\infin$ and $i-1$ , so a line passing through $i-1$ that is orthogonal to the line $y = -x$ , so a line with slope $1$ containing the point (-1, 1)

so $(y-1) = (x+1)$, $y = x +2$ 

##### Ex. 8 Show that any fractional linear transformation can be represented in the from $f(z) = (az+b)/(cz+d)$ where $ad-bc = 1$. Is this representation unique?

Suppose $g(z) = (Az + B)/(Cz +D)$ is a fractional linear transformation

with $AD - BC = \alpha$ where $\alpha \neq 0$ 

$(AD-BC)/\alpha = 1$, $(A/\sqrt{\alpha})(D/\sqrt{\alpha}) - (B/\sqrt{\alpha})(C/\sqrt{\alpha}) = 1 $

so we let $a = A/\sqrt{\alpha}, b = B/\sqrt{\alpha}, c = C/\sqrt{\alpha}, d = D/\sqrt{\alpha}$ 

and this still gives the same function:

$g(z)\times 1 = g(z) \times \frac{1/\sqrt{\alpha}}{1/\sqrt{\alpha}}=\frac{(A/\sqrt{\alpha})z + B/\sqrt{\alpha}}{(C/\sqrt{\alpha})z +D/\sqrt{\alpha}}$  

Not unique: we could also do $a = -A/\sqrt{\alpha}$, etc...

so multiplying $g(z)$ by $1 = \frac{-1/\sqrt{\alpha}}{-1/\sqrt{\alpha}}$ will give the same result, different representation and 

$(-A/\sqrt{\alpha})(-D/\sqrt{\alpha}) - (-B/\sqrt{\alpha})(-C/\sqrt{\alpha}) = 1$ 

##### Ex. 11 Two maps$f$ and $g$ are conjugate if there is $h$ such that $g = h\circ f \circ h^{-1}$ . Here the conjugating map is assumed to be one-to-one, with appropriate domain and range. We can think of $f$ and $g$ as the "same" map, after the change of variable $w = h(z)$. A point $z_0$ is a fixed point of $f$ if $f(z_0) = z_0$ Show the following

###### (a) If $f$ is conjugate to $g$, then $g$ is conjugate to $f$. 

Let $f$ be conjugate to $g$ then $\exists$ a map $h$ such that

$g = h\circ f \circ h^{-1}$  then:

$h^{-1} \circ g \circ h = h^{-1}\circ h \circ f \circ h^{-1} \circ h = f$ 

thus, $g$ is conjugate to $f$, with $h^{-1}$ being the conjugating map 

###### (b) If $f_1$ is conjugate to $f_2$ and $f_2$ to $f_3$, then $f_1$ is conjugate to $f_3$ 

We have:

$f_2 = h\circ f_1 \circ h^{-1}$ 

$f_3 = g \circ f_2 \circ g^{-1}$

Substituting $h\circ f_1 \circ h^{-1}$ for $f_2$ :

$f_3 = g\circ h \circ f_1 \circ h^{-1} \circ g^{-1} = (g\circ h) \circ f_1 (g\circ{h})^{-1}$ 

this proves the statement.

###### (c) If $f$ is conjugate to $g$, then $f \circ f$ is conjugate to $g \circ g$, and more generally, the $m$-fold composition $f \circ \cdots \circ f$ ($m$ times) is conjugate to $g \circ \cdots \circ g$ ($m$ times). 

$g = h\circ f \circ h^{-1}$ 

$g \circ g = h\circ f\circ h^{-1} \circ h \circ f\circ h^{-1} = h \circ f \circ f \circ h^{-1}$ 

We can use induction, as we've proven $n=2$, and assuming $(g\circ ... \circ g) = h\circ f ... \circ f\circ h^{-1}$ $k$ times $k>2$, we prove for $k+1$ 

$g\circ \cdots \circ g =(g\circ \cdots \circ g )\circ g $ , ($k$ times)(1 time)

= $(h \circ f \circ . . . \circ f \circ h^{-1})( \circ h \circ f \circ h^{-1} )\\ = h \circ f \circ... \circ f\circ f\circ h^{-1}$ 

So, for any natural number $m$, we have proven the statement

###### (d) If $f$ and $g$ are conjugate, then the conjugate function $h$ maps fixed points of $f$ to the fixed points of $g$. In particular $f$ and $g$ have the same number of fixed points 

Let $z_0$ be any point such that $f(z_0) = z_0$ 

$g = h \circ f \circ h^{-1}$ 

Let $w_0$ be the point such that $h^{-1}(w_0) = z_0 \equiv h(z_0) = w_0$  

then $g(w_0) = h(f(z_0)) = h(z_0) = w_0$ 

So we have that $h$ maps fixed point of $z_0$ to fixed point of $g$ 

and $h^{-1}$ maps fixed point of $g$ to fixed points of $f$ 

##### Ex. 12 Classify the conjugacy classes of fractional linear transformations by establishing the following:

###### (a) A fractional linear transformation that is not the identity has either 1 or 2 fixed points, that is points satisfying $f(z_0) = z_0$ 

$f(z) = \frac{az+b}{cz+d}$ 

$\frac{az+b}{cz+d} = z \\ az + b = cz^2+dz \\ cz^2+(d-a)z-b=0$

if every $z$ made this equal to 0, we'd have $f(z) = z$ for all $z$, but $f$ is not the identity so:

By solving for $z$ we find fixed points, 

if $c \neq 0$: since polynomials of degree 2 have 2 finite roots, we get 2 finite fixed points. 

​	$z = \frac{ a-d \pm \sqrt{(d-a)^2 +4cb}}{2c}$ 

​	If $(d-a)^2 +4cb =0$, we have one root with multiplicity 2

if $c =0$ , we have one finite fixed point, $z = b/(d-a)$ and $z = \infin$ is also a fixed point

​	if $d-a = 0$ and $b\neq 0$ then we only have one fixed point at $\infin$ 

###### (b) If a fractional linear transformation $f(z)$ has two fixed points, then it is conjugate to the dilation $z \mapsto az$ with $a \neq 0$, $a\neq 1$, that is, there is a fractional linear transformation $h(z)$ such that $h(f(z)) = ah(z).$ Is $a$ unique?

Let $f(z)$ have two fixed points: $z_0, z_1$, $f(z_0) = z_0, f(z_1) = z_1$ 

If $f(0) = 0$, $f(\infin) = \infin$ so $f(0) = \frac{b}{d} \implies b =0$ and $\lim_{z\rightarrow \infin} \frac{az}{cz+d} = \frac{a}{c}$, but we need it to be $\infin$, so $c = 0$  and so we have: $f(z) = \frac{az + b}{cz+d} = \frac{az}{d}$, which is a dilation $z \mapsto \frac{a}dz$

$f(z) = \frac{az+b}{cz+d}$ with $\frac{az_i +b}{cz_i +d} =z_i$ $i = 0, 1$ 

So, if we define $h$ to map fixed points of $f$ to 0 and $\infin$, $h^{-1}(0) = z_0$ so $h(z_0) = 0, h^{-1}(\infin)= z_1, h(z_1)=\infin$ 

We have  so $h\circ f\circ h^{-1}(0) = 0$ and $h\circ f \circ h^{-1}(\infin)  = \infin$

so $g = h\circ f \circ h^{-1}$ is a dilation, and $f$ is conjugate to $g$ 

Suppose $g: z \mapsto az$ 

If $g$ is conjugate with another dilation, $j$, then $f$ is conjugate to $j$, meaning, $a$ is not unique

So suppose this is true and $j: z \mapsto Az$, where $A \neq a$

then there exists a map $k$ s.t. $j = k \circ g \circ k^{-1}$ 

And $k$ must map fixed points of $g$ to a fixed point of $j$ 

so either $k(0) = 0$ and $k(\infin) = \infin$ so $k$ is a dilation, $k: z \mapsto cz$ 

or $k(0) = \infin$ and $k(\infin) = 0$, so $k$ is an inversion, $k: z \mapsto \frac{c}{z}$ 

suppose $k(z) = cz$ so $k^{-1}(z) = c^{-1}z$ 

$j = k(g(k^{-1}(cz))) = k(g(z)) = k(az) = caz = Acz$ so $a = A$

suppose $k(z) = c/z$ and $k^{-1} = c/z$ 

$j = k(g(k^{-1}(cz^{-1}))) = k(g(z)) = k(az) = c/(az) = Ac/z$ so $\frac{1}{a} = A$ 

so there exists a mapping $k$ s.t. $g$ is conjugate to $j: z \mapsto 1/a$

$a$ is not unique

###### (c) If a fractional linear transformation $f(z)$ has exactly one fixed point, then it is conjugate to the translation $\zeta\mapsto \zeta +1$. In other words, there is a fractional linear transformation $h(z)$ such that $h(f(h^{-1}(\zeta))) = \zeta + 1$ or equivalently, such that $h(f(z)) = h(z) +1$ 

if a fractional linear transformation only has one fixed point at $\infin$, then we must have (from (a))

$f(z) = z + b$, 

Let $h$ map the fixed point $z_0$ of $f$ to $\infin$ 

so we have $h^{-1}(\infin) = z_0$ 

so $g = h\circ f \circ h^{-1}(\infin) = \infin$ is the only fixed point

so we must have $g(z) = z+b$ , $b \neq 0$ (else 0 would be a fixed point)

we need to show there exists a map, $k$ s.t.

$k(g(k^{-1}(z))) = z +1$ 

this means $k(k^{-1}(z)+b) = k^{-1}(z)/b + 1$ so $k^{-1}(z) = bz$ 

and $k(z) = z/b$ 

so $(k\circ h \circ f \circ h^{-1} \circ k^{-1}(z) = k\circ g \circ k^{-1}(z) = z+1$

So, $(k\circ h)f(k\circ h)^{-1}(z) = z+1$  

$k\circ h$ is the linear mapping that takes $f(z)$ to $k(h(z)) +1$   

 