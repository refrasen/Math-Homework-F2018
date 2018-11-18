Renee Senining

Math 123

# Homework #2

#### Ex 2. Find the general solution of each of the following linear systems

##### (a) $X' = \begin{pmatrix} 1 & 2 \\ 0 & 3 \end{pmatrix}X$

Finding the eigenvalues and eigenvectors:

$(1-\lambda)(3-\lambda) - 2\times0 = (1-\lambda)(3-\lambda)$, meaning roots at $\lambda = 1, 3$ 

When $\lambda = 1$, eigenvector: $\begin{pmatrix} 1 \\ 0 \end{pmatrix}$, One Solution: $ e^{t}\begin{pmatrix}1 \\ 0 \end{pmatrix}$

When $\lambda = 3$, eigenvector: $\begin{pmatrix} 1 \\ 1\end{pmatrix}$ , One solution:  $e^{3t}\begin{pmatrix}1 \\ 1\end{pmatrix}$ 

General solution: $X(t) = \alpha e^{t}\begin{pmatrix}1 \\ 0 \end{pmatrix}+ \beta e^{3t}\begin{pmatrix}1 \\ 1\end{pmatrix}$ 

##### (b) $X' = \begin{pmatrix} 1 & 2 \\ 3 & 6 \end{pmatrix}X$

Finding eigenvalues: $(1- \lambda)(6 - \lambda) - 6 = \lambda^2 -7\lambda$, roots at $\lambda = 0, 7$ 

When $\lambda = 0$, eigenvector: $\begin{pmatrix} -2 \\ 1 \end{pmatrix}$ 

When $\lambda = 7$, eigenvector: $\begin{pmatrix} 1 \\ 3 \end{pmatrix}$ 

General solution: $X(t) = \alpha \begin{pmatrix} -2 \\ 1 \end{pmatrix} + \beta e^{7t} \begin{pmatrix} 1 \\ 3 \end{pmatrix}$ 

##### (c) $X' = \begin{pmatrix} 1 & 2 \\ 1 & 0 \end{pmatrix}X$

Finding eigenvalues: $(1-\lambda)(-\lambda) - 2 = \lambda^2 -\lambda - 2 = (\lambda -2)(\lambda+1)$, roots at $\lambda = -1,2$ 

When $\lambda = -1$, eigenvector: $\begin{pmatrix} 1 \\ -1 \end{pmatrix}$ 

When $\lambda = 2$, eigenvector: $\begin{pmatrix} 2 \\ 1 \end{pmatrix}$ 

General solution: $X(t) = \alpha e^{-t} \begin{pmatrix} 1 \\ -1 \end{pmatrix} + \beta e^{2t} \begin{pmatrix} 2 \\ 1 \end{pmatrix}$  

##### (d) $X' = \begin{pmatrix} 1 & 2 \\ 3 & -3 \end{pmatrix}X$

Finding eigenvalues: $(1 - \lambda)(-3 - \lambda) - 6 = \lambda^2 +2\lambda - 9$, roots at $\lambda = -1\pm\sqrt{10}$, (found using quadratic equation)

When $\lambda = -1 + \sqrt{10}$ , eigenvector: $\begin{pmatrix} 1 \\ -1 + \sqrt{10}/2 \end{pmatrix}$

When $\lambda = -1 - \sqrt{10}$, eigenvector: $\begin{pmatrix} 1 \\ -1 -1 \sqrt{10}/2 \end{pmatrix}$ 

General solution: $X(t) = \alpha e^{(-1 + \sqrt{10})t}\begin{pmatrix} 1 \\ -1 + \sqrt{10}/2 \end{pmatrix}+ \beta e^{(-1 - \sqrt{10})t}\begin{pmatrix} 1 \\ -1 -1 \sqrt{10}/2 \end{pmatrix}$ 

#### Ex 3. In Figure 2.2 you see four direction fields. Match each of these direction fields with one of the systems in the previous exercise.

![1535689770566](C:\Users\Renee\AppData\Local\Temp\1535689770566.png)

For (a) , when we look at $(1, 0)$, we get back the tangent vector $(1, 0)$, and when we look at $(1, 1)$, we get $(3,3)$ as the tangent vector

For (b), on the line $y = (-1/2)x$ , we should have no vectors

For (c) at $(-1, 1)$, we get the tangent vector $(1, -1)$, and at $(1, -1)$, the tangent vector $-1, 1$ 

and at $(2,1)$, the tangent vector $(4,2)$, also along the $y-$axis, when $y>0$, we should get vectors that go towards the right horizontally, and when $y<0$, vectors that go to the left horizontally.

For (d) along the line $y = x$, we should have vectors of the form $(3x, 0)$ 

So:

$(a) \rightarrow 4$ 

