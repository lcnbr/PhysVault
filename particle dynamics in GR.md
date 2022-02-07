---
alias:
tag: GR physics
---

In the absence of gravity, for an [[inertial frames of reference|inertial observer]]  with coordinates $\left\{\xi^{\mu}\right\}$, the four-velocity of a particle is
$$
V^{\mu}=\frac{\mathrm{d} \xi^{\mu}}{\mathrm{d} \tau} .
$$
For a free particle, the equations of motion [[particle dynamics in SR|read]]

$$
\frac{\mathrm{d} V^{\mu}}{\mathrm{d} \tau}=0 .
$$

^inertialEOM

In the presence of gravity, the four-velocity is in a "lab"-frame with coordinates $\left\{x^{\alpha}\right\}$. We can also define a four-velocity vector (under [[general coordinate transformation|general coordinate transformations]])
$$
V^{\mu} \equiv \frac{\mathrm{d} x^{\mu}}{\mathrm{d} \tau} .
$$
This equation is not covariant under [[general coordinate transformation|general coordinate transformations]]. We can make it covariant by replacing the derivative with a [[covariant derivative#Along a curve]]. An appropriate equation reads
$$
\begin{align}
\frac{\mathrm{D} V^{\mu}}{\mathrm{D} \tau}=0 \\
\Leftrightarrow \frac{\mathrm{d} V^{\mu}}{\mathrm{d} \tau}+\Gamma^{\mu}{ }_{\rho \sigma} V^{\rho} \frac{\mathrm{d} x^{\sigma}}{\mathrm{d} \tau}=0 \\
\Leftrightarrow \frac{\mathrm{d}^{2} x^{\mu}}{\mathrm{d} \tau}+\Gamma^{\mu}{ }_{\rho \sigma} \frac{\mathrm{d} x^{\rho}}{\mathrm{d} \tau} \frac{\mathrm{d} x^{\sigma}}{\mathrm{d} \tau}=0
\end{align}
$$

^genericEOM

which is what we had [[principle of equivalence#^eomGeneric|found]] by a more direct use of the [[principle of equivalence]].
It is easy to verify that the above equation $\left(\frac{\mathrm{DV}^{\mu}}{\mathrm{D} \tau}=0\right)$ satisfies the principle of equivalence. Indeed if we perform a coordinate transformation which brings us into a locally inertial frame in which gravity is cancelled at any point, it collapses back into [[#^inertialEOM]] $\left(g_{\mu \nu} \rightarrow \eta_{\mu \nu}, \Gamma^{\mu}{ }_{\rho \sigma} \rightarrow 0\right)$. The existence of such transformations is guaranteed by the covariance of [[#^genericEOM]] under general coordinate transformations.

What happens to an attached vector? Consider [[spin in GR]]