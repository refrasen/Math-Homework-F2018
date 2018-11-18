Renee Senining

Math 185

# Homework #2

#### Chapter 1, Sec. 3

##### Ex. 1 Sketch the image under the spherical projection of the following sets on the sphere:

###### (a) the lower Hemisphere $Z<0$

$x = X/(1-Z)$, $y = Y/(1-Z)$ 

We have that $1 - Z > 1$, since $Z < 0$ 

so $|x| < |X|$ and $|y| < |Y|$ 

and also because $Z \neq 0$, $X^2 + Y^2 < 1$ 

meaning, $x^2 + y^2 < X^2 +Y^2 <1$ 

![1535774343280](C:\Users\Renee\AppData\Local\Temp\1535774343280.png)

###### (b) the polar cap $\frac{3}{4}\leq Z\leq1$ 

When $Z = \frac{3}{4}$, $1-Z = \frac{1}{4}$, so we have: $x = 4X$ and $y = 4Y$ 

And $1 - Z^2 = 1 - \frac{9}{16} = \frac{7}{16} $ 

so: $x^2+y^2 = 16(X^2+Y^2) = 16\times\frac{7}{16} = 7$ 

The image will be the grey section.

![1535776307952](C:\Users\Renee\AppData\Local\Temp\1535776307952.png)

and as $Z$ goes towards 1, the radii of the circles on the plane centered at 0 tend towards $\infin$, so we have that $x^2+y^2 \geq 7$ when $Z \in [\frac{3}{4},1]$  

###### (c) lines of latitude $X = \sqrt{1 - Z^2}\cos \theta$ , $Y = \sqrt{1-Z^2}\sin\theta$, for $Z$ fixed and $0 \leq \theta \leq 2\pi$

so this will correspond to a circle on the plane centered at 0.

the radius will be $= \frac{\sqrt{1-Z^2}}{1-Z}$, since $x = \frac{X}{1-Z} = (\frac{\sqrt{1-Z^2}}{1-Z})\cos\theta = r\cos\theta$ 

So for each Z:

![1535777511530](C:\Users\Renee\AppData\Local\Temp\1535777511530.png)

###### (d) lines of longitude $X = \sqrt{1-Z^2}\cos\theta$, $Y = \sqrt{1-Z^2}\sin\theta$, for $\theta$ fixed and $-1 \leq Z \leq 1$ 

These will correspond to lines on the plane that pass through origin

and slope $m = y/x = \tan\theta$, $x = \frac{\sqrt{1-Z^2}}{1-Z}\cos\theta, y= \frac{\sqrt{1-Z^2}}{1-Z}\sin\theta$. 

For a fixed $\theta$, when $x$ is nonzero, $x$ has the same sign as $\cos\theta$, because $\sqrt{1-Z^2} \geq 0$ and $1-Z \geq 0$, and similarly for $y$ and $\sin\theta$ 

when $Z = -1, 1$, $x = y = 0$ , regardless of the value of $\theta$, so the origin is always included in the image. 

as $Z \rightarrow 1$, $x$ and $y$ approach either positive or negative infinity depending on $\theta$. 

![1535779605441](C:\Users\Renee\AppData\Local\Temp\1535779605441.png)

###### (e) the spherical cap $A \leq X \leq 1$, with center lying on the equator for fixed A. Separate into cases, according to various ranges of A.    

$A = 1$: We only have the point $(1, 0, 0)$, which means $x = 1$, $y = 0$ 

$A = 0$: We have the entire right half-plane. $X \geq 0 \implies x \geq 0$ 

$A = -1$: We get the whole sphere as the domain, which means the whole plane.

$A \in (0, 1)$: 

$-\sqrt{1-A^2}\leq Y, Z\leq \sqrt{1-A^2}$, 

Setting $Y = 0$: 

$\frac{A}{1+\sqrt{1-A^2}} \leq x \leq \frac{A}{1-\sqrt{1-A^2}}$, as $Z$ goes from $-\sqrt{1-A^2}$ to $\sqrt{1-A^2}$

In the plane $X= A$, the intersection with the unit sphere is the circle in the plane centered at $(0,0)$ with radius $\sqrt{1-A^2}$ 

this gives us the circle: $(x-\frac{1}{A})^2-y^2= \frac{1}{A^2} - 1 = \frac{1-A^2}{A^2}$

It is centered at $(\frac{1}{A}, 0)$ with radius $\frac{\sqrt{1-A^2}}{A}$ . 

