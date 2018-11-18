Renee Senining

Math 123

### Homework #11

#### 2, 10, 11, 15, 16

##### 2. Consider the three-dimensional system $r' = r(1-r) \\ \theta' = 1 \\ z' = -z$ 

Compute the Poincare map along the closed orbit lying on the unit circle given by $r = 1$ and show that this is asymptotically stable

---

if $z > 0$, $z' < 0$, 

and if $z < 0$, $z' > 0$ 

and if $z = 0, z' = 0$ 

so $z \rightarrow 0$ 

the closed orbit is given by $(\cos t, \sin t, 0)$, with initial condition $(1,0, 0)$

There is a local section lying along the half $xz-plane$ with $x > 0$, 

since $\theta ' = 1$ 

given any $x \in (0, \infin)$, $z \in (-\infin, \infin)$ 

$\theta_{2\pi}(x, 0, z)$ also lies in the half plane as described above.

so we have a Poincare map $P: \R^+ \times \R \rightarrow \R^+ \times \R$

$P(1, 0) = (1, 0)$ since the point $x = 1, y =0, z = 0$ is the initial condition for the periodic solution 

Finding $P$:

compute the solution starting at $(x_0, 0, z_0)$ 

$\theta(t) = t$ 

$\int \frac{dr}{r(1-r)} = t + C$

$\frac{1}{r(1-r)} = \frac{1}{r} + \frac{1}{1-r}$ 

so $\int\frac{dr}{r(1-r)} = \log(r) - \log(1-r)$ $= t + C$ 

$\equiv$ $\log(\frac{r}{1-r}) = t + C$

$\frac{r}{1-r} = Ce^{t}$ 

$r = Ce^t - rCe^t$ 

$r(1 + Ce^t) = Ce^t$ 

$r = \frac{Ce^t}{1+Ce^t}$ 

and $r(0) = \frac{C}{1+C} = x_0$

so $C = x_0(1+C)$

$C(1 - x_0) = x_0$ $\implies$ $C = \frac{x_0}{1-x_0}$ 

$r = \frac{x_0e^t}{1-x_0 + x_0e^t}$ 

and $z = z_0e^{-t}$ 

$r(2\pi) = \frac{x_0e^{2\pi}}{1 - x_0 + x_0e^{2\pi}}$ 

$z(2\pi) = z_0e^{-2\pi}$ 

so $P(x_0, z_0) = (r(2\pi), z(2\pi))$ 

$\frac{d}{dx}[r(2\pi)] = \frac{e^{2\pi}(1-x+xe^{2\pi}) - (e^{2\pi}-1)xe^{2\pi}}{(1-x+xe^{2\pi})^2}$

$= \frac{e^{2\pi }}{(1-x + xe^{2\pi})^2}$

$\frac{d}{dz}z(2\pi) = e^{-2\pi}$ 

$\nabla P(1, 0) = (e^{-2\pi}, e^{-2\pi})$

the max value of $P'(1, 0)$ 

$||\nabla P|| =  2e^{-4\pi} < 1$

so the closed orbit is AS by the proposition 219

##### 10. Show that a closed orbit of a planar system meets a local section in at most one point

Suppose $Y_1$ and $Y_2$ are distinct points on the closed orbit, $\gamma$ 

and $\mathcal{S}$ is a local section containing $Y_1$ and $Y_2$ 

we have that a closed orbit is the $\omega$-limit set for every point on it

so for any $X \in \gamma$, $\omega(X)$ contains $Y_1$ and $Y_2$ 

let $\mathcal{V}_k$ be the flow boxes at $Y_k$, which are defined by disjoint intervals $\mathcal{J}_k$ in the local section $\mathcal{S}$ 

(since $Y_1, Y_2$ are disjoint, we can find disjoint neighborhoods around these two points that contain disjoint segments of $\mathcal{S}$)

Since closed orbits are periodic, 

solutions on the closed orbit enter each flow box infinitely often, crossing $\mathcal{J}_k$ infinitely 

so there exists a sequence $a_1, b_1, a_2, b_2, a_3, b_3 $  that is monotone along the solution through $X$ with $a_n \in \mathcal{J}_1$ and $b_n \in \mathcal{J}_2$ for $n \in \N$ 

but this sequence isn't monotone along $\mathcal{S}$  since $\mathcal{J_1}, \mathcal{J_2}$ are disjoint 

so this contradicts the proposition on 221

##### 11. Show that a closed and bounded limit set is connected (that is, not the union of two disjoint nonempty closed sets)

so consider the limit set $\omega(X)$ for a solution curve passing through $X$

Suppose $\omega(X)$ is disconnected

let $S_1$ and $S_2$ be disjoint open sets s.t. $\omega(X) \sub S_1\cup S_2$

and $\omega(X) \cap S_k$ is nonempty $k = 1, 2$ 

Let $Y_1 \in S_1$ and $Y_2 \in S_2$ 

so there exists a sequence of $t_n \rightarrow \infin$ such that

$\lim_{n\rightarrow \infin}\phi_{t_n}(X) = Y_1$

