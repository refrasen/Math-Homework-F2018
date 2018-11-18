Renee Senining 

Math 185

### Homework #3

#### Chapter  2, Section 2:

##### Ex. 5: Show that if $f$ is analytic on D, then $g(z) = \overline{f(\bar{z})}$ is analytic on the reflected domain $D^* =${$\bar{z}: z \in D$} and $g'(z) = \overline{f'(\bar{z})}$ 

We check to see if $g(z)$ is differentiable at each point of $D^*$ 

Let $z_0$ be a point on $D$. Then  $\overline{z_0}$ is a point in the reflected domain. 

so for any $\bar{z} \in D^*$ s.t. $\overline{z} \rightarrow \overline{z_0}$ 

$\lim_{\overline{z} \rightarrow \overline{z_0}} \frac{g(\overline{z})-g(\overline{z_0})}{\overline{z}-\overline{z_0}} = \lim_{\overline{z}\rightarrow \overline{z_0}}\frac{\overline{f({z})}-\overline{f({z_0})}}{\overline{z}-\overline{z_0}} = \lim_{\bar{z}\rightarrow \bar{z_0}} \overline{(\frac{f({z})-f({z_0})}{z-z_0})}$ 

We have that for any $\delta > 0$, if $z \neq z_0$ and $0 < |z-z_0| < \delta$ then $0 < |\bar{z} -\bar{z_0}| = |\overline{z-z_0}| = |z-z_0| < \delta$, so as $z \rightarrow z_0$, $\bar{z} \rightarrow \bar{z_0}$  

so the limit above is equal to

$\lim_{z \rightarrow z_0} \overline{(\frac{f(z)-f(z_0)}{z-z_0})}$

and since $f$ is analytic on $D$, $\lim_{z\rightarrow z_0} \frac{f(z)-f(z_0)}{z-z_0}$ exists and is equal to $f'(z_0)$ 

