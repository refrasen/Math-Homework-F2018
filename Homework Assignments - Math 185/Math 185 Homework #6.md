Renee Senining

Math 185

### Homeowrk #6:

**Chapter III**, Sec. 3, ex. 2;  Sec. 4, ex. 2;  Sec. 5, ex. 3, 7;  

**Chapter IV**, Sec. 1, ex. 4, 6, 8;  Sec. 2, ex. 5.

---

#### Chapter III, Sec 3

##### Ex. 2: Show that a complex-valued function $h(z)$ on a star-shaped domain $D$ is harmonic if and only if $h(z) = f(z) + \overline{(g(z))}$, where $f(z)$ and $g(z)$ are analytic 

Suppose  $h(x+iy) = u(x,y) + iv(x,y)$ where $u, v$ are its real and imaginary parts, is a complex-valued function on a star-shaped domain is harmonic

$u,v$ are harmonic.

 $u$ has a harmonic conjugate $u_{c}$ and so does $v(x,y)$, $v_c$ 

 $F(x+iy) = u(x,y) + iu_c(x,y)$ and $G(x+iy) = v(x,y) + iv_c(x,y)$ are analytic 

 $u = \frac{F + \overline{F}}2$ , $v = \frac{G + \overline{G}}2$ 

  $h = \frac{1}{2}(F+\overline{F} + i(G + \overline{G}))$ $= \frac{1}{2}(F + iG + \overline{F} + i\overline{G})$ 

and linear combinations of analytic functions are analytic 

 $f(x+iy) = \frac{1}{2}(F + iG)$ is analytic and $g(x+iy) = {F} - i{G}$ is analytic, 

​	$\overline{g} = \overline{F - iG} = \overline{F} +\overline{-iG} = \overline{F} + i\overline{G}$	  

$h = f + \overline{g}$ , where $f, g$ are analytic

Suppose $h(z) = f(z) + \overline{g(z)}$ , where $f, g$ are analytic

so $h(z) = \text{Re }f + \text{Re }g + i(\text{Im }f - \text{Im }g)$ 

$\text{Re }f, \text{Re }g, \text{Im }f, \text{Im }g$ are all harmonic since $f, g$ are analytic

so $\Delta\text{Re} f = \frac{\partial^2 \text{Re }f}{\partial x^2} + \frac{\partial^2 \text{Re }f}{\partial y^2} = 0$

and $\Delta\text{Re } g = \frac{\partial^2 \text{Re }g}{\partial x^2} + \frac{\partial^2 \text{Re }g}{\partial y^2} = 0 $  

$ \Delta \text{Im } f = \frac{\partial^2 \text{Im }f}{\partial x^2} + \frac{\partial^2 \text{Im }f}{\partial y^2} = 0$

$ \Delta \text{Im } g = \frac{\partial^2 \text{Im }g}{\partial x^2} + \frac{\partial^2 \text{Im }g}{\partial y^2} = 0$ 

so $\frac{\partial^2 (\text{Re }f + \text{Re }g)}{\partial x^2} + \frac{\partial^2( \text{Re }f + \text{Re }g)}{\partial y^2}=  \Delta \text{Re }f + \Delta \text{Re }g = 0 + 0 = 0$ 

and $ \frac{\partial^2 (\text{Im }f - \text{Im }g)}{\partial x^2} + \frac{\partial^2( \text{Im }f - \text{Im }g)}{\partial y^2}=  \Delta \text{Im }f - \Delta \text{Im }g = 0 - 0 = 0$ 

#### Chapter III,  Sec 4

##### Ex. 2: Derive (4.2) from the polar form of the Cauchy-Riemann equations (Exercise II.3.8)

(4.2) $0 = r\int_0^{2\pi}[\frac{\partial u}{\partial x}\cos \theta + \frac{\partial u}{\partial y}\sin \theta]d\theta = r\int_0^{2\pi}\frac{\partial u}{\partial r}(z_0 + re^{i\theta})$ 

polar form: $\frac{\partial u}{\partial r} = \frac{1}{r}\frac{\partial v}{\partial \theta}$ ,    $\frac{\partial u}{\partial \theta} = -r\frac{\partial v}{\partial r}$ 

Laplace's equation in polar coordinates

$\frac{\partial ^2 u}{\partial r^2} + \frac{1}{r}\frac{\partial u}{\partial r} + \frac{1}{r^2}\frac{\partial ^2 u}{\partial \theta^2} = 0$ 

