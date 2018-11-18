Renee Senining

Math 123

### Homework #8

Chapter 8, Exercises 1 and 2

##### 1. For each of the following nonlinear systems

a. Find all of the equilibrium points and describe the behavior of the associated linearized system

b. Describe the phase portrait for the nonlinear system

c. Does the linearized system accurately describe the local behavior near the equilibrium points?

###### (i) $x' = \sin x, y' = \cos y$ 

$(x', y') = F(x,y) = (\sin x, \cos y)$ 

1. Finding equilibrium points:

   $F(x,y) = (0,0)$ when $\sin x = 0, \cos y = 0$ 

   $\sin x = 0$ whenever $x = 2\pi k, \pi + 2\pi k$, for $k \in \Z$  

   $\cos y = 0$ whenever $ y = -\frac{\pi}2 + 2\pi k, \frac{\pi}2 + 2\pi k$ , $k \in \Z$

2. Describe the behavior of the associated linearized system

   $DF_{X_0} = (\frac{\partial f_i}{\partial x_j})$ , so we have $DF_{X_0} = \begin{pmatrix} \cos x_0 & 0 \\ 0 & -\sin y_0\end{pmatrix}$, the Jacobian matrix of $X$ evaluated at $X_0$ 

   We have: $(2\pi k_1, \pi/2 + 2\pi k_2), (2\pi k_1, -\pi/2 + 2\pi k_2), (\pi + 2\pi k_1,  \pi/2 + 2\pi k_2), (\pi + 2\pi k_1, -\pi/2 + 2\pi k_2)$ as equilibrium points, where $k_1, k_2 \in \Z$ 

   So $DF_{X_0}$ for each of these points respectively are

   $\begin{pmatrix} 1 & 0 \\ 0 & -1\end{pmatrix}$, $\begin{pmatrix} 1 & 0 \\ 0 & 1\end{pmatrix}$, $\begin{pmatrix} -1 & 0 \\ 0 & -1 \end{pmatrix}$, $\begin{pmatrix} -1 & 0 \\ 0 & 1 \end{pmatrix}$

   So it seems we have saddles at 

   1. $(2\pi k_1, \pi/2 + 2\pi k_2)$
      1. The stable line being the $y$-axis around this point
      2. The unstable line being the horizontal line near the point and through $\pi/2 + 2\pi k_2$ 
   2. $(\pi + 2\pi k_1, -\pi/2 + 2\pi k_2)$
      1. the stable line is the horizontal line through $-\pi/2 + 2\pi k_2$ near the point
      2. The unstable line is the vertical line through $\pi + 2\pi k_1$ near the point 

   and a source at $(2\pi k_1, -\pi/2 + 2\pi k_2)$, and a sink at $(\pi + 2\pi k_1, \pi/2 + 2\pi k_2)$ 

3. Describe the phase portrait for the nonlinear system

   1. Using the intervals at which $\sin x, \cos y$ are positive, negative:
   2. Whenever $x \in (2\pi k, \pi + 2\pi k)$, $k \in \Z$ solutions move to the right, and whenever $x \in (\pi + 2\pi k, 2\pi (k+1))$ solutions move to the left
   3. Whenever $y \in (-\pi/2 + 2\pi k, \pi/2 + 2\pi k)$, solutions move up, and whenever $y \in (\pi/2 + 2\pi k, 3\pi/2 + 2\pi k)$, solutions move down 
   4. also in the upper half plane, fixing $y = \pi/2 + 2\pi k$ for some integer $k$, whenever $x = \pi m$, we have (locally) a saddle (m is even) or a sink, (m is odd)
   5. In the lower half plane, fixing $y = -\pi/2 + 2\pi k$ for some integer $k$, whenever $x = \pi m$, we have (locally) a source (m is even) or a saddle (m is odd)
   6. It appears that all solutions tend towards some equilibrium point, since
      1. for $x'$, 
         1. if $\sin x > 0$, $x$ must be in $(2\pi k, \pi + 2\pi k)$, and continues to increase towards $\pi$ since $x$ is continuous and $\sin x$ is continuous and positive in this interval, and as $x \rightarrow \pi + 2\pi k$, $\sin x \rightarrow 0$ , 
         2. if $\sin x = 0$, we are done
         3. if $\sin x < 0$, $x$ must be in $(\pi + 2\pi k, 2\pi + 2\pi k)$, and continues to decrease towards $\pi + 2\pi k$ since, again, $x$ is continuous and $\sin x$ is continuous and negative in this interval, and as $x \rightarrow \pi + 2\pi k$, $\sin x \rightarrow 0$ 
      2. for $y'$, we can make the same arguments as above, with the intervals $(-\pi/2 + 2\pi k, \pi/2 + 2\pi k)$ and $(\pi/2 + 2\pi k, 3\pi/2 + 2\pi k)$, to show that all solutions move towards an equilibrium point

