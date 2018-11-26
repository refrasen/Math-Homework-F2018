Renee Senining

Math 185

### Homework #13

#### Chapter VIII, Sec. 1, ex. 1;  Sec. 2, ex. 2, 8;  Sec. 3, ex. 2;  Sec. 4, ex. 4, 6

##### Chapter VIII, Sec. 1, ex. 1

Show that $z^4 + 2z^2 - z + 1$ has exactly one root in each quadrant:

This is a polynomial with real coefficients and no real zeros, 

$z^4 + 2z > 0$ for all $z \in \R$

and for all $z < 0$, $p(z) > 0$

for all $z \geq 1$, $z^2 \geq z$, so $2z^2 - z > 0$, meaning $p(z) > 0$ for $z \geq 1$

for $z = 0$, $p(z) = 1 > 0$

so for $0 < z < 1$:

$-1 < -z < 0$ $\implies$ $0 < -z +1 < 1$, so $p(z) > 0$ 

so in the end: $p(z) > 0$ for all $z \in \R$  

so we have 2 conjugate pairs of zeros. ($a_i \pm b_i, i = 1, 2$)

So we need only to check two quadrants: the first and second 

We have that there are $2$ zeros in the 1st and 2nd quadrant and 2 zeros in the 3rd and 4th quadrant

possibilities: $2$ in either the first or second, or one in each:

First Quadrant:

estimate the increase of $\arg p(z)$ around the boundary of the quarter disk $D_R$ of a large radius $R$

The increase in the argument of $p(z)$ around $\partial D_R$ $= 2\pi(N_0)$ (no singularities)

where $N_0$ is the number of zeros in $D_R$ 

$\partial D_R$ is made up of three paths: 

1. The real axis from $0$ to $R$ 

   $p(x) > 0$, so there is no increase in argument, i.e., $= 0$

2. The quarter-circle $\Gamma_R$ defined by $|z| = R$ and $0 \leq \arg z \leq \pi/2$, 

   the term $z^4$ "dominates"

   and $\arg p(z) \approx 4\arg z $

   so the increase is approximately $2\pi$ along this path

3. along the imaginary axis from $iR$ to $0$ 

   let $z = iy$ with $0 \leq y \leq R$

   $p(iy) = y^4 - 2y +1 - iy$ 

   $ \Re(p(iR)) \approx R^4 , \Im(p(iR)) =-R$ 

   so $p(iy)$ starts in the 4th quadrant with argument $\approx 0$ 

   At $0$, $p(0) = 1$ 

   So starts at about the real axis, ends at about the real axis

   Need to know $k$ for $2\pi k$ for increase in argument here

   so how many times does it cross the real axis?

   crosses once at $y = 0$, the terminal point

   so the increase is approximately $0$ here

So in the first quadrant, the increase in argument around $\partial D_R$ is approx. $2\pi$ and therefore exactly $2\pi$ by the theorem on page 226

the number of zeros we have in the first quadrant is $1$, so that means

1. there's a conjugate zero in the 4th quadrant
2. a zero in the 2nd quadrant with a conjugate zero in the 3rd

Therefore, one zero in each quadrant.

##### Chapter VIII, Sec. 2 ex. 2

How many roots does $z^9 + z^5 - 8z^3 + 2z + 1$ have between the circles {$|z| = 1$} and {$|z| = 2$}

Let $D$ be the region bounded by the two circles

Goal: find $f(z), h(z)$ analytic on $D$ and $\partial D$ with $|h(z)| < |f(z)|$ for $z \in \partial D$

$f(z) = z^9 + z^5 - 8z^3$, $h(z) = 2z + 1$

---

I want to use the property:

$|a-b| \geq ||a| - |b||$ but to prove it I need to show:

if $a, b \in \R$ with $b \geq 0$ then:

$|a| \leq b \iff -b \leq a \leq b$

Proof:

let $|a| \leq b$ $\equiv $ $-|a| \geq -b$

$\implies$ since $-|a| \leq a \leq |a|$

we immediately get $ -b \leq a \leq b$

Let $-b \leq a \leq b$:

$a$ is either $ = -|a|$ or $= |a|$ 

if $a = |a|$:

$|a| \leq b$ as desired

if $a = -|a|$

then $-|a| \geq - b$ $\equiv$ $|a| \leq b$ 

so proving $|a-b| \geq ||a| - |b||$:

