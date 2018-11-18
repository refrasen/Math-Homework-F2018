Renee Senining

Math 123

##### 4. Consider the system $x' = \sin x(-0.1\cos x - \cos y) \\ y' = \sin y (\cos x - 0.1 \cos y)$ 

Show that all solutions emanating from the source at $(\pi/2, \pi/2)$ have $\omega$-limit sets equal to the square bounded by $x = 0$, $\pi$ and $y = 0, \pi$ 

---

$x' = -0.1\sin x\cos x - \sin x \cos y$

$y' = \sin y\cos x - 0.1 \sin y \cos y$ 

$DF_X = \begin{pmatrix} -0.1\cos^2x + 0.1 \sin^2x - \cos x\cos y & \sin x \sin y \\ -\sin y\sin x& -0.1\cos^2 y + 0.1 \sin^2 y + \cos y \cos x   \end{pmatrix}$ 

The linearized system at $X_0 = (\pi/2, \pi/2)$ is

$\begin{pmatrix} 0.1 & 1 \\ -1 & 0.1\end{pmatrix}$

our equilibrium point has a real part $\alpha = 0.1$ and imaginary $\beta = \pm1$, so we have a spiral source, and since this is a hyperbolic system, solutions tend away from this equilibrium point.

On the square, we have heteroclinic solutions, and since the system is $C^1$, solutions are unique, so no solutions from within the square can cross out of the square.

$V = \frac{1}{\sin x \sin y}$ , not defined on the boundary of $Q$ = {$(x,y): 0 < x,y < \pi$} 

$\dot V = -\frac{x'\cos x \sin y }{(\sin x \sin y)^2} - \frac{y' \sin x \cos y}{(\sin x \sin y)^2}$

$= \frac{\cos x \sin y \sin x(0.1 \cos x + \cos y)}{(\sin x \sin y)^2} - \frac{\sin x \cos y \sin y(\cos x - 0.1 \cos y)}{(\sin x \sin y)^2}$

$= \frac{\sin y \sin x}{(\sin x \sin y)^2}[\cos x (0.1 \cos x + \cos y) - \cos y (\cos x -0.1\cos y)]$ 

$\frac{\sin y \sin x}{(\sin x \sin y)^2} > 0$ in $Q$

$\cos x (0.1 \cos x + \cos y) - \cos y (\cos x - 0.1 \cos y) =$

$0.1 \cos^2x + 0.1 \cos^2 y > 0$ for all $(x, y) \in Q$ except at $x = y = \pi/2$ 

so $\dot V > 0$ in $Q$ except at $(\pi/2, \pi/2)$ 

and $V > 0$ for all $(x,y) \in Q$ , so following $V$ along any solution curve emanating from the source at $(\pi/2, \pi/2)$, we have $V$ is strictly increasing (as long as the solution stays in $Q$)

if we had a closed orbit ($\in Q$), and therefore a periodic solution, then 

for some solution with $X(t) = (x(t), y(t))$ with $(x_0, y_0) \neq (\pi/2, \pi/2)$ 

$X(0) = (x_0, y_0) = X(T)$

so at $t = 0$ and $t = T$, $V$ would have the same value, but $V$ is strictly increasing in $Q$, so this isn't possible

Using Generalized Poincare-Bendixson Theorem:

with $\mathcal{M} $ being $Q \cup$ the boundary of $Q$, which is compact invariant since

1. it is closed and bounded in $\R^2$
2. solutions on the boundary are invariant, and no solutions emanating from the source within the square can cross the boundary due to uniqueness of solutions

and we only have $5$ equilibria in this set for the system above.

$\omega(X)$ must be 

(1) an equilibrium (we have multiple equilibrium), 

(2) a closed orbit (we have none of these), or 

(3) multiple equilibria $X_1, . . ., X_n$  and regular orbits such that if $\gamma \sub \omega(X)$, then $\omega(\gamma) = X_i$ and $\omega(\gamma) = X_j$ for some $1 \leq i, j \leq n$

As noted earlier, there are no closed orbits

and the only equilibrium that a solution $X​$ emanating from the source can tend to is one on the boundary of the square, meaning its limit point is on the square

Otherwise, it converges to the square which satisfies (3)