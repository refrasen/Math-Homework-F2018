Renee Senining

Math 185

### Homework #11

#### Chapter VI, 

#### Sec. 2, ex. 1g, 1e, 1i, 3, 12;  

##### 1g. $\text{Log }(1 - \frac{1}{z})$

Singularities occur when

$1 - \frac{1}{z} \leq 0$ 

so $\frac{1}{z} \geq 1$

$0 \leq z \leq 1$

there are no isolated singularities 

##### 1e. $z^2 \sin (\frac{1}{z})$ 

Singularity at $z = 0$ 

$\sin z = \sum_{k=0}^\infin \frac{(-1)^{k}z^{2k+1}}{(2k+1)!}$

so $\sin(\frac{1}{z}) = \sum_{k=0}^\infin \frac{(-1)^k}{(2k+1)!z^{2k+1}}$

so $z^2\sin(\frac{1}{z}) = \sum_{k=0}^\infin \frac{(-1)^k}{(2k+1)!z^{2k-1}}$

has infinitely many negative powers of $z$

so $z = 0$ is an essential singularity

##### 1i. $e^{1/(z^2+1)}$ 

singularities when

$z^2 + 1 = 0$, so $z = \pm i$

$z = re^{i\pi/2}$

as $r \rightarrow 1^+$, we have $1/(z^2+1) \rightarrow - \infin$  

so $e^{1/(z^2+1)} \rightarrow 0$ (not a pole)

as $r \rightarrow 1^{-}$, we have $1/(z^2+1) \rightarrow +\infin$, 

so $e^{1/z^2+1} \rightarrow \infin$ (not removable)   

and similarly for $z = -i$ with $z = re^{-i\pi/2}$

essential

##### 3. Consider the function $f(z) = \tan z$ in the annulus {$3 < |z| < 4$} Let $f(z) = f_0(z) +f_1(z)$ be the Laurent decomposition of $f(z)$, so that $f_0(z)$ is analytic for $|z| < 4$, and $f_1(z)$ is analytic for $|z| > 3$ and vanishes at $\infin$ 

###### (a) Obtain an explicit expression for $f_1(z)$ 

Singularities: $\frac{\pi}{2} + \pi m = \frac{(2m+1)\pi}{2}$ $m \in \Z$

$1/f(z) = \frac{\cos z}{\sin z}$, which is analytic at each $\frac{(2m+1)\pi}{2}$

$(1/f(z))' = \frac{-\sin^2z - \cos^2z}{\sin^2z} = -\frac{1}{\sin^2 z}$$\neq 0$ at $z = \frac{(2m+1)\pi}2$

so $1/f(z)$ has a zero of order $1$ at each $z = \frac{(2m+1)}2$

so each $\frac{(2m+1)\pi}{2}$ is a simple pole

$\pm\frac{\pi}{2}$ are the only isolated singularities in {$|z| < $4}

$\cos z = \sum_{k=0}^\infin a_k(z-\pi/2)^k$, if $k$ even, $a_k = 0$, and $a_1 = -1$, $a_3 = 1$, etc...

since $a_0 = \cos(\pi/2) = 0$, $a_1 = -\sin(\pi/2) = -1$, $a_2 = 0$, $a_3 = \sin (\pi/2)$ 

$\cos z = \sum_{k=0}^\infin \frac{(-1)^{k+1}(z-\pi/2)^{2k+1}}{(2k+1)!}$$= (z-\pi/2)\sum_{k=0}^\infin \frac{(-1)^{k+1}}{(2k+1)!}(z-\pi/2)^{2k}$

$= (z - \pi/2)(-1 + \frac{(z-\pi/2)^2}{3!} - . . . )$

$= -(z-\pi/2) + (z-\pi/2)\sum_{k=1}^\infin  \frac{(-1)^{k+1}}{(2k+1)!}(z-\pi/2)^{2k} $ 