using triangle inequality:

$|a - b + b| = |a| \leq |a-b| + |b|$ $\equiv$ $|a| - |b| \leq |a-b|$ 

$|b-a + a| = |b| \leq |b-a| + |a| = |a-b| + |a| \equiv |b| - |a| \leq |a-b|$ $\equiv$ $|a| - |b| \geq - |a-b|$ 

so $-|a-b| \leq |a| - |b| \leq |a-b|$  $\implies$ $||a| - |b|| \leq |a-b|$ 

---

for $|z| = 1$:

$|h(z)| = |2z + 1| \leq 2|z| + 1 = 3$

$|f(z)| = |z^9 + z^5 - 8z^3| \geq ||z^9 + z^5| - |8z^3||$

since $|z| = 1$, $|z^k| = 1$ for any $k \in \N$ 

so $z^9$ and $z^5$ are on the unit circle still and the longest length the resultant vector from adding any two vectors of length one gets is $2$

since $|z^9 + z^5| - 8$ gets smaller the closer $|z^9 + z^5|$ gets to $8$, and the closest it gets to $8$ is $2$:

so $||z^9+z^5|-|8z^3||= ||z^9+z^5| - 8| \geq 6$ 

so $|f(z)| > |h(z)|$ on $|z| = 1$

$|z| = 2$:

$|h(z)| = |2z +1| \leq 2|z| + 1 = 5$

$|f(z)| \geq ||z^9 + z^5| - |8z^3||$ $ = ||z^9+z^5|-64|$

$z^9$ will have length $2^9$ and $z^5$ will have length $2^5$ 

again, $|z^9 + z^5|$ $-64$ gets smaller in magnitude to the closer $|z^9 + z^5|$ gets to $64$

the smallest we can get from adding two vectors of these lengths, $2^9$ and $2^5$ is $480$

and $480 - 64 = 416$

so $|f(z)| \geq 416 $ for $|z| = 2$ so $|f(z)| > |h(z)|$ on $|z| = 2$

so we may use Rouche's Theorem: $f(z)$ has the same number of zeros as $f(z)+h(z)$ 

the number of zeros $z^9 + z^5 - 8z^3$ has in $D$:

$z^3(z^6 + z^2 -8)$

so $0$ is a root of multiplicity $3$, and we have $6$ remaining to find:

$|z^6 + z^2 - 8|$ when $|z| \geq 2$:

$|z^6 + z^2 - 8| \geq |z^6 + z^2| - 8$, and $|z^6 + z^2|$ is at least $2^6 - 2^2 = 60$ (if we consider adding two vectors, one of at least length $2^6$ and the other at least $4$, the shortest a resultant vector can get is if they are going the opposite direction, thus the length of this vector = absolute value subtracting one length from the other)

so we have $|z^6 + z^2 - 8| > 0$ when $|z| \geq 2$ , which means $z^6 + z^2 - 8 \neq 0$ when $|z| \geq 2$ 

so the roots must lie in the circle of radius $2$ 

and when $|z| \leq 1$:

if $z = re^{i\theta}$

$z^6 = r^6(\cos(6\theta) + i \sin(6\theta))$

$z^2 = r^2(\cos(2\theta) + i\sin(2\theta))$

$z^6 + z^2 - 8 = (r^6\cos(6\theta)+r^2\cos(2\theta)-8) + i (r^6\sin(6\theta) + r^2\sin (2\theta))$

The real part will be at least $-10$ and at most $-8$, which means we never obtain $0$ within the unit circle or on its boundary

so we must have $6$ roots lying in between the circle of radius 1 and the circle of radius 2

##### Chapter VIII, Sec. 2 ex. 8

Let $D$ be a bounded domain, and let $f(z)$ and $h(z)$ be meromorphic functions on $D$ that extend to be analytic on $\partial D$. Suppose that $|h(z)| < |f(z)|$ on $\partial D$. Show by example that $f(z)$ and $f(z) + h(z)$ can have different numbers of zeros on $D$. What can be said about $f(z)$ and $f(z)+h(z)$? Prove your assertion.

$f(z) = z$

$h(z) = \frac{1}{2z}$

$D$ is the region inside the unit circle

$f(z)$ has one zero in $D$ at $0$ 

$h(z)$ has an isolated singularity at $z = 0$ and is otherwise analytic on $\partial D$

