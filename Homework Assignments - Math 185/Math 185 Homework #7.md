Renee Senining

Math 185

### Homework #7

#### Chapter IV Sec. 3, ex. 1, 2;  Sec. 4, ex. 1f, 1g, 1h;  Sec. 5, ex. 2;  Sec. 6, ex. 2

#### Sec. 3

##### Ex. 1 By integrating $e^{-z^2/2}$ around a rectangle with vertices $\pm R, it \pm R$ and sending $R$ to $\infin$, show that $\frac{1}{\sqrt{2\pi}}\int_{-\infin}^{\infin}e^{-x^2/2}e^{itx}dx = e^{-t^2/2}$, $\infin < t < \infin$. Use the known value of the integral for $t = 0$. 

$f(z) = e^{-z^2/2}$ is analytic on the complex plane, so it is analytic on $D$ $=$ the rectangle with vertices $\pm R, it \pm R$ So:

$\int_{(-R,0)}^{(R, 0)}f(z) dz + \int_{(R,0)}^{(R, t)}f(z)dz + \int_{(R, t)}^{(-R,t)}f(z)dz +\int_{(-R,t)}^{(-R, 0)}f(z)dz$ $= 0$

$\equiv $

$\int_{-R}^R e^{-x^2/2} dx$ $+$ $i\int_0^t e^{(-R^2+y^2)/2}e^{-iRy} dy$ $+\int_R^{-R}e^{(-x^2 +t^2)/2}e^{-ixt}dx$ $+$ $i\int_t^0 e^{(-R^2+y^2)/2}e^{iRy}dy$ $= 0$

with $dy = 0$, moving from $(-R, 0)$ to $(R, 0)$ and from $(R,t)$ to $(-R, t)$ 

and $dx = 0$ moving from $(R, 0)$ to $(R, t)$ and from $(-R, t)$ to $(-R, 0)$ 

and $e^{(-R^2+y^2)/2 -iRy} = e^{-(R +iy)^2/2}$ and $e^{(-R^2+y^2)/2 + iRy} = e^{-(-R+iy)^2/2}$

and since $0 \leq y \leq t$, ($ \infin <t < \infin$) and as $R \rightarrow \infin$, $|e^{-(\pm R +iy)^2/2}|\rightarrow 0 $ $\implies$

by the $ML$ estimate, $|\int_0^t e^{-(\pm R + iy)^2/2}dy| \leq ML \rightarrow 0$ as $R \rightarrow \infin$

so: $\int_0^te^{-(\pm R + iy)^2/2} = 0$

so: $\int_{-R}^R e^{-x^2/2}dx = \int_{-R}^R e^{(-x^2 +t^2)/2}e^{-ixt} dx = \int_{-R}^R e^{-(x+it)^2/2}dx$ 

and when $t = 0$, $\frac{1}{\sqrt{2\pi}}\int_{-\infin}^{\infin} e^{-x^2/2}dx = 1$

so: $\int_{-R}^Re^{-x^2/2}e^{-ixt}e^{t^2/2}dx = \int_{-R}^Re^{-x^2/2} \rightarrow \sqrt{2\pi}$ as $R \rightarrow \infin$ 

$\implies$ $\frac{1}{\sqrt{2\pi}}\int_{-\infin}^{\infin}e^{-x^2/2}e^{-ixt}dx = e^{-t^2/2}$ 

##### Ex. 2 We define the Hermite polynomial $H_n(x)$ and Hermite orthogonal functions $\phi_n(x)$ for $n \geq 0$ by $H_n(x) = (-1)^ne^{x^2}\frac{d^n}{dx^n}(e^{-x^2}), \phi_n(x) = e^{-x^2/2}H_n(x)$ 

###### (a) Show that $H_n(x) = 2^nx^n + \cdots$ is a polynomial of degree $n$ that is even when $n$ is even, and odd when $n$ is odd

the derivative of an odd function is even, and the derivative of an even function is odd:

$f(x) = f(-x)$ 

letting $g(x) = -x$, we have $f(g(x)) = f(x)$ 

$\frac{d}{dx}f(g(x)) = \frac{df}{dx}(g(x))*\frac{d}{dx}g(x) = -\frac{d}{dx}f(-x)$ 

but also $\frac{d}{dx}f(g(x)) = \frac{d}{dx}f(x)$

