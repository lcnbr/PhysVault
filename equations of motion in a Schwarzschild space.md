---
alias: 
- Schwarzschiltrajectory
tag: GR physics
---
The [[Schwarzschild solution to Einstein's field equation#^ScwarzschildSol|Schwarzschild metric]] can be useto approximate the gravitational field due to the sun in our planetary system, ignoring the gravity of the planets. To calculate the trajectory of a particle in this gravitational field, we use the [[principle of equivalence#^eomGeneric|geodesics equation]]

$$
\dv[2]{ x^{\mu}}{ p}+\Gamma^\mu{}_{\nu \rho} \dv{ x^{\nu}}{ p} \dv{ x^{\rho}}{ p}=0
$$

^eom

where the coordinates read
$$
x^{\mu}=\{t, r, \theta, \varphi\}
$$
anthe parameter $p$ is the variable that we use in order to parameterize the trajectory $x^{\mu}(p)$ of the particle. For a start, we can let the evolution variable unspecified. Once we solve the equations of motion in terms of the arbitrary parameter $p$, we will relate the parameter $p$ to [[infinitesimal proper time interval in SR|proper time]] via

$$
\begin{aligned}
\dv{ \tau^{2}}{p^2} &=g_{\mu \nu} \dv{ x^{\mu}}{p} \dv{ x^{\nu}}{p} \\
&=B(r)\left(\dv{ t}{p}\right)^{2}-A(r)\left(\dv{ r}{p}\right)^{2}-r^{2}\left(\left(\dv{ \theta}{p}\right)^{2}+\sin ^{2} \theta\left(\dv{ \varphi}{p}\right)^{2}\right)
\end{aligned}
$$

^proptime

This procedure will show that for a massive particle, $p$ can be chosen to be proportional to [[infinitesimal proper time interval in SR|proper time]] $\tau$. However, for light particles [[infinitesimal proper time interval in SR|proper time]] intervals $\dd \tau$ vanish and a different variable needs to be chosen.
The [[#^eom| equations of motion]] have the explicit form using the [[Schwarzschild solution to Einstein's field equation#^AffineconnectionComp]]

$$
\begin{aligned}
&\dv{^{2}}{p^{2}} t(p)+\frac{\left(\dv{}{r} B(r)\right)\left(\dv{}{p} t(p)\right)\left(\dv{}{p} r(p)\right)}{B(r)}=0 \\
&\dv{^{2}}{p^{2}} r(p)+\frac{\left(\dv{}{r} B(r)\right)\left(\dv{}{p} t(p)\right)^{2}}{2 A(r)}+\frac{\left(\dv{}{r} A(r)\right)\left(\dv{}{p} r(p)\right)^{2}}{2 A(r)} \\
&\quad-\frac{r\left(\dv{}{p} \theta(p)\right)^{2}}{A(r)}-\frac{r\left(\sin ^{2}(\theta)\right)\left(\dv{}{p} \phi(p)\right)^{2}}{A(r)}=0 \\
&\dv{^{2}}{p^{2}} \theta(p)+\frac{2\left(\dv{}{p} r(p)\right)\left(\dv{}{p} \theta(p)\right)}{r}-\sin (\theta) \cos (\theta)\left(\dv{}{p} \phi(p)\right)^{2}=0 \\
&\dv{^{2}}{p^{2}} \phi(p)+\frac{2\left(\dv{}{p} r(p)\right)\left(\dv{}{p} \phi(p)\right)}{r}+\frac{2 \cos (\theta)\left(\dv{}{p} \theta(p)\right)\left(\dv{}{p} \phi(p)\right)}{\sin (\theta)}=0
\end{aligned}
$$
We can simplify the problem of solving these equations by using the isotropy property of the space and set the azimuthal angle to a convenient value $\theta=\frac{\pi}{2}$. We obtain, writing $\dv {p}\square=\dot{\square}$ and $\dv{r}\square=\square'$

$$
 \ddot{t}+\frac{B'\dot{t}\dot{r}}{B}=0 
$$

^tEom

$$
\ddot{r}+\frac{B'\dot{t}^2}{2 A}+\frac{A'\dot{r}^2}{2 A}-\frac{r\dot{\varphi}^2}{A}=0 
$$

^rEom

$$
\ddot{\varphi}+\frac{2\dot{r}\dot{\varphi}}{r}=0
$$

^phiEom

By recognizing that
$$
\dv{B(r(p))}{p}=B'\dot{r},
$$
we find that [[#^tEom]] takes the integrable form,
$$
\dv{}{p}\left(B \dot{t}\right)=0,
$$
This yields

$$
\dot{t}=\frac{f}{B(r)},
$$

^constf

where $f$ is a constant. We will see that the value of this constant is physically immaterial.
Similarly, [[#^phiEom]] takes an integrable form
$$
\dv{}{p}\left(r^{2} \dot{\varphi}\right)=0,
$$

which yields a constant of motion,

$$
f\cdot J=r^{2} \dot{\varphi} .
$$

^constJ

The constant of integration $J$ will turn out to be an analogous quantity to the magnitude of the Newtonian angular momentum (the multiplication with the other integration constant $f$ in the left-hand side will facilitate this identification).

Substituting the derivatives $\dv{ \phi}{p}$ and $\dv{ t}{p}$ from [[#^constf]] and [[#^constJ]] into [[#^rEom]] we obtain an equation which can be further brought to the integrable form (Exercise)
$$
\dv{}{p}\left[A(r)\dot{r}^{2}+\frac{J^{2} f^{2}}{r^{2}}-\frac{f^{2}}{B}\right]=0
$$
We therefore have

$$
A(r)\dot{r}^{2} \frac{1}{f^{2}}+\frac{J^{2}}{r^{2}}-\frac{1}{B}=-E
$$

^constE

We can now relate the parameter $p$ to [[infinitesimal proper time interval in SR|proper time]] more explicitly. Substituting $\theta=\frac{\pi}{2}$ and the results for $\dot  {\varphi} , \dot{r}, \dot{t}$ from [[#^constf]], [[#^constJ]] and [[#^constE]] into [[#^proptime]], we obtain
$$
\left(\dv{ \tau}{p}\right)^{2}=E f^{2} .
$$
As anticipated, the evolution parameter $p$ and proper-time are related linearly. The positivity of the left-hand side of the above equation sets the constraint
$$
E \geq 0 .
$$
For photons and other massless particles, $d \tau=0$, which corresponds to
$$
E_{\gamma}=0 \text {. }
$$
For massive particles, we must have $E>0$.
We can now trade the evolution parameter $p$ with time, as
$$
\dot{r}=\dv{ r}{t} \dot{t}=\dv{ r}{t} \frac{f}{B(r)}
$$
and similarly,
$$
\dot{ \varphi}=\dv{ \varphi}{t} \dot{ t}=\dv{ \varphi}{t} \frac{f}{B(r)} .
$$
Substituting into [[#^constJ]] and [[#^constE]], we obtain
$$
\frac{\dv{ \varphi}{t} r^{2}}{B(r)}=J
$$
and

$$
\frac{A(r)}{B(r)} \qty(\dv{ r}{t})^{2}+\left(\frac{J^{2}}{r^{2}}-\frac{1}{B(r)}\right)=-E
$$

^radEq

From the above equations we can derive the angular dependence of the radius

$$
\frac{A(r)}{r^{4}}\left(\dv{ r}{ \phi}\right)^{2}+\left(\frac{1}{r^{2}}-\frac{1}{J^{2} B(r)}\right)=-\frac{E}{J^{2}}
$$

^OrbitEq

To understand the physical meaning of the $E, J$ constants of motion, let us expand our results around the [[Newtonian limit]] $r_{S} / r \rightarrow 0$, recalling that
$$
B(r)=\frac{1}{A(r)}=1-\frac{r_{S}}{r} .
$$

We find (exercise) the Newtonian angular momentum:

$$J \approx r^{2} \dot{\varphi} \quad$$ 

^NewtAngMom


and Newtonian energy ($\frac{r_S}{r}\sim\frac{1}{r^2}$)

$$
\underbracket{\frac{1}{2} \dot{r}^{2}+\frac{J^{2}}{2 r}}_{\textclap{kinetic energy (spherical)}}\overbracket{-\frac{\frac{1}{2}r_{S}}{r}}^{-\frac{GM}{r} \text{ pot. E. }} \approx \frac{1-E}{2}
$$

^NewtEn


# Light

For light $E=0$, we use [[#^OrbitEq]], isolating $\dd{\varphi}$ and integrate:

$$
\int\mathrm{d} \varphi=\pm \int \frac{\sqrt{A} \mathrm{~d} r}{r^{2}}\left(\frac{1}{J^{2} B(r)}-\frac{1}{r^{2}}\right)^{-1 / 2}
$$
Let us assume a minimum distance $r=r_{0}\left(\left.\frac{\mathrm{d} r}{\mathrm{~d} \varphi}\right|_{r=r_{0}}=0\right)$ from the massive center. Then again using [[#^OrbitEq]]
$$
\frac{1}{J^{2} B\left(r_{0}\right)}-\frac{1}{r_{0}^{2}}=0 \Rightarrow J^{2}=\frac{r_{0}^{2}}{B\left(r_{0}\right)}
$$
and
$$
\begin{aligned}
\varphi &=\pm \int \sqrt{A(r)} \frac{\mathrm{d} r}{r^{2}}\left[\frac{B\left(r_{0}\right)}{r_{0}^{2} B(r)}-\frac{1}{r^{2}}\right]^{-1 / 2} \\
&=\pm \int \frac{\mathrm{d} r}{r^{2}} \frac{r_{0}}{\sqrt{r^{2}-r_{0}^{2}}}\left\{1+\frac{r_{s}}{2 r_{0}}\left[\frac{r\left(r+r_{0}\right)+r_{0}^{2}}{r\left(r+r_{0}\right)}\right]+\mathcal{O}\left(r_{s}^{2}\right)\right\} \\
&=\pm\left[\text { const. }-\arctan \left(\frac{r_{0}}{\sqrt{r^{2}-r_{0}^{2}}}\right)+\frac{\left(2-\frac{r_{0}}{r}\right)\left(1-\frac{r_{0}}{r}\right)}{\sqrt{1-\frac{r_{0}^{2}}{r^{2}}}} \frac{r_{s}}{2 r_{0}}+\mathcal{O}\left(r_{s}^{2}\right)\right]
\end{aligned}
$$
![[Pasted image 20220207091122.png#leftwrap|250]]With the above we can compute (Exercise) the deflection angle $\Delta \phi$ of light passing by the sun:

We find
$$
\Delta \phi=\frac{2 r_{s}}{r_{0}}=\frac{4 M G}{r_{0}}
$$
For the sun $\Delta \phi \sim 1.75^{\prime \prime}$.






# bound orbits

![[Pasted image 20220207093041.png#center|300]]Two extrema, maximum and minimum distance.
$$
\phi(r)=\phi\left(r_{-}\right)+\int_{r_{-}}^{r} \frac{\sqrt{A}}{r^{\prime 2}} \mathrm{~d} r^{\prime}\left[\frac{1}{J^{2} B(r)}-\frac{E}{J^{2}}-\frac{1}{r^{2}}\right]^{-1 / 2}
$$
We can trade both $E, J^{2}$ with $r_{+}, r_{-}$. Then we can expand in $r_{S} \rightarrow 0$. One finds
$$
\Delta \phi=2\left|\phi\left(r_{+}\right)-\phi\left(r_{-}\right)\right|=2 \pi+3 \pi M G\left(\frac{1}{r_{+}}+\frac{1}{r_{-}}\right) .
$$
For Mercury $\Delta \phi_{\text {precession }}=(\Delta \phi-2 \pi) \approx \frac{0.1038^{\prime \prime}}{\text { revolution }}$. In a century ( $\leftrightarrow 415$ revolutions) we have a precession of $43.03^{\prime \prime}$.