4. Does the linearized system accurately describe the local behavior near the equilibrium points?

   1. Yes, since the linearized system at each equilibrium point is hyperbolic. (The Linearization Theorem)

###### (ii) $x' = x(x^2 + y^2)$, $y' = y(x^2 + y^2)$ 

In polar coordinates:

$x' = (r\cos \theta)' = r'\cos \theta -r(\sin\theta)\theta' = r^3 \cos \theta$

$y' = (r\sin \theta)' = r' \sin \theta + r(\cos \theta)\theta' = r^3 \sin \theta$

$\implies$

$r' = r^3$

$\theta' = 0$ 

1. Finding equilibrium points:
   1. Know we have one at $(0,0)$
   2. $x' = 0$ when $x^3 + xy^2 = 0$ 
      1. $x^3 = -xy^2$
      2. if $x \neq 0$, we arrive at a contradiction:
         1. if $x < 0$ $\implies$ $x^3 < 0$, but $-xy^2 > 0$ 
   3. Trying to find an equilibrium point where $y\neq 0$ gives $y^3 = -yx^2$, which gives a similar contradiction as above.
   4. Alternatively, easy to see that for any nonzero $r$, $r' \neq 0$
      1. if $r > 0$, $r' > 0$
      2. if $r < 0$, $r' < 0$ 
   5. The only equilibrium point is $(0,0)$ 
2. Describing the behavior of the associated linearized system
   1. $DF_X = \begin{pmatrix} 3x^2 + y^2 & 2yx \\ 2xy & 3y^2 + x^2\end{pmatrix}$
   2. Since the equilibrium point is $(0,0)$, we drop all nonlinear terms and get the system
   3. $X' = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}X$ 
   4. every point is an equilibrium point
3. Describe the phase portrait of the nonlinear system
   1. straight rays are invariant: all solutions that start on a straight ray stay on that ray since $\theta' = 0$ 
   2. all solutions move away from origin, except for the equilibrium point at the origin
      1. for any 
4. No: no matter how close we get to origin, we will always find solutions moving away from the origin, since for any $r \neq 0$, $r' \neq  0$, when $r < 1$, $r$ increases slowly at first then faster. This is due to the linearized system at the equilibrium point being nonhyperbolic

###### (iii) $x' = x + y^2, y' = 2y$

1.  Finding equilibrium points
   1. $y' = 2y = 0$ if and only if $y = 0$ 
   2. so $x' = x + (0)^2 = 0$ iff $x = 0$ 
   3. Our only equilibrium point is $(0,0)$
2. Describe the behavior of the associated linearized system
   1. $DF_{X} = \begin{pmatrix} 1 & 2y \\ 0 & 2 \end{pmatrix}$ 
   2. Near equilibrium point $(0,0)$ : $DF_{0} = \begin{pmatrix} 1 & 0 \\0 & 2 \end{pmatrix}$ 
   3. We have a source near equilibrium, with all solutions eventually tending away from origin tangent to the $y-$axis 
3. Describe the phase portrait for the nonlinear system
   1. for solutions starting at point $(x_0, 0)$ for some $x_0 \in \R$
      1. these solutions stay on the $x-$axis (invariant)
      2. and depending on the sign of $x$:
         1. if $x > 0$, solution moves to the right
         2. $x < 0$, solution moves to the left
   2. if $y_0 \neq 0$, 
      1. if $y < 0$, $y$ continues to decrease and solutions move down
      2. if $y > 0$, $y$ continues to increase and solutions move up
      3. No matter what $x$ is, eventually the solution will keep moving right
         1. obvious for $x \geq 0$, since $x' > 0$ making $x > 0$ 
         2. even if $x < 0$, $y^2$ grows faster than $|x|$, so eventually, $y^2 > |x|$ and $x' > 0$
      4. Finding the flow of the nonlinear system
         1. $y = y_0e^{2t}$ $x_h(t) = \alpha e^t$ 
         2. $x_p(t) = \beta e^{4t}$
         3. $x_p'(t) = 4\beta e^{4t} = \beta e^{4t} + y_0^2 e^{4t}$
         4. $\beta = \frac{y_0^2}{3}$
         5. $x(t) = (x_0 - \frac{y_0^2}{3}) e^t + \frac{y_0^2}{3} e^{4t} $ 
      5. $x(t) = (x_0 - \frac{y_0^2}3)e^t + \frac{y_0^2}{3}e^{3t}e^t = (x_0 -\frac{y_0^2}{3} + \frac{y_0^2}{3}e^{3t})e^t$ 
         1. and $x_0 - \frac{y_0^2}{3} + \frac{y_0^2}{3}e^{3t} \rightarrow +\infin$ as $ t\rightarrow +\infin$, since $e^{3t}$ grows without bound 
         2. so $x(t) \rightarrow + \infin$ 
   3. $\frac{dy}{dx} = \frac{2y_0 e^{2t}}{(x_0 - y_0^2/3)e^t + (4y_0^2/3)e^{4t}}$ $= \frac{2y_0}{(x_0 - y_0^2/3)e^{-t} + (4y_0^2/3)e^{2t}}$ and as $ t\rightarrow \infin$, $\frac{dy}{dx} \rightarrow 0$, 
      1. so the solutions move away from origin tangentially to the $x-$axis 

