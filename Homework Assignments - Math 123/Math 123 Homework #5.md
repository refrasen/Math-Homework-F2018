Renee Senining

Math 123

### Homework #5

#### Chapter 5

##### Ex. 3: Describe the regions in $a, b, c$-space where the matrix $\begin{pmatrix} 0 & 0 & a \\ 0 & b & 0 \\ c & 0 & 0 \end{pmatrix}$ has real, complex, and repeated eigenvalues.

The characteristic polynomial = $\det \begin{pmatrix} -\lambda & 0 & a \\ 0 & b-\lambda & 0 \\ c & 0 & -\lambda \end{pmatrix}$ 

$ = (-\lambda)(b-\lambda)(-\lambda) + a(-c)(b-\lambda) = (b-\lambda)(\lambda^2 - ac)$ 

roots: $\lambda_1 = b, \lambda_2 = \sqrt{ac}, \lambda_3 = -\sqrt{ac}$ 

For real eigenvalues:

Either $a, c > 0$ or $a, c < 0$ 

​	so anywhere along the $b-$axis, and in the $ac-$plane, the first quadrant

​	or anywhere along the $b$-axis, and in the $ac-$plane, the third quadrant 

For repeated real eigenvalues, if we let $ac = b^2$

​	then depending on the sign of $b$ , either $\sqrt{ac} = b$ or $-\sqrt{ac} = b$  

​	So if we fix $a = k$, where $k$ is a constant, we have in the $bc$ plane, a parabola: $\frac{b^2}k = c$ 

​		$k > 0$ a parabola opening up towards the positive $c$ axis

​		$k < 0$ a parabola opening up towards the negative $c$ axis

​		as $a$ tends away from $0$ in positive/negative direction, the parabola opens up more

​		and the closer $|a|$ gets to 0, the more narrow the parabola is

Or, we could let $a = c = 0$ to get at least two zero eigenvalues, with two linearly independent eigenvectors $(1, 0, 0)$ and $(0, 0, 1)$ this would be the $b-$axis 

and if $b =0$ , then we get the zero matrix at the point $(0, 0, 0)$ in the space

​	if we fix $c = k$, we have in the $ab$ plane: $\frac{b^2}k = a$ 

​		$k > 0$ a parabola opening up towards the positive $a$ axis

​		$k < 0$ a parabola opening up towards the negative $a$ axis

​		as $c$ tends away from $0$ in positive/negative direction, the parabola opens up more

​		and the closer $|c|$ gets to 0, the more narrow the parabola is

For complex eigenvalues, if $a < 0$, we let $c > 0$ and if $a > 0$, we let $c < 0$ 

​	So anywhere along the $b$-axis, and in the $ac-$plane, the second quadrant

​	or the fourth quadrant

In this case, since we only have 3 eigenvalues, we can't have repeated complex values, since for every complex eigenvalue, its conjugate is an eigenvalue. 

##### Ex. 13: Which of the following subsets of $\R^n$ are open and/or dense? Give a brief reason in each case.

###### (a) $U_1 = ${$(x,y) | y > 0$} 

Open: for some point $(x,y)$ with $y > 0$: the ball with radius $y/2$ is contained in $U_1$ so that any point in the open ball must satisfy $y' \in (y/2, y + y/2)$ meaning $y' > 0$ 

