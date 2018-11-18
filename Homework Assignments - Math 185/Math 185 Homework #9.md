Renee Senining

Math 185

### Homework #9

#### **Chapter V**, Sec. 4. ex. 1d, 1f, 3;  Sec. 5, ex. 1c;  Sec. 6, ex. 3;  Sec. 7, ex. 1a, 1f, 1i;  Sec. 7, ex. 9, 11;

[Extra Problem (by the link)](https://math.berkeley.edu/~art/data/F18-185/HW9.pdf)

##### Sec. 4. ex 1: Find the radius of convergence of the power series for the following functions, expanded about the indicated point

###### (d) $\text{Log }z$, about $z = 1 + 2i$ 

The nearest singularity is $0$, since $(1,2)$ is in the first quadrant 

$R = |1 + 2i| = \sqrt{1 + 4} = \sqrt{5}​$ 

###### (f) $\frac{z -i}{z^3-z}$ about $z = 2i$ 

$z^3 - z = z(z^2 - 1) = z(z-1)(z+1)$ 

singularities at $0, -1, 1$ 

nearest is at $0$

$R = |2i| = \sqrt{2^2} = 2$

##### Sec. 4. ex. 3 Find the power series expansion of $\text{Log }z$ about the point $z = i -2$. Show that the radius of convergence of the series is $R = \sqrt{5}$. Explain why this does not contradict the discontinuity of $\text{Log }z $ at $z = -2$ 

$\text{Log }z = \sum_{k=0}^\infin a_k(z-(i-2))^k$

$a_0 = \text{Log}(i-2) = \log(\sqrt{5}) + \text{Arg }(i-2)$

$a_1 = \frac{1}{i-2}$

$a_2 = -\frac{1}{2(i-2)^2}$

$a_3 = \frac{2}{6(i-2)^3} = \frac{1}{3(i-2)^3}$

$a_k = (-1)^{k+1}\frac{1}{k(i-2)^k}$$, k \geq 1$ 

$|a_{k}/a_{k+1}| = |\frac{(k+1)(i-2)^{k+1}}{k(i-2)^k}| = |\frac{(k+1)(i-2)}{k}| \rightarrow |i-2|$ as $k \rightarrow \infin$

and $|i-2| = \sqrt{1^2 + (-2)^2} = \sqrt{5}$

so $R = \sqrt{5}$ 

$\text{Log }z = \text{Log}(i-2) + \sum_{k=1}^\infin \frac{(-1)^{k+1}}{k(i-2)^k} (z-(i-2))^k$

This power series has the same radius of convergence as that for $\frac{1}{z}$, which is analytic on any disk contained in $\C \setminus${$0$}. 

In the part of the disk that goes beyond the cut (the negative real axis and origin), the series expansion does not agree.

$\text{Log }z$ extends to be analytic for $|z-(i-2)| < \sqrt{5}$, though the extension does not coincide with $\text{Log }z$ in the part of the disk in the lower half plane

##### Sec. 5. ex. 1: Expand the following functions in power series about $\infin$:

###### (c) $e^{1/z^2}$

$g(w) = f(1/w) = e^{w^2}$ 

using $e^z = \sum_{k=0}^\infin z^k/k!$ 

$e^{w^2} = \sum_{k=0}^\infin \frac{w^{2k}}{k!}$ 

$ e^{1/z^2} = \sum_{k=0}^\infin \frac{1}{z^{2k}k!}$

##### Sec. 6. ex. 3: Show that $\frac{e^z}{1+z} = 1 + \frac{1}2 z^2 - \frac{1}3z^3 + \frac{3}{8}z^4 - \frac{11}{30}z^5 + . . . $ . Show that the general term of the power series is given by $a_n = (-1)^n [\frac{1}{2!}-\frac{1}{3!} + . . . +  \frac{(-1)^n}{n!}]$. What is the radius of convergence of the series?

$1/(1+z) = \sum_{k=0}^\infin (-1)^kz^k = b_k z^k$

$e^z = \sum_{k=0}^\infin z^k/k! = \sum a_k z^k$ 

$e^z/(1+z) = \sum c_k z^k$

so $a_k = 1/k!$, $b_k = (-1)^k$ $\implies$ 

$c_k = a_kb_0 + a_{k-1}b_1 + . . . + a_0b_k = \frac{1}{k!} -  \frac{1}{(k-1)!} + . . . + (-1)^{k-1}+(-1)^k = \frac{1}{k!} - \frac{1}{(k-1)!} + . . . + \frac{(-1)^{k-2}}{2}$

so $ c_k = (-1)^k[\frac{(-1)^{-2}}{2}  + \frac{(-1)^{-3}}{3!} + . . . + \frac{(-1)^{-k}}{k!}]$ 

which is equivalent to $c_k = (-1)^k[\frac{1}{2!} - \frac{1}{3!} + . .. + \frac{(-1)^{k}}{k!}]$

and $c_0 = 1, c_1 = (1*1)+(1*(-1)) = 0 $

and using the above equation:

$c_2 = 1/2$

$c_3 = -1/2 + 1/6 = -2/6 = -1/3$

$c_4 = 1/2 - 1/6 + 1/24 = \frac{12 - 4 + 1}{24} = \frac{9}{24} = \frac{3}{8}$

$c_5 = -1/2 + 1/6 - 1/24 + 1/120 = -\frac{3}{8} + \frac{1}{120} = \frac{-44}{120} = -11/30$

Since we are looking at the power series about $z_ 0 =0$, and the nearest singularity is at $z = -1$, The radius of convergence is $R = |-1| = 1$

##### Sec 7. ex. 1: Find the zeros and orders of zeros of the following functions

###### (a) $\frac{z^2+1}{z^2-1}$

$f(i) = 0$, $f(-i) = 0$

and $f'(z) = \frac{2z(z^2 -1) - 2z(z^2+1)}{(z^2-1)^2} = \frac{-4z}{(z^2-1)^2}$, which is not zero at $z = \pm i$

so each of the zeros, $\pm i$ are simple zeros

###### (f) $\frac{\cos z - 1}{z^2}$

zeros at $z = 2\pi n$ 

$f'(z) = \frac{-z^2\sin z - 2z(\cos z -1)}{z^4}$

$f'(2\pi n) = \frac{-(2\pi n)^2(0) - 4\pi n(0)}{16n^4\pi^4} = 0$

$f''(z) = \frac{(-2z\sin z -z^2\cos z -2(\cos z -1)+2z(\sin z))(z^4)- 4z^3(-z^2\sin z - 2z(\cos z -1))}{z^8}$ 

$f''(2\pi n) = \frac{(2\pi n)^4(-(2\pi n)^2}{(2\pi n)^8} \neq 0$

so double zeros at $z = 2\pi n$ when $n \neq 0$,

$\cos z - 1 = \sum_{k=1}^\infin \frac{(-1)^kz^{2k}}{(2k)!}$

and $\frac{\cos z - 1}{z^2} = \sum_{k=0}^\infin \frac{(-1)^{k+1}z^{2k}}{(2(k+1))!}$

so $z = 0$ is not a zero, since $a_0 = -1/2$ 

###### (i) $\frac{\text{Log }z}{z}$ (principal value)

$\text{Log 1} = \log(1) + \text{Arg }(1) = 0 + 0 = 0$, since $\text{Arg}(1) \in (-\pi, \pi] $ 

so $z = 1$ is a zero

$f'(z) = \frac{1 - \text{Log }z}{z^2}$, which is not $0$ at $z = 1$, so $z = 1$ is a simple zero

##### Sec. 7. ex. 9: Show that if the analytic function $f(z)$ has a zero of order $N$ at $z_0$, then $f(z)= g(z)^N$ for some function $g(z)$ analytic near $z_0$ and satisfying $g'(z_0) \neq 0$

we can write $f(z)$ as $f(z) = (z-z_0)^Nh(z)$, where $h(z)$ is analytic at $z_0$ and $h(z_0) \neq 0$

$g(z) = (z-z_0)e^{\text{log}(h(z))/N}$, for a branch of logarithm containing $h(z_0)$ so: $f_m(z) = \text{Log }z + 2\pi i m$, where $m \in (-\infin, \infin)$ 

$g'(z_0) = e^{\log(h(z_0))/N} + (z_0 - z_0)\frac{d}{dz}[e^{\log(h(z))/N}]_{z= z_0} \neq 0$

since $e^z \neq 0$ for all $z \in \C$ 

and obviously $g(z)^N = (z-z_0)^Nh(z) = f(z)$  

also $e^z$ is analytic, $(z-z_0)$ is analytic

and $\log(h(z))/N$ is analytic for the branch containing $h(z_0)$  

so $g(z)$ is a composition of functions that are analytic near $z_0$ , so it is analytic near $z_0$ 

##### Sec. 7. ex. 11: Show that if $f(z)$ is a nonconstant analytic function on a domain $D$, then the image under $f(z)$ of any open set is open.

at any point $z_0 \in D$, where $f'(z_0) \neq 0$, 

there is a small disk $U \sub D$ containing $z_0$ such that $f(z)$ is one-to-one on $U$, and the image $V = f(U)$ of $U$ is open

$f$ maps open disks to open sets, so for any $z_0$ where $f'(z_0 ) \neq 0$ , $f(D) $ contains an open disk centered at $f(z_0)$, so $f(D)$ is open

and since any open set in $D$ is a union of open disks, for any $z_0$ in an open set, 

there is a disk that is contained in $U$ and $D$ s.t. a disk centered at $f(z_0)$ is contained in the image of this set under $f$, so the image is open.

if $f'(z_0) = 0$:

What I will use:

1. $z \mapsto az+b$ is open when $a \neq 0$ 

   let $a = Ae^{i\phi}$, where $A \in \R^+$ and $\phi \in \R$ 

   for any open disk centered on $z_0$ with radius $r$, 

   $z$ in this disk satisfies $|z| - |z_0| \leq|z-z_0| < |re^{i\theta}|$, for any $\theta \in \R$ 

   let $w_0 = az_0 + b$, and for any $z$ in the disk, let $w = az + b$ 

   $|w-w_0| = |a(z-z_0)| = |Ae^{i\phi}||z-z_0| < |Ae^{i\phi}||re^{i\theta}| = Ar$

   so the image of any open disk is also an open disk

   $\implies$ since open sets are unions of open disks, this mapping is open

2. $z^k$ where $k \in \N$ is open

   Show for a disk centered at origin with radius $r$

   the image of this disk will be an open disk centered at origin with radius $r^k$ 

3. The composition of open mappings is open

   if $f$ is open on $D_1$ and $g$ is open on $D_2$ and $g(D_2) \sub D_1$

   then $f(g(D_2))$ is open

if $f(z_0) = 0$

then $f(z) = g(z)^N$ (as in exercise 9)

and from 2., $f(z)$ is open

if $f(z_0) \neq 0$ 

then we can define $ f^*(z) = f(z) - f(z_0)$, so $f^*(z_0) = 0$ 

and so $f^*(z) = g(z)^N$ (as in exercise 9)

and $f(z) = g(z)^N + f(z_0)$

and since $f(z)$ is a composition of $g(z)$, $z^N$, and $z + f(z_0)$ (each are open  maps)

$f(z)$ is open

#### [Extra Problem (by the link)](https://math.berkeley.edu/~art/data/F18-185/HW9.pdf)

##### 1. Let $C$ be the right half of the unit circle centered at origin. Does there exist an entire function $f: \C \rightarrow \C$ with the specified values on $C:$

$f(e^{i\theta}) = e^{i\theta/2}$ for all $\theta \in [-\frac{\pi}2, \frac{\pi}2]$ 

so $C$ is a set that has a non isolated point (every point on the right half of the unit circle gets arbitrarily close to each other)

and any function $f(z)$ s.t. $f$ maps $e^{i\theta}$ to $e^{i\theta/2}$ for all $ \theta \in [-\pi/2, \pi/2]$ 

is equal to $g(z) = \sqrt{z}$ on $C$, which is analytic on the entire slit plane $\C \setminus(-\infin, 0]$

and by the Uniqueness Principle, if $f(z)$ is also analytic on the slit plane, 

$f(z) = g(z)$ for all $z$ in the slit plane

however, $g(z)$ is not analytic for any point in $(-\infin, 0]$ (not continuous)

if $f(z)$ were entire, it would also need to be analytic on $(-\infin, 0)$ 

but as $z \rightarrow$ the negative axis, $f(z)$ has no limit, (approaching the $-r \in \R$ from the top, we have $f(z) \rightarrow i\sqrt{r}$ but coming up from the bottom, $f(z) \rightarrow - i \sqrt{r}$ )

so $f(z)$ is not continuous on $(-\infin, 0]$ 

so $f$ cannot be entire.