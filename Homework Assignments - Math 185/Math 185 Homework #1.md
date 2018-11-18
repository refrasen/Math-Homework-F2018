Renee Senining

Math 185

# Homework #1

## Section 1.1

##### Ex. 2: Verify from the definitions each of the identities

a. $\overline{z+w} = \overline{z} + \overline {w}$ 

If $z$ nd $w$ are comple numbers, they may be written in the form:

 $z = x + iy$, $w = u + iv$ with $x, y, u, v \in \R $ 

From the definition of the complex conjugate:

$\overline{z} = x - iy$ and $\overline{w} = u - iv$ , which are also complex numbers, so 

$\overline{z} + \overline{w} = (x+u) + i(-y+(-v))$ 

$\overline{z} + \overline{w}= (x+u) + i(-(y+v))$ 

= $(x+u) + (-i)(y+v) = (x+u) - i(y+v)$ 

since $z+w = (x+u) + i(y+v)$ 

We have $\overline{z+w} = (x+u) -i(y+v)$ 

so  $\overline{z+w} = \overline{z} + \overline {w}$



![1535244247415](C:\Users\Renee\AppData\Local\Temp\1535244247415.png) 

b. $\overline{zw} = \bar{z}\bar{w}$

letting $z$ and $w$ be expressed as  $z = x + iy$, $w = u + iv$ with $x, y, u, v \in \R $, 

$zw = xu - yv + i(xv + yu)$ 

meaning $\overline{zw} = xu-yv - i(xv+yu)$ 

taking $\overline{z}$ and $\overline{w}$ and multiplying them:

$\bar{z}\bar{w} = (x-iy)(u-iv)  = xu - (-y)(-v) +i(x(-v)+(-y)u)$

$ = xu - yv +i(-(xv+yu)) = xu-yv -i(xv+yu) = \overline{zw}$ 

c. $|\overline{z}| = |z|$ 

if $z = x+iy$, then $|z| = \sqrt{x^2+y^2}$ 

$\bar{z} = x - iy$ (by definition)

$|\bar{z}| = \sqrt{x^2+(-y)^2}$ and since $(-y)^2 = y^2$

$|\bar{z}| = \sqrt{x^2+y^2} = |z|$

![1535244482677](C:\Users\Renee\AppData\Local\Temp\1535244482677.png)

##### Ex. 6: For Fixed $a \in \C$, show that $|z-a|/|1-\bar{a}z| =1$ if $|z| = 1$ and $|1 - \bar{a}z| \neq 0$

Since $|z|$ = 1 and $\frac{1}{z} = \frac{\bar{z}}{|z|^2}$ we have

$\frac{1}{z} = \bar{z}$ $\equiv$ $ z\bar{z} = 1$ 

so we rewrite  $|z-a|/|1-\bar{a}z|$ as

$|z-a|/|z\bar{z}-\bar{a}z|$

$ = |z-a|/|z(\bar{z}-\bar{a})|$

and since $|zw| = |z||w|$ 

= $|z-a|/(|z||\bar{z}-\bar{a}|)$ 

and since $|z| = 1$ 

$= |z-a|/|\bar{z}-\bar{a}|$  

if we let $z = x + iy$ and $a = u + iv$ 

$z-a = (x-u) + i(y-v)$

$\bar{z} - \bar{a} = (x-u) +i(v-y)$ 

Meaning

$|z-a| = \sqrt{(x-u)^2 +(y-v)^2} = \sqrt{(x-u)^2+(v-y)^2} = |\bar{z}-\bar{a}|$

so $|z-a|/|\bar{z}-\bar{a}| = 1$ 

##### Ex. 10: Let $q(z)$ be a polynomial of degree $m \geq 1$. Show that any polynomial $p(z)$ can be expressed in the form $p(z) = h(z)q(z) + r(z)$ where $h(z)$ and $r(z)$ are polynomials and the degree of the remaining $r(z)$ is strictly less than m. 

###### Case 1: $deg(p(z)) = 0$ and in general $deg(p(z)) < m$

we have $p(z) = 0\times q(z) + p(z)$ 

We let $h(z) = 0, r(z) = p(z)$, so $p(z)$ can be expressed in the form $h(z)q(z) + r(z)$. And since $deg(p(z)) = deg(r(z)) < m$, we have proven the statement true for this case. 

