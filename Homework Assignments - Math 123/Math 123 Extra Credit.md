1. Let $A$ be an annular region in $\R^2$. Let $F$ be a planar vector field that points inward along the two boundary curves of $A$. Suppose also that every radial segment of $A$ is a local section. Prove there is a periodic solution in $A$ 

   the region $A\cup\partial A$ ($\partial A$ is the boundary of $A$) is closed and bounded, as well as positively invariant since the vector field points inward along the boundary curves

   So it contains either a limit cycle or an equilibrium point (Page 227, Corollary 2) in $A\cup \partial A$, but since the vector field points inward along $\partial A$, there are no equilibrium points on $\partial A$ nor is a limit cycle (fully) contained in $\partial A$ 

   so there is either an equilibrium point in $A$, which is a periodic solution or there is a limit cycle, $\gamma$ in $A \cup\partial A$

   if this limit cycle is fully contained in $A$, we have that there is a periodic solution in $A$

   otherwise, we look at the open region $U$, in the interior of $\gamma$. This region is fully contained in $A$, else we have its boundary, $\gamma$ crossing $\partial A$, a contradiction.

   and by corollary 3, $U$ and therefore $A$, contains either an equilibrium point or a limit cycle, both of which are periodic as stated earlier. 

   If equilibrium points are considered tangent with the local section, and therefore not possible in $A$, then we have for certain that there must be limit cycles and therefore periodic solutions.

   Also, since $A$ is positively invariant for any $X(t)$ in $A$, $\omega(X)$ $\sub A$, so solutions through $Y \in \omega(X)$ must be periodic since they can only cross local sections once, and each radial segment in $A$ is a local section. (there is a $T>0$ s.t. $\phi_T(Y)  = \phi_0(Y)$ $\implies \phi_{t+T}(Y) = \phi_{t}(Y)$ for all $t \in \R$)

2. Consider the system in polar coordinates

   $r' = r(1-r^2) +\mu r \cos \theta \\ \theta' = 1$

   If $0 \leq \mu < 1$, show that the system has a closed orbit

   ---

   fix $\mu \in [0, 1)$

   since $-\mu r < -\mu r \cos\theta < \mu r$ 

   if we choose $r> \sqrt{2}$ $\implies r^2 > 2$ 

   we have $1-r^2 < 1 -  2 = -1$ 

   so $r(1-r^2) < -r$

   and since $|\mu r \cos\theta| < \mu r < r$

   $\implies r(1-r^2) + \mu r \cos\theta < -r + r = 0$ 

   therefore, when $r > \sqrt{2}$, 

   $r' < 0$ for all $\theta \in \R$ 

   so let $C = \{(r, \theta)| r = 2\}$   

   so the vector field on $C$ points inside $C$ 

   which means the union of $C$ and the region bounded by $C$  is positively invariant, closed and bounded

   and since there are no equilibria in this system due to $\theta' = 1$, 

   there is a limit cycle, a closed orbit, contained in $C$ 

3. I couldn't come up with an explicitly defined system, but I imagine it is possible to have one as illustrated below where: 

   X is the gray curve with the red lines as its limit set, always approaching (closer and closer, but never crosses it), and the redlines are lines where each point is an equilibrium point

   ![1543907835065](C:\Users\Renee\AppData\Roaming\Typora\typora-user-images\1543907835065.png)


