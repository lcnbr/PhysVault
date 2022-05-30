# curved backgrounds

Consider strings propagating on a curved background described by the metric field $G_{\mu \nu}(x)$; a curious insight awaits.

The [[../String/3 Classical Bosonic String/Polyakov action#Action in conformal gauge|action in conformal gauge]] reads

$$
S=-\frac{1}{2 \pi \kappa^{2}} \int \mathrm{d} \xi^{2} \frac{1}{2} G_{\mu \nu}(X) \eta^{\alpha \beta} \partial_{\alpha} X^{\mu} \partial_{\beta} X^{\nu} .
$$

For a generic metric $G$, the equations of motion for $X$ are non-linear. This type of model is called a *non-linear sigma model*. The string background is called the *[[../String/embedding space|target space]]* of the model. The metric field $G_{\mu \nu}(x)$ acts as the coupling constants for the model. In fact, there are infinitely many coupling constants contained in the field $G(x)$ when Taylor expanding it around some point $x$.

In most QFT's, coupling constants need to be renormalised upon quantisation. The problem here is:

- The classical action has [[../String/conformal invariance|conformal symmetry]]. [[../String/conformal invariance|Conformal symmetry]] is indispensable to remove some degrees of freedom.

- The renormalised coupling $G(x, \mu)$ depends on a scale $\mu$ which is introduced by the quantisation or regularisation process. This new scale breaks quantum [[../String/conformal invariance]] of the string.

The behaviour of this regularisation scale is captured in what is called a $\beta$-function in quantum field theory: this describing the dependence of the coupling in question on the regularization scale. Conveniently, one can calculated the $\beta$-function using the so-called *[[background field method]]*, where one splits a field $X$ into a classical expectation value and a quantum correction,

$$
X=X_{0}+\kappa Y
$$

for which one derives Feynman rules and calculates UV-divergent terms up to a certain loop order. For the gravitational coupling $G_{\mu \nu}(x, \mu)$ one finds the (one-loop) $\beta$-function to read

$$
\frac{\mu \partial}{\partial \mu} G_{\mu \nu}(x, \mu)=\beta_{\mu \nu}(x)=\kappa^{2} R_{\mu \nu}, \quad R_{\mu \nu}=R^{\rho}{ }_{\mu \rho \nu},
$$

where $R^{\rho}{ }_{\mu \rho \nu}$ is the [[Riemann curvature tensor|Riemann tensor]] describing the local curvature of the [[../String/embedding space|target space]] manifold. The [[Riemann curvature tensor|Riemann tensor]] can be calculated from the (local) spacetime metric.

# Anomaly. 
We find that the stress-energy tensor has acquired a trace after renormalisation which is proportional to the above beta function: this is called conformal anomaly (or an anomaly of [[../String/Weyl invariance|Weyl symmetry]]):

$$
\eta^{\alpha \beta} T_{\alpha \beta}=-\frac{1}{2 \kappa^{2}} \beta_{\mu \nu} \eta^{\alpha \beta} \partial_{\alpha} X^{\mu} \partial_{\beta} X^{\nu} .
$$

We know that [[../String/Weyl invariance|Weyl symmetry]] is essential for obtaining the correct degrees of freedom for string theory. The only way to remove them and make string theory consistent is to set $\beta_{\mu \nu}=0$. Surprisingly, this yields the Einstein equation

$$
R_{\mu \nu}=0 .
$$

In other words, quantum strings can propagate only on Einstein backgrounds. We have thus found another way to recover general relativity from string theory, and we gain confidence that the spin-2 particles at level one are in fact [[../String/graviton|gravitons]]. 

# Higher Corrections. ... 
can again be calculated using the so-called [[background field method]]. They amount to the following two-loop beta function $^{3}$

$$
\beta_{\mu \nu}=\kappa^{2} R_{\mu \nu}+\frac{1}{2} \kappa^{4} R_{\mu \rho \sigma \kappa} R_{\nu}{ }^{\rho \sigma \kappa}+\ldots
$$

Absence of the conformal anomaly, $\beta_{\mu \nu}=0$, implies that in string theory the Einstein equations receive corrections at the Planck scale.