so: $\frac{d}{dx}f(-x) = -\frac{d}{dx}f(x)$ 

if $f(-x) = -f(x)$, again letting $g(x) = -x$, $f(g(x)) = -f(x)$ 

so $\frac{d}{dx}f(g(x))= \frac{d}{dx}(-1)f(x) = -\frac{d}{dx}f(x)$ 

and $\frac{d}{dx}f(g(x)) = \frac{df}{dx}(g(x))*\frac{d}{dx}g(x) = -\frac{d}{dx}f(-x)$ 

so $\frac{d}{dx}f(x) = \frac{d}{dx}f(-x)$ 

---

 $e^{-x^2}$ is an even function: $e^{-(-x)^2} = e^{-x^2}$ 

so the $n = 1$ derivative is going to be odd

and the $n=2$ derivative is the derivative of an odd function, so it will be even

and so on: if $n$ is odd the $nth$ derivative is odd, and if $n$ is even, the $nth$ derivative is even

the product of even functions is even: $f(-x)g(-x) = f(x)g(x)$, and the product of an even and odd function is odd: $f(-x)g(-x) = -f(x)g(x)$ (either $f(-x) = -f(x)$ and $g(-x) = g(x)$ or vice versa)

so $(-1)^n$ is a constant, so it is even, and $e^{x^2}$ is even: $(-1)^ne^{x^2}$ is even

and if $n$ is even: $\frac{d^n}{dx^n}(e^{-x^2})$ is even, so $H_n(x)$ is even

and if $n$ is odd: $\frac{d^n}{dx^n}(e^{-x^2})$ is odd, so $H_n(x)$ is odd

###### (b) By integrating the function $e^{(z-it)^2/2}\frac{d^n}{dz^n}(e^{-z^2})$ around a rectangle with vertices $\pm R, it \pm R$ and sending $R$ to $\infin$, show that $\frac{1}{\sqrt{2\pi}}\int_{-\infin}^{\infin}\phi_n(x)e^{-itx}dx = (-i)^n\phi_n(t)$ , $-\infin < t < \infin$ 

$f(z) = e^{(z-it)^2/2}\frac{d^n}{dz^n}(e^{-z^2})$ $= e^{(z^2 -2zit + t^2)/2}\frac{d^n}{dz^n}(e^{-z^2})$ 

$\int_{(-R,0)}^{(R, 0)}f(z) dz + \int_{(R,0)}^{(R, t)}f(z)dz + \int_{(R, t)}^{(-R,t)}f(z)dz +\int_{(-R,t)}^{(-R, 0)}f(z)dz$ $= 0$

$\equiv $ 

$\int_{-R}^R e^{(x-it)^2/2}\frac{d^n}{dx^n}(e^{-x^2})dx$ $+$ $i\int_0^t e^{(R+iy-it)^2/2}e^{-(R+iy)^2}$$-$$\int_{-R}^R e^{x^2/2}\frac{d^n}{dx^n}e^{-(x+it)^2}dx$ $- i\int_{0}^te^{(-R+iy-it)^2/2}\frac{d^n}{dy^n}(e^{-(-R+iy)^2})dy = 0$ 

as seen before, for $0 \leq y \leq t$, $R \rightarrow \infin$ $|e^{-(\pm R+iy)^2}|\rightarrow 0$ and similarly $|e^{(\pm R+iy-it)^2/2}|$$\rightarrow 0$ 

so: $\int_{-R}^R e^{(x-it)^2/2}\frac{d^n}{dx^n}(e^{-x^2})dx = \int_{-R}^R e^{x^2/2}\frac{d^n}{dx^n}e^{-(x+it)^2}dx$ 

Left side:

$\int_{-R}^R e^{(x-it)^2/2}\frac{d^n}{dx^n}(e^{-x^2})dx$ $= \int_{-R}^{R}e^{x^2/2}e^{-itx}e^{-t^2/2}\frac{d^n}{dx^n}(e^{-x^2})dx$ 

$= e^{-t^2/2}\int_{-R}^R e^{-itx}(-1)^n\phi_n(x)dx$

since $\phi_n(x) = (-1)^ne^{x^2/2}\frac{d^n}{dx^n}(e^{-x^2})$ 

Right side:

$\int_{-R}^R e^{x^2/2}\frac{d^n}{dx^n}e^{-(x+it)^2}dx$ $= \int_{-R}^{R}e^{x^2/2}\frac{d^n}{dx^n}(e^{-x^2 -2itx + t^2})dx$ 

