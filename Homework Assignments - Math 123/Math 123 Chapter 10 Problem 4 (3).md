# Math 123 Chapter 10 Problem 4

##### 4. Consider the system $x' = \sin x(-0.1\cos x - \cos y) \\ y' = \sin y (\cos x - 0.1 \cos y)$ 

Show that all solutions emanating from the source at $(\pi/2, \pi/2)$ have $\omega$-limit sets equal to the square bounded by $x = 0$, $\pi$ and $y = 0, \pi$ 

---

Obviously, there are no equilibrium points other than $(\pi/2, \pi/2)$ within the square (not including the boundary)

Suppose there is an $\omega$ set that is not the boundary of the square for some $X$ in the square (not including the boundary, particularly near $(\pi/2, \pi/2)$)

$\omega$ is closed and invariant (proof done in class)

and bounded by the square's boundaries (solutions cannot cross the heteroclinic solutions due to uniqueness of solutions; $F(X)$ is smooth)

since the only equilibrium point in the square (excluding the boundary) is a source, there are no equilibrium points in $\omega$ 

by the Poincare-Bendixson theorem, $\omega$ must be a closed orbit

but there is no closed orbit inside the square:

suppose there exists a solution $X(t)$ such that for some $T > 0$ ,$X(T) = X(0)$

with $X(0)$ within the square

let $L = \sin x \sin y$

$L> 0$ in the square, $L = 0$ only on the square's boundary

$\dot L = x'\cos x \sin y + y'\sin x \cos y$

$\dot L = \sin x \sin y \cos x(-0.1 \cos x - \cos y ) + \sin x \sin y \cos y (\cos x - 0.1 \cos y)$

$= -0.1(\sin x \sin y \cos^2 x + \sin x \sin y \cos^2 y)$

$ = -0.1\sin x \sin y(\cos^2 x + \cos^2 y)$

since $\sin x \sin y \geq 0$ (0 on the square) and $\cos^2 x + \cos^2 y > 0$

$\dot L < 0$ in the square

but we also have

$0 = L(X(T)) - L(X(0)) = \int_0^T \dot L dt$

but the integral must be strictly smaller than $0$ since $\dot L < 0​$, a contradiction