and a sequence $s_n \rightarrow \infin$ such that

$\lim_{n \rightarrow \infin} \phi_{s_n}(X) = Y_2$ 

and $t_n < s_n < t_{n+1}$ (possibly for some subsequence)

since: for each $1/n$, $n \in \N$ 

we can find indices $N_1(n), N_2(n)$

s.t. for all $n \geq N_1(n)$, $|\phi_{t_n}(X) - Y_1| < 1/n$ 

for all $n \geq N_2(n)$, $|\phi_{s_n}(X) - Y_2| < 1/n$

and defining subsequences:

for each $k $: let $t_k = N_1(k)$ , and $s_k = N_2(k)$ if $N_2(k) > N_1(k)$ or let $s_k = $ some integer $ > N_1(k) \geq N_2(k)$, then let $t_{k+1} = $ an integer greater than $s_k$ and greater than or equal to $N_1(k+1)$. We continue like this and obtain:

1.  $|\phi_{t_k}(X) - Y_1| < 1/k$, $|\phi_{s_k}(X) - Y_2| < 1/k$, so as $k \rightarrow \infin$, $t_k, s_k \rightarrow \infin$ $\phi_{t_k}(X) \rightarrow Y_1$, $\phi_{s_k}(X) \rightarrow Y_2$ 
2. $t_k < s_k < t_{k+1}$ 

---

there exists an $N_1 \in \N$ s.t. 

for all $n \geq N_1$, $\phi_{t_n}(X) \in \mathcal{S_1}$ since $\phi_{t_n}(X) \rightarrow Y_1$, and $S_1$ is open and $Y_1 \in S_1$ (i.e. there is an open ball centered on $Y_1$ contained in $S_1$ and since the terms of $\phi_{t_n}$ get arbitrarily close to $Y_1$, there are infinitely many terms of $\phi_{t_n}$ contained in any ball centered on $Y_1$)

and similarly, there exists an $N_2 \in \N$  s.t.

for all $n \geq N_2$, $\phi_{s_n}(X) \in \mathcal{S_2}$ 

so let $N_0 = \max(N_1, N_2)$

for all $n \geq N_0$, 

$\phi_t(X)$ with $t \in (t_n, s_n)$  is the part of the solution curve connecting a point in $ S_1$and a point in $S_2$, so $\exists r_n \in (t_n, s_n)$ s.t. $\phi_{r_n}(X) \notin S_1\cup S_2$ (since they are disjoint)

and so we have a sequence $r_n \rightarrow \infin$  as $ n\rightarrow \infin$ 

if $\phi_{r_n}(X)$ converges:

$\lim_{r_n \rightarrow \infin}\phi_{r_n}(X) = Z \in \omega(X)$ 

so for each open ball around $Z$, there are infinitely many terms of $\phi_{r_n}(X)$ in it

but since each $\phi_{r_n}(X) \notin S_1 \cup S_2$ and there exists an open ball centered on $Z$ fully contained in $S_1 \cup S_2$ since $\omega(X) \sub S_1 \cup S_2$ we have a contradiction since we would need infinitely many terms of $\phi_{r_n}(X)$ to be in this ball and therefore in $S_1 \cup S_2$ 

or $\lim_{r_n \rightarrow \infin}\phi_{r_n}(X) $ doesn't have a limit

then it is possible that

$\lim_{r_n \rightarrow \infin}\phi_{r_n}(X) \rightarrow \infin$, which means $\omega(X)$ is unbounded, a contradiction

or if the set {$\phi_{r_n}(X)$} is bounded, by the Bolzano-Weierstrass Theorem, it has a convergent subsequence, with a limit in $\omega(X)$ 

and we still have that each term is not in $S_1 \cup S_2$, but there are infinite terms in any open ball centered on the limit, but there is an open ball contained in $S_1 \cup S_2$, therefore we have a contradiction 

(a similar argument works for $\alpha(X)$, we simply consider limits with $t_n, s_n \rightarrow - \infin$ )

##### 15. Let $X$ be a recurrent point of a planar system; that is, there is a sequence $t_n \rightarrow \pm \infin$  such that $\phi_{t_n}(X) \rightarrow X$ 

##### (a) Prove that either $X$ is an equilibrium or $X$ lies on a closed orbit

so $X$ $\in \omega(X)$ and in $\alpha(X)$ 

and $\omega(X)$ is closed and invariant, which means $\phi_t(X) \in \omega(X)$ , $\alpha(X)$ for all $t \in \R$ 

so for any $Y$ lying on the solution curve through $X$, 

$\omega(Y) = \omega(X)$, $\alpha(Y) = \alpha(Y)  = \alpha(X)$, which means

$\exists s_n \rightarrow \pm \infin$ such that $\phi_{s_n}(Y) \rightarrow Y$

Assuming that there exists a point $Y$ on the solution curve with $Y \neq X$, i.e., $X$ is not an equilibrium:

Take any $Y$ on the solution curve and consider the local section $\mathcal{S}$ at $Y$. 

