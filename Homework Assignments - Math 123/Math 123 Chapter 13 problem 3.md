# Math 123 Chapter 13 problem 3

What does a particle moving away from origin at $t=0$ tell us about how the particle is moving in accordance with this central force system?

What are the initial conditions we want to consider?

- is it position and velocity?

This system is conservative and a central force field.

The system without polar coordinates:

$X' = V$ 

$V' = -\frac{X}{|X|^3}$ 



------

The system with polar coordinates: (when we have the system as above)

$r' = v_r$

$\theta' = v_\theta/r$

$v'_r = -\frac{1}{r^2} + v_\theta^2/r$ 

$v_\theta' = -v_rv_\theta/r$ 

------

$r'(t) = v_r(t)$ 

$\theta'(t) = v_\theta(t) /r(t)$ 

$v_\theta(t) = r(t)\theta'(t)$

$v_r'(t) = -\frac{1}{r(t)^2} + r(t)\theta'(t)$ 

$v_\theta' = -\frac{v_r(t)v_\theta(t)}{r(t)}$ 

  

------

$X' = V$

$m_p V' = -gm_sm_p \frac{X}{|X|^3}$ 

so $V' = -gm_s \frac{X}{|X|^3}$, where $m_s = $ $\text{mass of the sun}$

Things to consider as well:

- restrict attention to particles moving in the plane $\R^2$
- Configuration space: $C = \R^2 - \{0\}$ 
- Phase space: $P = (\R^2 - \{0\}\times \R^2)$ 
  - the collection of all tangent vectors at each point $X \in C$ 
- $T_X = \{(X, V)| V \in \R^2\}$ : the tangent plane to the configuration at $X$
- $P = \cup_{X \in C}T_X$

So at each point in the plane $X$, we associate a plane of tangent vectors with it.

Why can we do this again?

-  How does total energy and angular momentum play into this?

Describing each solution curve $(r(t), v(t))$ with $v = r'$ i.e. $(r, v_r)$ 

$r(v)$ (the graph of)

$r' = v_r$

$\frac{dr}{dt} = v_r$

$\frac{d v_r}{dt} = -\frac{1}{r^2} + \frac{v_\theta^2}{r}$ 

$v_\theta' = -\frac{v_rv_\theta}{r}$

$dv_\theta/v_\theta = -\frac{v_r(t)}{r(t)}dt = -\frac{r'(t)}{r(t)}dt$

$\int \frac{1}{v_\theta} dv_\theta = -\int\frac{r'(t)}{r(t)}dt$

$\ln(v_\theta) = -\ln(r) + C$

$v_\theta = Ce^{-\ln(r)} = \frac{C}{r}$, $C = rv_{\theta, 0}$ ?????

$v_\theta^2 = C^2/r^2$, for some constant $C$

 $\frac{dv_r}{dt} = -\frac{1}{r^2} + \frac{C^2}{r^3}$ 

$\frac{dv_r}{dt} = -\frac{r + C^2}{r^3}$

$\frac{dt}{dv_r} = \frac{r^3}{r+C^2}$ 

$\frac{dr}{dt}\frac{dt}{dv_r} = \frac{v_r r^3}{r + C^2}$ 

$\frac{dr}{dv_r} = \frac{v_r r^3}{r + C^2}$  

$x_1' = v_1 \\ x_2'  = v_2 \\ v_1' = -x_1/(x_1^2 + x_2^2)^{3/2} \\ v_2' = -x_2/(x_1^2 + x_2^2)^{3/2}$

