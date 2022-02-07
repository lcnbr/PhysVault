---
alias:
- relativistic force
- equations of motion
tags: GR SR
---
See also [[relativistic particle.md]]
We can directly generalize the equations of classical mechanics so that they can be consistent with [[Lorentz transformation|Lorentz transformations]]. We introduce a relativistic force
$$

f^{\mu}=m \frac{\mathrm{d}^{2} x^{\mu}}{\mathrm{d} \tau^{2}}

$$

^relForce

where $m$ is the mass of a particle and $\tau$ is [[infinitesimal proper time interval in SR.md|proper time]]. $f^{\mu}$ relates to the Newtonian force. Let us work in the [[instantaneous rest frame]] of the particle $(\vec{v}=0)$. Then
$$
f_{\text {rest }}^0=m \frac{\mathrm{d}^{2} x^0}{\mathrm{~d} \tau^{2}}=m \frac{\mathrm{d}^{2} x^0}{\mathrm{~d} x^{0^{2}}}=0
$$

^frest0

and
$$
f_{\text {rest }}^i=m \frac{\mathrm{d}^{2} x^i}{\mathrm{~d} \tau^{2}}=m \frac{\mathrm{d}^{2} x^i}{\mathrm{~d} t^{2}}=F_{\text {Newton }}^i
$$
^fresti

Let us now look at what happens in the frame where the particle has an instantaneous velocity $\vec{v}$. we use a [[Lorentz transformation.md#^boost|Lorentz boost]]
$$
f^{\mu}=\underbracket{\Lambda^{\mu}{ }_\nu(\vec{v})}_{\text {boost }} f^\nu_{\text {rest }},
$$
and
$$
\begin{aligned}
f^0  &=\Lambda^0{}_\nu(\vec{v}) f^\nu_{\text {rest }} \\
     &=\Lambda^0{}_0 \underbracket{f^0_{\text {rest }}}_{=0}+\Lambda^0{}_i f^i_{\text {rest }} \\
     &=\gamma v_i F_{\text {Newton }}^i \\
\Rightarrow & f^0=\frac{\vec{v} \cdot \vec{F}_{\text {Newton }}}{\sqrt{1-\vec{v}^{2}}}
\end{aligned}
$$

For the "space" components we have
$$
\begin{aligned}
f^i  &=\Lambda^i{}_\nu(\vec{v}) f^\nu_{\text {rest }} \\
     &=\Lambda^i{}_0 \underbracket{f^0_{\text {rest }}}_{=0}+\Lambda^i{}_j f^j_{\text {rest }} \\


&=\left(\delta_{i j}+\frac{v_i v_{j}}{v^{2}}(\gamma-1)\right) F_{\text {Newton }}^{j} \\
\Rightarrow & \vec{f}=\vec{F}_{\text {Newton }}+\frac{\vec{v} \cdot \vec{F}_{\text {Newton }}}{\vec{v}^{2}}(\gamma-1) \vec{v}
\end{aligned}
$$
>Exercise: Work out Lorentz's force starting from the electrostatic force.

So, now we want to know how to use the [[Newtonian limit]] (zero velocity) in order to construct a relativistic force that satisfies [[#^relForce]], generalized as above from the [[Newtonian limit]]. It is a second order differential equation (or better, 4 of them for $\mu=0,1,2,3$ ). In order to solve it, we also need boundary conditions, but here we must be careful! In Newtonian physics
$$
\vec{F}=m \frac{\mathrm{d}^{2} \vec{x}}{\mathrm{~d} t^{2}} .
$$
We need $\vec{x}(0)$ and $\dot{\vec{x}}(0)$, i.e. six boundary conditions. For [[special relativity]] we may be tempted to require eight boundary conditions $x^{\mu}\left(\tau_{0}\right)$ and $\frac{\mathrm{d} x^{\mu}}{\mathrm{d} \tau}\left(\tau_{0}\right)$. However, the relativistic "velocities" $\frac{\mathrm{d} x^{\mu}}{\mathrm{d} \tau}$ must satisfy
$$
\begin{aligned}
\eta_{\mu \nu} \frac{\mathrm{d} x^{\mu}}{\mathrm{d} \tau} \frac{\mathrm{d} x^{\nu}}{\mathrm{d} \tau} &=1 \\
\implies \left(\frac{\mathrm{d} t}{\mathrm{~d} \tau}\right)^{2}-\left(\frac{\mathrm{d} \vec{x}}{\mathrm{~d} \tau}\right)^{2} &=1
\end{aligned}
$$

^properTimeCond

for every value of $\tau$. So, when we choose boundary conditions at $\tau=\tau_{0}$, we should respect the above identity. Once we have found our boundary conditions consistently at $\tau=\tau_{0}$, we can rest assured that [[#^properTimeCond]] will be satisfied for all values of $\tau$. Indeed,
$$
\begin{aligned}
m \frac{\mathrm{d}}{\mathrm{d} \tau}\left(\eta_{\mu \nu} \frac{\mathrm{d} x^{\mu}}{\mathrm{d} \tau} \frac{\mathrm{d} x^{\nu}}{\mathrm{d} \tau}\right) &=2 \eta_{\mu \nu}\left(m \frac{\mathrm{d}^{2} x^{\mu}}{\mathrm{d} \tau^{2}}\right) \frac{\mathrm{d} x^{\nu}}{\mathrm{d} \tau} \\
&=2 \eta_{\mu \nu} f^{\mu} \frac{\mathrm{d} x^{\nu}}{\mathrm{d} \tau} \\
& \equiv K(x)
\end{aligned}
$$
Notice that $K(x)$ is invariant under [[Lorentz transformation|Lorentz transformations]]. Indeed,
$$
\begin{aligned}

K'(x) &=2 \eta_{\mu \nu} (f^\mu)' \dv{(x^{\nu})'}{\tau} \\
&=2 \eta_{\mu \nu} \Lambda^{\mu}{}_{\rho} f^{\rho} \Lambda^{\nu}{}_{\sigma} \frac{\mathrm{d} x^{\sigma}}{\mathrm{d} \tau} \\
&=2 \underbracket{\eta_{\mu \nu} \Lambda^{\mu}{}_{\rho} \Lambda^{\nu}{}_{\sigma}}_{=\eta_{\rho \sigma}} f^{\rho} \frac{\mathrm{d} x^{\sigma}}{\mathrm{d} \tau} \\
&=2 \eta_{\rho \sigma} f^{\rho} \frac{\mathrm{d} x^{\sigma}}{\mathrm{d} \tau}=K(x)
\end{aligned}
$$
Let us compute it in the [[instantaneous rest frame|rest frame]] (thus we have [[#^frest0]]). Due to the above result it will then be same in all inertial frames.
$$
\left.f^{\mu} \frac{\mathrm{d} x^{\mu}}{\mathrm{d} \tau} \eta_{\mu \nu}\right|_{\text {rest }}=\underbracket{f_{\text {rest }}^{0}}_{=0} \dv{x^0}{\tau}-f_{\text {rest }}^{i} \underbracket{\dv{ x^i}{ \tau}}_{=0}=0 .
$$
Thus
$$
\frac{\mathrm{d}}{\mathrm{d} \tau}\left(\eta_{\mu \nu} \frac{\mathrm{d} x^{\mu}}{\mathrm{d} \tau} \frac{\mathrm{d} x^{\nu}}{\mathrm{d} \tau}\right)=0,
$$
and $\eta_{\mu \nu} \frac{\mathrm{d} x^{\mu}}{\mathrm{d} \tau} \frac{\mathrm{d} x^{\nu}}{\mathrm{d} \tau}$ is independent of proper time.