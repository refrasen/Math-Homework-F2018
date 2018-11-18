Renee Senining

Math 123

### Homework #4

##### Ex. 1: Consider the one-parameter family of linear systems given by $X' = \begin{pmatrix} a & \sqrt{2} + (a/2) \\ \sqrt{2} - (a/2) & 0 \end{pmatrix}X$ 

###### (a) Sketch the path traced out by this family of linear systems in the trace-determinant plane as $a$ varies

Trace = $a$, Determinant = $-(2 - a^2/4) = a^2/4 - 2$ = T$^2/4 - 2$ 

so treating trace as $x$ and determinant as $y$:

![1536859574714](C:\Users\Renee\AppData\Local\Temp\1536859574714.png)

###### (b) Discuss any bifurcations that occur along this path and compute the corresponding values of $a$

since  $ D=T^2/4-2$  

  $D <T^2$ 

So the graph never crosses into complex eigenvalues.

and $T^2 - 4D = 8$ , so we never get real repeated eigenvalues

When $a^2 >8$, $a > \sqrt{8}$ or $a < -\sqrt{8}$ 

	if $a < -\sqrt{8}$ a sink

	If $a > \sqrt{8}$ a source

When $a^2 < 8$ 

	we have a saddle, since the determinant < 0, so $\sqrt{T^2 - 4D} > |T|$ 

	we have that $a + \sqrt{a^2 - 4D}$ is positive and $a - \sqrt{a^2-4D}$ is negative 

And when $a = -\sqrt{8}$ or $a = \sqrt{8}$ 

	$D = 8/4 -2 = 2-2 = 0$ 

##### Ex. 2: Sketch the analog of the trace-determinant plane for the two-parameter family of systems $X' = \begin{pmatrix} a & b \\ b & a \end{pmatrix}X$ in the $ab$- plane. That is, identify the regions in the $ab$-plane where this system has similar phase portraits.

$T = 2a$, $D = a^2 - b^2$ 

$T^2 - 4D = 4a^2-4a^2+4b^2 = 4b^2 \geq 0$ for any value of $a, b$ so we never have complex eigenvalues.

Our eigenvalues: $\lambda = a\pm |b|$

when $b = 0$, we have real repeated eigenvalues at $a$ (with two linearly independent eigenvectors)

	if $a > 0$ then all solutions go away from origin

	if $a <0$ then all solutions go towards origin

when $D< 0 \equiv b^2 > a^2 \equiv |b| > |a|$, we have a saddle:

	$a + |b| > a + |a| \geq 0$ and $a - |b| < a - |a| \leq 0$

	$a-|b| < 0 < a + |b|$ 

when $D>0 \equiv|b| < |a|$ we have either a source or a sink

if $a < 0$, then we have a sink ($T  < 0$)

	$| a - |b|\,| > |a + |b|\,| $

if $a > 0$ we have a source $(T > 0$)

	$|a + |b| | > |a - |b||$ 

![1536865563522](C:\Users\Renee\AppData\Local\Temp\1536865563522.png)

##### Ex. 3: Consider the harmonic oscillator equation (with m = 1) $x'' + bx' +kx = 0$ where $b \geq 0$ and $k>0$. Identify the regions in the relevant portion of the $bk$-plane where the corresponding system has similar phase portraits.

letting $y = x'$, we have $X' = \begin{pmatrix} 0 & 1 \\ -k & -b \end{pmatrix}X$ 

$T = -b$, $D = 0(-b) - (1)(-k) = 0 +k = k$ 

$T^2 - 4D = b^2 -4k$ 

Eigenvalues: $\lambda = \frac{-b \pm \sqrt{b^2-4k}}{2}$

Plotting $D = T^2/4$ (when we have real repeated eigenvalues) is the same as looking at $k = b^2/4$ 

so when $b^2-4k < 0$ or $k > b^2/4$  we have complex eigenvalues, and since $b \geq 0$, we must have spiral sinks or a center traveling clockwise

When $b^2 -4k > 0$ or $k < b^2/4$ we have real eigenvalues, and $b^2-4k > b^2$ since $k > 0$, 

so we must have a sink

![1536867820542](C:\Users\Renee\AppData\Local\Temp\1536867820542.png)