$ = e^{t^2}\int_{-R}^R e^{x^2/2}\frac{d^n}{dx^n}(e^{-x^2-2itx})dx$ 

justifying the hint: $\frac{d^n}{dx^n} e^{-(x+it)^2} = \frac{1}{i^2}\frac{d^n}{dt^n}e^{-(x+it)^2}$ 

​	since: $\frac{dF}{dx} = \frac{1}{i}\frac{dF}{dy}$ and $F$ in this case has continuous partial derivatives of all orders

​	so: $\frac{\partial^n F}{\partial x^n} = (\frac{1}{i})^n \frac{\partial^n F}{\partial y^n}$ , and in this integral, $y = t$ since it goes from $(-R, t)$ to $(R, t)$ 

So using the hint we get:

$=\int_{-R}^R e^{x^2/2}\frac{1}{i^n}\frac{d^n}{dt^n}(e^{-x^2-2itx+t^2})dx$  and using $1/i = -i$:

$ = (-i)^n\frac{d^n}{dt^n}e^{t^2}\int_{-R}^R e^{-x^2/2}e^{-2itx}dx =$

as $R \rightarrow \infin$... $\int_{-R}^Re^{-x^2}e^{-i(2t)x} dx \rightarrow \sqrt{2\pi} e^{-(2t)^2/2}$ (from exercise 1 with 2t in place of t)

$(-i)^n\frac{d^n}{dt^n}e^{t^2}\int_{-R}^R e^{-x^2/2}e^{-2itx}dx \rightarrow$  $\sqrt{2\pi} (i)^n(-1)^n \frac{d^n}{dt^n}e^{-t^2}$ 

$ = \sqrt{2\pi}i^n e^{-t^2/2}[(-1)^ne^{t^2/2}\frac{d^n}{dt^n}e^{-t^2}]$ $= \sqrt{2\pi} i^n e^{-t^2/2}\phi_n(t)$ 

Equating both sides:

$e^{-t^2/2}\int_{-R}^R e^{-itx}(-1)^n\phi_n(x)dx = \sqrt{2\pi} i^n e^{-t^2/2}\phi_n(t)$ 

and sending $R$ to $\infin$

$\frac{1}{\sqrt{2\pi}}\int_{-\infin}^\infin e^{itx}\phi_n(x)dx = (-i)^n\phi_n(t)$ 

###### (c) Show that $\phi_n''-x^2\phi_n + (2n+1)\phi_n = 0$ 

$\phi_n'' = e^{-x^2/2}H_n''(x) + (-x)e^{-x^2/2}H_n'(x) + (-x)e^{-x^2/2}H'_n(x) + (x^2e^{-x^2/2} -e^{-x^2/2})H_n(x)$ 

$ = e^{-x^2/2}H_n''(x) - 2xe^{-x^2/2}H_n'(x) + x^2\phi_n$ $-\phi_n(x)$ 