and if we continue to look at circles that come from the intersection of the sphere with the planes of the form $X = D$, with $D \in (A, 1)$. As $D$ increases, we get circles that are contained within the one before, each with center $(1/D, 0)$ and radius $\frac{\sqrt{1-D^2}}{D}$. Our image is therefore the section within the circle centered at $(1/A, 0)$ with radius $\frac{\sqrt{1-A^2}}{A}$

![1535786301086](C:\Users\Renee\AppData\Local\Temp\1535786301086.png)

When $A \in (-1,0)$, If we looked at the spherical cap $-1 \leq X \leq A$, we'd get a similar situation as the one before. Since we're looking at the projection from the rest of the sphere, we'd get the image being the exterior of the circle. 

![1535786842119](C:\Users\Renee\AppData\Local\Temp\1535786842119.png)

##### Ex. 6 We define the chordal distance $d(z,w)$ between two points $z, w \in \C^*$ to be the length of the straight line segment joining the points $P$ and $Q$ on the unit sphere whose stereographic projections are $z$ and $w$ respectively.

###### (a) Show that the chordal distance is a metric, that is, it is symmetric, $d(z,w) = d(w,z)$; it satisfies the triangle inequality $d(z,w) \leq d(z, \zeta) + d(\zeta, w)$, and $d(z,w) = 0$ if and only if $z=w$ 

let $P = (X_1, Y_1, Z_1)$ and $Q = (X_2, Y_2, Z_2)$, and let $z = x_1 +iy_1$ and $w = x_2 + iy_2$

then we have the length of the line segment $\overline{PQ}$ $= \sqrt{(X_2-X_1)^2+(Y_2-Y_1)^2+(Z_2-Z_1)^2} = \sqrt{(X_1-X_2)^2+(Y_1-Y_2)^2+(Z_1-Z_2)^2}$ $=$ the length of $\overline{QP}$ so $d(z,w) = d(w,z)$ 

For the Triangle Inequality: the length of the segment is the distance between the two points, where the distance is the usual metric on $\R^3$,  and by the definition of a metric, the triangle inequality is satisfied. Also, if we let $R$ be a point on the unit sphere with the stereographic projection $\zeta$, we could find the angles between $\overline{PQ}, \overline{QR},$ and $\overline{RP}$ by identifying the vectors, say $u_1$ from $P$ to $Q$, $u_2$ from $Q$ to $R$, and $u_3$ from $P$ to $R$, using these vectors to find the cosine of the angle $\theta_1$ between $u_1$ and $u_3$, and $\theta_2 $ between $-u_1$  and $u_2$, and use:

$||u _1|| = ||u_3||\cos\theta_1 + ||u_2||\cos\theta_2 $ since these angles are going to be less than $\pi$, $\cos\theta_1, \cos\theta_2 \in (0,1)$

$d(z,w) = ||u_1|| \leq||u_3|| + ||u_2|| = d(z, \zeta) + d(\zeta, w)$ 

For $d(z,w)$ = 0, we'd need $X_1 - X_2 = 0, Y_1 - Y_2 = 0, Z_1 - Z_2 = 0$, which means

$P = (X_1, Y_1, Z_1) = (X_2, Y_2, Z_2) = Q$, which means they have the same stereographic projection $z = w$

###### (b) Show that the chordal distance from $z$ to $w$ is given by $d(z,w)  = \frac{2|z-w|}{\sqrt{1+|z|^2}\sqrt{1+|w|^2}}, \; z,w \in \C$ 

We rewrite $d(z,w)$ in terms of $x_1, y_1, x_2, y_2$ and $|z|, |w|$ 

$\sqrt{(\frac{2x_1}{|z|^2+1}-\frac{2x_2}{|w|^2+1})^2+(\frac{2y_1}{|z|^2+1}-\frac{2y_2}{|w|^2+1})^2 + (\frac{|z|^2-1}{|z|^2+1}-\frac{|w|^2-1}{|w|^2+1})^2}$

$(\frac{|z|^2-1}{|z|^2+1}-\frac{|w|^2-1}{|w|^2+1})^2 = \frac{(|z|^2-1)^2}{(|z|^2+1)^2}-2\frac{(|w|^2-1)(|z|^2-1)}{(|z|^2+1)(|w|^2+1)} +\frac{(|w|^2-1)^2}{(|w|^2+1)^2}$ 

$(\frac{2x_1}{|z|^2+1}-\frac{2x_2}{|w|^2+1})^2 =4(\frac{x_1^2}{(|z|^2+1)^2}-2\frac{x_1x_2}{(|z|^2+1)(|w|^2+1)}+\frac{x_2^2}{(|w|^2+1)^2}) $ 

For the part containing $y_1, y_2$ can replace the $x_i$'s' with the corresponding $y_i$'s  