$(b) \rightarrow 2$ 

$(c) \rightarrow 1$ 

$(d) \rightarrow 3$ 

#### Ex 4. Find the general solution of the system $X' = \begin{pmatrix} a & b \\ c & a \end{pmatrix}$ , where $bc > 0$.

Assuming $a, b, c$ are real:

Finding eigenvalues: $(\lambda -a)^2 - bc = \lambda^2 -2a +(a^2-bc)$

Using quadratic equation: we get roots at $a \pm \sqrt{bc}$, which is real, since $bc >0$ 

For $\lambda = a + \sqrt{bc}$, the eigenvector is $\begin{pmatrix} \sqrt{|b|} \\ \sqrt{|c|} \end{pmatrix}$

For $\lambda = a - \sqrt{bc}$, the eigenvector is $\begin{pmatrix} \sqrt{|b|} \\ -\sqrt{|c|} \end{pmatrix}$ 

General solution: $X(t) = \alpha e^{(a + \sqrt{bc})t}\begin{pmatrix} \sqrt{|b|} \\ \sqrt{|c|} \end{pmatrix} + \beta e^{(a-\sqrt{bc})t}\begin{pmatrix} \sqrt{|b|} \\ -\sqrt{|c|} \end{pmatrix} $   

#### Ex 6. For the harmonic oscillator system $x'' + bx' + kx = 0$, find all values of $b$ and $k$ for which this system has real, distinct eigenvalues. Find the general solution of this system in these cases. Find the solution of the system that satisfies the initial condition $(0, 1)$. Describe the motion of the mass in this particular case.

$x' = y$

$y' = -kx - by$ 

We now have: $X' = \begin{pmatrix} 0 & 1 \\ -k & -b \end{pmatrix}X$ 

Finding the eigenvalues: $(-\lambda)(-b-\lambda) + k = \lambda^2+b\lambda +k$

We get: $\frac{-b \pm \sqrt{b^2-4k}}{2}$ 

setting $\lambda_1 = (-b+\sqrt{b^2-4k})/2, \lambda_2 = (-b - \sqrt{b^2-4k})/2$

General solution: $X(t) = \alpha e^{\lambda_1t} \begin{pmatrix} 1 \\ \lambda_1 \end{pmatrix} +\beta e^{\lambda_2t} \begin{pmatrix}1 \\ \lambda_2 \end{pmatrix}$ 

To find the solution that satisfies the initial condition $(0 ,1)$, we must solve

$\begin{pmatrix} 1 & 1 \\ \lambda_1 & \lambda_2 \end{pmatrix} \begin{pmatrix} \alpha \\ \beta \end{pmatrix} = \begin{pmatrix} 1 \\ 0 \end{pmatrix}$ 

When we row reduce the augmented matrix:

$\begin{pmatrix} 1 & 0 & \lambda_2/(\lambda_2-\lambda_1) \\ 0 &1 & -\lambda_1/(\lambda_2-\lambda_1) \end{pmatrix}$

We end up with $\alpha = \lambda_2/(\lambda_2 - \lambda_1)$ , $\beta = -\lambda_1/(\lambda_2-\lambda_1)$ 

$X(t) = \frac{\lambda_2}{\lambda_2-\lambda_1} e^{\lambda_1t} \begin{pmatrix} 1 \\ \lambda_1 \end{pmatrix} -\frac{\lambda_1}{\lambda_2-\lambda_1} e^{\lambda_2t} \begin{pmatrix}1 \\ \lambda_2 \end{pmatrix}$

1. If $k > 0$, we need $b^2 - 4k > 0$ to have real, distinct values, so $b >2\sqrt{k}$ or $b <- 2\sqrt{k}$   

   1. If $b > 0$ 

      $\lambda_2 < 0$, since $(-b - \sqrt{b^2-4k})/2 < 0$  

      $\lambda_1 < 0$, since $b^2 -4k < b^2$, so $\sqrt{b^2 - 4k} < b$ 

      for all $t > 0$, and because $\lambda_2 < \lambda_1$ 

      $e^{\lambda_1t}> e^{\lambda_2}t > 0$

      $\lambda_2/(\lambda_2-\lambda_1) > \lambda_1/(\lambda_2-\lambda_1) > 0$

      so:

      $x(t) =  \frac{\lambda_2}{\lambda_2-\lambda_1} e^{\lambda_1t} -\frac{\lambda_1}{\lambda_2-\lambda_1} e^{\lambda_2t} >0$ for all $t$, and as $t$ increases, both $e^{\lambda_1t}$ and $e^{\lambda_2t}$ go towards 0, so the mass moves towards the origin.

   2. If $b<0$

      $\lambda_1 > 0$, $\lambda_2> 0$ 

      and $\lambda_2 < \lambda_1$, so $\lambda_2 - \lambda_1<0$ 

      And we have $x(t) =  \frac{\lambda_2}{\lambda_2-\lambda_1} e^{\lambda_1t} -\frac{\lambda_1}{\lambda_2-\lambda_1} e^{\lambda_2t}$ 

      and when $e^{(\lambda_1-\lambda_2)t} >\frac{\lambda_1}{\lambda_2}$, which will happen eventually, since $e^{(\lambda_1-\lambda_2)t} \rightarrow\infin$ as $t \rightarrow \infin$ 

      we have that $x(t) < 0$, and in fact, $x(t) \rightarrow -\infin$ as $t \rightarrow \infin$ 

      which means the mass moves back to origin and the spring keeps compressing. 