$\frac{1}{\cos z} = -\frac{1}{(z-\pi/2)}\frac{1}{1-\sum_{k=1}^\infin \frac{(-1)^{k+1})}{(2k+1)!}(z-\pi/2)^{2k}}$

$\frac{1}{\cos z} = -\frac{1}{z-\pi/2} + \text{analytic}$, the analytic part is  $\sum_{l=1}^\infin(\sum_{k=1}^\infin\frac{(-1)^{k+1}}{(2k+1)!}(z-\pi/2)^{2k-1} )^l$

$\sin z = \sum_{k=0}^\infin \frac{(-1)^k}{(2k)!}(z-\pi/2)^{2k} = 1 + \sum_{k=1}^\infin \frac{(-1)^k}{(2k)!}(z-\pi/2)^{2k}$

since $a_0 = \sin(\pi/2) = 1$, $a_1 = \cos(\pi/2) = 0$, $a_2 = -\sin(\pi/2)/2! = -1/2!$, $a_3 = 0$  

so $\sin z/\cos z = \tan z = -\frac{1}{z-\pi/2} + \text{analytic} $

for $-\pi/2$, 

$a_k = 0$ still when $k = 0$, but this time $a_1 = 1$, $a_3 = -1$, so

$\cos z = (z+\pi/2)\sum_{k=0}^\infin \frac{(-1)^k}{(2k+1)!}(z+\pi/2)^{2k}$

so we have $\frac{1}{\cos z} = \frac{1}{z + \pi/2} + \text{analytic}$ 

$\sin z = \sum_{k=0}^\infin \frac{(-1)^{k+1}}{(2k)!}(z+\pi/2)^{2k} = -1 + \sum_{k=1}^\infin \frac{(-1)^{k+1}}{(2k)!}(z-\pi/2)^{2k}$

$\tan z = -\frac{1}{z+\pi/2} + \text{analytic}$ 

so since $\tan z + \frac{1}{z-\pi/2} + \frac{1}{z+\pi/2}$ is analytic for {$|z| < 4$}

$f_1(z) = -(\frac{1}{z-\pi/2}+\frac{1}{z+\pi/2})$ , and is obviously analytic for $|z| > 3$

and as $z \rightarrow \infin$, $f_1(z) \rightarrow 0$, so with $f_0 = \tan z - f_1$

$f_0(z) + f_1(z)$ is unique Laurent Decomposition

###### (b) Write down the series expansion for $f_1(z)$, and determine the largest domain on which it converges

$-\frac{1}{z-\pi/2} = - \frac{1}{z}\frac{1}{1 - \pi/2z}$

and this is equal to a geometric series: $-\frac{1}{z}\sum_{k=0}^\infin \frac{\pi^kz^{-k}}{2^k}$

$-\frac{1}{z+\pi/2} = -\frac{1}{z} \sum_{k=0}^\infin (-1)^k \frac{\pi^k z^{-k}}{2^k}$ 

adding the two:

$f_1(z) = -\frac{1}{z}\sum_{k=0}^\infin [(-1)^k + 1] \frac{\pi^k z^{-k}}{2^k}$

so when $k$ is odd, $a_k = 0$, so

$f_1(z) = -2\sum_{k=0}^\infin \frac{\pi^{2k}z^{-2k-1}}{4^{k}}$

$f_1(z) = -2\sum_{k=-\infin}^0 \frac{\pi^{-2k}}{4^{-k}}z^{2k-1}$

converges for all $|z| > \pi/2$ 

###### (c) Obtain the coefficients $a_0, a_1,$ and $a_2$ of the power series expansion of $f_0(z)$

since $\tan z$ is an odd function, 

$a_ 0 = a_2 = 0$ 

Since $f_0(z)$ is a power series centered at $0$ and 

$f_0(z) = \tan z + \frac{1}{z-\pi/2} + \frac{1}{z+\pi/2}$