and so for every $\epsilon > 0$, $\exists \; \delta>0$ such that $\forall z \in D $, with $z \neq z_0$ if $0 <|z - z_0|<\delta$ then $|\frac{f(z)-f(z_0)}{z-z_0} - f'(z_0)| < \epsilon$  this also means that if $0 < |z-z_0| < \delta$ $|\overline{(\frac{f(z)-f(z_0)}{z-z_0})}-\overline{f'(z_0)}| = |\overline{(\frac{f(z)-f(z_0)}{z-z_0})-f'(z_0)}| = |\frac{f(z)-f(z_0)}{z-z_0} - f'(z_0)| < \epsilon $

so $\lim_{\overline{z}\rightarrow\overline{z_0}} \frac{g(\bar{z})-g(\bar{z_0})}{\bar{z}-\bar{z_0}} = \overline{f'(z_0)} $ = $g'(\overline{z_0})$ 

so since $\overline{z_0}$ was an arbitrary point in $D^*$, for every $z \in D^*$, we have that $g'(z) = \overline{f'(\bar{z})}$ 

#### Chapter 2, Section 3

##### Ex. 3: Show that if $f$ and $\bar{f}$ are both analytic on a domain, then $f$ is constant.

$Re(f) = \frac{1}{2}(f + \bar{f})$ and $Im(f) = \frac{1}{2}(f-\bar{f})$ 

and since $f, \bar{f}$ are analytic, $Re(f), Im(f)$ are analytic along with being real-valued, meaning they are constant, which means $f = Re(f) + iIm(f)$ is constant.

##### Ex. 4: Show that if $f$ is analytic on a domain $D$, and if $|f|$ is constant, then $f$ is constant

If $f(z) = 0$ for some $z \in D$, then $|f(z)| = 0$, and since $|f|$ is constant, we must have $f \equiv 0$ on $D$ 

Otherwise, $f(z) \neq 0$ for all $z \in D$,  and therefore $\bar{f} = |f|^2/f$ is defined for all $z \in D$  

Since $f$ is analytic, and it is differentiable, $1/f$ is differentiable since $f(z) \neq 0$ for all $ z \in D$ and $g(z) = 1$ is differentiable. 

and since $|f|^2$ is a constant, $\bar{f} = |f|^2/f$ is differentiable at all $z \in D$ and therefore analytic on $D$ 

​	Also, $\overline{f}' = -|f|^2/f^2$, which is continuous, since products and sums of continuous functions are continuous... so $\overline{f}$ is analytic.

and if $f$ and $\bar{f}$ are both analytic, by exercise 3, then $f$ is constant.

#### Chapter 2, Section 4

##### Ex. 8: Sketch the image of the circle ${|z-1| \leq 1}$ under the map $w = z^2$. Compute the are of the image.

the domain is any $(x,y)$ satisfying $(x-1)^2 + y^2 = 1$ 

since $x = |z|\cos\theta$ and $y = |z|\sin\theta$ , where $\theta = \arg z$

we have that $|z|^2  \cos^2\theta -2|z|\cos\theta +1 + |z|\sin^2\theta = 1 \\ |z|^2-2|z|\cos\theta = 0 \\ |z|^2 = 2|z|\cos\theta \\ |z| = 2\cos\theta$ 

$z = 2\cos\theta e^{i\theta}$  

$z^2 = 4\cos^2\theta e^{i2\theta}​$ = $4\cos^2(\theta/2)e^{i\theta}​$ 

So  $|z-1| \leq 1$ : ![1536520329716](C:\Users\Renee\AppData\Local\Temp\1536520329716.png)gets mapped to ![1536520470087](C:\Users\Renee\AppData\Local\Temp\1536520470087.png)

From the graphs above, the function $f(z) = z^2$ is bounded. Also, it is analytic, since polynomials are differentiable, and one to one over the bounded domain $D$ = {$z: |z-1| \leq 1$}: $f(w) = f(z) \implies w^2 = z^2$

$\implies$ $w$ and $z$ are square roots of $w^2 = z^2$

since $z$ is a square root, another root would be $w = -z$.

But for $z$ to be in the domain, $Re(z) > 0$ , since  $|z -1|  = \sqrt{(Re(z)-1)^2+Im(z)^2}\geq |Re(z)-1|$ and if $Re(z) < 0$, then $Re(z) -1 < -1$ $\implies |Re(z)-1| > 1$  

so if $z$ is in the domain, $-z$ cannot be, so if $f(z)= f(w) \implies z = w$ Therefore, $f(z) = z^2$ over $D$ is one to one so:

The area of the image = $\int \int \det J_f dx dy$ 

$\det J_f = |f'(z)|^2 = |2z|^2 = 4|z|^2 = 4(x^2+y^2)$

so $D$ = {$(r,\theta)| -\pi/2 \leq \theta \leq \pi/2, 0 \leq r \leq 2\cos\theta$}

So we have $4\int\int_D(x^2+y^2) dA=$ $4\int_{-\pi/2}^{\pi/2} \int_{0}^{2cos\theta}r^3d\theta dr$

$= 16\int_{-\pi/2}^{\pi/2}\cos^4\theta d\theta = 16\int_{-\pi/2}^{\pi/2}(\frac{1+\cos2\theta}{2})^2d\theta = 4\int_{-\pi/2}^{\pi/2}(1 + 2\cos2\theta + (\frac{1 + \cos4\theta}{2}))$

$= 4[\theta + \sin2\theta + \theta/2 + (\sin4\theta)/8]_{-\pi/2}^{\pi/2} = 4[3\pi/4 + 3\pi/4] = 6\pi$ 

#### Extra Problems

##### 1. Let $f: \C \rightarrow \C$ be analytic function on the complex plane and $f(0) =0$. Suppose that for all real numbers $x,y \in \R$ we have $Re(f(x+iy)) = e^{-y}(x\cos(x)-y\sin(x))$.

##### Find an expression for $f(z)$ as a function of a complex variable $z = x+iy$ 

so $u(x,y) = e^{-y}(x\cos(x)-y\sin(x))$ 

since $f$ is analytic:

$\frac{\partial u}{\partial x} = \frac{\partial v}{\partial y} = e^{-y}(\cos(x)-x\sin(x) -y\cos(x))$

$-\frac{\partial u}{\partial y} = \frac{\partial v}{\partial x} = -[-e^{-y}(x\cos(x)-y\sin(x)) +e^{-y}(-\sin(x))] = e^{-y}(x\cos(x)-y\sin(x)) +e^{-y}\sin(x)$

$ = e^{-y}(x\cos(x)+\sin(x)-y\sin(x))$ 

So:

$v(x,y) = \int e^{-y}(\cos(x) -x\sin(x)) -ye^{-y}\cos(x )dy$ = $e^{-y}(x\sin(x)-\cos(x)) +(ye^{-y} +e^{-y})(\cos(x)) +C(x)$ 

$= e^{-y}(x\sin(x) +y\cos(x)) +C(x)$, then we derive this w.r.t. to $x$ and equate it to $-\frac{\partial u}{\partial y}$

$e^{-y}(x\cos(x)+\sin(x)-y\sin(x)) +C'(x)  = e^{-y}(x\cos(x)+\sin(x)-y\sin(x))$ 

$e^{-y}(x\cos(x) +\sin(x) +\sin(x))  + (ye^{-y}+e^{-y})(\cos(x))$

Simplifying:

$C'(x) = 0$ meaning $C(x)$ is a real constant.

$u(x,y) +iv(x,y) = e^{-y}(x\cos(x)-y\sin(x)) + i[e^{-y}(x\sin(x) +y\cos(x)) +C]​$

$f(0) = u(0,0) +iv(0,0) = 0 + iC = 0$ 

so $f(x+iy) = e^{-y}(x\cos(x)-y\sin(x)) + i[e^{-y}(x\sin(x) +y\cos(x))]$

$f(x+iy) = e^{-y}[(x+iy)(\cos(x) +i\sin(x))] = e^{-y}ze^{ix} = ze^{iz}$   

##### 2. Let $f: D \rightarrow \C$ be an analytic function on a domain $D \sub \C$. Denote the real and imaginary part of $f$ as $u(x,y)$ and $v(x,y)$ such that $f(x+iy) = u(x,y) + iv(x,y)$ 

##### Let $\nabla u$ and $\nabla v$ denote the gradient vector fields,

###### 1. Find the angle between the horizontal axis and the vector ($\nabla u$)($x_0, y_0$),

###### 2. Find the angle between the horizontal axis and the vector $(\nabla v)$(x_0, y_0)$ 

##### if $f'(z_0) = 5e^{i\pi/6}$ at the point $z_0 = x_0  + iy_0$ 

We have $f'(z_0) = f'(x_0 + iy_0) = \frac{\partial u}{\partial x}(x_0,y_0) + i\frac{\partial v}{\partial x}(x_0, y_0) = \frac{\partial v}{\partial y}(x_0, y_0) - i\frac{\partial u}{\partial y}(x_0, y_0) = 5e^{i\pi/6} \\ = 5(\cos\frac{\pi}{6} + i\sin\frac{\pi}{6})$ 

$\frac{\partial u}{\partial x}(x_0, y_0) = \frac{\partial v}{\partial y}(x_0, y_0) = 5\cos(\pi/6) = 5(\sqrt3/2)$

$\frac{\partial v}{\partial x}(x_0, y_0) = -\frac{\partial u}{\partial y}(x_0, y_0) = 5\sin(\pi/6) = 5/2$ 

so $\nabla u(x_0, y_0) = (5(\sqrt{3}/2), -5/2)$ and $\nabla v (x_0, y_0) = (5/2, 5(\sqrt{3}/2))$

We can find the angle between any two vectors $a, b$ using

$\theta = \arccos(\frac{a \cdot b}{|a||b|})$ 

so $|\nabla u| = |\nabla v| = |5e^{i\pi/6}|= 5$ 

letting the vector $w = <1, 0>$

1. $\theta = \arccos(\frac{5\sqrt{3}/2}{5}) = \pi/6$  specifically, $\pi/6$ below the $x$-axis
2. $\theta = \arccos(\frac{5/2}{5}) = \pi/3 $, above the $x$-axis 

