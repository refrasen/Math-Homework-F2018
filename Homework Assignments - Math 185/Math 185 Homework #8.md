Renee Senining

Math 185

### Homework #8

#### **Chapter V**, Sec. 1, ex. 7;  Sec. 2, ex. 3, 8, 9;  Sec. 3, ex. 1b, 1e, 1i

##### Chapter V, Sec. 1, Ex. 7:

Suppose $\sum a_k$ converges

This means the sequence of partial sums, {$S_k$} converges

and that $a_k \rightarrow 0$ as $k \rightarrow \infin$ 

The sequence of partial sums is a sequence of complex numbers

and convergent sequence of complex numbers are Cauchy Sequences

so, as $m, n \rightarrow \infin$, $|S_n - S_m| \rightarrow 0$

$|S_n - S_m| = |a_0 + . . . + a_n - (a_0 + . . . + a_m)| = |a_{m+1} + . . . + a_n| $

and so for any $\epsilon > 0$, $\exists$ $N_1 \geq 1$ s.t. if $m, n \geq N_1$, $|S_n - S_m| < \epsilon/2$ 

and also, $\exists N_2 \geq 1$ s.t. if $m \geq N_2$, $|a_m| < \epsilon /2$ 

so taking $N = \max(N_1, N_2)$ , if $m, n \geq N$, 

$|S_n - S_m + a_m| = |a_m + . . .  + a_n| \leq |a_m| + |a_{m+1}+ . . . + a_n| < \epsilon/2 + \epsilon /2 = \epsilon$ 

this means that $a_m + . . . + a_n \rightarrow 0$ $\equiv$ $\sum_{k = m}^{k =n}a_k $ converges to 0 as $m,n  \rightarrow \infin$ 

Now suppose $\sum_{k=m}^{k=n}a_k \rightarrow 0$  as $m, n \rightarrow \infin$ 

this means $a_{m} + . . . + a_n \rightarrow 0$ as $m,n \rightarrow \infin$ 

so for any $\epsilon > 0$, $\exists N \geq 1$ s.t. $|a_m + . . . + a_n| < \epsilon$ for all $m, n \geq N$ 

and $|a_{m+1} + . . . + a_n| \leq |a_m + a_{m+1} + . . . + a_n| < \epsilon$ for all $m,n \geq N$

$\implies$ $|S_n - S_m| < \epsilon$ for all $m,n \geq N$ ($\epsilon$ was arbitrary)

so {$S_k$} is a cauchy sequence $\implies$ it is a convergent sequence

which means $\sum a_k$ converges

##### Chapter V, Sec. 2, Ex. 3

1. $\frac{z^k}{k}$ converges uniformly for $|z| < 1$, $E = ${$z: |z| < 1$}
   1. I will show {$f_k$} converges to $0$ uniformly as $k \rightarrow \infin$ 
   2. $|z^j| = |z|^j$ and $|z| < 1$, so $|z|^j < 1^j = 1$ for all $j \in \N $ 
   3. so for all $z \in E$, $j \in \N$:
   4. $|f_j(z)| = |\frac{z^j}{j}| < \frac{1}{j}$ and as $j \rightarrow \infin$, $\frac{1}{j} \rightarrow 0$, 
   5. which means $|f_j(z) - 0| \leq \frac{1}{j}$, and $\frac{1}{j} \rightarrow 0$, for all $z \in E$ 
   6. so {$f_k$} converges to $0$ uniformly.