(the $x$-axis shouldn't be included, since $y = k> 0$) 

##### Ex. 4: Prove that $H(x,y) = (x, -y)$ provides a conjugacy between $X' = \begin{pmatrix} 1 & 1 \\ -1 & 1 \end{pmatrix}X$ and $Y' = \begin{pmatrix} 1 & -1 \\ 1 & 1 \end{pmatrix}Y$

So let $A = \begin{pmatrix} 1 & 1 \\ -1 & 1 \end{pmatrix}$ and let $B = \begin{pmatrix} 1 & -1 \\ 1 & 1 \end{pmatrix}$ 

$H(x,y)$ is a conjugacy if it is one-to-one, onto, and continuous whose inverse is also continuous

and $\phi^B(t, H(X_0)) = H(\phi^A(t, X_0))$ 

$H(x,y)$ is one-to-one:

	If $H(x_1, y_1) = H(x_2, y_2)$ $\implies$ $(x_1, -y_1) = (x_2, -y_2)$ 

	so $x_1 = x_2$ and $y_1 = y_2$, so $(x_1, y_1) = (x_2, y_2)$ 

$H(x,y)$ is onto:

	for any point $(x,y)$, $H(x, -y) = (x, -(-y)) = (x, y)$ 

	therefore, any point in the plane has a pre-image $(x, -y)$ 

To show $H(x,y)$ is continuous, we prove that for any point $(x_0, y_0)$: for all $\epsilon > 0$, $\exists \delta > 0$ such that whenever a point $(x,y)$ in the plane satisfies $|(x,y)- (x_0, y_0)| < \delta$ then $|H(x,y) -H(x_0, y_0)| < \epsilon$ 

For any point $(x_0, y_0)$ and any $\epsilon > 0$, take $\delta \leq \epsilon$ 

so whenever $\sqrt{(x-x_0)^2 - (y-y_0)^2} < \delta \leq \epsilon$, we have $\sqrt{(x-x_0)^2 + (-y - (-y_0))^2} = \sqrt{(x-x_0)^2 +(y_0-y)^2} = |(x,y) - (x_0, y_0)|< \epsilon$

so for any $\epsilon > 0$, we have shown there exists a $\delta$ such that the statement above is satisfied $\implies$ as $(x,y) \rightarrow (x_0, y_0)$, $H(x,y) \rightarrow H(x_0, y_0)$ 

So $H(x,y)$ is continuous.

The $H$ is its own inverse: $(H\circ H)(x,y) =  H(H(x,y)) = H(x, -y) = (x, y)$  

and since we showed $H$ is continuous, it follows that $H^{-1} = H$ is continuous.

So solutions for $X' = AX$ will be of the form:

$\phi^A_t(X_0) = e^t(x_0\cos t, -x_0\sin t) + e^t(y_0\sin t, y_0\cos t)$

And solution for $Y' = BY$ will be of the form

$\phi_t^B(X_0) = e^t(x_0\cos t, x_0\sin t) + e^t(-y_0\sin t, y_0 \cos t)$ 

So $H(X_0) = (x_0, -y_0)$ 

$\phi^B_t(H(X_0)) = e^t(x_0\cos t, x_0 \sin t) + e^t(y_0\sin t, -y_0 \cos t)$ 

$H(\phi_t^A(X_0)) = e^t(x_0\cos t, x_0 \sin t) + e^t(y_0 \sin t, -y_0 \cos t$ )

So we indeed have $\phi^B_t(H(X_0)) = H(\phi_t^A(X_0))$ 

##### Ex. 5(a) Find an explicit conjugacy between the flows of $X' = \begin{pmatrix} -1 & 1 \\ 0 &2 \end{pmatrix}X$ and $Y' = \begin{pmatrix} 1 & 0 \\ 1 & -2 \end{pmatrix}Y$ 

Solutions for $X' = AX$

$\phi_t^A(X_0) = (x_0-\frac{y_0}{3})e^{-t}\begin{pmatrix} 1 \\ 0 \end{pmatrix} + \frac{y_0}{3}e^{2t}\begin{pmatrix} 1 \\ 3\end{pmatrix}$

Putting this solution in terms of a solution for the canonical form left multiplied by $T =  \begin{pmatrix} 1 & 1 \\ 0 & 3 \end{pmatrix}$ 

$= \begin{pmatrix} 1 & 1 \\ 0 & 3 \end{pmatrix}((x_0-\frac{y_0}{3})e^{-t}\begin{pmatrix} 1 \\ 0 \end{pmatrix} + \frac{y_0}{3}e^{2t}\begin{pmatrix} 0 \\ 1\end{pmatrix})$

= $\phi_t^{T^{-1}AT}(x_0 - \frac{y_0}{3}, \frac{y_0}{3})$ 

noting that $\begin{pmatrix} 1 & 1 \\ 0 & 3 \end{pmatrix}\begin{pmatrix} x_0 - y_0/3 \\ y_0 /3 \end{pmatrix} = (x_0, y_0)$ 

so $\phi_t^{T^{-1}AT}(T^{-1}X_0) = T^{-1}(\phi_t^A)$

Solution for $Y' = BY$ 

$\phi_t^B(X_0) = (y_0 - \frac{x_0}{3})e^{-2t}\begin{pmatrix} 0 \\1 \end{pmatrix} + (\frac{x_0}{3})e^t\begin{pmatrix} 3 \\ 1\end{pmatrix}$ 

To put in terms of a solution for the canonical form left multiplied by $S = \begin{pmatrix} 0 & 3 \\ 1 & 1 \end{pmatrix}$ 

$ = \begin{pmatrix} 0& 3 \\ 1 & 1 \end{pmatrix}((y_0 - \frac{x_0}{3})e^{-2t} \begin{pmatrix} 1 \\ 0\end{pmatrix} + \frac{x_0}{3}e^t\begin{pmatrix} 0 \\ 1 \end{pmatrix})$ 

= $\phi_t^{S^{-1}BS}(y_0 - \frac{x_0}{3}, \frac{x_0}{3})$  

So to find a conjugacy $G$ s.t. $G(\phi_t^A(X_0))$ = $\phi_t^{T^{-1}AT}(G(X_0))$ 

$G(x,y) = T^{-1}\begin{pmatrix}x\\y\end{pmatrix}$  (can be easily seen from above)

For the canonical forms, $H(\phi_t^{T^{-1}AT}(X_0)) = \phi_t^{S^{-1}BS}(H(X_0))$

$H = (h_1(x), h_2(y))$ where $h_1(x) = \begin{cases} x^2 & x \geq 0 \\ -|x^2| & x < 0 \end{cases}$, $h_2(y) = \begin{cases} y^{1/2} & y \geq 0 \\ -|y^{1/2}| & y < 0 \end{cases}$ 

And for $J(\phi_t^{S^{-1}BS}(X_0)) = \phi_t^B(J(X_0))$

$J(x,y) = S\begin{pmatrix} x \\ y \end{pmatrix}$ 

So define the conjugacy $K(x,y)$ s.t. $K(\phi_t^{A}(X_0)) = \phi_t^B(K(X_0))$

to be $K(x,y) = (J\circ H\circ G)(x,y)$ 

So from above, we know that we have $G(\phi_t^A(X_0)) = (x_0-\frac{y_0}{3})e^{-t}\begin{pmatrix} 1 \\ 0 \end{pmatrix} + \frac{y_0}{3}e^{2t}\begin{pmatrix} 0 \\ 1\end{pmatrix} $ 

and then $H(G(\phi_t^A{X_0})) = (x_0-\frac{y_0}{3})^2e^{-2t}\begin{pmatrix} 1 \\ 0 \end{pmatrix} + (\frac{y_0}{3})^{1/2}e^{t}\begin{pmatrix} 0 \\ 1\end{pmatrix}$  

and then $J(H(G(\phi_t^A(X_0)))) =  (x_0-\frac{y_0}{3})^2e^{-2t}\begin{pmatrix} 0 \\ 1 \end{pmatrix} + (\frac{y_0}{3})^{1/2}e^{t}\begin{pmatrix} 3 \\ 1\end{pmatrix}$ 

To show equality to $\phi_t^B(K(X_0))$: $(J\circ H\circ G)(X_0) = (3(\frac{y_0}{3})^{1/2}, (x_0 - \frac{y_0}3)^2 +(\frac{y_0}3)^{1/2})$ 

And $\phi_t^B((J\circ H \circ G)(X_0)) = ((x_0-\frac{y_0}{3})^2 + (\frac{y_0}{3})^{1/2} - (\frac{y_0}{3})^{1/2})e^{-2t}\begin{pmatrix} 0 \\ 1 \end{pmatrix} + (\frac{y_0}{3})^{1/2}e^{t}\begin{pmatrix} 3 \\ 1 \end{pmatrix}$ 

So we indeed have have that $K(\phi_t^A(X_0)) = \phi_t^B(K(X_0))$ 

We know that $H$ is a homeomorphism

The matrices $T^{-1}$ and $S$ have columns that are linearly independent, so $J$ and $G$ are one-to-one and onto, and their inverses exist. And since left multiplying by a matrix is linear transformation, and we are working with finite-dimensional space $\R^2$[^footnote] $J$ and $G$ are continuous (the same applies to the inverses, which use matrices $T$ and $S^{-1}$. Both these matrices are one-to-one and over a finite-dimensional space) 

[^footnote]: http://pfister.ee.duke.edu/courses/ecen601/notes_ch5.pdf 

##### Ex. 6: Prove that any two linear systems with the same eigenvalues $\pm i \beta, \beta \neq 0$ are conjugate. What happens if the systems have eigenvalues $\pm i \beta$ and $\pm i \gamma$ with $\beta \neq \gamma$> what if $\gamma = -\beta$ 

Since there always exists a linear map that converts linear systems into canonical form, we work with the canonical matrices of the form $\begin{pmatrix} 0 & \beta \\ -\beta & 0\end{pmatrix}$ 

Let the two systems be $X' = AX$ and $X' = BX$ 

##### Case 1: For both $X' = AX$ and $X' = BX$ $\exists$ two matrices, $S, T$ such that $T^{-1}AT = S^{-1}BS = \begin{pmatrix} 0 & \beta \\ - \beta & 0 \end{pmatrix}$  ($A$ and $B$ correspond to the same canonical matrix)

Then we have $ST^{-1}ATS^{-1} = B$ 

So for any solution to $B$, $X_B$, we claim $TS^{-1}X_B$ is a solution for $X' = AX$ 

$(TS^{-1}X_B)' = TS^{-1}BX_B = T(S^{-1}S)T^{-1}ATS^{-1}X_B = (TT^{-1})ATS^{-1}X_B = ATS^{-1}X_B = A(TS^{-1}X_B)$ so we have $H(x,y) = TS^{-1}\begin{pmatrix} x \\ y \end{pmatrix}$ is a conjugacy that takes solutions for $X' = BX$ to $X' = AX$ 

Since $TS^{-1}$ is a linear transformation mapping a finite-dim. space back to itself, with an inverse, $ST^{-1}$ that also maps a finite-dim space back to itself, it is a homeomorphism. 

##### **Case** 2: $A$ has the canonical form $\begin{pmatrix} 0 & \beta \\ -\beta & 0 \end{pmatrix}$ and $B$ has the canonical form $\begin{pmatrix} 0 & -\beta \\ \beta & 0 \end{pmatrix}$ (this describes what happens when $\gamma = -\beta$ )

solutions to the canonical for for $A$ are of the form: $x_0\begin{pmatrix} \cos\beta t \\ -\sin\beta t \end{pmatrix} + y_0 \begin{pmatrix}\sin\beta t \\ \cos\beta t \end{pmatrix}$ 

and for $B$'s canonical form: $x_0 \begin{pmatrix} \cos \beta t \\ \sin \beta t \end{pmatrix} + y_0 \begin{pmatrix} -\sin\beta t \\ \cos \beta t \end{pmatrix}$ (using the fact that $\cos$ is even and $\sin$ is odd)

$H(x,y) = (x, -y)$ provides a conjugacy between the two canonical forms. 

$H(\phi_t^{T^{-1}AT}(X_0)) = (x_0\cos\beta t + y_0\sin\beta t, x_0\sin\beta t - y_0\cos\beta t)$

$\phi_t^{S^{-1}BS}(H(X_0)) = (x_0\cos\beta t -y_0(-\sin\beta t), x_0\sin\beta t -y_0\cos \beta t)$ = $H(\phi_t^{T^{-1}AT}(X_0))$ 

##### Case 3: $A$ has canonical form $\begin{pmatrix} 0 & \beta \\ -\beta & 0 \end{pmatrix}$ and $B$ has canonical form $\begin{pmatrix} 0 & \gamma \\ -\gamma & 0 \end{pmatrix}$

solutions to the canonical for for $A$ are of the form: $x_0\begin{pmatrix} \cos\beta t \\ -\sin\beta t \end{pmatrix} + y_0 \begin{pmatrix}\sin\beta t \\ \cos\beta t \end{pmatrix}$ 

solutions to the canonical for for $B$ are of the form: $x_0\begin{pmatrix} \cos\gamma t \\ -\sin\gamma t \end{pmatrix} + y_0 \begin{pmatrix}\sin\gamma t \\ \cos\gamma t \end{pmatrix}$

They have different periods: for $A$: $2\pi/|\beta|$ for $B$: $2\pi/|\gamma|$ , but if they go through the same $(x_0, y_0)$ point, then they are travelling the same circle of radius $\sqrt{x_0^2+y_0^2}$

suppose $|\gamma| \neq |\beta|$ and $\gamma, \beta \neq 0$. Then the system that contains the value with larger magnitude - without loss of generality, let this be $\beta$ - is traversing the circle "faster." 

I shall prove these two systems aren't conjugate by contradiction.

Suppose that $h(x,y)$ is a conjugacy from $X'=AX$ to $X' = BX$ 

this means $\phi^B_t(h(X_0)) = h(\phi_t^A(X_0))$ 

and since $\phi_t^A(X_0) = \phi_{t+2\pi/|\beta|}^A(X_0)$ this would mean

$\phi_t^B(h(X_0)) = h(\phi_t^A(X_0)) = h(\phi_{t+2\pi/|\beta|}^A(X_0)) = \phi_{t+2\pi/|\beta|}^B(h(X_0))$  

this implies that $\phi_t^{B}(X_0)$ is periodic with period $2\pi/|\beta|$, a contradiction since this means

$2\pi/|\beta| = 2\pi/|\gamma|$ which contradicts $|\beta| > |\gamma|$ 

or that $2\pi/|\beta| = 2\pi k/|\gamma|$, where $k$ is a positive integer, which is also a contradiction since $2\pi/|\beta| < 2\pi/|\gamma|$  

##### Ex. 7: Consider all linear systems with exactly one eigenvalue equal to 0. Which of these systems are conjugate? Prove this.

The canonical form of these linear systems will be of some form $\begin{pmatrix} 0 & 0 \\ 0 & \lambda \end{pmatrix}$ or $\begin{pmatrix} \lambda & 0 \\ 0 & 0 \end{pmatrix}$ 

$\lambda$ must be real, since if a complex number is a root, its conjugate is also a root.

We then have a straight line of equilibrium solutions on either the $x$ or $y$ axis.

Then on the other axis, we have a line where solutions go away from origin or towards origin depending on the sign of $\lambda$ 

So first I show that if they have the same eigenvalues, $0, \lambda$ they are conjugate:

Case 1: if they have the same canonical form : if $S^{-1}$ transforms solutions from $X' = AX$ to solutions for the canonical form and $T$ transforms solutions from the canonical from to $X' = BX$ then left multiplying solutions for $X' = AX$ by $TS^{-1}$ will transform them to solutions for $X' = BX$ 

Case 2: One's canonical form has solutions of the form $ \begin{pmatrix} x_0 \\ 0\end{pmatrix} +e^{\lambda t}\begin{pmatrix} 0 \\ y_0 \end{pmatrix}$ 

and the other's canonical form has solutions of the form $e^{\lambda t}\begin{pmatrix} x_0 \\ 0 \end{pmatrix} + \begin{pmatrix} 0 \\ y_0 \end{pmatrix}$ 

$H(x,y) = (y,x)$ is a conjugacy:

$H( \begin{pmatrix} x_0 \\ 0\end{pmatrix} +e^{\lambda t}\begin{pmatrix} 0 \\ y_0 \end{pmatrix}) = (e^{\lambda t}y_0, x_0)$ 

and plugging $(y_0, x_0)$ into $e^{\lambda t}\begin{pmatrix} x_0 \\ 0 \end{pmatrix} + \begin{pmatrix} 0 \\ y_0 \end{pmatrix}$ we get the above

$H$ is one-to-one, onto, is continuous as $|(x-x_0,y-y_0)|$ = $|H(x, y) - H(x_0, y_0)|$ , and it is its own inverse, so it follows that its inverse is continuous.

So if they have the same eigenvalues, $0, \lambda$ they are conjugate

Now I show what happens for when their nonzero eigenvalues are not equal.

$X' = AX$ has eigenvalues $0, \lambda$ and $X' = BX$ has eigenvalues $0, \mu$, where $\lambda \neq \mu$ 

and $\lambda, \mu$ have the same sign:

Working with canonical forms:

$\phi_t^{T^{-1}AT}(X_0) = \begin{pmatrix} x_0 \\ 0 \end{pmatrix} + e^{\lambda t}\begin{pmatrix} 0 \\ y_0 \end{pmatrix}$ , $\phi^{S^{-1}BS}_t(X_0) = \begin{pmatrix} x_0 \\ 0 \end{pmatrix} + e^{\mu t}\begin{pmatrix} 0 \\ y_0 \end{pmatrix}$ 

We have $H(x,y) = (x, y^{\mu/\lambda})$ if $y \geq 0$ 

and $H(x,y) = (x, -|y^{u/\lambda}|)$ if $y < 0$   

if $y_0 \geq 0$: $H(\phi_t^{T^{-1}AT}(X_0) = (x_0, e^{\mu t}y_0^{\mu/\lambda})$ and $H(x_0,y_0) = (x_0, y_0^{\mu/\lambda})$ so $\phi_t^{S^{-1}BS}H(X_0)) = (x_0, y_0^{\mu/\lambda}e^{\mu t})$

if $y_0 < 0$ :$H(\phi_t^{T^{-1}AT}(X_0) = (x_0, -e^{\mu t}|y_0^{\mu/\lambda}|)$ and $H(x_0,y_0) = (x_0, y_0^{\mu/\lambda})$ so $\phi_t^{S^{-1}BS}H(X_0)) = (x_0, -|y_0^{\mu/\lambda}|e^{\mu t})$ 

 if $\mu$ and $\lambda$ had different signs, $|h_2(0)| = \infin$, contradicting that $H(x,y) = (h_1(x), h_2(y))$ is continuous, so there would be no homeomorphism.

So, those that have a nonzero eigenvalue > 0 are conjugate with each other

Those that have a nonzero eigenvalue < 0 are conjugate with each other

##### Ex. 8: Consider all linear systems with two zero eigenvalues. Which of these systems are conjugate? Prove this.

The only two canonical forms are: $A =\begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}$ and $B = \begin{pmatrix} 0 & 1 \\ 0 & 0 \end{pmatrix}$ 

