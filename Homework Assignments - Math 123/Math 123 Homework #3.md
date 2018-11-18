Renee Senining

Math 123

### Homework 3

#### Ex. 1

![1536214157470](C:\Users\Renee\AppData\Local\Temp\1536214157470.png)

##### (a) $\begin{pmatrix} 3 & 5 \\ -2 & -2 \end{pmatrix}$ 

Characteristic equation: $(3-\lambda)(-2 - \lambda) +10 = \lambda^2 -\lambda +4$

Eigenvalues: $\lambda_1 = \frac{1 + i\sqrt{15}}{2}$, $\lambda_2 =  \frac{1 - i\sqrt{15}}{2}$

$\alpha = 1/2, \beta = \sqrt{15}/2$ 

since $\alpha > 0$, spiral source, so 3 or 7.

The direction the graph goes at $(1,0)$ is going be tangent to the vector from that point $(3, -2)$, so it goes to the right and down, and that matches more to phase portrait 3 than 7.

##### (b) $\begin{pmatrix} -3 & -2 \\ 5 & 2 \end{pmatrix}$ 

Characteristic equation: $(-3-\lambda)(2-\lambda) +10 = \lambda^2 + \lambda +4$ 

Eigenvalues: $\lambda = \frac{-1 \pm i\sqrt{15}}{2}$

since $\alpha < 0$, spiral sink, so 4 or 5

at $(1,0)$, the directional vector is $(-3, 5)$, so the graph is going up and to the left, and that matches to phase portrait 5. 

##### (c) $\begin{pmatrix} 3 & -2 \\ 5 & -2 \end{pmatrix}$ 

Characteristic equation: $(3 - \lambda)(-2 -\lambda) +10 = \lambda^2 -\lambda +4$

Eigenvalues: $\lambda_1 = \frac{1 + i\sqrt{15}}{2}$, $\lambda_2 =  \frac{1 - i\sqrt{15}}{2}$

$\alpha = 1/2, \beta = \sqrt{15}/2$ 

since $\alpha > 0$, spiral source, must be phase portrait 7, since 3 is taken.

##### (d) $\begin{pmatrix} -3 & 5 \\ -2 & 3 \end{pmatrix}$

Characteristic equation: $(-3 - \lambda)(3 - \lambda) +10 = \lambda^2 +1$,

So $\alpha = 0, \beta = 1$ a center, must be either 1 or 2

at $(1,0)$, the directional vector is $(-3, -2)$, sothe graph should be going to the left and down, 

and this matches more to phase portrait 1.

##### (e) $\begin{pmatrix} 3 & 5 \\ -2 & -3 \end{pmatrix}$

Characteristic equation: $(3 - \lambda)(-3 - \lambda) +10$ , has same eigenvalues as **(d)** 

So $\alpha = 0, \beta = 1$, a center, so must be phase portrait 2, since 1 is taken.

##### (f) $\begin{pmatrix} -3 & 5 \\ -2 & 2 \end{pmatrix}$ 

Characteristic equation: $(-3 -\lambda)(2 - \lambda) + 10$

has the same eigenvalues as **(b)**, as it's the transpose, so its also a sink, and the directional vector at $(1,0)$ is $(-3, -2)$, so the graph is going to the left and down, and that matches with phase portrait 4.

#### Ex. 2(vi) $A = \begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}$ 

##### (a) Find the eigenvalues and eigenvectors

$(\lambda-1)(\lambda+1) -1 = \lambda^2 -2$, eigenvalues: $\pm \sqrt{2}$ 

eigenvector associated with $\sqrt{2}$: $V_1=$$(1, \sqrt{2}-1 )$ 

eigenvector associated with $-\sqrt{2}$: $(1, -\sqrt{2}-1)$ 

##### (b) Find the matrix T that puts A in canonical form

$TE_1 = (1, \sqrt{2}-1 )$ , $TE_2 = (1, -\sqrt{2}-1)$ 

$T = \begin{pmatrix} 1 & 1 \\ \sqrt{2} -1 & -\sqrt{2} -1 \end{pmatrix}$ 

##### (c) Find the general solution of both $X' = AX$ and $Y' = (T^{-1}AT)Y$ 