2. If $k = 0$, we have eigenvalues: $\lambda_1= 0, \lambda_2 = -b$ with eigenvectors: $(1, 0)$ and $(1, -b)$ respectively. For distinct, real, we must have $b \in \R\setminus$ $0$. 

   The solution that satisfies $X(0) = (1, 0)$ is $\alpha = 1, \beta = 0$ , since which means that $X(t) = (1, 0)$ for all $t$, so the mass isn't moving: this makes sense as the velocity is 0, and the spring constant is 0, so there's no restorative force to bring the mass back to its natural resting place, $x = 0$ 

3. If $k < 0$, $b$ must be real, 

   1. regardless of the sign of $b$, since $b^2-4k > b^2$,  $\sqrt{b^2-4k} > |b|$ 

      $\lambda_1 > 0$, $\lambda_2 < 0$ 

      $\lambda_2/(\lambda_2-\lambda_1) > 0$, and $\lambda_1/(\lambda_2-\lambda_1) < 0$

      so as $t \rightarrow +\infin$ : $\frac{\lambda_2}{(\lambda_2-\lambda_1)}e^{\lambda_1t} \rightarrow +\infin$ and $\frac{\lambda_1}{(\lambda_2-\lambda_1)}e^{\lambda t} \rightarrow 0$   

      so $x(t) \rightarrow +\infin$ , meaning the mass keeps moving away from origin



#### Ex 7. Consider the $2 \times 2$ matrix $A = \begin{pmatrix} a & 1 \\ 0 &1\end{pmatrix}$ Find the value of $a_0$ of the parameter of $a$ for which $A$ has repeated real eigenvalues. What happens to the eigenvectors of this matrix as $a$ approaches $a_0$? 

the characteristic polynomial: $(\lambda -a)(\lambda -1)$ 

So when $a = 1$, we have repeated eigenvalues, and the corresponding eigenvector will be:

$(1, 0)$ 

When $a \neq 1$, we have two eigenvectors, so as $a \rightarrow 1$, we go from 2 eigenvectors:

$(1, 0)$ corresponding to the eigenvalue $a$, and

$(1, 1-a)$ corresponding to the eigenvalue 1.  

and we notice as $a \rightarrow 1$ the eigenvector corresponding to 1 approaches the eigenvector corresponding to $a$ 

#### Ex 9. Give an example of a linear system for which $(e^{-t}, \alpha)$ is a solution for every constant $\alpha$. Sketch the direction field for this system. What is the general solution of this system?

$Y(t) = e^{-t} \begin{pmatrix} 1 \\ 0 \end{pmatrix}+\alpha\begin{pmatrix} 0 \\ 1 \end{pmatrix}$ and $Y'(t) = \begin{pmatrix} -e^{-t} \\ 0\end{pmatrix}$ 

$\begin{pmatrix} -1 & 0 \\ 0& 0\end{pmatrix} \begin{pmatrix} e^{-t} \\ \alpha \end{pmatrix} = \begin{pmatrix} -e^{-t} \\ 0 \end{pmatrix}$, for all $\alpha, t$ 

The general solution is $X(t) = \alpha \begin{pmatrix} 0 \\ 1\end{pmatrix} + \beta e^{-t}\begin{pmatrix} 1 \\ 0 \end{pmatrix}$ 

$x' = -x \\ y' = 0$  

![1535977136866](C:\Users\Renee\AppData\Local\Temp\1535977136866.png)

#### Ex 11 Prove that two vectors $V = (v_1, v_2)$ and $W = (w_1, w_2)$ are linearly independent $\iff$ $\det\begin{pmatrix} v_1 & w_1 \\ v_2 & w_2 \end{pmatrix} \neq 0$

We can prove this by proving: $V$ and $W$ are linearly dependent $\iff \det \begin{pmatrix} v_1 & w_1 \\ v_2 & w_2 \end{pmatrix} = 0$ 

