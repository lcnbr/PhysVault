Consider a clock which is at rest in our lab-frame. We will assume that the clock is inside a non-zero gravitational field. We would like to compare its ticking rate with the ticking rate that the same clock has when it is also at rest in absence of the gravitational field.

$$\left.\Delta t\right|_{\text {gravity \& at rest }} \quad \text{vs}\left.\quad \Delta t\right|_{\text {no gravity \& at rest }}$$
To perform this comparison we will use the [[principle of equivalence|equivalence principle]]. First, we will perform a coordinate transformation (not a [[Lorentz transformation]]) which will have the effect to cancel gravity in the spacetime region of the clock ($S_{\text{einstein}}$). Second, we will perform a [[Lorentz transformation]] which will bring us to an equivalent [[inertial frames of reference|inertial frame]] with gravity cancelled out and the clock at rest: $S'_{\text{einstein}}$. Schematically:
![[Untitled 4.svg#center|600]]
In the $S'_{\text{einstein}}$ frame, the time interval in between two ticks of the clock is also a [[infinitesimal proper time interval in SR|proper time interval]]
$$
\mathrm{d} \xi^{\prime 0}=\mathrm{d} \tau
$$
because the clock is at rest as viewed in an [[instantaneous rest frame]].
However, the proper time interval is the same for all inertial observers and thus
$$
\mathrm{d} \tau=\mathrm{d} \xi^{\prime 0}=\sqrt{\eta_{\mu \nu} \mathrm{d} \xi^{\mu} \mathrm{d} \xi^{\nu}} .
$$
Now it remains to make our [[general coordinate transformation]] which expresses $\mathrm{d} \tau$ (the ticking time interval at rest and in the absence of gravitation) to the spacetime intervals which separate two successive tickings in our lab-frame. We get
$$
\begin{aligned}
\mathrm{d} \tau &=\sqrt{\eta_{\mu \nu} \mathrm{d} \xi^{\mu} \mathrm{d} \xi^{\nu}}=\sqrt{\underbracket{\eta_{\mu \nu} \frac{\partial \xi^{\mu}}{\partial x^{\rho}} \frac{\partial \xi^{\nu}}{\partial x^{\sigma}}}_{=g_{\rho \sigma}} \mathrm{d} x^{\rho} \mathrm{d} x^{\sigma}} \\
&=\sqrt{g_{\rho \sigma}(x) \mathrm{d} x^{\rho} \mathrm{d} x^{\sigma}} .
\end{aligned}
$$
In the lab-frame the clock is at rest, $\mathrm{d} x^{1}=\mathrm{d} x^{2}=\mathrm{d} x^{3}=0, \mathrm{~d} x^{0} \equiv \Delta t \neq 0$. Thus

$$
\begin{aligned}
\mathrm{d} \tau &=\sqrt{g_{00}(x) \mathrm{d} x^{0} \mathrm{~d} x^{0}}=\sqrt{g_{00}(x)} \Delta t \\
\Rightarrow \Delta t &=\frac{\mathrm{d} \tau}{\sqrt{g_{00}(x)}}
\end{aligned}
$$

^grTimedilation

Here $\Delta t$ is the time elapsed in between ticks of the clock at rest inside the gravitational field and $\mathrm{d} \tau$ is the time elapsed in between ticks of the clock at rest outside the gravitational field.

[[#^grTimedilation]] allows to make a comparison of clock rates when placed at rest at various places within the gravitational field. This is more practical than taking our clock to a place with no gravity. For two points $x_{A}$ and $x_{B}$ we have
$$
\begin{aligned}
\Delta t_{A} &=\frac{\mathrm{d} \tau}{\sqrt{g_{00}\left(x_{A}\right)}}, \quad \Delta t_{B}=\frac{\mathrm{d} \tau}{\sqrt{g_{00}\left(x_{B}\right)}}, \\
\Rightarrow \frac{\Delta t_{A}}{\Delta t_{B}} &=\sqrt{\frac{g_{00}\left(x_{B}\right)}{g_{00}\left(x_{A}\right)}} .
\end{aligned}
$$
The ticking frequency of the clocks $\nu \equiv(\Delta t)^{-1}$ is then
$$
\begin{aligned}
\frac{\nu_{B}}{\nu_{A}} &=\sqrt{\frac{g_{00}\left(x_{B}\right)}{g_{00}\left(x_{A}\right)}}, \\
\Rightarrow \nu_{B} &=\nu_{A} \sqrt{\frac{g_{00}\left(x_{B}\right)}{g_{00}\left(x_{A}\right)}} .
\end{aligned}
$$
Let us now go to [[Newtonian limit]]. We use [[Newtonian limit#^newtonMetric]]. Thus, in a weak field $\nu_{B} \approx \nu_{A}\left(1+2 \phi\left(x_{B}\right)\right)^{1 / 2}\left(1+2 \phi\left(x_{A}\right)\right)^{-1 / 2}$, or, after a Taylor expansion
$$
v_{B} \approx \nu_{A}\left(1+\phi\left(x_{B}\right)-\phi\left(x_{A}\right)\right)
$$
This equation applies not only to traditional clocks. It refers to the frequency of all processes. For example, $\nu_{A}$ and $\nu_{B}$ could refer to the frequency of light produced with identical mechanisms (same atomic transitions) at points $A$ and $B$ in spacetime. Let us choose $A$ to be a point at the surface of the earth $\oplus$ and $B$ a point at the surface of the sun $\odot$. Then
$$
\nu_{\odot} \approx \nu_{\oplus}\left(1+\phi_{\odot}-\phi_{\oplus}\right) .
$$
We already calculated the gravitational field of the earth on its surface to be about $\phi_{\oplus} \approx-10^{-9}$. The sun has mass which is about $10^{6}$ times the mass of the earth and a radius which is about $10^{3}$ times the radius of the earth. We then have (very rough back of the envelope computation)
$$
\phi_{\odot} \approx \frac{10^{6}}{10^{3}} \phi_{\oplus} \approx-10^{-6}
$$
We conclude that
$$
\nu_{\odot} \approx \nu_{\oplus}\left(1-10^{-6}\right), \quad \Rightarrow \frac{\nu_{\odot}-\nu_{\oplus}}{\nu_{\oplus}} \approx-10^{-6} .
$$
For a photon in the optical spectrum, this corresponds to a red-shift (negative) by one millionth. This is really tiny and difficult to discern, but there have been measurements which are consistent which such a shift.