Not Dense: if we have a point $(x', y')$ where $y' < 0$, and have $\epsilon = |y'|/2$ any point in this ball must satisfy $y \in (y' - |y'|/2, -|y'|/2)$ so $y$ cannot be greater than 0.

###### (b) $U_2 =$ {$(x,y)| x^2 + y^2 \neq 1$}

So for point in the $xy$-plane, where $(x,y)$ is not on the unit circle

the ball with the radius $r = $  $ \begin{cases}(\sqrt{x^2 +y^2} - 1)/2,  & x^2 + y^2 > 1 \\ (1-\sqrt{x^2+y^2})/2, & x^2+y^2 < 1\end{cases}$  is fully contained in $U_2$ 

So $U_2$ is open.

Dense:

if a point $(x, y)$ is in $U_2$, then, a point in $U_2$ that gets arbitrarily close to $(x,y)$ is itself.

Otherwise: for any point $(x', y')$ on the unit circle and for any $\epsilon > 0$ 

the point $(x' - \epsilon/2, y')$ satisfies $\sqrt{(x' - \epsilon/2 - x')^2 + (y' - y')} = \epsilon/2 < \epsilon$

and $(x'-\epsilon/2)^2 + y'^2 = x'^2 + y'^2 + \epsilon^2/4 > 1$ 

###### (c) $U_3 = $ {$(x,y)|x$ is irrational} 

From real analysis: because there are infinitely many irrational and real numbers between any two numbers, for any open ball with radius $r$ > 0, there always exists $w \in (x - r, x +r)$ such that $w$ is rational

Not open, but dense: if $(x,y)$ is any point in $\R^n$ and $r>0$, there always exists an irrational in $(x-r, x+r)$

###### (d) $U_4 =$ {$x, y$ are not integers}

so $\exists$ $m_x, m_y$ integers such that

$m_x < x < m_x+1$ and $m_y < y < m_y +1$ 

if we take the radius of an open ball to be $ r= \min(x-m_x, m_x+1 - x, y - m_y, m_y+1 - y)$

then we have for any $(w,z)$ satisfying $|(w,z) - (x,y)| < r$, $(w,z) \in U_4$ :

so $w \in (x-r, x+r), z \in (y-r, y+r)$ 

$ m_x<x-r<w < x +r < m_x+1$ and similarly, $z \in (m_y, m_y+1)$ 

so $U_4$ is open.

For any point $(x', y')$:

for any $\epsilon > 0$, there exists infinitely many irrationals, and therefore non-integers, in $(x-\epsilon, x + \epsilon)$ and in $(y-\epsilon, y+\epsilon)$ so $U_4$ is dense.

###### (e) $U_5$ is the complement of a set $C_1$, where $C_1$ is closed and not dense;

$U_5$ is open, since the definition of a closed set is one whose complement is open.

Also: $C_1$ also contains its boundary: any point $(x,y)$ such that for any open ball centered on $(x,y)$ there are points in both $C_1$ and $U_5$ 

So if $U_5$ weren't open, there would exist a point in $U_5$ such that every open ball centered on it would contain points in $C_1$ and itself, so a point in $U_5$, but this is a contradiction, since $C_1$ contains these points, but $C_1$ is the set not containing any points in $U_5$ 

$U_5$ may or may not be dense...

See (a) and (b)

(a) is open and not dense

​	The set $\R^n \setminus U_1 =$ {$(x,y)| y \leq 0$} is closed, since it contains its boundary points, $y =0 $ 

​	$\R^n\setminus U_1$ is not dense, since $U_1$ is open, so it can't get arbitrarily close to every point in $\R^n$ 

(b) is open and dense

​	the set $\R^n\setminus U_2$ contains all points on the unit circle and:

​	is closed since it is its own boundary

​	is not dense, since $U_2$ is open. 

###### (f) $U_6$ is the complement of a set $C_2$ which contains exactly 6 billion and two distinct points

each point in $C_2$ is closed set.

The union of finitely many closed sets is a closed set.

​	So $C_2$  is closed $\implies$ $U_6$ is open.

Also, for any point $P$ in $U_6$ if we center a ball with radius $r$ > 0, s.t. $r$ is less than the distance between $P$ and the shortest distance between $P$ and a point in $U_6$ (this is possible since there finitely many points in $C_2$), the ball is contained in $U_6$ 

To show $U_6$ is dense: for any point $P$ in $\R^n$ 

If  $P$ in $U_6$, then $P$ gets arbitrarily close to itself

If $P$ in $C_2$, and there exists an open ball centered on $P$ s.t. there are no points of $U_6$ in the ball $\implies$ the ball is contained in $C_2$: that would mean there's infinitely many points in $C_2$, therefore, there must always be points of $U_6$ in any open ball centered on any point.

##### Ex. 14: Each of the following properties defines a subset of real $n\times n$  matrices. Which of these sets are open and/or dense in the $L(\R^n)?$ Give a brief reason in each case.

###### (a) $\det A \neq 0$ 

Dense: For any matrix $B$ with $\det B = 0$, and for any $\epsilon > 0$ 

changing just one of the entries in $B$ by at most $\epsilon$  will produce a matrix within $\epsilon$ distance from $B$ that has a nonzero determinant. 

Open: For any matrix $A$ with $\det A \neq 0$, if we choose $\epsilon$ small enough, matrices within $\epsilon$ from $A$ will have determinants that are within some $\delta > 0$ of $\det A$ s.t. $0 \notin (\det A - \delta, \det A + \delta)$  

###### (b) Trace $A$ is rational

Not open: For every small positive number, there is a smaller positive irrational number, and adding a rational number (the trace in this case) and an irrational number (there always exist an irrational within $(0, \epsilon)$) will produce an irrational number, so there exist matrices arbitrarily close to matrices with rational traces that have irrational traces.

Dense: if the trace of some matrix $B$ is irrational, there always exists rational numbers arbitrarily close to the trace, so for example, if we must keep matrices within $\epsilon > 0$ of $B$, there exists a rational number in $(Trace A-\epsilon, Trace A + \epsilon)$, so it is possible to add or subtract a number smaller than $\epsilon$  to any of the diagonal entries of $A$ to produce a matrix within $\epsilon$ of $A$ with a rational trace. 

###### (c) Entries of $A$ are not integers

Open: integers are $1$ apart from each other, and between any non-integer and integer, there are infinitely many non-integer numbers. So if the smallest distance between an entry in $A$ and an integer is $d$, then the matrices that are less than $d$ away from $A$ will have  non integer entries.

Dense: For any matrix that has one or more integer entries, there will always be matrices nearby that have non-integer entries, since for any $\epsilon > 0$, for each of the integer entries, there is a non-integer entry within $\epsilon/n^2$ , for any $n > 0$ 

###### (d) $3 \leq \det A < 4$ 

Not open: if $\det A = 3$ , for any $\epsilon > 0$ , it is possible to change one entry by $\epsilon$ or less s.t. the determinant is less than 3. So for matrices with determinants = 3, it is not possible to find an $\epsilon>0$ s.t. all matrices within $\epsilon$ have determinants of at least 3 and less than 4

e.g: $\begin{pmatrix} 1 & 0 \\ 0 & 3\end{pmatrix}$ , for any $\epsilon > 0$, we have $\begin{pmatrix} 1 - \epsilon/2 & 0 \\ 0 & 3 \end{pmatrix}$ is within $\epsilon$ from the original matrix and the determinant is $3 - 3\epsilon /2 < 3$  

Not dense: If we have a matrix $B$ with $\det B > 4$, for a small enough $\epsilon$ , all matrices within $\epsilon$  of $B$ will have determinants > 4. 

$\begin{pmatrix} 5 & 0 \\ 0 & 5 \end{pmatrix}$  $(5+\delta_1)(5+\delta_2) - (\delta_3)(\delta_4)$ with $\sqrt{\delta_1^2 + \delta_2^2 + \delta_3^2 + \delta_4^2} < 0.1$ , we have $-0.1 < \delta_i < 0.1$ for each $i = 1, 2, 3, 4$ 

$25 + 5\delta_1 +5 \delta_2 +\delta_1\delta_2 - \delta_3\delta_4 >25  -.5 - .5 - .001 -.001 > 4$ 

###### (e) $-1 < |\lambda| < 1$ for every eigenvalue $\lambda$ 

Open: Let $A$ be an matrix with such eigenvalues. We can choose an $\epsilon$ small enough such that the coefficients of the characteristic polynomial do not change significantly, meaning the eigenvalues of matrices within $\epsilon$ of the $A$ stay within $(-1, 1)$ 

Not Dense: (using the same logic as above) If a matrix has an eigenvalue $\lambda > 1$ or $\lambda < -1$ , if we choose $\epsilon$ small enough, the matrices within $\epsilon$ will still have an eigenvalue $\lambda > 1$ or $\lambda < -1$ 

###### (f) $A$ has no real eigenvalues

Open: Varying the entries of $A$ slightly will only vary the coefficients of the characteristic polynomial slightly, so for $\epsilon$ sufficiently small, the eigenvalues of matrices within $\epsilon$  of $A$ will still be complex. 

If we have the number  $z = x+iy$ as an eigenvalue, for all $w$ s.t. $|w - z| < |y|$, we have that

$y - |y| <\text{Im } w < y + |y|$ so $\text{Im }w$ $\neq 0$, so if we choose $\epsilon$ so that all matrices within $\epsilon$  of $A$ have eigenvalues that each satisfy being within $|y|$ of at least one of $A's$ eigenvalues, where $y$ is the imaginary part of an eigenvalue of $A$ of smallest magnitude, then the eigenvalues of these matrices are all complex. 

Not dense: For example, a matrix in $L(\R^2)$ $B= \begin{pmatrix} -1 & 0 \\ 0 & 1 \end{pmatrix}$ 

$T= 0$ , $D = -1$ if we have $\begin{pmatrix} -1 +\delta_1 & \delta_2 \\ \delta_3 & 1 + \delta_4\end{pmatrix}$ 

where $\epsilon = \sqrt{\delta_1^2 + \delta_2^2 + \delta_3^2 + \delta_4^2}$ is the distance between this matrix and $B$ 

$T = \delta_1 + \delta_4$ , $D = (-1+\delta_1)(1+\delta_4) - \delta_2\delta_3 = -1 + \delta_1 - \delta_4 + \delta_1\delta_4 - \delta_2\delta_3 $ 

If the determinant remains negative, we get real eigenvalues, and this happens if we make it so

$\delta_1 - \delta_4 + \delta_1\delta_4 - \delta_2\delta_3 < 1$ and so if we choose $\epsilon < \frac{1}{4}$

each $|\delta_i| < 1/4$  so

$\delta_1 - \delta_4 + \delta_1\delta_4 -\delta_2\delta_3 < \frac{1}{4} + \frac{1}{4} + \frac{1}{16} + \frac{1}{16} < 1$ 

So, for $\epsilon$ small enough, we have that for matrices $B$ with real eigenvalues, all matrices within $\epsilon$ of $B$ will have real eigenvalues.

###### (g) Each real eigenvalue of $A$ has multiplicity one.

Open: again, it is possible to find $\epsilon$ small enough such that the eigenvalues of matrices within $\epsilon$ of $A$ do not vary too much from those of $A$, meaning, they'll still have distinct real eigenvalues.

Dense: If we have a matrix $B$ where there is at least one eigenvalue of multiplicity > 1, just as in page 103 of the book, if we take the canonical form, and replace each diagonal entry in block/blocks corresponding to repeated real eigenvalues with distinct values $\lambda_j$ s.t. $|\lambda- \lambda_j|$ is sufficiently small, we have a new matrix $A$ with distinct real eigenvalues that is close to the canonical form of $B$, $T^{-1}BT$ so $TAT^{-1}$ will be arbitrarily close to $B$ 

##### Ex. 15: Which of the following properties of linear maps on $\R^n$ are generic?

###### (a) $|\lambda| \neq 1$ for every eigenvalue $\lambda$ 

​	generic:

​	open: if all eigenvalues of a matrix $A$ have $|\lambda| \neq 1$, if $\delta > 0$ is the smallest distance between $|\lambda|$ and $1$ for some eigenvalue $\lambda$, we can choose $\epsilon > 0$ s.t. the modulus/ absolute value of eigenvalues of matrices within $\epsilon$ of $A$ are each within $\delta$  of the $|\lambda|$ 's of $A$ 

​	Dense: If we have a matrix $A$ with $|\lambda| \neq 1$ for all eigenvalues $\lambda$, we are done.

​	Otherwise, if a matrix $A$ has one or more eigenvalues with $|\lambda| = 1$ , if we look at the canonical form $T^{-1}AT$ and the blocks in it containing these $\lambda$s , we may replace each of them with some $\lambda'$ s.t. $|\lambda' - \lambda|$ is sufficiently small and $|\lambda'| \neq 1$ 

​	(obvious for 1, -1, and for complex numbers, we just need to find a point really close to the unit circle on the complex plane)

Then this new matrix $B$ is arbitrarily close to $T^{-1}AT$ with eigenvalues that satisfy property $(a)$ and the matrix $TBT^{-1}$ is arbitrarily close to $A$ also having property $(a)$ 

###### (b)  $n = 2$; some eigenvalue is not real

since $n =2$ and we have 2 complex eigenvalues as they come in pairs,  this is equivalent to 14(f)

not generic, because it's not dense. Also, in the Trace Determinant plane, we have that "most" of the plane represents matrices with real eigenvalues.

###### (c) $n = 3$; some eigenvalue is not real

​	we can only have 2 non real eigenvalues, so in this case we must have distinct eigenvalues: a real eigenvalue, a complex eigenvalue, and its conjugate, so this is generic.

###### (d) No solution of $X' = AX$ is periodic (except the zero solution)

For solutions to be periodic, we must have eigenvalues of the form $\pm i\beta$ 

Dense: Let $B$ be a matrix with eigenvalues of the form $\pm i\beta_j$ 

for any block in the canonical form $T^{-1}BT$ with blocks of the form $\begin{pmatrix} 0 & \beta_j \\ -\beta_j & 0 \end{pmatrix}$ 

we can choose $\epsilon_j$ small enough and get $\begin{pmatrix} \epsilon_j & \beta_j \\ -\beta_j & \epsilon_j \end{pmatrix}$ 

so we obtain a matrix $A$ that is both arbitrarily close to the canonical form of $B$ and doesn't eigenvalues of the form $\pm i \beta$ and instead eigenvalues of the form $\epsilon_j \pm i \beta_j$ which won't give us periodic solutions, so the matrix $TAT^{-1}$ will be arbitrarily close to $B$ and have no periodic solutions except the zero solution.

Open: varying the entries of $A$ won't change it's eigenvalues too much, so it is possible to find an $\epsilon >0$ such varying $A$ to obtain a matrix within $\epsilon$  of $A$ won't give us eigenvalues of the form $\pm i\beta$ 

Generic

###### (e) There are $n$ distinct eigenvalues, each with distinct imaginary parts 

Generic,

Open: slightly changing entries in a matrix changes the eigenvalues only slightly, so nearby matrices will still have distinct imaginary parts.

Dense: If we have a matrix $B$ that had complex eigenvalues that had the same imaginary part, $\beta$ 

For each block $\begin{pmatrix} \alpha & \beta \\ -\beta & \alpha \end{pmatrix}$  in the canonical form $T^{-1}BT$ that this is the case, 

we can leave one block alone, and look at the remaining and replace each $\beta$ with a distinct $\beta_j$ s.t. $|\beta - \beta_j|$  is small enough to obtain a new matrix $A$ s.t. $TAT^{-1}$ is arbitrarily close to $B$  that satisfies property (e)

###### (f) $AX \neq X$ and $AX \neq -X$ for all $X \neq 0$ 

So, $A$ does not have $1$ or $-1$ as eigenvalues.

This is a generic property

Open: varying entries of $A$ will vary eigenvalues only slightly, so possible to find $\epsilon$ s.t. all matrices within $\epsilon$ of $A$ will have this property.

Dense: Take a matrix $B$ that has $1$ or $-1$ or both as eigenvalues.

take each block in the canonical form $T^{-1}BT$ that has $1$ or $-1$ as eigenvalues

We can replace each $1$ or $-1$ with some $\lambda_j \neq 1, -1$  s.t. $|\lambda_j - 1|$ is sufficiently small to obtain $A$ s.t. $TAT^{-1}$ is arbitrarily close to $B$ with no eigenvalues equal to 1 or -1

#### Chapter 6

##### Ex. 1: Find the general solution for $X' = AX$ where A is given by:

###### a. $\begin{pmatrix} 0 & 0 & 1 \\ 0 & 1 & 0 \\ 1 & 0 & 0 \end{pmatrix}$ 

Characteristic polynomial: $(-\lambda)(1-\lambda)(-\lambda) + (0 - (1-\lambda))$ 

$ = (1-\lambda)(\lambda^2 -1) = (1-\lambda)(\lambda-1)(\lambda+1)$ eigenvalues: $\lambda_1 = 1, \lambda_2 = 1, \lambda_3 = -1$ 

$V_1 = (0, 1, 0)$, $V_2 = (1, 0, 1)$, $V_3 = (1, 0, -1)$

$X(t) = \begin{pmatrix} c_2e^t + c_3e^{-t} \\ c_1e^{-t} \\ c_2e^t -c_3e^{-t}\end{pmatrix}$

###### b. $\begin{pmatrix} 1 & 0 & 1 \\ 0 & 1 & 0 \\ 1 & 0 & 1 \end{pmatrix}$ 

Characteristic polynomial: $(1-\lambda)(1-\lambda)(1-\lambda) - (1-\lambda)$

$= (1-\lambda)(\lambda^2 - 2\lambda ) = \lambda(\lambda-2)(1-\lambda)$

$\lambda_1 = 0, \lambda_2 = 2, \lambda_3 = 1$ 

$V_1 = (1, 0, -1)$ $V_2 = (1, 0, 1)$ , $V_3 = (0, 1, 0)$ 

$X(t) = \begin{pmatrix} c_1 + c_2e^{2t} \\ c_3e^t \\ -c_1 + c_2e^{2t} \end{pmatrix}$

###### c. $\begin{pmatrix} 0 & 1 & 0 \\ -1 & 0 & 0 \\ 1 & 1 & 1 \end{pmatrix}$ 

Characteristic polynomial: $(-\lambda)(-\lambda)(1-\lambda) -(-1)(1-\lambda) $

$= (1-\lambda)(\lambda^2 +1)$ 

$\lambda_1 = 1, \lambda_2 = i, \lambda_3 = -i$

$V_1 = (0, 0, 1)$

$V_2 = (i, -1,1) = (0, -1, 1) + i (1, 0, 0)$  

$e^{it} = \cos t + i\sin t$

$e^{it}V_2 = (-\sin t, -\cos t, \cos t) + i(\cos t, -\sin t, \sin t)$ 

$X(t) = \begin{pmatrix} -c_2\sin t +c_3\cos t \\ -c_2 \cos t - c_3\sin t \\ c_1e^t + c_2 \cos t + c_3 \sin t \end{pmatrix}$ 



##### Ex. 12:

$\exp(A) = \sum_{k=0}^\infin \frac{A^k}{k!}$ 

If $B = T^{-1}AT$ then $\exp(B) = T^{-1}\exp(A)T$ 

###### a. $\begin{pmatrix} 5 & -6 \\ 3 & -4 \end{pmatrix}$ 

$(5 - \lambda)(-4 - \lambda) + 18 = \lambda^2 -\lambda -2$

eigenvalues: $\frac{1 \pm \sqrt{1^2 - 4(-2)}}{2} = \frac{1 \pm 3}2 $

So $\lambda_1 = 2, \lambda_2 = -1$ 

$T = \begin{pmatrix} 2 & 1\\ 1 & 1 \end{pmatrix}$  

$B = T^{-1}AT = \begin{pmatrix} 2 & 0 \\ 0 & -1\end{pmatrix}$

$\exp(B) = \begin{pmatrix} e^2 & 0 \\ 0 & e^{-1} \end{pmatrix} = T^{-1}\exp(A)T$

$\exp(A) = T\exp(B)T^{-1}$ 

= $\begin{pmatrix} 2 & 1 \\ 1 & 1\end{pmatrix}\begin{pmatrix} e^2 & 0 \\ 0 & e^{-1} \end{pmatrix}\begin{pmatrix} 1 & -1\\ -1 &2\end{pmatrix} $

$= \begin{pmatrix} 2e^2 & e^{-1} \\ e^2 & e^{-1}\end{pmatrix}\begin{pmatrix} 1 & -1\\ -1 &2\end{pmatrix} $  

$= \begin{pmatrix} 2e^2 -e^{-1} & -2e^2 +2e^{-1}\\ e^2 - e^{-1} &-e^2+2e^{-1}  \end{pmatrix}$ 

###### b. $\begin{pmatrix} 2 & -1 \\ 1 & -2\end{pmatrix}$

$Trace = 0$, $D = -4 + 1 = -3$ 

$\frac{\pm \sqrt{12}}{2} = \pm \sqrt{3}$ 

$T = \begin{pmatrix} 1 & 1 \\ 2 - \sqrt{3} & 2 + \sqrt{3}\end{pmatrix}$ 

$\exp(T^{-1}AT) = \begin{pmatrix} e^{\sqrt{3}} & 0 \\ 0 & e^{-\sqrt{3}} \end{pmatrix}$ 

$\begin{pmatrix} 1 & 1 \\ 2 - \sqrt{3} & 2 + \sqrt{3}\end{pmatrix}\begin{pmatrix} e^{\sqrt{3}} & 0 \\ 0 & e^{-\sqrt{3}} \end{pmatrix}\begin{pmatrix} \frac{2 + \sqrt{3}}{2\sqrt{3}} & -\frac{1}{2\sqrt{3}} \\ \frac{ \sqrt{3}-2}{2\sqrt{3}} & \frac{1}{2\sqrt{3}}  \end{pmatrix}$ 

$ = \begin{pmatrix} e^{\sqrt{3}} & e^{-\sqrt{3}} \\ 2e^{\sqrt{3}}-\sqrt{3}e^{\sqrt{3}} & 2e^{-\sqrt{3}} + \sqrt{3}e^{-\sqrt{3}} \end{pmatrix}\begin{pmatrix} \frac{2 + \sqrt{3}}{2\sqrt{3}} & -\frac{1}{2\sqrt{3}} \\ \frac{ \sqrt{3}-2}{2\sqrt{3}} & \frac{1}{2\sqrt{3}}  \end{pmatrix}$ 

$ = \frac{1}{2\sqrt{3}}\begin{pmatrix}  {2(e^{\sqrt{3}}- e^{-\sqrt{3}}) + \sqrt{3}(e^{\sqrt{3}} + e^{-\sqrt{3}})}  & e^{-\sqrt{3}} - e^{\sqrt{3}}  \\ e^{\sqrt{3}} - e^{-\sqrt{3}} & 2(e^{-\sqrt{3}} - e^{\sqrt{3}}) + \sqrt{3}(e^{\sqrt{3}} + e^{-\sqrt{3}}) \end{pmatrix}$

###### c. $\begin{pmatrix} 2 & -1 \\ 0 & 2 \end{pmatrix}$

Eigenvalues: $2 \pm \frac{\sqrt{4^2 - 4(4)}}2 = 2$ 

 $V_1 = (1,0)$ 

Solving for

$(A - 2I)X = V_1$ we get

$V_2 = (0, -1)$

$T = $ $\begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$ , $T^{-1}$ $= \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$  

$B =T^{-1}AT = \begin{pmatrix} 2 & 1 \\ 0 & 2\end{pmatrix}$ 

$B^2 = \begin{pmatrix} 2^2 & 2 + 2 \\ 0 & 2^2\end{pmatrix}$

$B^3 = \begin{pmatrix} 2^3 & 2^2(3) \\ 0 & 2^3 \end{pmatrix}$ 

$B^4 = \begin{pmatrix} 2^4  & 2^3(4)\\ 0 & 2^4\end{pmatrix}$ 

So $B^k = \begin{pmatrix} 2^k & k2^{k-1} \\ 0 & 2^k \end{pmatrix}$ 

In the top right entry: $1 + \sum_{k =0}^{\infin}\frac{2^k}{k!}$

$\exp(B) =$$\begin{pmatrix} \sum_{k=0} ^{\infin}\frac{2^k}{k!}  &   \sum_{k=0} ^{\infin}\frac{2^{k}}{k!}  \\ 0 & \sum_{k=0} ^{\infin}\frac{2^k}{k!} \end{pmatrix}$ $= \begin{pmatrix} e^2 & e^2 \\ 0 & e^2 \end{pmatrix}$

$\begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}\begin{pmatrix} e^2 & e^2 \\ 0 & e^2 \end{pmatrix} \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$ 

$ = \begin{pmatrix} e^2  &  e^2 \\ 0 & -e^2 \end{pmatrix}$$\begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$ 

$\begin{pmatrix} e^2 & -e^2\\ 0 & e^2 \end{pmatrix}$

###### d. $\begin{pmatrix} 0 & 1 \\ 1 & 0 \end{pmatrix}$ 

$\lambda^2 -1 = 0 ​$ eigenvalues are $1, -1​$ 

$V_1 = (1, 1)$ $V_2 = (1, -1)$ 

$T =$$\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}$ , $T^{-1} = $ $\frac{1}{2}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}$ 