Solutions are of the form $\phi_t^A(X_0) = (x_0, y_0)$ or $\phi_t^B(X_0) = \begin{pmatrix} x_0 \\ 0 \end{pmatrix} + y_0 \begin{pmatrix} t \\ 1 \end{pmatrix}$ 

if $C = \begin{pmatrix} 0 & 0 \\ 1 & 0 \end{pmatrix}$ can be considered a canonical form, then solutions for $X' = CX$  can be transformed to solutions to $X' = BX$ by $H(x,y) = (y,x)$ )

Those that send every vector to $0$ (i.e, have two linearly independent eigenvectors, a 2-dim kernel) are conjugate with each other, because they are the same system:

We've proven before that if a system has 2 linearly independent eigenvalues corresponding to a repeated eigenvalue, the matrix corresponding to the system must be the diagonal matrix with its diagonal entries being that eigenvalue.

So all systems of this type must be $X' = 0X$

Those that have only one linearly independent eigenvector associated with $0$ are conjugate:

if $T^{-1}$ sends solutions of one system (1) to solutions for $X' = BX$ 

and $S$ sends solutions of $X' = BX$ to solutions for another system (2)

then $ST^{-1}$ sends solutions from (1) to solutions for (2) 

so $H(x,y) = ST^{-1}\begin{pmatrix} x \\ y \end{pmatrix}$ is a conjugacy

