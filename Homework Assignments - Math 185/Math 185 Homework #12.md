Renee Senining

Math 185

### Homework #12

#### Chapter VII, Sec. 1, ex. 1e, 1g, 1h, 3b, 3e;  Sec. 2, ex. 5;  Sec. 3. ex. 4; Sec. 4, ex. 8

#### Sec. 1

##### Ex. 1e $\text{Res}[\frac{\cos z}{z^2}, 0]$ 

$\frac{\cos z}{z^2} = \frac{1}{z^2} - 1 + z^2 - z^4 + \cdots$

$a_{-1} = 0$ 

also rule 2:

$\frac{d}{dz}[z^2*\cos z/z^2] = - \sin z$, which $= 0$ at $z= 0$ 

##### Ex. 1g $\text{Res}[\frac{z}{\text{Log }z}, 1]$

Can use Rule 3:

$\text{Log }z$ has a simple zero at $z = 1$ since

$\frac{d}{dz}[\text{Log }z] = \frac{1}{z}$ and at $z = 1$ is equal to $1$ 

so $f(z) = z$, $g(z) = \text{Log }z$ 

$f(z)/g'(z) = \frac{z}{1/z} = z^2$ and at $z = 1$ is equal to $1$ 

##### Ex. 1h $\text{Res}[\frac{e^z}{z^5}, 0]$ 

$\frac{e^z}{z^5} = \frac{1}{z^5}\sum_{k = 0}^\infin \frac{z^k}{k!}$ $= \sum_{k = -5}^\infin \frac{z^k}{(k+5)!}$

and at $k = -1$, $a_{-1} = \frac{1}{4!} = \frac{1}{24}$

##### Ex. 3b

$\oint_{|z| = 2}\frac{e^z}{z^2 - 1}dz = \oint_{|z| = 2} \frac{e^z}{(z+1)(z-1)} dz$

Using Residue Theorem:

We have isolated singularities: $z = \pm 1$ 

We may use Rule 3 for both:

$f(z) = e^z, g(z) = (z+1)(z-1)$, since $g(z)$ has simple zeros at $\pm 1$ and both are analytic over the entire complex plane

$g'(z) = 2z$

$\text{Res}[\frac{e^z}{z^2-1}, 1] = \frac{e}{2}$

$\text{Res}[\frac{e^z}{z^2 - 1}, -1] = -\frac{e^{-1}}{2} $

so $\oint_{|z| = 2}\frac{e^z}{z^2 - 1} dz = 2\pi i (\frac{e^1 - e^{-1}}2) = 2\pi i \sinh (1)$

or just $\pi i(e^1 - e^{-1})$  

##### Ex. 3e

$\oint_{|z-1| = 1} \frac{1}{z^8 - 1}dz$ 

$z^8 -1 = 0$ for $z^8 = 1$

at the 8 roots of unity

however, we only need to consider the singularities in $|z-1| \leq 1$, a disk that is fully contained in the right half-plane except at $z = 0$ 

so only the roots of unity in the right half-plane should be considered:

$e^{-i \pi /4}, 1, e^{{i \pi /4}}$ 

$z^8 - 1 = \prod_{k = 0}^{7} (z-e^{i \pi k/4})$

so $g(z) = z^8 - 1$ has simple zeros at each root, we may use rule 4

$g'(z) = 8z^7$ 

$g'(e^{i\pi k/4}) = 8e^{i7\pi k/4}$

the integral is equal to 

$2\pi i \sum_{k = -1}^1 \frac{1}{8e^{i7\pi k/4}}$

$= \frac{\pi i}{4}[\frac{1}{e^{-7\pi /4}} + 1 + \frac{1}{e^{7\pi/4}}] $

$\frac{7\pi}{4} = 2\pi - \pi/4 \equiv - \pi/4$

$-\frac{7\pi}{4} = -2\pi + \pi/4 \equiv \pi/4 $

so $= \frac{\pi i}{4}[e^{- \pi/4}+ 1 + e^{-(-\pi/4)}]$

and $e^{-\pi/4} = \frac{1 - i}{\sqrt{2}}$ , $e^{\pi/4} = \frac{1+i}{\sqrt{2}}$ 

$= \frac{\pi i}{4}[1 + \frac{2}{\sqrt{2}}] = \frac{\pi i}{4}[1 + \sqrt{2}]$

#### Sec. 2

##### Ex. 5 Using the residue theory, show that $\int_{0}^\infin \frac{x^2}{x^4 + 1}dx = \frac{\pi}{2\sqrt{2}}$ 

Using $(2.4)$ on page 200:

the poles of $z^2/(z^4+1)$ in the upper half-plane:

$z^4 = -1$

$e^{i(\pi +2\pi k)/4} = e^{i\pi/4 + \pi k/2}$

$e^{i\pi/4}$, $e^{i3\pi/4}$ are the (simple) poles in the upper half-plane