$f'_0(z) = \frac{1}{\cos^2(z)} - \frac{1}{(z-\pi/2)^2} - \frac{1}{(z+\pi/2)^2}$

and $f_0'(0) = 1 - 8/\pi^2$  

so $a_1 = f'_0(0)/1 = 1 - 8/\pi^2$

I'm currently using the 2nd edition, and the back of the book says $1 + 8/\pi^2$, but a list of errata changes it to $1 - 8/\pi^2$ 

http://www.math.ucla.edu/~twg/errata.pdf see the 3rd page

###### (d) What is the radius of convergence of the power series expansion for $f_0(z)?$ 

$f_0(z) = \tan z - f_1(z)$ is analytic except at $z = \pm 3\pi/2$, so the radius of convergence is $3\pi/2$ 

##### 12. Show that if $z_0$ is an isolated singularity of $f(z)$ that is not removable, then $z_0$ is an essential singularity for $e^{f(z)}$

if $z_0$ is essential for $f(z)$ 

then for any $w_0 \in \C$, there is a sequence $z_n \rightarrow z_0$ such that 

$f(z_n) \rightarrow w_0$ 

so there are two sequences $z_{n} \rightarrow z_0$ and $z_n' \rightarrow z_0$ 

with $f(z_n) \rightarrow w_0$, $f(z_n') \rightarrow w_0'$ 

which means $e^{f(z)}$ as $z \rightarrow z_0$  has no limit

so $|e^{f(z)}|$doesn't $\rightarrow \infin$  as $z \rightarrow z_0$ 

but also $e^{f(z)}$ isn't bounded near $z_0$ 

for any $M > 0$, we may choose $w_0$ with $ \log|w_0| > \log M$ such that $f(z_n) \rightarrow w_0$ for some sequence $z_n \rightarrow z_0$ 

and there exists some $N$, such that for $n \geq N$, $|f(z_n)| > \log M$

which means $|e^{f(z_n)}| > M$ for $n \geq N$

so $z_0$ is essential 

if $z_0$ is a pole of order $N$ for $f(z)$ 

then $f(z) = g(z)/(z-z_0)^N$ where $g(z)$ is analytic at $z_0$ and $g(z_0) \neq 0$ 

and $|f(z)| \rightarrow \infin$ 

we're always able to approach $z_0$ in a way that $(z-z_0)^N$ is positive/negative or neither (for example, approaching $z_0$ from the positive real direction so that $(z-z_0)^N > 0$ or we may build a sequence $z-z_0 \rightarrow 0$ so that every other term is real or pure imaginary)

so depending on the value of $g(z_0)$, we may choose a way to approach $z_0$ so that $f(z) \rightarrow +\infin$ or $f(z) \rightarrow - \infin$ 

which means $e^{f(z)}$ isn't bounded at $z_0$, so $z_0$ isn't removable

but also, $e^{f(z)}$ doesn't have a limit, so $|e^{f(z)}|$ doesn't approach $\infin$ as $z \rightarrow z_0$ so it isn't a pole

so $z_0$ is essential 

#### Sec. 3, ex. 1 (for (g),(e),(i));  

##### 1g. $\text{Log }(1- \frac{1}{z})$ 

by definition $f(z)$ has an isolated singularity at $\infin$ if $f(z)$ is analytic outside some bounded set, 

so $f(z)$ is analytic for $|z| > 1$, since for $z \in [0, 1]$, it isn't analytic

so there is an isolated singularity at $\infin$ 

From earlier problem:

if $z_0$ is an isolated singularity of $f(z)$ that is not removable, then $z_0$ is an essential singularity for $e^{f(z)}$

$\equiv$ if $z_0$ is not essential for $e^{f(z)}$ then $z_0$ is a removable singularity of $f(z)$ $g(w) = \text{Log}(1-w)$  is analytic at $w = 0$ (if there were an isolated singularity at $w = 0$, it is removable)

$e^{g(w)} = 1 - w$, so since $a_k = 0$ for all $k < 0$, $w = 0$ is not essential for $e^{g(w)}$, 

which means $0$ is a removable singularity for $g(w)$ 

 $\equiv$ $\infin$ is removable for $\text{Log }(1- \frac{1}{z})$ 

##### 1e. $z^2 \sin (\frac{1}{z})$

from its Laurent series, $z^2\sin(\frac{1}{z}) = \sum_{k=0}^\infin \frac{(-1)^k}{(2k+1)!z^{2k-1}}$

we have $N = 1$, where $b_1 = 1$, and for all $k > 1$, $b_k = 0$ 

so we have a simple pole at $\infin$ 

##### 1i. $e^{1/(z^2+1)}$ 

$g(w) = f(1/w) = e^{1/(\frac{1}{w^2}+1)}$

has an isolated singularity at $w = 0$, so $f(z)$ has an isolated singularity at $\infin$ 

as $w \rightarrow 0$, $\frac{1}{w^2} \rightarrow \infin$, so $\frac{1}{\frac{1}{w^2}+1} \rightarrow 0$ and $e^{1/(\frac{1}{w^2}+1)} \rightarrow 1$

which means near $0$, $g(w)$ is bounded, so $g(w)$ has a removable singularity at $0$ 

which means $f(z)$ has a removable singularity at $\infin$ 

#### Sec. 4, ex. 1c, 1f, 2c, 3

##### 1c. $\frac{1}{(z+1)(z^2 + 2z + 2)}$ 

$\frac{A}{z+1} + \frac{B}{z + 1 - i} + \frac{C}{z + 1 +i}$

since: $(z + 1 + i)(z+ 1 -i) = z^2 + 2z + 2$

$A(z^2 + 2z + 2) + B(z+1)(z+1 + i) + C(z+1)(z+1-i) = 1$

$(z+1)(z+1+i) = z^2 + z + iz + z + 1 + i = z^2 + (2+i)z + (1+i)$

$(z+1)(z+1 -i) = z^2 + z - iz + z + 1 -i = z^2 +(2-i)z + (1-i)$

$A + B + C = 0$

$2A + (2 +i)B + (2-i)C = 0$

$2A + (1+i)B + (1-i)C = 1$ 

$(2+i)B + (2-i)C = (1+i)B + (1-i)C -1$

$2B + 2C = (2+i)B + (2-i)C$

$B + C = -1$

$B -C = 0$

$B = C$

$B = -\frac{1}{2}$ $= C$ 

$A = 1$ 

$\frac{1}{(z+1)(z^2 + 2z + 2)} = \frac{1}{z+1} - \frac{1/2}{z+1 -i} - \frac{1/2}{z+1 +i}$ 

##### 1f. $\frac{z^2 - 4z + 3}{z^2 - z- 6}$ 

$z^2 - 4z + 3 = (z^2 - z - 6) -3z + 9$

$\frac{z^2 - 4z + 3}{z^2 - z - 6} = 1 + \frac{-3z + 9}{z^2 - z - 6}$

$z^2 - z - 6 = (z-3)(z+2)$

poles at $-2, 3$ 

$\frac{A}{z-3} + \frac{B}{z+2}$ 

$A + B = -3$

$-3B + 2A = 9$ 

$-5B = 15$

$B = -3$, $A = 0$ 

also $\frac{-3(z - 3)}{(z-3)(z+2)} = \frac{-3}{z+2}$

so $\frac{z^2 - 4z + 3}{z^2 - z- 6} = 1 - \frac{3}{z+2}$

#####  2c $\frac{z^6}{(z^2+1)(z-1)^2}$ 

$(z^2+1)(z-1)^2 = (z^2+1)(z^2 - 2z +1) = z^4 -2z^3 + z^2 +z^2 -2z + 1 = z^4 -2z^3 + 2z^2 -2z +1$

$z^6 = z^2(z^4 - 2z^3 + 2z^2 - 2z + 1) + 2z^5 -2z^4 + 2z^3 -z^2$

$2z^5 - 2z^4 + 2z^3 - z^2 = 2z(z^4 - 2z^3 + 2z^2 - 2z + 1) + 2z^4 - 2z^3 + 3z^2 - 2z$

$2z^4 - 2z^3 + 3z^2 - 2z = $ $2(z^4 - 2z^3 + 2z^2 - 2z + 1) + 2z^3 -z^2  + 2z -2$

$z^6 = (z^2 + 2z + 2)(z^4 - 2z^3 + 2z^2 - 2z + 1) + 2z^3 - z^2 + 2z - 2$ 

$\frac{z^6}{(z^2+1)(z-1)^2} = z^2 + 2z + 2 + \frac{2z^3 - z^2 + 2z - 2}{(z^2 + 1)(z-1)^2}$

$\frac{A}{z + i} + \frac{B}{z-i} + \frac{C}{(z-1)^2} + \frac{D}{z-1}$ 

$A(z-i)(z-1)^2 = A(z-i)(z^2 - 2z + 1) = A(z^3 - 2z^2 + z -iz^2 + 2iz -i)$$= A(z^3 -(2+i)z^2 + (1 + 2i)z - i$ )

$B(z+i)(z^2 - 2z + 1) = B(z^3 -2z^2 + z + iz^2 - 2iz + i) = B(z^3 +(-2 + i)z^2 + (1 -2i)z + i)$

$C(z^2 + 1)$

$D(z^2 + 1)(z-1) = D(z^3 -z^2 + z - 1)$

---

(1) $A + B + D = 2$

(2) $-(2+i)A + (-2 +i)B + C - D = -1$

(3) $(1+2i)A + (1-2i)B + D = 2$

(4) $-iA + iB + C - D = -2$ 

---

(1) and (3) $\implies$ $A+B = (1+2i)A + (1-2i)B$ 

$\equiv$ $-A + B = 0$, $A = B$  (5)

(5) and (1) $\implies 2A + D = 2$

$D = 2 - 2A$ (6)

(5) and (4) and (6): $C - D = -2$ $\implies$ $C - 2 + 2A = -2$ $\implies $$2A + C = 0$ 

so $C = -2A$ (7) 

(2) and (5) and (7) and (6): $-(2+i)A + (-2+i)A -2A - 2 + 2A = -1$

$-2A -2A = 1$, $A = -\frac{1}{4} = B$

$D = 2 +\frac{1}{2} = \frac{5}{2}$

$C = \frac{1}{2}$ 

$\frac{z^6}{(z^2+1)(z-1)^2} = \frac{-1/4}{z + i} + \frac{-1/4}{z-i} + \frac{1/2}{(z-1)^2} + \frac{5/2}{z-1}$ 

##### 3. Let $V$ be the complex vector space of functions that are analytic on the extended complex plane except possibly at the points $0$ and $i$, where they have poles of order at most two. What is the dimension of $V$? Write down explicitly a vector space basis for $V$ 

$V = ${$f(z): f(z) = f_{\infin}(z) + \frac{B}{z} + \frac{C}{z^2} + \frac{D}{z-i} + \frac{E}{(z-i)^2}$}

so $f_{\infin}(z) = A$, where we let $A$ be a complex constant

this is equivalent to finding all vectors:

$(A, B, C, D, E)$ $\in \C^5$ 

 The dimension is therefore equal to 5

and using standard bases in $\C^5$:

$(1, 0, 0, 0, 0), (0, 1, 0, 0, 0), (0, 0, 1, 0, 0), (0, 0, 0, 1, 0), (0, 0, 0, 0, 1)$ 

$1, 1/z, 1/z^2, 1/(z-i), 1/(z-i)^2$

is a basis for $V$ 