$B = \begin{pmatrix} 1 & 0 \\ 0 & -1 \end{pmatrix}$ 

$\exp(B) = \begin{pmatrix} e & 0 \\ 0  & e^{-1} \end{pmatrix}$ 

$\exp(A) = TAT^{-1} = $$\frac{1}{2}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}\begin{pmatrix} e & 0 \\ 0  & e^{-1} \end{pmatrix}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}$

$ = \frac{1}2\begin{pmatrix} e & e^{-1}\\ e & - e^{-1} \end{pmatrix}\begin{pmatrix} 1 & 1 \\ 1 & -1 \end{pmatrix}$ 

$ = \frac{1}2\begin{pmatrix} e + e^{-1} & e - e^{-1} \\ e - e^{-1} & e + e^{-1} \end{pmatrix}$ 

##### Ex. 13: Find an example of two matrices $A, B$  such that $\exp(A + B) \neq \exp(A)\exp(B)$

$A = \begin{pmatrix} 1 & -1 \\ 0 & -1\end{pmatrix}$ , $B = \begin{pmatrix} 1 & 1 \\ 0 & 1 \end{pmatrix}$ $C = A+B = \begin{pmatrix} 2 & 0 \\ 0 & 0\end{pmatrix}$

Eigenvalues for $A$: $\lambda_1 = 1, \lambda_2 = -1$ , $V_1 = (1, 0)$, $V_2 = (1, 2)$ 