Finding the residue at each of these poles

using Rule 3:

with $g(z) = z^4 + 1$, we have $g'(z) = 4z^3$

we have $f(z)/g(z) = z^2/4z^3 = 1/4z$

and so $\frac{f(e^{i\pi/4})}{g'(e^{i\pi/4})} = \frac{1}{4z}|_{z = e^{i\pi/4}} = \frac{\sqrt{2}}{4(1+i)}$

and at $z = e^{i3\pi/4}$

$\frac{f(e^{i3\pi/4})}{g(e^{i3\pi/4})} = \frac{1}{4z}|_{z= e^{i3\pi /4}} = \frac{\sqrt{2}}{4(-1+i)}$

so $\int_{-\infin}^\infin \frac{x^2}{x^4 + 1}dx = $

$2\pi i (\frac{\sqrt{2}(1+i -1 +i)}{4(-2)}) = 2\pi (\frac{\sqrt{2}(2)}{8}) = \frac{\pi}{\sqrt{2}}$

since $\frac{x^2}{x^4+1}$ is an even function, it is symmetric about the $x$-axis, and we have

$\int_{-\infin}^\infin \frac{x^2}{x^4+1}dx = 2\int_0^\infin \frac{x^2}{x^4+1}dx $

so we have $\int_0^\infin \frac{x^2}{x^4+1} = \frac{\pi}{2\sqrt{2}}$ as desired

#### Sec. 3

##### Ex. 4 Show using residue theory that $\int_{-\pi}^\pi \frac{d\theta}{1 + \sin^2\theta} = \pi \sqrt{2}$ 

$z = e^{i\theta}$ 

$d\theta = \frac{dz}{iz}$ 

$\sin^2\theta = (\frac{z - 1/z}{2i})^2 = \frac{z^2 - 2+ 1/z^2}{-4}$

$1 + \sin^2\theta = 1 - \frac{z^2 -2 + 1/z^2}{4} = \frac{4-z^2 + 2 -1/z^2}{4} = $$-\frac{z^2 -6 + 1/z^2}{4}$ 

$\int_{-\pi}^\pi \frac{d\theta}{1 + \sin^2\theta} = \oint_{|z| = 1}\frac{4}{-z^2 + 6 - 1/z^2}\frac{dz}{iz} $

$ = \frac{4}{i}\oint_{|z| = 1}\frac{dz}{-z^3 + 6z - 1/z}$ 

$= \frac{4}{i}\oint_{|z|=1}\frac{z}{-z^4+6z^2-1}dz$ 

$-z^4 + 6z^2 - 1 = 0$ 

$w = z^2$

$-w^2 + 6w-1 = 0$

$w^2 - 6w + 1$

$\frac{6 \pm \sqrt{36 - 4}}{2} = 3 \pm \sqrt{8} $

$z^2 = 3 \pm \sqrt{8}$ 

roots:

zeros are at

$z = \pm\sqrt{2}\pm1$ 

with $-\sqrt{2}+1$, $\sqrt{2}-1$ being the only roots inside the unit circle 

each of these roots are simple poles

Using rule 3:

$\frac{f(z)}{g'(z)} = \frac{z}{-4z^3 + 12z} = \frac{1}{-4z^2 +12}$

so at $-\sqrt{2} +1$ and $\sqrt{2}-1$ 

$(-\sqrt{2}+1)^2 = 2 - 2\sqrt{2} + 1 = 3 - 2\sqrt{2} = (\sqrt{2}-1)^2$

The residues are $\frac{1}{8\sqrt{2}}$ 

so the integral is

$= \frac{4}{i}2\pi i(\frac{2}{8\sqrt{2}}) = \pi \sqrt{2}$ 

#### Sec. 4

##### Ex. 8

By integrating a branch of $(\log z)/(z^3 +1)$ around the boundary of an indented sector of aperture $2\pi /3$, show that

$\int_0^\infin \frac{\log x}{x^3 + 1}dx = \frac{-2\pi^2}{27}$, $\int_0^\infin \frac{1}{x^3+1}dx = \frac{2\pi}{3\sqrt{3}}$ 

$\log{z} = \frac{\log |z| + i\arg z}{(z - e^{i\pi/3}(z-e^{i\pi })(z- e^{i5\pi /3}))}$

the sector is from $0 < \theta < 2\pi /3$ and we consider the branch cut : $\C \setminus (-\infin, 0]  $

The only pole contained in this sector is at $e^{i\pi/3}$ (is a simple pole)

$\text{Res}[\frac{\log|z| + i\arg z}{z^3 +1}, e^{\pi i/3}] = \frac{\log |z| +i\arg z}{3z^2}|_{z = e^{\pi i/3}} = \frac{\log(1) + i\pi /3}{3e^{2\pi i/3}} = \frac{i\pi}{9}e^{-2\pi i/3}$

we have four integrals:

$\gamma_1$ :one from $\epsilon$ to $R$ along the real axis, 

$\int_{\epsilon}^R \frac{\log x}{x^3 +1}dx $ 

$\Gamma_R$ is the path along the circle of radius $R > 0$ from $(R, 0)$ to $Re^{i2\pi/3}$ , $(-\frac{R}{2}, \frac{\sqrt{3}R}{2})$ , going counterclockwise

$\gamma_2$  from $(-\frac{R}{2}, \frac{\sqrt{3}R}{2})$ to $(-\frac{\epsilon}2, \frac{\sqrt{3}\epsilon}2)$ 

$\gamma_{\epsilon}$ is the path along the circle of radius $\epsilon > 0$ (small) from $(-\frac{\epsilon}{2}, \frac{\sqrt{3}\epsilon}{2})$ ($\epsilon e^{i2\pi/3})$ clockwise to $(\epsilon , 0)$ 

$|\log |z| + i \arg z |\leq \sqrt{ \log ^2R + (\frac{2\pi }{3})^2}$

$z^3 + 1 \leq R^3 +1$

and the length of $\Gamma_R$ is $2\pi R/3$ 

 $|\int_{\Gamma_R} \frac{\log|z| + i\arg z}{z^3 +1} dz| \leq \frac{\sqrt{ \log ^2R + (\frac{2\pi }{3})^2}}{R^3-1}\cdot \frac{2\pi R}{3} \sim \frac{2\pi \log R}{3R^2} \rightarrow 0$ as $R \rightarrow \infin$ 

and along $\gamma_2$ (straight line, so can treat "like" the real line)

letting $z = x e^{2\pi i/3}$ and $dz = e^{2\pi i/3}dx$ 

$\int_{R}^\epsilon \frac{\log x + 2\pi i/3}{x^3 +1 }e^{2\pi i/3}dx$

$= -e^{2\pi i/3}\int_{\epsilon}^R \frac{\log x + 2\pi i/3}{x^3 + 1}dx$

$ = -e^{2\pi i/3}[\int_{\epsilon}^R \frac{\log x}{x^3 +1}dx + \frac{2\pi i}{3}\int_\epsilon ^R \frac{1}{x^3 + 1}dx]$

and along $\gamma_{\epsilon}$ :

$|\int_{\gamma_\epsilon} \frac{\log|z| + i\arg z}{z^3 +1} dz| \leq $ $\frac{\sqrt{\log^2 \epsilon + (\frac{2\pi}3)^2}}{1 - \epsilon ^3}\cdot \frac{2\pi \epsilon }{3} \sim \frac{2\pi \epsilon |\log \epsilon| }{3}$ and as $\epsilon \rightarrow 0^+$

$\epsilon \log \epsilon = \frac{\log \epsilon}{1/\epsilon}$

using L'hospital's

$\frac{1/\epsilon}{-1/\epsilon^2} = \frac{1}{-1/\epsilon} \rightarrow 0$ as $\epsilon \rightarrow 0^+$ 

so we have

$(1 - e^{2\pi i/3})\int_{\epsilon}^R \frac{\log x}{x^3 +1}dx -\frac{2\pi ie^{2\pi i/3}}{3}\int_\epsilon ^R \frac{1}{x^3 + 1}dx  = 2\pi i\frac{ i\pi}{9}e^{-2\pi i/3}$

multiplying both sides by $e^{-\pi i/3}$ we have:

(using $(e^{-\pi i/3} - e^{\pi i /3}) = 2i \sin (\pi/3)$)

$-2i \sin (\pi/3)\int_\epsilon ^R \frac{\log x}{x^3 + 1}dx - \frac{2\pi i e^{\pi i/3}}{3}\int_\epsilon ^R \frac{1}{x^3 + 1}dx = \frac{2\pi^2}{9}$ 

$\equiv$ 

$-\sqrt{3} i \int_\epsilon ^R \frac{\log x}{x^3 + 1} - \frac{\pi i }{3}\int_{\epsilon}^R \frac{1}{x^3 +1}dx + \frac{\pi \sqrt{3}}{3}\int_{\epsilon}^R \frac{1}{x^3 +1}dx = \frac{2\pi ^2}{9}$

so 

$\int_{\epsilon }^R \frac{1}{x^3+1} = \frac{2\pi }{3\sqrt{3}}$

and

$-\sqrt{3}i \int_{\epsilon }^R \frac{\log x}{x^3+1} - \frac{\pi i}{3}\int_{\epsilon}^R \frac{1}{x^3 +1}dx = 0$ 

so $\int_{\epsilon }^R \frac{\log x}{x^3 +1} = \frac{\pi}{3}\frac{2\pi}{3\sqrt{3}}\frac{-1}{\sqrt{3}}$$= $ $-\frac{2\pi^2}{27}$  