Proof: Given that $\frac{\partial^2 u}{\partial x^2} + \frac{\partial^2 u}{\partial y^2} = 0$ 

$\frac{\partial^2 u}{\partial r^2} = \frac{\partial ^2 u}{\partial x^2} \cos^2\theta + \frac{\partial ^2 u}{\partial y^2}\sin^2\theta$ 

$\frac{\partial ^2 u}{\partial \theta^2} = \frac{\partial ^2 u}{\partial x^2}(r^2\sin^2\theta) + \frac{\partial ^2 u}{\partial y^2}(r^2\cos^2\theta) + \frac{\partial u}{\partial x}(-r\cos\theta) + \frac{\partial u}{\partial y}(-r\sin\theta)$ 

and $\frac{\partial u}{\partial r} = \frac{\partial u}{\partial x}\cos\theta + \frac{\partial u}{\partial y}\sin\theta$ 

it easily follows that$\frac{\partial ^2 u}{\partial r^2} + \frac{1}{r}\frac{\partial u}{\partial r} + \frac{1}{r^2}\frac{\partial ^2 u}{\partial \theta^2} = 0$ 

and since we are looking at an open disk for the theorem, the harmonic conjugate $v$ for $u$ exists

and $u+iv$ is an analytic, so we may use the CR equations for the polar form:

$\frac{\partial^2 u}{\partial r^2} = \frac{1}{r}\frac{\partial}{\partial r}\frac{\partial  v}{ \partial \theta} = \frac{1}{r}\frac{\partial }{\partial \theta}\frac{\partial v}{\partial r} = -\frac{1}{r^2}\frac{\partial ^2 u}{\partial \theta^2}$ 

so we have that $\frac{1}{r}\frac{\partial u}{\partial r} = 0$ from the Laplace's equation (in polar coordinates)

so $r^2 \frac{1}{r} \frac{\partial u}{\partial r} = 0 * r^2 $ $\implies$ $r\frac{\partial u}{\partial r} = 0$ 

Now consider the line integral:

 $\oint_{|z-z_0| = r} r \frac{\partial u}{\partial r}d\theta$ 

since $P = r\frac{\partial u}{\partial r} = 0$ and $Q = 0$ 

we have $\frac{\partial P}{\partial \theta} = \frac{\partial }{\partial \theta} (r\frac{\partial u}{\partial r} )= \frac{\partial }{\partial \theta}(0) = 0$ and so by Green's Theorem:

$0 = r\int_0^{2\pi}\frac{\partial u}{\partial r}d\theta$ , which is equation (4.2)

#### Chapter III, Sec 5

##### Ex. 3: Use the maximum principle to prove the fundamental theorem of algebra, that any polynomial $p(z)$ of degree $n \geq 1$ has a zero, by applying the maximum principle to $1/p(z)$ on a disk of large radius.

$p(z)$ is a polynomial $\implies$ $p(z)$ is analytic $\implies$  $p(z)$ is harmonic since it's real and imaginary parts are harmonic

so $1/p(z)$ is analytic and harmonic whenever $p(z) \neq 0$ 

---

Suppose $p(z)$ doesn't have a zero

This means $1/p(z)$ is defined for all $z \in \C$ , and is harmonic on all points in $\C$ 

and if $p(z) = a_nz^n + ... + a_1z + a_0$ 

as $|z| \rightarrow \infin$ , $|p(z)| \geq |a_n||z^n|  \rightarrow \infin$ 

so $|p(z)|$ attains its minimum in $\C$, meaning $|1/p(z)|$ attains its max, $M$ at some point $z_0$ in $\C$ 