2. $f'_k(z)$ doesn't converge uniformly for $|z| < 1$ 
   1. Suppose $f_k'(z)$ does converge uniformly to $g(z)$for $|z| < 1$ 
   2. so let $z$ be any point in $E$ . $f_k(z)$ is analytic everywhere assuming, $k \geq 1$, so $f'_k(z)$ is analytic by the corollary on page 115 ($E$ is a domain) and $E$ is a star-shaped domain so:
   3. $f_k(z) = \int_{0}^z f'_k(\zeta)d\zeta$ , where the integral can be taken over any path from $0$ to $z$
      1. since $z^k/k - 0^k/k = \int_0^{z}\zeta^{k-1}d\zeta$
   4. let $\gamma$ be a broken line segment contained in $E$ (which is possible since $E$ is a domain and star-shaped with respect to $0$) that goes from $0$ to $z$, $z \in E$ 
   5. and since $f_k'$ is analytic on $E$, it is continuous over $E$
   6. and $\gamma \in E$, so $f_k'$ is continuous on $\gamma$ 
   7. and assuming {$f_k'$} converges uniformly to $g(z)$ on $E$ (and therefore $\gamma$)
   8. $\int_{\gamma} f'_k(z)dz = \int_{0}^zf_k'(\zeta)d\zeta = f_k(z) \rightarrow \int_{\gamma}g(z)dz$
   9. and since {$f_k'$} is a sequence of analytic functions, $g$ is analytic (on $E$)
   10. and $\int_{\gamma}g(z)dz = \int_0^zg(\zeta)d\zeta = G(z) - G(0)$
       1. where $G$ is a primitive for $g$
   11. so {$f_k$} converges uniformly to $G(z) -G(0)$, but it also converges to $0$
   12. so $G(z) - G(0) = 0$ 
   13. which means $G(z) = G(0)$ for any $z \in E$, so $G(z)$ is constant over $E$ 
   14. which means $G'(z) = g(z) = 0$
   15. so ${f_k'} \rightarrow 0$ 
   16. but for every $j \geq 1$, $|f'_j| = |z^{j-1}| \leq 1 = \epsilon_j$, so $\epsilon_j$ does not converge to $0$ as $j \rightarrow \infin$, which is a contradiction: $f'_k$ does not converge uniformly for $|z| < 1$
3. However, using the theorem on page 136
   1. since $f_k(z)$ is analytic for $|z| \leq R$ for each $R < 1$ and converges uniformly to 0 for $|z| \leq R$
   2. For each $r < R<1$, {$f_k'(z$)} converges uniformly to $0$ for $|z| \leq r$
      1. for any $\epsilon > 0$, taking $R = 1 - \epsilon/2$, we have that the above is true for $r = 1 - \epsilon$ 

##### Chapter V, Sec. 2, Ex. 8:

Show that $\sum \frac{z^k}{k^2}$ converges uniformly for $|z| < 1$ 

define $g_k(z) = \frac{z^k}{k^2}$ 

Let $M_k = \frac{1}{k^2} \geq 0$

for all $z$ such that $|z| < 1$, 

$|g_k(z)| \leq |\frac{z^k}{k^2}| = \frac{|z|^k}{k^2} <\frac{1}{k^2} = M_k$

so $\sum g_k(z)$ converges uniformly for $|z| < 1$

##### Chapter V, Sec. 2, Ex. 9:

Show that $\sum \frac{z^k}{k}$ does not converge uniformly for $|z| < 1$ $\sum_{k=1}^\infin \frac{1}{k} $ diverges

and the terms $\frac{z^k}{k} \rightarrow \frac{1}{k}$ as $z \rightarrow 1$ from the left side (and in this case, $z$ is increasing towards 1 along the positive real axis)

so letting $z \rightarrow 1$ as above, $\sum \frac{z^k}{k} \rightarrow \sum \frac{1}{k} \rightarrow \infin$ 

##### Chapter V, Sec. 3, Ex 1b. 

$\sum_{k=0}^\infin \frac{k}{6^k}z^k$ 

define $w = \frac{z}{6}$ 

so $w^k = \frac{z^k}{6^k}$ 

$\sum_{k=0}^\infin kw^k$ 

from the example on page 142, 

the ratio test gives the radius of convergence $R = 1$ for $\sum_{k=0}^\infin kw^k$

so $|w| = |\frac{z}{6}|< 1$ $\equiv$ $|z| < 6$ 

so $R = 6$ 

##### Chapter V, Sec. 3, Ex 1e

$\sum_{k=1}^\infin \frac{2^kz^{2k}}{k^2+k}$

$w = 2z^2$ 

$\sum_{k=1}^\infin \frac{w^k}{k^2+k}$

so $a_k = \frac{1}{k^2+k}$ 

$|a_k/a_{k+1}| = \frac{(k+1)^2 + k+1}{k^2+k} = \frac{k^2 + 2k + 1 + k+1}{k^2+k} = \frac{k^2+3k + 2}{k^2+k} = \frac{1 + 3/k + 2/k^2}{1 + 1/k} \rightarrow 1$ as $k \rightarrow \infin$ 

so $|2z^2|<1  \equiv |z| < 1/\sqrt{2} $, so $R = \frac{1}{\sqrt{2}}$ 

##### Chapter V, Sec. 3, Ex 1i

$\sum_{k=1}^\infin\frac{k!z^k}{k^k}$ 

using ratio test:

$|a_k/a_{k+1}| = \frac{k!/k^k}{(k+1)!/(k+1)^{k+1}} = \frac{k!(k+1)^{k+1}}{(k+1)k!k^k}$

$R = \lim_{k\rightarrow \infin} \frac{(k+1)^k}{k^k} = e$ 

#### Extra Problems: https://math.berkeley.edu/~art/data/F18-185/HW8.pdf

##### 1. Give an example of a power series (centered at $z_0 = 0$) with radius of convergence $R = 1$ which converges at $z = i$ and diverges at $z = -i$. Justify your answer

$\sum a_k z^k$ 

where $\sum a_k (i)^k$ converges but $\sum a_k (-i)^k$ diverges

so consider the series $\sum_{k =1}^\infin \frac{i^k}{k}z^k$

at $z = i$, we obtain $\sum_{k=1}^\infin \frac{(-1)^k}{k}$, which converges (conditionally)

at $z = -i$, we obtain $\sum_{k=1}^\infin \frac{1}{k}$, which diverges.

##### 2. 

##### $f'(z) = \sum_{k=1}^\infin ka_k z^{k-1}$

$f''(z) = \sum_{k=2}^\infin k(k-1)a_{k}z^{k-2}$

taking the differential equation:

$z^2f''(z) + zf'(z) + (z^2 -1)f(z) = 0$

and substituting each $f^{(m)}(z)$ with the corresponding series:

$\sum_{k=2}^\infin k(k-1)a_kz^k + \sum_{k=1}^{\infin}ka_kz^k + \sum_{k=0}^\infin a_kz^{k+2} - \sum_{k=0}^\infin a_k z^k = 0$ 

Letting $\sum_{k=2}^\infin k(k-1)a_k z^k = \sum_{k=0}^\infin (k+2)(k+1)a_{k+2}z^{k+2}$ 

$\sum_{k=1}^\infin ka_k z^k = \sum_{k=0}^\infin (k+1)a_{k+1}z^{k+1}$ 

$\sum_{k=0}^\infin (k+2)(k+1)a_{k+2}z^{k+2} + \sum_{k=0}^\infin(k+1)a_{k+1}z^{k+1} + \sum_{k=0}^\infin a_{k}z^{k+2} - \sum_{k=0}^\infin a_k z^k = 0$

$-a_0 -a_1z + a_1z + \sum_{k=0}^\infin (k+2)(k+1)a_{k+2}z^{k+2} + \sum_{k=1}^\infin(k+1)a_{k+1}z^{k+1} + \sum_{k=0}^\infin a_k z^{k+2} - \sum_{k=2}^\infin a_kz^k = 0$

Letting:

$\sum_{k=1}^\infin (k+1)a_{k+1}z^{k+1} = \sum_{k=0}^\infin (k+2)a_{k+2}z^{k+2}$

$\sum_{k=2}^\infin a_k z^k = \sum_{k=0}^\infin a_{k+2}z^{k+2}$ 

then substituting and simplifying:

$\sum_{k=0}^\infin [(k+2)(k+1)a_{k+2} + (k+2)a_{k+2}+a_k - a_{k+2}]z^{k+2} = a_0$

$(k+2)(k+1)a_{k+2} + (k+2)a_{k+2} + a_k - a_{k+2} = (k+3)(k+1)a_{k+2}  +a_k$

so $\sum_{k=0}^\infin [(k+3)(k+1)a_{k+2} +a_k]z^{k+2} = a_0$

---

plugging in $z = 0$ to the differential equation:

$(0-1)f(0) = 0 \implies -f(0) = 0 \implies f(0) = 0 = a_0$

$(k+3)(k+1)a_{k+2} = -a_k$

$a_{k+2} = -\frac{a_k}{(k+3)(k+1)}$

$k = 1$: $a_{3} = -\frac{1/2}{4*2} = -\frac{1}{16}$

$k = 3:$ $a_5 = -\frac{a_3}{6*4} = \frac{-1}{24}*\frac{-1}{16} = \frac{1}{384}$  