since $Y$ is a limit point of the solution through $X$, there are infinitely many points in time $s_n$ such that $\phi_{s_n}(X) \in $ the flow box $\mathcal{V}$. In particular, if $\phi_\tau(X) = Y$ at some time $\tau$, then there is some $s_N > \tau$ (if we're consider $s_N \rightarrow \infin$) or $s_N < \tau$, (if we're considering $s_N \rightarrow - \infin$ 

such that for all $n \geq N$, $\phi_{s_n}(X) \in \mathcal{V} $, which means that at infinitely many points in time, the solution curve goes into the flow box and crosses the local section at $Y$ 

since the entire solution curve is in $\omega(X)$, we have that the solution through $X$ crosses any local section at no more than one point, so the solution curve goes back through $Y$ infinitely many times for any point $Y$. 

Note, it isn't that multiple paths of the solution curve converging to cross through $Y$ else we'd have a local section such that the solution crosses it multiple times.

![1542148097281](C:\Users\Renee\AppData\Roaming\Typora\typora-user-images\1542148097281.png)

So, because the solution returns to each point more than once, there exists a time $t > 0$ s.t. $\phi_t(Y) = Y$ 

which means for any $s$, $\phi_s(Y)$, we have $\phi_{s+t}(Y) = \phi_{s}(Y)$ 

so the solution is a periodic function and thus a closed orbit

##### (b) Show by example that there can be a recurrent point for a nonplanar system that is not an equilibrium and does not lie on a closed orbit.

all points of the torus $T^2$ are recurrent with respect to an irrational flow:

![1542114419605](C:\Users\Renee\AppData\Roaming\Typora\typora-user-images\1542114419605.png)

The orbits are "dense", but not periodic.

projected on a two dimensional square:



![1542114908697](C:\Users\Renee\AppData\Roaming\Typora\typora-user-images\1542114908697.png)

where black lines are a first "lap," for lack of a better word, around and red lines are a second.

the system itself looks like

$\frac{d\theta_n}{dt} = \omega_n$, for $n = 1, 2, . . $ 

##### 16. Let $X' = F(X)$ and $X' = G(X)$ be planar systems. Suppose that $F(X)\cdot G(X) = 0$ for all $X \in \R^2$. If $F$ has a closed orbit, prove that $G$ has an equilibrium point

so $F(X) = (f_1(X), . . ., f_n(X))$, $G(X) = (g_1(X), . . ., g_n(X))$ 

$F(X)\cdot G(X) = f_1(X)g_1(X) + . . . + f_n(X)g_n(X) = 0$ 

so $F(X)\cdot G(X) = ||F(X)||||G(X)||\cos(\theta) = 0$

Assuming $F$ has a closed orbit $\gamma$ 

at each $X \in \gamma$, $F(X) \neq 0$ so we must have $G(X) = 0$  or $\theta =\frac{\pi}{2}$ 

if $G(X) = 0$ for some point, $G$ has an equilibrium on the closed path and we are done.

Otherwise: Suppose the angle between $F(X)$ and $G(X)$ is $\frac{\pi}{2}$ for all $X \in \gamma$ and $G(X) \neq 0$ 

this means that solutions of $G(X)$ emanate from or flow into $\gamma$ 

$\gamma$ can be divided into two sets, since $G(X)$ is never tangent with $\gamma$:

1. points on $\gamma$ such that $G(X)$ points out
2. points on $\gamma$ such that $G(X)$ points in

Suppose both are nonempty:

On a point $X$ of the boundary of either one, we must have that any neighborhood of $X$ must contain at least one point of each set. 

We consider a local section of $X$ and its flow box $\mathcal{V}$: (associated with $G$)

This vector $G(X)$ either points out from $\gamma$ or into $\gamma$, since the angle between $\gamma$ at $X$ and $G(X)$ is $\pi/2$, and so for each point $Y$ in the local section, $G(Y)$ points out from $\gamma$ if $G(X)$ points out or points in if $G(X)$ points in 

a part of $\gamma$ is contained in the flow box $\mathcal{V}$, since $\gamma$ is continuous and $\mathcal{V}$ is a neighborhood of $X$, so each point of $\gamma$ in the flow box must have its vector associated with $G$ going in the same direction as $G(X)$, so there is a neighborhood of $X$ s.t. all vectors of $\gamma$ associated with $G$ point in the same direction (out or in $\gamma$). This is a contradiction, so we must have that all vectors associated with $G$ on $\gamma$ point in one direction: in or out of $\gamma$ 

Let $K$ be a set containing the region bounded by $\gamma$ (assuming $\gamma$ is simple closed) and $\gamma$ 

So we either have that solutions to $X' = G(X)$ stay in $K$ or exit $K$, making $K$ positively or negative 

so $K$ contains either a limit cycle or an equilibrium point for $G(X)$ (Corollary 2)

If $K$ contains an equilibrium point, we are done.

Otherwise $K$ contains a limit cycle, $\beta$ for $X' = G(X)$, and by Corollary 4, there is an equilibrium point in the region bounded by the limit cycle



 





