Renee Senining

Math 185

### Homework #10

#### Chapter VI, Sec. 1, ex. 1, 3, 5

##### 1. Find all possible Laurent expansions centered at 0 of the following functions:

###### (a) $\frac{1}{z^2 -z}$

$\frac{1}{z^2 -z} = \frac{1}{z(z-1)}$ 

$0 <|z| < 1$ : $\frac{1}{z(z-1)} = \frac{1}{z-1} - \frac{1}{z}$, $f_0(z) = \frac{1}{z-1}$ is analytic for $|z| < 1$, and $f_1(z) = -\frac{1}{z}$ is analytic for $|z| > 0$

$f_0(z) = -\frac{1}{1-z} = -\sum_{k=0}^\infin z^k$

$f_1(z) = -\frac{1}{z} $

$f(z) = -\sum_{k=-1}^\infin z^k$

$1 < |z| < \infin$: The function is analytic at $\infin$ and vanishes there, so its Laurent decomposition with respect to this exterior domain is $f(z) = f_1(z)$, $f_0(z) = 0$  

$f(z) = \frac{1}{z^2}\frac{1}{1-\frac{1}{z}} = \frac{1}{z^2}\sum_{k=0}^\infin(\frac{1}{z})^k$ $= \sum_{k=2}^\infin (\frac{1}{z})^k$ 

$ = \sum_{k=-\infin}^{-2} z^k$

###### (b) $\frac{z-1}{z+1}$ 

singularity at $z = -1$

$|z| < 1$: $f_0(z) + 0 = \frac{z-1}{z+1} = \frac{z + 1 -2}{z+1} = 1 - \frac{2}{z+1} = 1 - 2\frac{1}{1 - (-z)}$

$= 1 - 2\sum_{k=0}^\infin (-z)^k$ $= 1 - 2\sum_{k=0}^\infin (-1)^kz^k$$ = 1 -2 - 2\sum_{k=1}^\infin (-1)^kz^k$ $= -1 - 2\sum_{k=1}^\infin (-1)^kz^k$ 

$1 < |z| < \infin$, $f(z)$ is analytic, but doesn't disappear at $\infin$ 

so we obtain $f(z) = 1 - \frac{2}{z+1}$ again with $f_0(z) = 1$, $f_1(z) = -\frac{2}{z+1}$ 

$f_1(z) = -2\frac{1}{z+1} = -\frac{2}{z} \frac{1}{1 +(1/z)}$= $-\frac{2}{z}\sum_{k=0}^\infin (-1)^k(\frac{1}z)^k$

$2\sum_{k=1}^\infin (-1)^{k}(\frac{1}{z})^k$ 

$f(z) = 1 +2\sum_{k=1}^\infin (-1)^{k}(\frac{1}{z})^k$ 

###### (c) $\frac{1}{(z^2-1)(z^2-4)}$ 

$f(z) = \frac{A}{z^2-4} + \frac{B}{z^2-1}$

$A + B = 0$

$-A -4B = 1$, $A = -4B -1$

$-4B -1 + B = 0$ $\equiv B = -1/3$ 

$A = 1/3$ 

$f(z) = \frac{1}{3}\frac{1}{z^2 -4} - \frac{1}{3}\frac{1}{z^2-1}$ 

$|z| < 1$: 

$f(z)$ is analytic for all $|z| < 1$

so $f(z) = -\frac{1}{12}\frac{1}{1 - \frac{z^2}{4}} +\frac{1}{3}\frac{1}{1-z^2}$

$= \frac{-1}{12}\sum_{k=0}^\infin \frac{z^{2k}}{4^k} + \frac{1}{3}\sum_{k=0}^\infin z^{2k}$ $= \frac{-1}{12}\sum_{k=0}^\infin \frac{z^{2k}}{4^k} + \frac{1}{3*4}\sum_{k=0}^\infin 4z^{2k}$

$\frac{1}{12}\sum_{k=0}^\infin (4-4^{-k})z^{2k}$ 

$1 < |z| < 2$

$f_0(z) = \frac{1}{3}\frac{1}{z^2-4}$

$f_1(z) = -\frac{1}{3}\frac{1}{z^2-1}$ 

$f_0(z) = -\frac{1}{12}\frac{1}{1 - \frac{z^2}{4}} = -\frac{1}{12}\sum_{k=0}^\infin \frac{z^{2k}}{4^k}$

$f_1(z) = -\frac{1}{3}\frac{1}{z^2-1} = -\frac{1}{3z^2}\frac{1}{1- (1/z^2)} = \frac{-1}{3z^2}\sum_{k=0}^\infin \frac{1}{z^{2k}} = \frac{-1}{3}\sum_{k=1}^\infin\frac{1}{z^{2k}}$

$= \frac{-1}{3}\sum_{k= -\infin}^{-1}z^{2k}$ 

$f(z) = \sum_{k=-\infin}^\infin a_k z^{2k}$

where $a_k = -1/3$ for $k < 0$ and $a_k = \frac{-1}{12*4^k}$ for $k \geq 0$ 

$2 < |z| < \infin$ 

$f(z) = \frac{1}{3z^2}\frac{1}{1 - \frac{4}{z^2}} - \frac{1}{3z^2} \frac{1}{1 - \frac{1}{z^2}}$