$Y(t) = \alpha e^{\sqrt{2}t}(1,0) + \beta e^{-\sqrt{2}t}(0,1)$ 

$X(t) = \alpha e^{\sqrt{2}t}(1, \sqrt{2}-1) + \beta e^{-\sqrt{2}t}(1, -\sqrt{2}-1)$ 

##### (d) Sketch the phase portraits of both systems.

For $Y' = (T^{-1}AT)Y$, we have a saddle, with straight line solutions on the axes, and as time increases, the solutions look more like $\alpha e^{\sqrt{2}t}(1,0)$ , and as time decreases, look more like $\beta e^{-\sqrt{2}t}(0,1)$ 

![1536218097535](C:\Users\Renee\AppData\Local\Temp\1536218097535.png)

For $X' = AX$: 

![1536218861547](C:\Users\Renee\AppData\Local\Temp\1536218861547.png)

#### Ex. 5

$\det A = 0$, for all $a$ , so $0$ will always be an eigenvalue, and in general, there will be a straight line of equilibrium solutions through origin and $(1, -a)$

The characteristic equation: $\lambda^2 - (a+2)\lambda = \lambda(\lambda -a-2)$ 

When $a = -2$, $A = \begin{pmatrix} -2 & 1 \\ -4 & 2 \end{pmatrix}$ 

we have repeated eigenvalues at 0, but only one linearly independent eigenvector: $(1, 2)$,

Setting $W = (1,0)$, $AW = (-2, -4) = \mu(1,2) + 0\times W$ so $\mu = -2$, and $U = -\frac{1}{2}W = (-1/2, 0)$   

and we have $T = \begin{pmatrix} 1 & -1/2 \\ 2& 0 \end{pmatrix}$ , and $T^{-1}AT = \begin{pmatrix} 0 & 1 \\ 0  & 0 \end{pmatrix}$ 

The general solution for $Y' = T^{-1}ATY$ is $Y(t) = \alpha (1, 0) + \beta (t, 1)$ and  $X(t) = TY(t) = \alpha(1,2) + \beta(t - 1/2, 2t)$ = $(\alpha - \beta, 2\alpha) +\beta t (1, 2)$, a line going through point $(\alpha - \beta, 2\alpha)$ in the direction of the vector $(1,2)$ is the general solution for $X' = AX$ 

Along the line $y = 2x$, we have equilibrium solutions, so there's no vectors on these points, and everywhere else on the phase portrait is going to be a line with slope $2$,

and lines below $y = 2x$ are going to be going down to the left as $t$ increases, and lines above $y = 2x$ are going to be going up and to the right as $t$ increases

 For other cases of $a$, in general, the solution will be:

$X(t) = \alpha (1, -a) + \beta e^{(a+2)t}(1, 2)$ 

All solutions will be a line with slope 2, either going up to the right or down to the left depending on where it starts with respect to the line of equilibrium solutions and the value of $a$ 

When $a < -2$, we have $\lambda_1 = 0, \lambda_2 = a +2 < 0$, a sink 

and one straight line that goes through origin and $(1, 2)$, where all points on that line go towards origin.

note, as $t$ increases, $X(t)$ $\rightarrow \alpha(1, -a)$, so all solutions will eventually come back to some point on the line of equilibrium solutions. 

When $a > -2$, we have $\lambda_1 = 0, \lambda_2 = a + 2 > 0$, a source

and one straight line that goes through origin and $(1,2)$, where all points on that line go away from origin.

and for any solution, as $t$ increases, they will go further away from the line going through $(1, -a)$ 

#### Ex. 8

Let $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$ be a real valued matrix.

The characteristic equation: $(a-\lambda)(d-\lambda) -bc = \lambda^2 -(a+d)\lambda + ad -bc$

so eigenvalues = $\frac{a+d \pm \sqrt{(a+d)^2 - 4(ad-bc)}}{2}$ 

For complex eigenvalues: $(a+d)^2 -4(ad-bc) < 0$ 

so $(a+d)^2 < 4(ad-bc)$ 

and if we want eigenvalues with no real parts, so eigenvalues of the form $\pm i\beta$ 

$a+d = 0$ so $a = -d$ 

We need: $0 < 4(-a^2 - bc)$ 

so $a^2 < -bc$ 

