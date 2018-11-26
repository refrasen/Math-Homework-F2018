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

for $|z| = 1$:

$|h(z)| = |2z + 1| \leq 2|z| + 1 = 3$

$|f(z)| = |z^9 + z^5 - 8z^3| \geq |z^9 + z^5| - 8|z^3|$



##### Chapter VIII, Sec. 2 ex. 8