$T =$ $\begin{pmatrix} 1 & 1 \\ 0 & 2 \end{pmatrix}$ , $T^{-1}=$$\frac{1}2$$\begin{pmatrix} 2 & -1 \\ 0 & 1\end{pmatrix}$

$\exp(A) = \frac{1}2 \begin{pmatrix} 1 & 1 \\ 0 & 2 \end{pmatrix}\begin{pmatrix} e & 0 \\ 0 & e^{-1}\end{pmatrix}\begin{pmatrix} 2 & -1 \\ 0 & 1\end{pmatrix}$ $ = \frac{1}2\begin{pmatrix} 2e & -e + e^{-1} \\ 0 & 2e^{-1}  \end{pmatrix}$ 

$\exp(B) = \begin{pmatrix} e & e \\ 0 & e \end{pmatrix}$ 

$\exp(A)\exp(B) = \frac{1}2\begin{pmatrix} 2e^2 & e^2  + 1 \\ 0 & 2 \end{pmatrix}$ 

But $\exp(A+B) = \begin{pmatrix} e^2 & 0 \\ 0 & 1 \end{pmatrix}$ 

##### Ex. 14: Show that if $AB = BA$ then

###### (a) $\exp(A)\exp(B) = \exp(B)\exp(A)$ 

Because $AB = BA$ 

$\exp(A+B) = \exp(A)\exp(B)$ 

$\exp(B+A) = \exp(B)\exp(A)$ 

but also: 

$BA = AB$ 

$A+B = B+A$ 

so $\exp(A + B) = \exp(B+A)$ 

$\implies$ $\exp(A)\exp(B) = \exp(B)\exp(A)$

###### (b) $\exp(A)B = B\exp(A)$ 

Because $AB = BA$ 

$B^{-1}AB = A$ and using if $ B = T^{-1}AT$, then $\exp(B) = T^{-1}\exp(A)T$ 

but replacing $B$ with $A$, and $T$ with $B$ 

So because $A = B^{-1}AB$, $\exp(A) = B^{-1}\exp(A)B$ 

giving: $B\exp(A) = \exp(A)B$ 