And using $|z|^2 = x_1^2+y_1^2$ , when combining terms with denominator $(|z|^2+1)^2$

When we combine$ (|z|^2-1)^2+4|z|^2 = |z|^4-2|z|^2+1+4|z|^2 = (|z|^2+1)^2 $ (and similarly for $|w| = x_2^2 +y_2^2$ 

Under the radical we now have:

$2(\frac{-4x_1x_2-4y_1y_2 -(|w|^2-1)(|z|^2-1)+(|w|^2+1)(|z|^2+1)}{(|z|^2+1)(|w|^2+1)})$  $= 2\frac{-4x_1x_2-4y_1y_2 +2|w|^2+2|z|^2 }{(|z|^2+1)(|w|^2+1)} = 2\frac{2(x_1-x_2)^2+2(y_1-y_2)^2}{(|z|^2+1)(|w|^2+1)}$

squaring this we get: $2\frac{\sqrt{(x_1-x_2)-(y_1-y_2)}}{\sqrt{1+|z|^2}\sqrt{1+|w|^2}}$ and the numerator is, by definition, $|z-w|$

###### (c) What is $d(z, \infin)$? 

as $w \rightarrow \infin$, 

$d(z,w) = \frac{2|z-w|}{\sqrt{1+|z|^2}\sqrt{1+|w|^2}} = \frac{2|z/w - 1||w|}{\sqrt{1+|z|^2}(\sqrt{1/|w|^2 + 1})|w|} = \frac{2|z/w-1|}{\sqrt{1+|z|^2}\sqrt{1/|w|^2+1}} \rightarrow \frac{2|-1|}{\sqrt{1+|z|^2}} = \frac{2}{\sqrt{1+|z|^2}}$ 

 

#### Chapter 1, Sec. 5

##### Ex. 4 Show that the only periods of $e^z$ are the integral multiples of $2\pi i$, that is, if $e^{z+\lambda} = e^z$ for all $z$, then \lambda is an integer times $2\pi i$ 

Let $e^{z+\lambda} = e^z$

$e^{z+\lambda} = e^{z}e^\lambda = e^z$ (because of the addition formula property)

multiplying by $e^{-z}$ : $e^\lambda = 1$ = $\cos(2\pi k) + i\sin(2\pi k) = e^{i2\pi k }$, where $k$ is an integer. 

multiplying by $e^{-i2\pi k}$ we have $e^{\lambda}e^{-i2\pi k} = 1$,

$e^{\lambda-i2\pi k } = e^0 $

$\lambda - i2\pi k = 0 \equiv \lambda = i2\pi k$

#### Chapter 1, Sec. 6

##### Ex. 1 Find and plot $\log z$ for the following complex numbers $z$. Specify the principal value. 

###### (a) 2, principal value =  $\log|2|$

$x = \log|2|$, $y = 0$ 

###### (b) $i$, principal value $= 0 + i\pi/2$

|$i$| = 1

$x = 0, y = \pi/2$

###### (c) $1+i$, principal value $= \log(\sqrt{2}) + i\pi/4  = (1/2)\log(2) +i\pi/4$

$x = \log{\sqrt{2}}, y = \pi/4 $

###### (d) $(1+i\sqrt{3})/2$, principal value $= \log(\sqrt{1/4+3/4 } = 1) + i\pi/3$ 

$x = 0$, $y = \pi/3$ 

![1535801933211](C:\Users\Renee\AppData\Local\Temp\1535802392124.png)

##### Ex. 4 How would you make a branch cut to define a single-value branch of function $\log(z+i-1)$? How about $\log(z-z_0)$ 

Each branch of $f_m(z) = Log(z+i-1) +2\pi im$ 

We want to make a slit in the $z$-plane where $z + i - 1 \in (-\infin, 0]$, and this will allow us to define a single-value branch of the function similar to the way we define one for $\log(z)$ 

so any $z = x -i$, where $x \in (-\infin, 1]$ 

So:  ![1535805213683](C:\Users\Renee\AppData\Local\Temp\1535805213683.png)

Where the red line is the slit in the complex plane. 

Basically, started at the point $(1, -1)$ and drew a horizontal line towards $-\infin$ from there.

It's like treating $(1, -1)$ as a new origin and moving the axes over to the right by 1 and down by 1. 

For example: For any point on the red line, $(x, -1)$the function maps this point to $(\log(\sqrt{(x-1)^2}, \pi)$  

In general, for any $z_0$, we start at $z_0$ and draw a horizontal line towards $-\infin$ 

#### Chapter 2, Sec. 1

##### Ex. 10 At what points are the following functions continuous? Justify your answer.

###### (a) $z$

Let $$z_0  \in \C$$ and let $\epsilon > 0$

Let $\delta = \epsilon$ 

then for any $z$ s.t. $|z-z_0|<\delta \implies |f(z) -f(z_0)| = |z-z_0| <\epsilon$

so as $z$ approaches $z_0$, $f(z)$ approaches $f(z_0)$, and since $z_0$ was an arbitrary point in $\C$, $z$ is continuous at any point in $\C$ 

###### (b) $z/|z|$

from (a), $z$ is continuous everywhere. $|z|$ is a function that maps $\C$ to $\R$ 

From triangle inequality: $|(z-z_0 )+ (z_0)| = |z| \leq |z-z_0|  + |z_0| \implies |z| - |z_0| \leq |z-z_0|$ 

so let $z_0 \in \C$ and let $\delta = \epsilon$, then: 

for any $z$ in $\C$ s.t. $|z-z_0| < \delta \implies | |z| - |z_0| | < \delta = \epsilon$

so $|z|$ is continuous everywhere. 

However, $z/|z|$ must have $|z| \neq 0$ for this to be continuous, and $|z| = 0$ when $z = 0$ 

so continuous everywhere except $z= 0$  

###### (c) $z^2/|z|$

From page 37, and (a), $z^2$ is continuous on every point in $\C$ 

From (b), we have that $1/|z|$ is not continuous at $z = 0$ 

so continuous everywhere except at 0.

If we were to define this function to be $0$ at $z =0$, then it would be continuous since the limit as $z$ approaches 0 is 0:

for any $\epsilon>0$, we have that if $|z| < \epsilon$

Using the fact that for any 2 complex numbers, $|zw| = |z||w|$

then $|f(z) - 0| = |\frac{z^2}{|z|}|= \frac{|z|^2}{|z|} = |z| <\epsilon$  

###### (d) $z^2/|z|^3$ 

Continuous everywhere except at 0.

There is no limit as $z \rightarrow 0$, since $|z^2/|z|^3| = |z|^2/|z|^3= 1/|z| \rightarrow \infin$ 

##### Ex. 15 Which of the following sets are open subsets of $\C$? Which are closed? Sketch the sets.

###### (a) The punctured plane $\C\setminus${$0$} 

Let $z = x +iy$ be a point in $\C$, $(x,y)$ 

Let $\rho = |z|$  $>0$, since $z \neq 0$ 

let $w$ be a point in the open disk centered at $z$ with radius $p$ 

then $|w-z| <\rho$

by triangle inequality: $|z| \leq |z-w| + |w| \equiv |w| \geq |z| - |z-w| > 0$, since $|z-w| = |w-z| < \rho$

so $w \neq 0$,  and since $w$ was arbitrary, the disk is contained in the punctured plane.   

It is open.

![1535824065080](C:\Users\Renee\AppData\Local\Temp\1535824065080.png)

###### (b) the exterior of the open unit disk in the plane, {$|z| \geq 1$}

Not open, and also:

Closed, because the complement of the set is open.

![1535824180770](C:\Users\Renee\AppData\Local\Temp\1535824180770.png)

###### (c) the exterior of the closed unit disk in the plane, {$|z| > 1$}

Open, you can take any point $z$ and the open disk centered around it with radius $|z|-1$ is contained in the set.  Also it is the complement of a closed set.

![1535824240175](C:\Users\Renee\AppData\Local\Temp\1535824240175.png)

###### (d) the plane with the open unit interval removed, $\C\setminus (0,1)$

Not Open, if you take $z = 0$ or $z= 1$, then any open disk with radius > 0  will contain points in the open unit interval, such as $(0, .9999999....)$.  (if the radius is $\geq1$, then all of the open unit interval will be contained in the disk, if the $\rho = $ radius is < 1, then the point $(0, 1-\rho/2) $ is a point in the interval and in the disk.

Not closed: $(0,1)$ is not an open subset: let $z = (x,0)$ be in $(0,1)$. Any disk centered at the point with radius $\rho$ will contain the point $(x, \rho/2)$, which is not in the open unit interval

![1535824410462](C:\Users\Renee\AppData\Local\Temp\1535824410462.png)

###### (e) the plane with the closed unit interval removed, $\C\setminus[0,1]$ 

open: let $z$ $\notin [0,1]$. there exists a point $w$ $\in [0,1]$  such that for all $w' \in [0,1]$

$|z-w'| > |z-w|$ . In other words, $w$ is the closets point to $z$ 

We define the radius for the open disk to be $< |z-w|$, which is possible since $|z-w| > 0$, and there are infinitely many real numbers between any two real numbers, in this case: (0, $|z-w|$) .

So, for every point in the set there is an open disk centered around it that is contained in the set. 

![1535824539775](C:\Users\Renee\AppData\Local\Temp\1535824539775.png)

###### (f) the semidisk {$|z| <1, Im(z) \geq0$}

not closed: the complement of this set contains the points on the boundary of the disk, such as $(0, 1)$. And any open disk centered around $(0,1)$ with radius $\rho <1$ will contain $(0, 1- \rho/2) $in the semidisk, so the complement is not open, meaning this set is not closed.

not open:Let $z$ be in the semidisk with $x \in (-1,1), y = 0$ . Any open disk centered on $z$ with radius $\rho$ will contain the point $(x,  -\rho/2)$, which is not in the semidisk, since $Im(z) = -\rho/2 < 0$, so there exists points where no open disk centered on them will be contained in the set. 

![1535825039822](C:\Users\Renee\AppData\Local\Temp\1535825039822.png)

###### (g) the complex plane $\C$

Both open and closed.

Any disk centered on any point in $\C$ is in $\C$, so open. 

The empty set is considered open, so $\C$ is closed.

Also, there are no points in the empty set, so it does satisfy

whenever a point is in the set, there exists an open disk such that the disk is contained in the set. 

![1535825171929](C:\Users\Renee\AppData\Local\Temp\1535825171929.png)

##### Ex. 19 Give a proof of the fundamental theorem of algebra along the following lines. Show that if $p(z)$ is a nonconstant polynomial, then $|p(z)|$ attains its minimum at some point $z_0 \in \C$ Assume that the minimum is attained at $z_0 = 0$, and that $p(z) = 1 + az^m + . . .,  $ where $m \geq 1$ and $a \neq 0$. Contradict the minimality by showing that $|P(\epsilon e^{i\theta_0})| < 1$ for an appropriate choice of $\theta_0$ 

Let $p(z) = a_nz^n + . . . + a_1z +a_0$, $a_n \neq 0$ and $n \geq 1$ 

If we were to take the limit of $|p(z)|/|z|^n$ as $|z| \rightarrow \infin$

We would get $\frac{|z^n||(a_0/z^n + a_1/z^{n-1} + ...+a_n)|}{|z|^n}$ and since $|z^n| = |z|^n$ we have

$|(a_0/z^n+a_1/z^{n-1}+...+a_n)| \rightarrow |a_n|$ as $z \rightarrow \infin$

So for any $\delta > 0$ 

so $\exist N > 0$ such that for $|z| > N$, $|p(z)|/|z|^n \in(|a_n|-\delta ,|a_n|+\delta)$

Restricting $\delta < |a|$ , so $|a| - \delta >0$ , we have for all $|z| > N$ 

$|p(z)|/|z|^n > |a_n| - \delta \equiv |p(z)|>(|a_n|-\delta)(|z|^n) >0$

So we know that a minimum for $|p(z)|$ is obtained when $|z| \leq R$, and this minimum is at most $(|a_n|-\delta)(|z|^n)$

Now looking at $p(z) = 1 + az^m + ...$ higher order terms, 

Assuming $z_0 = 0$ is when $|p(z)|$ has its minimum, $|p(0) = 1| = 1$ 

let $|a|e^{i\phi}$ be the polar representation of $a \neq 0$ 

Then $a\epsilon^me^{i\phi}= |a|e^{i\phi}\epsilon^me^{im\theta_0} = |a|\epsilon^me^{i(\phi+m\theta_0)}$ 

if we choose $\theta_0$ such that $\phi + m\theta_0 = \pi$, then $e^{i(\phi+m\theta_0)} = -1$ 

so we get

$p(z) = 1 -|a|\epsilon^m + C_1\epsilon^{m+1}e^{i(m+1)\theta_0}+... $ and if we choose $\epsilon$ to be sufficiently small, we'll have $|p(z)| =|1 - |a|\epsilon^m +C_1\epsilon^{m+1}e^{i(m+1\theta_0)} + ...|<1$

this is because no matter how large the coefficient, $C_i$,  for any number $n >0$ there always exists an $\epsilon > 0$ s.t. $|C_i|\epsilon <n$ .

We could for example have a condition on $\epsilon$ to make $|1 - |a|\epsilon^m|$ $< 1/2$ 

and  $|C_1\epsilon^{m+1}e^{i(m+1\theta_0)} + ...| <1/2$

so that by triangle inequality:

$|p(z)| = |1 - |a|\epsilon^m + C_1\epsilon^{m+1}e^{i(m+1\theta_0)} + ...| < 1/2 + 1/2 = 1$





 