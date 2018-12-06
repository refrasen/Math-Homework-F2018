Worksheet on Poincare-Bendixson

Theorem: Suppose $\omega(X)$ is compact (closed and bounded in $\R^n$ and contains no equilibrium point, Then $\omega(X)$ is a closed orbit)

## Part I: show that if $Y \in \omega(X)$ $\implies$ $O(Y)$ (orbit of Y) is closed

### Step I.1: Assume $Y \in \omega(X)$. Then $\omega(Y)$ is non-empty and $\omega(Y)$ $\sub \omega(X)$ Explain why

$Y \in \omega(X)$ $\implies$ 

$\exists$ a sequence of $t_n$ with $t_n \rightarrow \infin$  such that

$\lim_{t_n \rightarrow \infin} \phi_{t_n}(X) = Y$

since $\omega(X)$ is invariant, for any $Y \in \omega(X)$, $\phi_t(Y)$ is defined and in $\omega(X)$ for all $t$ 

and since $\omega(X)$ is closed, the limit of any sequence, which will be in $\omega(Y)$,  $\phi_{t_n}(Y) \in \omega(X)$

---

#### $\omega(X)$ is positively invariant:

How to show that if $Y \in \omega(X)$, then the solution through $Y$, $\phi_t(Y)$ is in $\omega(X)$ for all $t$?:

**First**: Continuous Dependence of solutions:

$\phi$ is a continuous function of $X$ $\implies$

for any $X_0$ $\in \R^n$, (fixing $t$ $\R$?) for any $\epsilon > 0$, $\exists \delta$, s.t. 

if $X$ satisfies $|X-X_0| <\delta$, then $\phi_t(X) \in (\phi_t(X_0) -\epsilon, \phi_t(X_0)+\epsilon)$ 

because

if $X(t)$, defined on [$t_0, t_1$] ($X(t_0) = X_0$) is a solution of $X' = F(X)$ where $F: \R^n \rightarrow \R^n$ is $C^1$, then there is a neighborhood $U \sub \R^n$ of $X_0$ and a constant $K$ such that if $Y_0 \in U$, then there is a unique solution $Y(t)$ also defined on [$t_0, t_1$] with $Y(t_0) = Y_0$

so we have

$|Y(t)-X(t)| \leq |Y_0 - X_0| \exp(K(t-t_0))$ 

so fixing $t = \tau$, and making $t_0 = 0$ 

$\exp(K(t-t_0)) = e^{K\tau}$ as the largest it gets from $[0, \tau]$ 

and if we make $|Y_0 - X_0|$ small enough, we can get

$|Y_0 -X_0|e^{K\tau} < \epsilon$ 

and therefore obtain $|\phi_t(Y) - \phi_t(X)| \leq |Y_0 - X_0|\exp(Kt) < \epsilon$ for all $t \in [0, \tau]$

so fix $t \in \R^+$, my aim is to show that there exists a sequence of $t_n$ $\rightarrow \infin$ s.t. $\phi_{t_n}(X) \rightarrow \phi_t(Y)$ 

i.e., for all $\epsilon > 0$, there exists a $N \geq 1$ s.t. for all $n \geq N$:

$|\phi_{t_n}(X) - \phi_t(Y)| < \epsilon$ 

So we know that there are infinitely many $s_n$ s.t.

$\phi_{s_n}(X)$ is arbitrarily near $Y$ 

so taking some $\phi_{s_k}(X)$ as an "$X_0$", 

we have: $|\phi_t(Y) - \phi_{t+s_k}(X)| \leq |Y-\phi_{s_k}(X)|\exp(Kt)$ 