4. The linearized system accurately describes the local behavior near the equilibrium point at origin in an appropriately small neighborhood of origin: solutions tend away towards origin and in a really small neighborhood, the term in $x(t)$, $(y_0^2/3)(e^{4t}-e^t)$ will be really small, and $x(t)$ will look more like $x_0e^t$. Also, since the linearized system is hyperbolic, the linearization theorem states that the nonlinear flow is conjugate to the flow of the linearized system in a neighborhood of $X_0$

###### (iv) $x' = y^2, y' = y$ 

1. Find equilibrium points
   1. equilibrium points: $(x, 0)$, for any $x \in \R$ 
2. Describe the behavior of the associated linearized system
   1. $DF_{(x,0)} = \begin{pmatrix} 0 & 0 \\ 0 & 1\end{pmatrix}$ (note this is for any $x$)
   2. every point on the $x-$axis is an equilibrium point
   3. $X(t) = \begin{pmatrix} x_0 \\ 0 \end{pmatrix} + \begin{pmatrix} 0 \\y_0 \end{pmatrix}e^t$ 
      1. $x(t) = x_0 , y(t) = y_0e^t$  
   4. vertical lines are invariant, since $x'(t) = 0$ for all $t$
   5. and if $y_0 < 0$, the solution moves down, if $y_0 > 0$, the solution moves up as $ t\rightarrow \infin$ 