on $\partial D$, $|z| = 1$

$|f(z)| = |z| = 1$

$|h(z)| = \frac{1}{2|z|} = \frac{1}{2} < |f(z)| = 1$ 

$f(z)+h(z) = z + \frac{1}{2z}$ for $|z| < 1$ has 2 zeros:

$z + \frac{1}{2z} = 0 \equiv z^2 + \frac{1}{2} = 0$

$z = \sqrt{-1/2} = \pm i/\sqrt{2}$, which are both in the unit circle

We still have that the increase in argument for $f(z)$ is the same as for $f(z) +h(z)$

so $\int d \arg (f(z)) = \int d\arg(f(z)+h(z))$

and these are each equal to $2\pi(N_0 - N_\infin)$ (for respective $N_0$, $N_{\infin}$)

so while they may not have the same number of zeros, they have the same value for $N_0 - N_{\infin}$ :

$f(z$): $N_0 = 1$, $N_{\infin} = 0$

$f(z)+h(z): N_0 = 2, N_{\infin} = 1$

##### Chapter VIII, Sec. 3 ex. 2

Let $S$ be the family of univalent functions $f(z)$ defined on the open unit disk {$|z| <1$} that satisfy $f(0)= 0$ and $f'(0)=1$. Show that $S$ is closed under normal convergence, that is, if a sequence in $S$ converges normally to $f(z)$, then $f \in S$.

Remark: It is also true, but more difficult to prove, that $S$ is a compact family of analytic functions, that is, every sequence in $S$ has a normally convergent subsequence.

Univalent: analytic and one-to-one on a domain $D$ (in this case the open unit disk)

let {$f_k(z)$} be a sequence of univalent functions on the open disk.

We know that the sequence converges normally to a function $f(z)$ that is either univalent or constant

for each $f_k(z)$, $f_k(0) = 0$, $f_k'(0)= 1$ 

for any $k$, $f_k(z)$ has at least one zero at $0$ and we must have that the zeros of the functions in the  sequence converge to the zeros of the limit function, 

so $f(z)$ must have at least one zero at $0$ 

---

also, by the theorem on page 137, 

the sequence of first derivatives {$f_k'(z)$} also converges normally to $f'(z)$

if we were to take $f_k'(z)-1$ as a new sequence

since converging normally means to converge uniformly on any closed disk in $D$:

if {${f_k}(z)$}, {$g_k(z)$} each converge uniformly to $f(z), g(z)$ respectively

$\implies$ $|f_j(x)-f(x)| \leq \epsilon_j$ for all $x \in D$ , $|g_j(x)-g(x)| \leq \delta_j$

with $\epsilon_j, \delta_j \rightarrow 0$ as $j \rightarrow \infin$ 

and so we have $\epsilon_j + \delta_j \rightarrow 0$ 

taking $|f_j(x)+g_j(x)-(f(x)+g(x))| = |f_j(x)-f(x)+g_j(x)-g(x)| \leq \epsilon_j + \delta_j$ by triangle inequality, so $f_k +g_k \rightarrow f+g$ 

therefore:${f_k'(z)-1}$ would converge normally to $f'(z)-1$

and since these functions have a zero at $0$, by the same logic as above

since $f_k'(0)-1 = 0$ for all $k$ and the zeros of $f'_k-1$ converge to the zeros of $f'-1$

$0$ is a zero for $f'(z)-1$ $\implies$ $f'(0) = 1$ 

##### Chapter VIII, Sec 4, ex. 4

Let $f(z)$ be an analytic function on the open unit disk $D =$ {$|z| <1$}. Suppose there is an annulus $U =$ {$r < |z| < 1$} such that the restriction of $f(z)$ to $U$ is one-to-one. Show that $f(z)$ is one-to-one on $D​$ 

for each $w_0$ in $f(U)$, there is exactly one $z_0 \in U$ such that $f(z_0) = w_0$ 

in some open disk with radius $\rho$ around each $z_0$ $\in U$, the values of $f(z)$ on this disk include the disk centered at $w_0$ of some radius $\delta$ so that $N(w) = N(w_0)$ for $|w - w_0| < \delta$

let $N(w_0) = m$, and since $f$ is 1-1 on $U$:

on $U$: $f(z) -w_0= (z-z_0)^mg(z)$ for some function $g(z)$ that is analytic at $z_0$ and $g(z_0) \neq 0$

 