since $\exp(Kt)$ is fixed, as $t$ is fixed (need to specify that I'm looking at a specific neighborhood of $Y$, so that $K$ is fixed, and we look at all $k$ s.t. $\phi_{s_k}(X)$ is in this neighborhood)

and because we know that $|Y- \phi_{s_k}(X)| \rightarrow 0$

$|\phi_t(Y)- \phi_{t+s_k}(X)| \rightarrow 0$

we define $t_k = t+s_k$ as a sequence $t_k \rightarrow \infin$ so that $\phi_{t_k}(X) \rightarrow \phi_t(Y)$ 

making $\phi_t(Y) \in \omega(X)$, and (we had to fix $t \in \R^+$ to use the continuous dependence theorem)

so we have positive invariance

---

#### $\omega(X)$ is closed:

if we were to take a sequence $Y_n$ $\in \omega(X)$, the limit would be some $Y \in \omega(X)$:

so let $t_n^k$ be the sequence for $X(t)$ st. $\lim_{t_n^k \rightarrow \infin} X_k(t_n) = Y_k$ 

for each $k$, $\exists$, $N(k)$ s.t.

$|X(t_n^k) - Y_k| < \frac{1}{k}$ for each $n \geq N(k)$ 

so we make a sequence:

$t_1 = t_{N(1)}^1$, so $|X(t_1) - Y_1| < 1$ 

and in general:

$t_k = \begin{cases} t^k_{N(k)} & t^k_{N(k)} > t_{k-1} \\ t_{k-1} + 1 & t^k_{N(k)} \leq t_{k-1}\end{cases}$

so we have:

for each $n$, $|X(t_n)-Y_n| < \frac{1}{n}$ 

and so for any $\epsilon > 0$, $\exists N_1 \geq 1$ s.t.

for all $n \geq N_1$, $|Y_n - Y| < \epsilon/2$ 

and $\exists N_2 \geq 1$ s.t. for all $n \geq N_2$, $|\frac{1}{n}| < \epsilon/2$ 

and there for, for all $n$, $|X(t_n) - Y_n| < \epsilon/2$ 

so $|X(t_n) - Y| \leq |X(t_n) - Y_n| + |Y_n - Y| < \epsilon$ 

so there exists a sequence of $t_n \rightarrow \infin$ such that $X(t_n) \rightarrow Y$  $\implies Y \in \omega(X)$ 

---

#### $\omega(X)$ is invariant

Using closed and positive invariance:

* Let $Y(t)$ be a solution with $Y(0) \in \omega(X)$, so $Y(t) \in \omega(X)$ for all $ t \geq 0$ 
* since $\omega(X)$ is closed, there is a sequence $t_n \rightarrow \infin$ and $Z \in \omega(X)$ s.t. $Y(t_n) \rightarrow Z$
* so $\phi_t(Y(t_n))$ is defined and in $\omega(X)$ for all $t \in [-t_n, t]$ 
* and since $t_n$ is an increasing sequence, $\phi_t(Y(t_{n+k}))$ is defined and in $\omega(X)$ for all $t \in [-t_n, t]$, $k \geq 0$ 
* so since $Y(t_{n+k}) \rightarrow Z$ as $k \rightarrow \infin$, from continuous dependence on initial conditions, because $\phi_t(Z)$ will get arbitrarily close to $\phi_t(Y(t_{n+k}))$, elements of $\omega(X)$, $\phi_t(Z)$ is defined and in $\omega(X)$ for all $t \in [-t_n, 0]$ 

### Step I.2 Let $Z \in \omega(Y)$, then $Z$ is not an equilibrium: Why?

if $Z$ $\in \omega(Y)$, which is in $\omega(X)$, if $Z$ is an equilibrium, then there is an equilibrium in $\omega(X)$, a contradiction.

### Step I.3 Let $\Sigma$ be a local section at $Z$ and denote by $V$ the flow box associated with $\Sigma$. Draw a picture and show that $O(Y)$ intersects $\Sigma$ at a single point

I'm gonna go ahead and assume $O(Y)$ is the solution curve passing through $Y$ 

since $Z \in \omega(Y)$, $O(Y)$ gets arbitrarily close to it infinitely many times

if there was another point, $Y_1$ on the solution curve $O(Y)$ that was on $\Sigma$, since $\omega(X)$ is invariant, $Y_1$ $\in \omega(X)$ and since $Z \in \omega(Y) \sub \omega(X)$, so is $Z$ 

this contradicts that a sequence that is monotone along the solution curve will be monotone along the local section since the solution goes back and forth along the local section between two disjoint neighborhoods/intervals

### Step I.4 Explain why the positive orbit of $Y$ must intersect $\Sigma$ infinitely often. Then conclude that there exist $r$ and $s$, with $r > s$ such that $\phi_r(Y) = \phi_s(Y) \in \Sigma$

so $Z \in \omega(Y)$, there are infinitely many $Y(t_n)$ that get close to $Z$, and therefore must intersect $\Sigma$, as there are no equilibrium points in $\omega(Y)$

and since $Y(t_n)$ intersects $\Sigma$ at a single point infinitely many times, we have $\phi_r(Y) = \phi_s(Y) \in \Sigma$ with $r > s$ 

### Step I.5 Conclude that the orbit of $Y$ is closed

the orbit of $Y$ repeats itself, so it is closed.

