---
alias:
tags:
- qftII
---
 Let us briefly summarise the equation of motion for non-abelian gauge theory. They directly reflect the equations of motion for [[../GR/electrodynamics in GR|electrodynamics]], but due to the non-abelian nature of the gauge group, the partial derivatives need to be replaced by covariant derivatives.

The homogeneous Maxwell equation, also known as a Bianchi identity, derives from the [[../math/Lie bracket|Jacobi identity]] of three covariant derivatives. For Yang-Mills theory it can be written as
$$
\left[D_{\rho}, F_{\mu \nu}\right]+\left[D_{\nu}, F_{\rho \mu}\right]+\left[D_{\mu}, F_{\nu \rho}\right]=0 \quad \text { or } \quad \varepsilon^{\mu v \rho \sigma}\left[D_{\rho}, F_{\mu \nu}\right]=0 .
$$

# [[YM covariant derivative]]

![[YM covariant derivative#For a Gauge field]]

# Gauge eom
The extension of the inhomogeneous Maxwell equation reads
$$
\frac{2}{g_{\mathrm{YM}}^{2}}\left[D_{\mu}, F^{\mu \nu}\right]=J^{v} .
$$
The current $J^{v}$ is a hermitian $N \times N$ matrix of fermion bilinears
$$
\left(J^{v}\right)^{i}{ }_{k}=i \bar{\psi}_{k} \gamma^{v} \psi^{i} .
$$

# Matter eom
Finally, the matter equations of motion take the usual Dirac form with a [[YM covariant derivative|covariant derivative]] to replace the ordinary one
$$
\left(D^{\mu} \gamma_{\mu}-m\right)^{i}{ }_{k} \psi^{k}=0 .
$$
Note that the equations of motion imply that the current is covariantly conserved
$$
\left[D_{\mu}, J^{\mu}\right]=0
$$