3. The phase portrait for the nonlinear system:
   1. all points $(x,0)$ are equilibrium points
   2. all solutions move to the right as long as $y \neq 0$:
      1. $x' = y^2 > 0$, so $x$ is always increasing
   3. in the upper plane, solutions move up and to the right initially, but $y$ is always positive since $y' = y > 0$ is always increasing, and as $y$ increases, $y^2 \rightarrow \infin$ faster than $y \rightarrow \infin$, so eventually all solutions will tend tangentially to the $x$-axis
   4. In the lower plane, solutions move down and to the right initially, but for the same reason as above, ($y < 0$, so $y'$ is decreasing, so $y^2$ is increasing towards $\infin$) all solutions will tend tangentially to the $x$-axis as $t\rightarrow \infin$ 
4. Does the linearized system accurately describe the local behavior near the equilibrium points?
   1. We still have equilibrium points on the $x$-axis in either system
   2. and solutions in the upper/lower move away from the $x$-axis in both systems similarly in a small neighborhood (up/down away from $x$-axis)
   3. and in a small enough neighborhood, $y^2$ will be really small so $x$ won't change much, but $y' = y$ is still the same as in the linear system, so the solutions look similar in both linear and nonlinear systems in a really small neighborhood
   4. Being picky, the difference is that as long as $y \neq 0$, the solution will begin to curve towards the right as $t$ increases, although it seems that it could be possible to find a neighborhood small enough that the curves look like vertical lines.

##### (v) $x' = x^2, y' = y^2$

1. Find equilibrium points
   1. $x^2 = 0, y^2 = 0$, so the only equilibrium is $(0,0)$ 
2. Describe the behavior of the associated linearized system
   1. $DF_0 = \begin{pmatrix} 0 & 0 \\ 0 & 0 \end{pmatrix}$
   2. every point is an equilibrium point
3. Describe the phase portrait for the nonlinear system
   1. $x' > 0$, $y' > 0$ for all $x, y \in \R\setminus${$0$}, solutions are always increasing if
   2. when $x = y$, $x' = y'$, so $x,y$ are increasing at the same rate and remain equal
      1. the line $y = x$ is invariant
   3. solutions on the $x$ or $y$ axes stay on the $x$ or $y$ axes
      1. $x \neq 0$, $y = 0$, then $x' > 0$, $y' = 0$ and vice versa
      2. solutions on the $x$-axis move to the right
      3. solutions on the $y$-axis move up
   4. Starting within a reasonable neighborhood around origin, 
      1. solutions in the 4th quadrant (lower right) will always tend away from origin tangentially to the $x-$ axis
         1. $x > 0$, $x' > 0$, $x \rightarrow \infin$
         2. $y < 0$, $y' > 0$, $y \rightarrow 0$, $y' \rightarrow 0$ 
      2. solutions in the 3rd quadrant (lower left) will always tend towards origin.
         1. $y < 0$, but $y' > 0$, so $y \rightarrow 0$ and $y' \rightarrow 0$, 
         2. also, $x < 0$, $x' > 0$, $x\rightarrow 0$, $x' \rightarrow 0$  
      3. solutions in the 2nd quadrant (upper left) will tend away from origin tangentially to the $y$-axis 
      4. solutions in the 1st quadrant (upper right)
         1. will tend away from origin tangentially to the $y-$axis if $x$ is small enough
         2. will stay on $y = x$ if it starts on $y = x$ 
         3. will tend away from origin tangentially to the $x-$ axis if $x$ is large enough
4. Does the linearized system accurately describe the local behavior near equilibrium points?
   1. No, the linear system has equilibrium points everywhere
   2. but in the nonlinear system, we have in any neighborhood of origin
      1. if $x \neq 0$, $y = 0$, no matter how small $x$ is, the solution moves to the right
      2. if $x = 0, y \neq 0$, solutions move up 
      3. basically as long as $x, y \neq 0$, they won't be an equilibrium point and that is not shown in the linearized system

##### 2. Find the global change of coordinates that linearizes the system

$x' = x + y^2 \\ y' = -y \\ z' = -z + y^2$

$y(t) = y_0 e^{-t}$

$y^2 = y_0^2 e^{-2t}$ 

Solving for $x(t)$:

$x_h(t) = \alpha e^t$, homogeneous

$x_p(t) = \beta e^{-2t}$, particular solution

$x'_p(t)  =-2\beta e^{-2t} = \beta e^{-2t} + y_0^2e^{-2t}$ 

$x_p'(t) = -3\beta e^{-2t} = y_0^2 e^{-2t}$ 

$\beta = -\frac{y_0^2}{3}$

$\alpha = x_0 + \frac{y_0^2}{3}$

$x(t) = (x_0 + \frac{y_0^2}{3})e^t -\frac{y_0^2}{3}e^{-2t}$ 

Solving for $z(t)$:

$z_h(t) = \alpha e^{-t}$

$z_p(t) = \beta e^{-2t}$

$z_p'(t) = -2\beta e^{-2t} = -\beta e^{-2t} + y_0^2 e^{-2t}$

$-\beta e^{-2t} = y_0^2 e^{-2t}$

$\beta = -y_0^2$ $\implies z_p(t) = -y_0^2e^{-2t}$ 

$\alpha + \beta = \alpha -y_0^2 = z_0$, $\alpha = z_0 + y_0^2$ 

$z(t) = (z_0 + y_0^2)e^{-t} - y_0^2 e^{-2t} = z_h(t) + z_p(t)$ 

for an equilibrium point:

$x' = 0 \implies x + y^2 = 0$

$y' = 0 \implies -y = 0 \implies x = 0$ 

$z' = 0 \implies -z + y^2 = 0 \implies -z = 0$

our only equilibrium point is origin

So:

lines on the $y -$ axis are going to tend towards the equilibrium point

since $y_0 e^{-t} \rightarrow 0$

and similarly, lines on the $z-$axis are going to tend towards the equilibrium point

$e^{-t}, e^{-2t} \rightarrow 0$, and so $z(t) \rightarrow 0$ 

$x(t)$ however is going to blow up unless $x_0 + \frac{y_0 ^2}{3} = 0$

then for any $(x_0, y_0)$ satisfying $x_0 + \frac{y_0^2}{3} = 0$

we have $x(t) = -\frac{y_0^2}{3}e^{-2t}$$= -y^2/3$ for all of $t$ 

$y(t) = y_0e^{-t}$ 

so all solutions with initial conditions on the curve $x + y^2/3 = 0$ will remain on the curve for all time and tend towards origin as $ t \rightarrow \infin$ 

Similarly:

$z_0+ y_0^2 = 0$

$z(t) = -y_0^2e^{-2t} \equiv z + y^2 = 0$

so all solutions starting on $z+y^2 = 0$ will remain on the curve for all time and tend towards origin since $z(t) -y_0^2e^{-2t} \rightarrow 0$ $t\rightarrow \infin$ 

$y(t) \rightarrow 0$ as $t \rightarrow \infin$ 

so introducing $u, v, w$ variables

$u = x + y^2/3$

$v = y$

$w = z + y^2$ 

so the system becomes in these new coordinates:

$u' = \frac{\partial u}{\partial x}\frac{\partial x}{\partial t} + \frac{\partial u}{\partial y}\frac{\partial y}{\partial t} = x' + 2yy'/3 = x + y^2 -2y^2/3 = x + \frac{1}{3}y^2 = u$ 

$v' = y' = -y = -v$

$w' = z' +2yy' = -z+y^2 -2y^2 = -(z + y^2) = -w$ 

the change of variables

$\Phi(x,y,z) = (x+\frac{y^2}{3}, y, z + y^2)​$ 