###### Case 2: $deg(p(z)) \geq m$  

we do a proof by induction on the degree of $p(z)$

Base Case: Starting with $deg(p(z)) = 1$

since $1 \leq m \leq deg(p(z)) = 1$ , we have $m=1$ 

$p(z) = p_1z + p_0$, some constants $p_1, p_0$ 

$q(z) = q_1z + q_0$ 

multiplying $q(z)$ by $p_1q_1^{-1}$ we get

$p_1q_1^{-1}q(z) = p_1z + p_1q_1^{-1}q_0$ 

and if we add $p_0 - p_1q_1^{-1}q_0$ 

we get $(p_1q_1^{-1})q(z) + (p_0 - p_1q_1^{-1}q_0) = p_1z + p_0 = p(z)$ 

So setting $h(z) = p_1q_1^{-1}$ and $r(z) = p_0 - p_1q_1^{-1}q_0$ 

we can express $p(z)$ in the form $h(z)q(z) + r(z)$. 

and since $r(z)$ is a constant, it has degree 0, which is less than m = 1. 

So we have proven the base case. 

Assume any polynomial of degree < $n$ can be expressed in the form $h(z)q(z) +r(z)$, where $h(z), r(z)$ are polynomials with $r(z)$ having degree less than m. 

let $q(z) = q_mz^m + q_{m-1}z^{m-1} + . . . + q_1z+q_0$ , where $q_0, . . ., q_m$ are constants, $q_m \neq 0$ and $ m \geq 1$ 

let $p(z) = p_nz^n + p_{n-1}z^{n-1} + . . . p_1z + p_0$ 

Since we still have $m \leq n $, $n-m \geq 0$ 

so we can multiply $q(z)$ by $p_nq_m^{-1}z^{n-m}$ to get:

$ p_nq_m^{-1}z^{n-m}q(z) = p_nz^n + p_nq_m^{-1}q_{m-1}z^{n-1} + . . . + p_nq_m^{-1}q_0z^{n-m}$

and subtract it from $p(z)$:

$p(z) - p_nq_m^{-1}z^{n-m}q(z) $, which is a polynomial of degree $n-1$, since $p(z)$ and $p_nq_m^{-1}z^{n-m}q(z)$ have the same leading coefficient are of the same degree $n$. 

So by Induction Hypothesis, we can express this polynomial in the form

$p(z) - p_nq_m^{-1}z^{n-m}q(z) = h(z)q(z) + r(z)$ 

this means:

$p(z) = (h(z)+ p_nq_m^{-1}z^{n-m})q(z) +r(z)$ 

and $r(z)$ has degree less than m, and $h(z) + p_nq_m^{-1}z^{n-m}$ is a polynomial. 

### Section 1.2 

##### Ex. 1 Express All values of the following expressions in both polar and Cartesian coordinates, and plot them. 

###### Ex. 1c: $\sqrt[4]{-1}$ 

$-1$ would be expressed as $(-1, 0)$ and $e^{i\pi}$

So if $\sqrt[4]{-1} = re^{i\theta}$

$r = 1^{1/4} = 1$

$\theta = \frac{\pi}{4} +\frac{2\pi k}{4} $

which means $\sqrt[4]{-1} = e^{i\frac{(2k+1)\pi}{4}} =\frac{1}{\sqrt{2}} + i\frac{1}{\sqrt{2}} = -\frac{1}{\sqrt{2}} +i\frac{1}{\sqrt{2}} = \frac{-1}{\sqrt{2}} -i\frac{1}{\sqrt{2}} = \frac{1}{\sqrt{2}} -i\frac{1}{\sqrt{2}} $

$(\frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}}), (-\frac{1}{\sqrt{2}}, \frac{1}{\sqrt{2}}), (-\frac{1}{\sqrt{2}}, -\frac{1}{\sqrt{2}}), (\frac{1}{\sqrt{2}}, -\frac{1}{\sqrt{2}})$

Polar coordinates, $(r, Arg$ $z)$

$(1, \pi/4), (1, 3\pi/4), (1, -3\pi/4), (1, -\pi/4)$

![1535338305052](C:\Users\Renee\AppData\Local\Temp\1535338305052.png)

###### Ex. 1g: $(1+i)^{8}$

$(1+i)^2 = 2i$ and $(2i)^4 = 16$

$(1+i)^8 = 16$ $(+ i0)$