$\phi''_n - x^2\phi_n + \phi_n= e^{-x^2/2}(H_n''(x) -2xH_n'(x))$ **$(*)$**

$H'_n(x) = (-1)^n2xe^{x^2}\frac{d^n}{dx^n}(e^{-x^2}) + (-1)^ne^{x^2}\frac{d^{n+1}}{dx^{n+1}}(e^{-x^2})$ $ = 2xH_n(x) -H_{n+1}(x)$ 

$2xH_n'(x) = (-1)^n[4x^2e^{x^2}\frac{d^n}{dx^n}(e^{-x^2}) +2xe^{x^2}\frac{d^{n+1}}{dx^{n+1}}(e^{-x^2})]$ 

$H_n''(x) = (-1)^n[(2e^{x^2} +4x^2e^{x^2})\frac{d^n}{dx^n}(e^{-x^2})+4xe^{x^2}\frac{d^{n+1}}{dx^{n+1}}(e^{-x^2}) + e^{x^2}\frac{d^{n+2}}{dx^{n+2}}(e^{-x^2})]$

$\implies$  

$H_n''(x) -2xH_n'(x) = $$(-1)^n[2e^{x^2}\frac{d^n}{dx^n}(e^{-x^2})+ 2xe^{x^2}\frac{d^{n+1}}{dx^{n+1}}(e^{-x^2})+e^{x^2}\frac{d^{n+2}}{dx^{n+2}}(e^{-x^2})]$ 

$H_n''(x) -2xH_n'(x) = $$(-1)^n2e^{x^2}\frac{d^n}{dx^n}(e^{-x^2}) -(-1)^{n+1}2xe^{x^2}\frac{d^{n+1}}{dx^{n+1}}(e^{-x^2}) +(-1)^{n+2}e^{x^2}\frac{d^{n+2}}{dx^{n+2}}(e^{-x^2})$ 

$ H_{n+2}(x) = (-1)^{n+2}e^{x^2}\frac{d^{n+2}}{dx^{n+2}}(e^{-x^2}) = 2xH_{n+1}(x) - (2(n+1))H_n(x)$ 

​	This comes from $H_n'(x) = 2xH_n(x) -H_{n+1}(x)$ (shown earlier)

​	and that Hermite polynomials constitute an Appell sequence, so

​	$H_n'(x) = 2nH_{n-1}(x)$ 

$H_{n+1}(x) = (-1)^{n+1}e^{x^2}\frac{d^{n+1}}{dx^{n+1}}(e^{-x^2})$ 

$H''_n(x) -2xH_n'(x) = 2H_n(x) - 2xH_{n+1}(x) + 2xH_{n+1}(x) - 2(n+1)H_n(x)$

$\implies$ $H_n''(x) - 2xH_n'(x) = 2H_n(x) -2(n+1)H_n(x) = -2nH_n(x)$

So plugging this back in $(*)$ 

$\phi_n''-x^2\phi_n + \phi_n = -2n\phi_n$ $\equiv$ $\phi_n'' - x^2\phi_n +(2n+1)\phi_n = 0$

###### (d) Using $\int \phi_n''\phi_mdx = \int\phi_n\phi_m''dx$ and (c) show that $\int_{-\infin}^{\infin}\phi_n(x)\phi_m(x)dx = 0$, $n \neq m$

$\int_{-\infin}^{\infin}\phi_n\phi_mdx = $ ( using (c) )

$\int_{-\infin}^{\infin}(-\phi_n'' +x^2\phi_n -2n\phi_n)\phi_mdx$

=$\int_{-\infin}^{\infin}(-\phi_n''\phi_m +x^2\phi_n\phi_m - 2n\phi_n\phi_m) dx$

$= \int_{-\infin}^{\infin}(-\phi_n''\phi_m)dx + \int_{-\infin}^{\infin}x^2\phi_n\phi_m dx - 2n\int_{-\infin}^{\infin}\phi_n\phi_m dx$

= $\int_{-\infin}^{\infin} -\phi_n\phi_m''dx + \int_{-\infin}^{\infin}x^2\phi_n\phi_m dx - 2n\int_{-\infin}^{\infin}\phi_n\phi_m dx$ 

​	using: $-\phi_n\phi_m''= -\phi_n(x^2\phi_m -(2m+1)\phi_m) = (2m-x^2+1)\phi_n\phi_m $

$ = 2m\int_{-\infin}^{\infin} \phi_n\phi_m dx -\int_{-\infin}^{\infin}x^2\phi_n\phi_m dx + \int_{-\infin}^{\infin}\phi_n\phi_m dx + \int_{-\infin}^{\infin}x^2\phi_n\phi_m dx - 2n\int_{-\infin}^{\infin}\phi_n\phi_m dx$ 

$\int_{-\infin}^{\infin} \phi_n(x)\phi_m(x)dx = (2m-2n)\int_{-\infin}^{\infin}\phi_m\phi_n dx + \int_{-\infin}^{\infin}\phi_n(x)\phi_m(x)$

$\implies$$(2m-2n)\int_{-\infin}^{\infin}\phi_m\phi_n dx = 0$ , and $2m -2n \neq 0$, since $m \neq n$ 

so $\int_{-\infin}^{\infin}\phi_m\phi_ndx = 0$ 

#### Sec. 4

$f^{(m)}(z) = \frac{m!}{2\pi i}\int_{\partial D} \frac{f(w)}{(w-z)^{m+1}}dw$, $z \in D, m \geq 0$ 

$D$ is a bounded domain with piecewise smooth boundary

$f(z)$ is analytic on $D$ that extends smoothly to the boundary of $D$ 

##### 1f $\int_{|z-1-i| = 5/4} \frac{\text{Log }z}{(z-1)^2}dz = 2\pi i$ 

$1 \in$ {$|z-1-i| <5/4 $}, since $|1-1-i| = |i| = 1 < 5/4 $

$\text{Log }z$ $= f(z)$ is analytic on $D$, since for any $w$ $\in (-\infin, 0]$ 

$|w-1-i| = |-(|w|+1+i)| = ||w| + 1+i| \geq |1+i| = \sqrt{2} > 5/4$, $w$ is not in $D$ and not on the boundary of $D$ 

so: $\frac{1}{1} = \frac{1}{2\pi i}\int_{|z-1-i| = 5/4}\frac{\text{Log }z}{(z-1)^2} dz$ , which gives the final answer $2\pi i$ 

##### 1g $\oint_{|z|=1} \frac{dz}{z^2(z^2-4)(e^z)}$

$f(z) =e^{-z}$ is analytic everywhere

$\oint_{|z|=1}\frac{e^{-z}}{z^2(z^2-4)}dz$

$f(z) = \frac{e^{-z}}{z^2-4}$

$\oint_{|z|=1}f(z)/z^2dz = 2\pi i[\frac{-e^{-z}(z^2-4)-e^{-z}(2z)}{(z^2-4)^2}]_{z=0}$ 

$= 2\pi i[\frac{-(-4)}{(-4)^2}] = 2\pi i\frac{1}{4} = \frac{\pi i}{2}$ 

##### 1h $\oint_{|z-1| = 3}\frac{e^{-z}}{z(z^2-4)}dz$

$0, 2 \in$ {$|z-1| < 3$}

Let $D_\epsilon$ be the domain obtained from punching out small disks around $0, 2$ from {$|z-1| < 3$}

so we obtain

$\oint_{|z-1| = 3} \frac{e^{-z}}{z(z^2-4)}dz = $$\oint_{|z| = \epsilon}\frac{e^{-z}/(z^2-4)}{z}dz + \oint_{|z-2| = \epsilon}\frac{e^{-z}/(z(z+2))}{z-2}dz$

$ = 2\pi i (\frac{1}{-4} + \frac{e^{-2}}{8})$ $ = -\frac{\pi i}{2} + \frac{\pi i}{4e^2}$ 

#### Sec 5

##### Ex. 2 Show that if $f(z)$ is an entire function, and there is a nonempty disk such that $f(z)$ does not attain any values in the disk, then $f(z)$ is a constant

$f(z)$ is entire $\implies$ $f(z)$ is analytic on the entire complex plane

and $\exists$ a disk $D$ with center $z_0$ and radius $\rho$ s.t. $f(z) \notin D$ for all $z$ 

so $1/(f(z) - z_0)$ is an entire function, $f(z) \neq z_0$, and $f(z)$ and $z_0$ are analytic everywhere

and is bounded:

for all $z$, since $f(z)$ doesn't attain any value in the disk $D$ $|f(z) -z_0| \geq \rho$ $\implies \frac{1}{|f(z)-z_0|}\leq 1/\rho$ for all $z$ 

so $1/(f(z)-z_0)$  is equal to some constant $C$ by Liouville's theorem

which means $f(z) = 1/C+z_0$, a constant

#### Sec 6

##### Ex. 2 Let $h(t)$ be a continuous function on the interval $[a,b]$. Show that the Fourier transform $H(z) = \int_a^b h(t)e^{-itz}dt$ is an entire function that satisfies $|H(z)| \leq Ce^{A|y|}$, $z = x +  iy \in \C$, for some constants $A, C > 0$ 

$H(z)$ is an entire function if it is analytic on the entire complex plane

We have that $h(t)e^{-itz}$ is continuous for $t \in [a,b]$ since the product of continuous functions are continuous.

Also, for each fixed $t$, $h(t)e^{-itz}$ is an analytic of $z \in$ $\C$, as $h(t)$ is a constant, and $e^{az}$ is analytic over all of $\C$, and in this case $a = -it$,

so we have $H(z)$ is analytic over all of $\C$ by the theorem on page 121

since $h(t)$ is continuous on the interval 

$|H(z)| \leq (b-a)|h(t)||e^{-itz}|$ 

$|e^{-itz}| \leq |e^{-it(x+iy)}| \leq |e^{yt-itx}| = |e^{yt}e^{-itx}| = |e^{yt}|$ 

let $A = \max(|a|, |b|)$

let $C = M(b-a)$, where $|h(t)| \leq M$ for all $t$

$|H(z)| \leq Ce^{A|y|}$ 

#### Extra Problems

https://math.berkeley.edu/~art/data/F18-185/HW7.pdf

##### Ex 1 

If we can continuously deform $\gamma_1$ to a small circular path around $z_1$ contained in $\gamma_3$ 

and continuously deform $\gamma_2$ to a small circular path around $z_2$ contained in $\gamma_3$ 

​	(so $w$ is not in these disks)

We can define a region $D$ to be the region inside $\gamma_3$ with punched out disks at $z_1$ and $z_2$ 

the disk centered at $z_1$ has the same orientation as $\gamma_1$, clockwise around $z_1$ 

the disk centered at $z_2$ doesn't have the same orientation as $\gamma_2$, which goes counterclockwise around $z_2$ 

and using the Cauchy Integral formula

$f(w) = \frac{1}{2\pi i}(I_3-I_2 +I_1)$ 

When deforming closed paths, we can allow the starting point to move (page 81)

Let $\gamma_0'(t) = z_i +r(t)e^{i\theta(t)}$ , $0 \leq t \leq 1$ 

We move the starting point such that $r(t) \geq r(0) = r(1)$ for all $t \in (0,1)$ 

Define $\gamma_1'(t) = z_i + r(0)e^{i\theta(0) + i2\pi mt}$, for some integer $m$ 

 we define subdivisions of $[0,1]​$, $0 = t_0 < \cdots < t_n = 1​$ s.t. $t_j​$ is a point where we have intersections

1. $\theta_j(t_j) = \theta_{j+1}(t_j)$ since the path is continuous
2. $\theta_j(t_j) - \theta_j(t_{j-1}) = \begin{cases} 2\pi & \text{if the path went around counterclockwise once} \\ 0 & \text{if the path came back to }\gamma(t_{j-1}) \text{ from where it left} \\ -2\pi &\text{if the path went around clockwise once} \end{cases}$ 

So: $\sum_{i =1}^n \theta_i(t_i)-\theta_i(t_{i-1}) = m2\pi $, where $m$ is an integer

also: $\sum_{i=1}^n \theta_i(t_i)-\theta_i(t_{i-1}) = \theta_n(t_n)-\theta_1(t_0) = \theta(1)-\theta(0) = m2\pi$ 

so $\gamma'_1(0) = \gamma_0'(0)$ and $\gamma_1'(1)  = \gamma_0'(1)$ 

Define $\gamma_s'(t) = z_i + ((1-s)r(t)+sr(0))e^{i((1-s)\theta(t)+s(\theta(0)+2\pi m))}$ 

$\gamma_s'(t)$ depends continuously on $s,t$ for $0 \leq s, t \leq 1$ 

let $M $ be the max value of $r(t)$

we have that $z_i + Me^{i\theta(t)}$ is fully contained in the region bounded by $\gamma_3$ 

$r(0) \leq (1-s)r(t) + sr(0) \leq (1-s)M +sr(0) \leq (1-s)M + sM = M$ 

so $\gamma_s(t)$ remains inside the region bounded by $\gamma_3$ 

##### Ex 2 

###### Determine if B is a domain

Domains must be open sets, but $0 \in B$

and for every open disk around $0$, with radius $\epsilon > 0$, 

$-\epsilon/2$ is contained in this disk, so not every element in $B$ has an open disk centered on them contained in $B$, so $B$ is not open.

$B$ is not a domain.

###### How many times is $g(z)$ is complex diff. at $z= 0$ 

$g(z)$ is differentiable at 0 if 

$\frac{g(z)-g(0)}{z}$ has a limit as $z \rightarrow 0$ 

if the limit exists, then the limit coming from the left must be the same as the limit coming from the right, but $z \rightarrow 0^-$ is not defined

so none.

###### How many times is $g(z)$ complex diff. at $z=1$

restricting the function to an open disk $D$ at $1$ with an appropriately small radius,

$g(z) = z^2\text{Log }z$ for all $z $ in $D$ 

$z^2$ is analytic on $D$ and so is $\text{Log }z$, so $g(z)$ is analytic on $D$ 

thus by the corollary on 115, $g(z)$ is infinitely differentiable at $z= 1$ 







 