If we fix a (large) disk around this point, $z_0$ we have that $1/p(z)$ is a harmonic function on a bounded domain (the disk), and it extends continuously to the boundary (since $1/p(z)$ is defined and continuous for all $z \in \C$ since $p(z)$ doesn't have a zero)

so we have that for all $z$ in this disk, $|1/p(z)| \leq M$, and $|1/p(z_0)| = M$, so $1/p(z)$ is constant on this disk

and if we keep extending the disk, we can keep applying the strict maximum principle, and have that $1/p(z)$ is constant and $|1/p(z)| = M$ for all $z \in \C$ 

and since $1/p(z)$ is constant for all $z \in \C$, this means $p(z)$ must be constant for all $z \in \C$

So we have that if $p(z)$ doesn't have a zero, it must be a constant function.

$\equiv$ if $p(z)$ isn't a constant function, it has a zero.

##### Ex. 7: Let $f(z)$ be a bounded analytic function on the open unit disk $\mathbb{D}$. Suppose there are a finite number of points on the boundary such that $f(z)$ extends continuously to the arcs of $\partial\mathbb{D}$ separating the points and satisfies $|f(e^{i\theta})| \leq M$ there. Show that $|f(z)| \leq M$ on $\mathbb{D}$. 

Hint: In the case that there is only one exceptional point $z = 1$, consider the function $(1-z)^\epsilon f(z)$ 

so $|f(z)| \leq C$ since $f(z)$ is bounded

Suppose there exists a $\delta$, satisfying $0 < \delta \leq C-M$, s.t. at some point $z_0 \in \mathbb{D}$  $|f(z_0)| = M + \delta$ 

Define $g(z) = (z_1-z)^\epsilon(z_2 - z)^\epsilon \cdots(z_n - z)^\epsilon f(z)$ 

$g(z)$ is continuous for all points of $z$ where $f(z)$ is continuous 

and as $z \rightarrow z_i$ for $i =1, . ., n$, $g(z) \rightarrow 0$, and $g(z_i) = 0$ so $g$ is continuous on $\mathbb{D}\cup\partial\mathbb{D}$  

and $| (z_1-z)^\epsilon(z_2 - z)^\epsilon \cdots(z_n - z)^\epsilon|^\epsilon M\leq | (z_1-z)^\epsilon(z_2 - z)^\epsilon \cdots(z_n - z)^\epsilon f(z)| \\ \leq | (z_1-z)^\epsilon(z_2 - z)^\epsilon \cdots(z_n - z)^\epsilon|(M + \delta)$ 

we can choose an value of $\epsilon > 0$ s.t.

$1\leq| (z_1-z)^\epsilon(z_2 - z)^\epsilon \cdots(z_n - z)^\epsilon| \leq \frac{M + \delta/2}{M}$  

and $g(z)$ is analytic, (at the points where $f(z)$ is not continuous, the derivative of $g(z)$ is $\infin$ which is in the extended complex plane) and therefore harmonic, on $\mathbb{D}\cup\partial\mathbb{D}$  so we may apply the Maximum Principle

on the boundary, $|f(z)| \leq M$ where it is defined, 

so on the boundary, $|g(z)| \leq (M+\delta/2)$ so for all $z \in \mathbb{D}$, $|g(z)| \leq M+\delta/2$ 

and at $z_0$, $|g(z_0)| \geq (M+\delta)$ 

but since $z_0 \in \mathbb{D}$ we must also have $|g(z_0)| \leq M+\delta/2 < M + \delta$ 

a contradiction.

#### Chapter IV, Sec 1

##### Ex. 4: Show that if $D$ is a bounded domain with smooth boundary, then $\int_{\partial D}\overline{z}dz = 2i\text{Area}(D)$ 

So $\int_{\partial D}\overline{z}dz = \int_{\partial D} x - iy dx + \int_{\partial D} y + ix dy$

$P(x,y) = x -iy, Q(x,y) = y+ix$ and so 

Green's Theorem: $= \int \int_D i -(-i) dxdy = 2i \int \int_D dA = 2i (\text{Area}(D))$ 

the last equality comes from multivariable calculus

##### Ex. 6: Show that $|\oint_{|z| = R} \frac{\text{Log }z}{z^2}dz| \leq 2\sqrt{2}\pi\frac{\log R}{R}, R > e^\pi$ 

$|\oint_{|z| = R} \frac{\text{Log }z}{z^2}dz| \leq \oint_{|z| = R} |\frac{\text{Log }z}{z^2}||dz|$ 

$z = Re^{i\theta}$, $-\pi \leq \theta \leq \pi$ 

$|\text{Log }z| = |\log R + i\theta| = \sqrt{(\log R)^2 + \theta^2}$ $\sqrt{(\log R)^2 + \pi^2} \leq \sqrt{2(\log R)^2} = \sqrt{2}\log R $

​	since $R > e^\pi$ , $\log R > \pi$  

$|z^2| < R^2$ 

$|dz| = |-R\sin \theta + i R\cos\theta| = R$ $d\theta$ 

$|\oint_{|z| = R} \frac{\text{Log }z}{z^2}dz| \leq \int_{-\pi}^\pi \frac{\sqrt{2}\log R}{R^2}*R\; d\theta = 2\pi\frac{\sqrt{2} \log R}{R}$  

##### Ex. 8: Suppose the continuous function $f(e^{i\theta})$ on the unit circle satisfies $|f(e^{i\theta})| \leq M$ and $|\int_{|z| = 1}f(z)dz| = 2\pi M$ . Show that $f(z)= c\overline{z}$ for some constant $c$ with modulus $|c| = M$ 

$\int_{|z| = 1}|f(z)||dz| = \int_0^{2\pi} |f(e^{i\theta})|d\theta$

​	if we parameterize $z = e^{i\theta}$ 

​	and $|dz| = |ie^{i\theta} | d\theta = d\theta $ 

From the hypothesis and using the triangle inequality:

$2\pi M = |\int_{|z| = 1} f(z)dz| \leq $ $\int_0^{2\pi} |f(e^{i\theta}) |d\theta \leq 2\pi M$  

so $|f(e^{i\theta})| = M$ 

---

taking $g(e^{i\theta}) = ie^{i\theta}f(e^{i\theta})$   

$|g(e^{i\theta})| = |i||e^{i\theta}||f(e^{i\theta})| = M$ 

we may multiply $g$ by a unimodular constant $\lambda$ s.t.

$\lambda g(e^{i\theta}) = M$,

so we have $\lambda i e^{i\theta}f(e^{i\theta}) = M$   

$f(e^{i\theta}) = -i\lambda^{-1}Me^{-i\theta}$ 

and $|-i\lambda^{-1}M| = M$, since $|-i| =1, |\lambda^{-1}| = 1/|\lambda| = 1$ 

#### Chapter IV, Sec 2

##### Ex. 5: Show that an analytic function $f(z)$ has a primitive in $D$ if and only if $\int_\gamma f(z)\, dz = 0$ for every closed path $\gamma$ in $D$ 

Let $f(z)$ have a primitive, $F(z)$ in $D$ 

since $f(z)$ is analytic, it is continuous on $D$, 

so $\int_A^B f(z) \, dz = F(B) - F(A)$ 

for any path in $D$ from $A$ to $B$ 

for a closed path $\gamma$ from $A$ to $B$, $A = B$, so $\int_\gamma f(z)\, dz = \int_A^A f(z)\, dz = F(A) - F(A) = 0$ 

since $\gamma$ was an arbitrary closed path, we have for any closed path $\int_\gamma f(z)\, dz = 0$ 

Now suppose for every closed path $\gamma$ in $D$, $\int_\gamma f(z) \, dz = 0$ 

so $\int_\gamma f(z)(dx + idy)$ $= $ $\int_\gamma f(z)\, dx + i f(z)\, dy$ 

so since it is independent of path, the differential $f(z)\, dx + i f(z) \, dy$ is exact

so there exists a functin $F(z)$ s.t. $dF = f(z)dx + i f(z)dy$ 

$\frac{\partial F}{\partial x} = f(z)$ and $\frac{\partial F}{\partial y} = if(z)$ 

for any function $g = u + iv$, where $u, v$ are the real, imaginary parts of $g$

$\frac{\partial }{\partial x} \text{Re }g = \frac{\partial u}{\partial x}$ , $\text{Re }\frac{\partial g}{\partial x} = \text{Re }(\frac{\partial u}{\partial x} + i \frac{\partial v}{\partial x})$ $=$ $\frac{\partial u}{\partial x}$ 

and similarly for $\frac{\partial }{\partial y}$ and/or $\text{Im }g$. Finding the partial derivative of a real/imaginary part of a function is the same as finding the real/imaginary part of the partial derivative 

so $\frac{\partial }{\partial x}\text{Re }F = \text{Re } f = \text{Im } if = \text{Im } \frac{\partial F}{\partial y} = \frac{\partial }{\partial y} \text{Im }F $  

and $\frac{\partial }{\partial y}\text{Re } F = \text{Re }\frac{\partial F}{\partial y} = \text{Re }if = - \text{Im }f = -\text{Im }\frac{\partial F}{\partial x} = - \frac{\partial }{\partial x}\text{Im }F$  

so $F$ is analytic since it satisfies the CR equations

and $F'(z) = \frac{\partial F}{\partial x} = \frac{1}{i}\frac{\partial F}{\partial y} = f(z)$ 

so $f$ has a primitive in $D$, $F$ 