Let $V = \lambda W$, which means $V$ and $W$ are linearly dependent $\iff$$v_1 = \lambda w_1$ and $v_2 = \lambda w_2$ $\iff$ $\lambda = v_1/w_1 = v_2/w_2$ $\iff$ $v_1w_2 = v_2w_1$ $\iff v_1w_2 - v_2w_1 = 0 \iff \det\begin{pmatrix} v_1 & w_1 \\ v_2 & w_2 \end{pmatrix} = 0$ 

#### Ex 12 Prove that if $\lambda, \mu$ are real eigenvalues of a $2 \times 2$ matrix, then any  nonzero column of the matrix $A - \lambda I$ is an eigenvector for $\mu$ 

let $A = \begin{pmatrix} a & b \\ c & d \end{pmatrix}$ , since $\lambda, \mu$ are eigenvalues, 

The characteristic polynomial: $x^2 - (a+d)x - (ad -bc)$ 

We let $\lambda = \frac{(a+d)+\sqrt{(a+d)^2-4(ad-bc)}}{2}$

and $\mu =$ $\frac{(a+d)-\sqrt{(a+d)^2-4(ad-bc)}}{2}$  without loss of generality.

Let's take the column vector from $A - \lambda I$, $\begin{pmatrix} a- \lambda \\ c \end{pmatrix}$ and multiply $A - \mu I$ by this vector.

We get $\begin{pmatrix} a-\lambda& b \\ c & d-\lambda \end{pmatrix} \begin{pmatrix} a - \mu \\ c \end{pmatrix}$  = $\begin{pmatrix} (a-\lambda)(a-\mu) +bc \\ c(a+d -(\mu + \lambda)) \end{pmatrix}$ 

If we prove this is equal to the 0 vector, then $\begin{pmatrix} a- \lambda \\ c \end{pmatrix}$is an eigenvector, provided $\mu \neq a$ and $c \neq 0$ 

$(a-\lambda)(a-\mu)=$ $a^2 -a(\lambda +\mu) - \lambda\mu$ 

$(\lambda + \mu) = $$(a+d)$, so the second entry of the vector is $= c(a+d - (a+d)) = 0$ 

and $\lambda\mu=$$((a+d)^2 - (a+d)^2 + 4(ad-bc))/4 = ad-bc$ 

So $(a-\lambda)(a-\mu) = a^2 -a^2 -ad +ad -bc = -bc$, 

so: $\begin{pmatrix} (a-\lambda)(a-\mu) +bc \\ c(a-\mu + d - \lambda) \end{pmatrix}$ = $\begin{pmatrix} 0 \\ 0 \end{pmatrix}$ 

So now we prove the other column vector is an eigenvector in the same way:

$\begin{pmatrix} a-\lambda& b \\ c & d-\lambda \end{pmatrix} \begin{pmatrix} b \\ d-\mu \end{pmatrix}$ = $\begin{pmatrix} b(a+d - (\lambda + \mu)) \\ bc + (d-\lambda)(d-\mu) \end{pmatrix}$ 

From earlier, we know $b(a+d - \lambda - \mu) = 0$ 

and replacing $(d-\lambda)(d-\mu) = d^2 -ad - d^2 + ad - bc = -bc$, 

so: $\begin{pmatrix} (a-\lambda)(a-\mu) +bc \\ c(a-\mu + d - \lambda) \end{pmatrix} = \begin{pmatrix} 0 \\ 0 \end{pmatrix}$

As long as $\mu \neq d$ and $b\neq 0$, the vector $\begin{pmatrix} b \\ d - \mu \end{pmatrix}$ is an eigenvector

#### Ex 14 Prove that the eigenvectors of a $2 \times 2$ matrix corresponding to distinct real eigenvalues are always linearly independent. 

Let $A$ be a $2 \times 2$ matrix with $2$ eigenvalues: $\lambda, \mu$ where $\lambda \neq \mu$ let $v_\lambda$ and $v_\mu$ be the (nonzero) eigenvectors corresponding to $\lambda$ and $\mu$ respectively. 

Suppose $v_\lambda$ and $v_\mu$ are linearly dependent $\implies v_\lambda = cv_\mu$ for some constant $c \in \R\setminus {0}$, since both vectors must be nonzero. 

$Av_\lambda = \lambda v_\lambda = \lambda(cv_\mu)$

$A(cv_\mu) = \mu(cv_\mu)$

equating the two: $\lambda(cv_\mu) = \mu(cv_\mu)$ 

$\lambda(cv_\mu) - \mu(cv_\mu) = 0 \equiv (\lambda - \mu)(cv_\mu) = 0$

which means, since $cv_\mu$ is nonzero, $\lambda - \mu = 0$, a contradiction. So these two eigenvectors must be linearly independent. 