$r = \sqrt{2}^8 = 16$

$\theta = 2\pi k$

$16e^{2\pi k}$

$(16, 0)$  for both Cartesian and Polar coordinates  

![1535339899595](C:\Users\Renee\AppData\Local\Temp\1535339899595.png)

##### Ex. 5: For $n \geq 1$, show that

###### (a) $1+z+z^2+ . . . +z^n = (1-z^{n+1})/(1-z)$, $z \neq 1$

Proof by Induction:

Base Case: $n = 1$, $1 + z $

$(1-z^2)/(1-z) = (1-z)(1+z)/(1-z) = 1+z$

Assume true for n < k.

Take $1+z + . . .+z^k

 + z^{k+1}$

Using Inductive Hypothesis:

$(1 + z + . . . + z^k) + z^{k+1} = (1-z^{k+1})/(1-z) +z^{k+1} $

multiplying $z^{k+1}$ by ${(1-z)/(1-z)}$ we get:

$(1-z^{k+1}+z^{k+1}-z^{k+2})/(1-z) = (1-z^{k-2})/(1-z)$, proving this true for $k+1$. 

Therefore, (a) is true for all $n \geq 1$

###### (b) $1 + cos\,\theta + cos\,2\theta + . . . + cos\, n\theta = \frac{1}{2}+ \frac{sin(n+\frac{1}{2})\theta}{2sin\theta/2}$ 

Starting with two equations:

1. $1 + z + . . . + z^n$, with $z = e^{i\theta} = cos\theta + isin\theta$  to get

   $1 + (cos\theta + isin\theta ) + (cos2\theta +isin2\theta) + . . +(cosn\theta +isin\,n\theta) =$ $(1-e^{i(n+1)\theta})/(1-e^{i\theta})$

2. This time, with $z^{-i\theta} = cos(-\theta) +isin(-\theta)$ and since $cos$ is even and $sin$ is odd, $z^{-i\theta} = cos\theta -isin\theta$ to get 

   $1 + (cos\theta - isin\theta ) + (cos2\theta -isin2\theta) + . . +(cosn\theta -isin\,n\theta) =$ $(1-e^{-i(n+1)\theta})/(1-e^{-i\theta})$ 

Adding the two equations:

$2(1+cos\theta + cos2\theta + . . . + cosn\theta) = (1-e^{i(n+1)\theta})/(1-e^{i\theta}) + (1-e^{-i(n+1)\theta})/(1-e^{-i\theta})$

$= \frac{(1 - e^{i(n+1)\theta})(1-e^{-i\theta})+ (1-e^{-i(n+1)\theta})(1-e^{i\theta})}{(1-e^{i\theta})(1-e^{-i\theta})}$ 

$= \frac{2 -e^{i(n+1)\theta}-e^{-i\theta}+e^{in\theta}-e^{-(n+1)\theta}-e^{i\theta}+e^{-in\theta}}{2(1-cos\theta)}$ , since $e^{i\theta}$ and $e^{-i\theta}$ are conjugates, adding them will result in $cos\theta$ (for any $\theta$)

$= \frac{1 - cos\theta - cos(n+1)\theta) +cosn\theta}{1-cos\theta} = 1 + \frac{cosn\theta-cos(n+1)\theta}{1-cos\theta}$ 

 And using the following:

1. $1-cos\theta = 2sin^2\theta/2$
2. $cos(n+1)\theta = cosn\theta cos\theta - sin\,n\theta sin\theta$
3. $sin\theta = 2sin(\theta/2)cos(\theta/2)$

 $= 1 + \frac{cosn\theta(2sin^2\theta/2)  + sin\,n\theta(2sin\theta/2cos(\theta/2)) }{2sin^2\theta/2}$

cancelling out $2$ and $sin\theta/2$ gives:

$= 1 + \frac{cosn\theta sin\theta/2 + sin\,n\theta cos(\theta/2)}{sin^2\theta/2}$, and $sin(n\theta + \theta/2) = sin\,n\theta cos\theta/2 + sin\theta/2 cosn\theta$ 

$= 1 + \frac{sin(n+1)\theta}{sin^2\theta/2}$

And dividing both sides by $2$ gives:

$1 + cos\theta + . . . + cosn\theta = 1/2 + \frac{sin(n+1)\theta}{2sin^2\theta/2}$