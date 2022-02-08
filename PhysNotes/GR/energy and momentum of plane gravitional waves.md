---
alias:
tag: GR physics
---

We remind that we can rewrite [[Einstein's field equations|Einstein's equations]]
![[Einstein's field equations#^EinsteinfieldEq|Einstein's equation]]
as
![[energy, momentum and angular momentum with gravity#^newEinstein]]
with ![[energy, momentum and angular momentum with gravity#^LinG]] and ![[energy, momentum and angular momentum with gravity#^newT]]

where $R\ind{(1)}{\mu\nu}$ is the [[Ricci tensor#weak field approximation|linear part of the Ricci tensor]], $R^{(1)}\equiv \eta^{\mu\nu}R\ind{(1)}{\mu\nu}$ is the [[Ricci scalar#Weak field approximation|linear part of the curvature scalar]].
We showed in [[energy, momentum and angular momentum with gravity]] that:
![[energy, momentum and angular momentum with gravity#^tCons]]

and we have thus associated $t^{\mu\nu}$ to the energy-momentum tensor of matter and gravitation. For plane waves $T_{\mu\nu}=0$ (empty space) and we can therefore write
$$
    -8\pi Gt_{\mu\nu} = -R_{\mu\nu}+\frac{g_{\mu\nu}}{2}R+R\ind{(1)}{\mu\nu}-\frac{\eta_{\mu\nu}}{2}R^{(1)}.
$$
We can decompose the [[Ricci tensor]] in powers of $h_{\mu\nu}$, where $g_{\mu\nu} = \eta_{\mu\nu} + h_{\mu\nu}$. We write
$$
    R_{\mu\nu} = R\ind{(1)}{\mu\nu}+R\ind{(2)}{\mu\nu}+\cdots.
$$
Then
$$
\begin{split}
    8\pi Gt_{\mu\nu} &= \left(R\ind{(1)}{\mu\nu}+R\ind{(2)}{\mu\nu}+\cdots\right)-\frac{\eta_{\mu\nu}+h_{\mu\nu}}{2}\left(\eta^{\alpha\beta}+h^{\alpha\beta}\right)\left(R\ind{(1)}{\alpha\beta}+R\ind{(2)}{\alpha\beta}+\cdots\right) \\
    &\qquad -R\ind{(1)}{\mu\nu}+\frac{\eta_{\mu\nu}}{2}\eta^{\alpha\beta}R\ind{(1)}{\alpha\beta} \\
    &\approx R\ind{(2)}{\mu\nu}-\frac{\eta_{\mu\nu}\eta^{\alpha\beta}}{2}R\ind{(2)}{\alpha\beta}-\frac{\eta_{\mu\nu}h^{\alpha\beta}+h_{\mu\nu}\eta^{\alpha\beta}}{2}R\ind{(1)}{\alpha\beta}+\mathcal{O}(h^3).
\end{split}
$$
Plane wave solutions satisfy the linearized Einstein equation:

![[solutions of the linearized field equations#^hSolHom]]

Therefore the energy-momentum tensor associated to a gravitational wave is of second order in the weak field approximation and reads
$$
\begin{split}
    t_{\mu\nu} &\approx \frac{1}{8\pi G}\left[R\ind{(2)}{\mu\nu}-\frac{1}{2}\eta_{\mu\nu}\eta^{\alpha\beta}R\ind{(2)}{\alpha\beta}\right] \\
    &= \frac{1}{8\pi G}\left[\delta\ind{\alpha}{\mu}\delta\ind{\beta}{\nu}-\frac{1}{2}\eta_{\mu\nu}\eta^{\alpha\beta}\right]R\ind{(2)}{\alpha\beta}.
\end{split}
$$
With an explicit calculation ($\rightarrow$Exercise) we find 
$$
\begin{split}
    R\ind{(2)}{\mu\kappa} = -\frac{1}{2}h^{\lambda\nu}R\ind{(1)}{\lambda\nu}\eta_{\mu\kappa} &+ \frac{1}{4}\left[2\frac{\partial h\ind{\nu}{\sigma}}{\partial x^\nu}-\frac{\partial h\ind{\nu}{\nu}}{\partial x^\sigma}\right]\left[\frac{\partial h\ind{\sigma}{\mu}}{\partial x^\kappa}+\frac{\partial h\ind{\sigma}{\kappa}}{\partial x^\mu}-\frac{\partial h_{\mu\kappa}}{\partial x^\sigma}\right] \\ 
    & - \frac{1}{4}\left[\frac{\partial h_{\sigma\kappa}}{\partial x^\lambda}+\frac{\partial h_{\sigma\lambda}}{\partial x^\kappa}-\frac{\partial h_{\lambda\kappa}}{\partial x^\sigma}\right]\left[\frac{\partial h\ind{\sigma}{\mu}}{\partial x_\lambda}+\frac{\partial h^{\sigma\lambda}}{\partial x^\mu}-\frac{\partial h\ind{\lambda}{\mu}}{\partial x_\sigma}\right].
\end{split}
$$
In the above we raise and lower indices with the Minkowski part of the metric only. The first term vanishes due to $R\ind{(1)}{\mu\nu}=0$. The second part vanishes due to the [[solutions of the linearized field equations#^HarmCond|harmonic coordinate condition]]

The last line needs to be computed explicitly, substituting the wave solution
![[solutions of the linearized field equations#^ansatz]]
We will need products of the type
$$
\begin{split}
    \frac{\partial h_{\alpha\beta}}{\partial x^\gamma}\frac{\partial h_{\mu\nu}}{\partial x^\rho} &= \im k_\gamma\left(\varepsilon_{\alpha\beta}e^{+\im k\cdot x}-\varepsilon\ind{\ast}{\alpha\beta}e^{-\im k\cdot x}\right)\im k_\rho\left(\varepsilon_{\mu\nu}e^{+\im k\cdot x}-\varepsilon\ind{\ast}{\mu\nu}e^{-\im k\cdot x}\right) \\
    &= -k_\gamma k_\rho\left[\varepsilon_{\alpha\beta}\varepsilon_{\mu\nu}e^{+2\im k\cdot x}+\varepsilon\ind{\ast}{\alpha\beta}\varepsilon\ind{\ast}{\mu\nu}e^{-2\im k\cdot x}-\varepsilon_{\alpha\beta}\varepsilon\ind{\ast}{\mu\nu}-\varepsilon\ind{\ast}{\alpha\beta}\varepsilon_{\mu\nu}\right].
\end{split}
$$

^8c7014

We can now average the energy and momentum over the period of the wave. The averaging will require integrals of the form
$$
    \int_0^T\dd{t}e^{\pm4\pi\im t/T}=0.
$$
Then, we are left with 
$$
    \left\langle\frac{\partial h_{\alpha\beta}}{\partial x^\gamma}\frac{\partial h_{\mu\nu}}{\partial x^\rho}\right\rangle = k_\nu k_\rho\left(\varepsilon_{\alpha\beta}\varepsilon\ind{\ast}{\mu\nu}+\varepsilon\ind{\ast}{\alpha\beta}\varepsilon_{\mu\nu}\right).
$$
Taking the average then yields
$$
    \left\langle R\ind{(2)}{\mu\nu}\right\rangle = \cdots = \frac{k_\mu k_\nu}{2}\left(\varepsilon^{\ast\lambda\rho}\varepsilon_{\lambda\rho}-\frac{1}{2}\left|\varepsilon\ind{\lambda}{\lambda}\right|\right).
$$

Then
$$
    8\pi G\left\langle t_{\mu\nu}\right\rangle\approx \langle R\ind{(2)}{\mu\nu}\rangle - \frac{\eta^{\mu\nu}}{2}\langle\underbracket{R^{(1)}}_{=0}\rangle=\frac{k_\mu k_\nu}{2}\left(\varepsilon^{\ast\lambda\rho}\varepsilon_{\lambda\rho}-\frac{1}{2}\left|\varepsilon\ind{\lambda}{\lambda}\right|\right).
$$

^timeAvgT

Notice that $\left\langle t_{\mu\nu}\right\rangle$ is a gauge invariant. Under
$$
    \varepsilon_{\mu\nu}\to\varepsilon\ind{\prime}{\mu\nu} = \varepsilon_{\mu\nu}+k_\mu\varepsilon_\nu+k_\nu\varepsilon_\mu,
$$
we have
$$
    \varepsilon^{\ast\mu\nu}\varepsilon_{\mu\nu} = \varepsilon^{\ast\mu\nu}\varepsilon_{\mu\nu}+2k_\mu k_\nu\varepsilon^{\ast\mu}\varepsilon^\nu + 2k_\mu\mathrm{Re}[\varepsilon\ind{\ast}{\nu}\varepsilon^{\mu\nu}],
$$
and
$$
\begin{split}
    \varepsilon\ind{\mu}{\mu}&\to \varepsilon\ind{\mu}{\mu}+2k_\mu\varepsilon^\mu \\
    \left|\varepsilon\ind{\mu}{\mu}\right|^2&\to\left|\varepsilon\ind{\mu}{\mu}\right|^2+4\mathrm{Re}[k_\nu\varepsilon^{\ast\nu}\varepsilon\ind{\mu}{\mu}]+4\mathrm{Re}[k_\mu\varepsilon\ind{\ast}{\nu}\varepsilon^{\mu\nu}],
\end{split}
$$
which leaves
$$
    \varepsilon^{\ast\mu\nu}\varepsilon_{\mu\nu}-\frac{1}{2}\left|\varepsilon\ind{\lambda}{\lambda}\right|\to\varepsilon^{\ast\mu\nu}\varepsilon_{\mu\nu}-\frac{1}{2}\left|\varepsilon\ind{\lambda}{\lambda}\right|,
$$
invariant. If we take $k^\mu=k(1,0,0,1)$ and choose the gauge so that $\varepsilon_{11},\varepsilon_{12}\neq0$ and all other $\varepsilon_{\mu\nu}=0$, we have

$$
    \left\langle t_{\mu\nu}\right\rangle = \frac{k_\mu k_\nu}{8\pi G}\left[\left|\varepsilon_{11}\right|^2+\left|\varepsilon_{12}\right|^2\right] = \frac{k_\mu k_\nu}{16\pi G}\left[\left|e_+\right|^2+\left|e_-\right|^2\right],
$$

^timeAverageTsimple

with

$$
    e_\pm = \varepsilon_{11}\mp\im\varepsilon_{12}.
$$

^ePM


Exercise: Compare with the corresponding expression for an electromagnetic wave.

The continuity equation gives
$$
    \partial_\mu t^{\mu\nu} =0\ \Rightarrow\ \frac{\partial t^{0\nu}}{\partial t}+\frac{\partial t^{i\nu}}{\partial x^i}=0.
$$
For $\nu=0$ we have
$$
\begin{split}
    \frac{\partial }{\partial t}\left\langle t^{00}\right\rangle &= -\frac{\partial}{\partial x^i}\left\langle t^{0i}\right\rangle \\
    \Rightarrow\ \frac{\partial}{\partial t}\int_V\dd[3]{x}t^{00}  &= -\int_V\dd[3]{x}\frac{\partial}{\partial x^i}t^{0i} \\
    \Rightarrow\ \frac{\partial E}{\partial t} &= -\int_{S(V)}\dd{S} \hat{n}_it^{0i},
\end{split}
$$

^dadd12

the energy flux.

We will soon see that sources (mass distributions) in limited regions of space give rise to spherical gravitational waves. Considering a volume $V$ with surface $S(V)$ far away from the source, the above integral gives us the total power of radiation
$$
    P_{\mathrm{rad}} = -\int_{S(V)}\dd{S}\hat{n}_it^{0i}.
$$
Note that in [[electrodynamics in GR|Electrodynamics]] $t^{00}$ corresponds to the energy density of an electromagnetic wave while $t^{0i}$ is the Poynting vector. 
For a spherical volume $\dd{S}=r^2\dd{\Omega}$
$$
\begin{split}
    P_{\mathrm{rad}} &= \int\dd{\Omega}\dv{P_{\mathrm{rad}}}{\Omega} \\
    &= -\int\dd{\Omega} r^2n_i\left\langle t^{0i}\right\rangle \\
    \Rightarrow\ \dv{ P_{\mathrm{rad}}}{\Omega} &= -r^2n_i\left\langle t^{0i}\right\rangle.
\end{split}
$$

Now we can explore the [[generation of gravitional waves]]