if $H(x,y)$ is a conjugacy between $X' = AX$ and $X' = BX$ 

then we must have $\phi_t^B(H(X_0)) = H(\phi_t^A(X_0)) = H(x_0, y_0) = (h_1(x_0), h_2(y_0))$

this means that for all $t$,  $\phi_t^B(x,y) = (x,y)$, which is impossible, since $\phi_t^B(x,y) = (x+yt, y)$ 

and once $t \neq 0$, $(x + yt, y) \neq (x,y)$ 

So systems that have two LI eigenvectors associated with $0$ are not conjugate with systems that only have one LI eigenvector associated with $0$

So those that have the same canonical form are conjugate with each other.

##### Ex. 9: Provide a complete description of the conjugacy classes for $2 \times 2$ systems in the nonhyperbolic case.

If they have $\alpha = 0$ and $\beta \neq 0$ 

1. They are all conjugate with each other if they have the same eigenvalues, $\pm i\beta$ (even if they go in different directions clockwise or counterclockwise) 

If they have exactly one eigenvalue equal to 0 

1. Those that have a second positive eigenvalue are conjugate with each other (all solutions go away from equilibrium solution line)
2. Those that have a second negative eigenvalue are conjugate with each other (all solutions go towards equilibrium solution line)

If they have repeated eigenvalues equal to 0

1. Those that send all vectors to $0$ must be the zero matrix.
2. Those that have only one linearly independent eigenvector corresponding to 0 are conjugate with each other (one line of equilibrium solutions, all other solutions are lines parallel to this equilibrium solution)