$f(z) = \frac{1}{3z^2}\sum_{k=0}^\infin \frac{4^k}{z^{2k}} - \frac{1}{3z^2}\sum_{k=0}^\infin \frac{1}{z^{2k}}$

$f(z) = \frac{1}{3}\sum_{k=-\infin}^{-1} (4^{-k-1} -1)z^{2k}$ 

##### 3. Recall the power series for the Bessel function $J_n(z), n \geq 0$, given in Exercise V.4.11, and define $J_{-n} = (-1)^nJ_n(z)$. For fixed $w \in C$, establish the Laurent series expansion $\exp[\frac{w}{2}(z-1/z)] = \sum_{n=-\infin}^\infin J_n(w)z^n, 0 < |z| < \infin$. From the coefficient formula $(1.4)$ deduce that $J_n(z) = \frac{1}{2\pi}\int_0^{2\pi}e^{i(n\theta - z\sin\theta)}d\theta, z \in \C$

$J_n(z) = \sum_{k=0}^\infin \frac{(-1)^kz^{n+2k}}{k!(n+k)!(2^{n+2k})}$

$J_{-n} = \sum_{k=0}^\infin \frac{(-1)^{n+k}z^{n+2k}}{k!(n+k)!(2^{n+2k})}$ 

$a_n = \large {\frac{1}{2\pi i}\oint_{|z-z_0| = r}\frac{e^{\frac{w}{2}(z-1/z)}}{(z-z_0)^{n+1}}} \normalsize dz $

$z = z_0 + re^{-i\theta}$

The negative sign is for the circle going clockwise, since $\exp[\frac{w}{2}(z-1/z)]$ is analytic on the punctured complex plane, so 

$dz = ire^{i\theta}d\theta$ 

$a_n = \large \frac{1}{2\pi }\int_0^{2\pi}\frac{e^{\frac{w}{2}(z_0 + re^{i\theta} - \frac{1}{z_0 + re^{i\theta}})}}{r^{n}e^{in\theta}} d\theta$

 $a_n = \large {\frac{1}{2\pi i}\oint_{|z| = 1}\frac{e^{\frac{w}{2}(z-1/z)}}{(z)^{n+1}}} \normalsize dz $

$z = e^{-i\theta}$, $dz = -ie^{-i\theta}d\theta$ 

$a_n = -\frac{1}{2\pi}\int_0^{2\pi}\frac{e^{\frac{w}{2}(e^{-i\theta} - \frac{1}{e^{-i\theta}})}}{e^{-in\theta}}$

and using $\cos(-\theta) + i\sin(-\theta) - \frac{1}{\cos(-\theta) + i\sin(-\theta)} =$

$\cos(\theta) - i\sin(\theta) - \frac{1}{\cos(\theta) - i\sin(\theta)} =​$

$\frac{\cos^2\theta - 2i\cos\theta\sin\theta - \sin^2\theta -1}{\cos\theta - i\sin\theta}$

$= \frac{-2i\cos\theta\sin\theta - 2\sin^2\theta}{\cos\theta - i \sin\theta}$ 

$ = \frac{-2i\sin\theta(\cos\theta -i\sin\theta)}{\cos\theta - i\sin\theta}$

$ = -2i\sin\theta$ 

we obtain $a_n = \frac{1}{2\pi}\int_0^{2\pi}\frac{e^{-iw\sin\theta}}{e^{-in\theta}}$ $= \frac{1}{2\pi}\int_0^{2\pi}e^{i(n\theta -w\sin\theta)}d\theta$

and since $J_n(w) = a_n$, we have shown  $J_n(z) = \frac{1}{2\pi}\int_0^{2\pi}e^{i(n\theta - z\sin\theta)}d\theta, z \in \C$ 

replacing $w$ with $z$ 

##### 5. Suppose $f(z)$ is analytic on the punctured plane $D = \C\setminus${0}. Show that there is a constant $c$ such that $f(z) -c/z$ has a primitive in $D$. Give a formula for $c$ in terms of an integral of $f(z)$ 

we need $f(z) - c/z$ to be analytic on $D$ 

on $D$, we can express $f(z) = \sum_{k = -\infin}^\infin a_k z^k$ 

and from $(1.4)$

$a_{-1} = \frac{1}{2\pi i}\oint_{|z-z_0| r} \frac{f(z)}{z^0}dz$, where $r > 0$ 

so $f(z) - \frac{a_{-1}}{z} = \sum_{k \neq -1, -\infin < k < \infin}a_k z^k$

so let $c = a_{-1}$ 

a function is analytic on $D$ if and only if $f(z)dz$ is closed 

which means on any closed path containing a region in $D$, 

$\int_{\gamma}f(z) - c/z \;\;dz = 0$ 

and we've learned before that any closed path in an annulus can be continuously deformed to a circular path $C$ in the annulus, so 

$\int_{\gamma} f(z) - c/z dz = \int_{C} \sum_{k\neq -1}a_kz^k$

and since the power series converges uniformly on any circle strictly smaller than $\infin$ 

$\int_{C}\sum_{k\neq -1}a_kz^k = \sum_{k\neq -1}a_k\int_{C}z^k$

and from earlier, we know that $\int_{|z-z_0| = r} z^m$ $= 0$ whenever $ m \neq -1$ so the above is equal to $0$ 

so $f(z) - c/z$ is analytic on a star-shaped domain $D$, so it has a primitive in $D$ 