#### Ex. 9

Suppose $A$ is a real valued matrix with eigenvalues of the form $\alpha \pm i\beta$, where $\beta \neq 0$ \If we look at the vector $AE_1$, and the $y$ component > 0, then the solution at this point is moving up away from the $x$-axis, meaning it is moving counterclockwise.

Also, if we look at the vector $AE_2​$, and the $x​$ component is < 0, then the solution is moving to the left away from the $y​$-axis, which also means it is moving counterclockwise.

So if $A = \begin{pmatrix} a & b \\ c & d\end{pmatrix}$, and $c > 0$ and $b < 0$ AND $A$ has complex eigenvalues, then we have solutions traveling counterclockwise. 

#### Ex. 11

$x' = y \\ y' = 0$ 

so we have that $y = \beta$, where $\beta$ is a constant. 

$x' = \beta\implies x = \beta t +\alpha$, where $\alpha$ is another constant

The general solution is $X(t) = \alpha (1,0) + \beta(t, 1)$

$X(0) = (\alpha, \beta)$ , so $\phi(t, X_0) = x_0(1,0) + y_0(t,1)$ 

The phase portrait is going to have equilibrium solutions along the $x$-axis

All other solutions will be straight-lines parallel to the $x$-axis. In particular, a specific solution $x_0(1,0) + y_0(t,1)$ will be lying on the line $y = y_0$ 

Depending on the value of $y_0$, a solution will be moving to the right of the point $(x_0, y_0)$ as $t$ increases if $y_0 > 0$ or to the left as $t$ increases if $y_0 < 0$ 

So all solutions below the $x$-axis are moving to the left parallel to the $x$-axis

and all solution above are moving to the right parallel to the $x$ -axis

#### Ex. 14

The previous problem states that if $\lambda^2 +\alpha \lambda + \beta = 0$ is the characteristic equation for a $2 \times 2$ matrix $A$, then $A^2 + \alpha A + \beta I$ is the $0$ matrix

We assume a $2\times2$ matrix $A$ has repeated eigenvalues

If $V$ is an eigenvector, we have that $(A-\lambda I)V = AV - \lambda V = \lambda(V -V) = 0$

	so since eigenvectors must be nonzero, $(A-\lambda I)V$ is not an eigenvector if $V$ is an eigenvector.	 

Otherwise, we assume $V$ is not an eigenvector, and show that $(A-\lambda I)V$ is an eigenvector

Since $A$ has repeated eigenvalues $\lambda$, we have that the characteristic equation is equal to $(x - \lambda)^2$ 

Multiplying $A - \lambda I$ by $(A-\lambda I)V$, we obtain: $(A-\lambda I)(A - \lambda I)V = (A - \lambda I)^2V$

Since $A$ satisfies its own characteristic equation $(A-\lambda I)^2$ is the zero matrix, meaning:

$(A - \lambda I)^2V = 0 \equiv \\ A(A - \lambda I)V - \lambda I(A-\lambda I)V = 0 \equiv \\A(A-\lambda I)V = \lambda(A-\lambda I)V$ 

meaning, $(A-\lambda I)V$ is an eigenvector.  

#### Ex. 15

Suppose we have a matrix $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$ with repeated real eigenvalues $\lambda$ and two linearly independent eigenvectors.

if $V_1, V_2$ are linearly independent eigenvectors

For any vector $V \in \R^2$, $\exists c_1, c_2 \in \R$ such that $c_1V_1 + c_2V_2 = V$  

So $AV = A(c_1V_1 + c_2V_2) = c_1\lambda V_1 + c_2 \lambda V_2 = \lambda(c_1V_1 + c_2V_2) = \lambda V$

This means:

for any vector $V$ in $\R^2$, $AV = \lambda V$$\equiv$ $(A - \lambda I)V = 0$ for all $V \in \R^2$ 

We must have that $(A-\lambda I)$ is the zero matrix, 

	Otherwise: If $\exists$ a nonzero entry in $(A-\lambda I)$, say $(A-\lambda I)_{ij}$, 

	then $(A-\lambda I)E_j$ , the column of $(A-\lambda I)$ containing $(A-\lambda I)_{ij}$ would be nonzero, 

	a contradiction.

which means $A = \lambda I$ 