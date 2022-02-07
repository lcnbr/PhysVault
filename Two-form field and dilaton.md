# Two-form field and dilaton

What about the [[closed string spectrum#First Level|other]] (massless) fields: two-form $B_{\mu \nu}$ and dilaton scalar $\Phi$ ? If we view them as fields in/of the background manifold, can we couple them to the string action as well?
## [[Kalb-Ramond 2-form]]
The two-form naturally couples via antisymmetric combination of [[worldsheet]] derivatives

$$
\frac{1}{2 \pi \kappa^{2}} \int \mathrm{d} \xi^{2} \frac{1}{2} B_{\mu \nu}(X) \varepsilon^{\alpha \beta} \partial_{\alpha} X^{\mu} \partial_{\beta} X^{\nu}=\frac{1}{2 \pi \kappa^{2}} \int B .
$$

In fact, this is the canonical coupling of a two-dimensional [[worldsheet]] to a two-form in direct analogy to the coupling of a charged particle worldline to the electromagnetic field. The string carries a two-form charge as we shall see a little later.
## [[dilaton]]
The dilaton couples to the [[worldsheet]] Riemann scalar

$$
\frac{1}{4 \pi} \int \mathrm{d} \xi^{2} \sqrt{-\operatorname{det} g} \Phi(X) R[g] .
$$

This is interesting for several reasons:

- The [[Euler characteristic]] $\chi$ of the [[worldsheet]] appears.
- The coupling is not [[Weyl invariance|weyl invariant]].
- The scalar can mix with gravity.
- We can get away from 26 dimensions.

Let us discuss them in more detail below.

# Low-Energy Effective Action. 
First we discuss the various beta functions ([[curved backgrounds#Anomaly|trace of the renormalised stress-energy tensor $T$]] ) which appear in string theory coupled to a generalised background consisting of $G, B$ and $\Phi$ (c.f. [[Graviton vertex operator#Background Metric Construction]])

$$
\begin{aligned}
g^{\alpha \beta} T_{\alpha \beta}=&-\frac{1}{2 \kappa^{2}}\left(\sqrt{-\operatorname{det} g} \beta_{\mu \nu}^{G} g^{\alpha \beta}+\beta_{\mu \nu}^{B} \varepsilon^{\alpha \beta}\right) \partial_{\alpha} X^{\mu} \partial_{\beta} X^{\nu} \\
&-\frac{1}{2} \beta^{\Phi} R[g],
\end{aligned}
$$

where

$$
\begin{aligned}
\beta_{\mu \nu}^{G} &=\kappa^{2} R_{\mu \nu}+2 \kappa^{2} D_{\mu} D_{\nu} \Phi-\frac{1}{4} \kappa^{2} H_{\mu \rho \sigma} H_{\nu}{ }^{\rho \sigma}, \\
\beta_{\mu \nu}^{B} &=-\frac{1}{2} \kappa^{2} D^{\lambda} H_{\mu \nu \lambda}+\kappa^{2} D^{\lambda} \Phi H_{\mu \nu \lambda}, \\
\beta^{\Phi} &=-\frac{1}{2} \kappa^{2} D_{\mu} D^{\mu} \Phi+\kappa^{2} D^{\mu} \Phi D_{\mu} \Phi-\frac{1}{24} \kappa^{2} H_{\mu \nu \rho} H^{\mu \nu \rho} .
\end{aligned}
$$

Quantum consistency of ([[conformal invariance|conformal symmetry]] in) string theory requires $\beta^{G}=\beta^{B}=\beta^{\Phi}=0$  . These are the standard equations for a [[graviton]], a two-form field and a scalar. They follow from an action in spacetime

$$
S \sim \int \mathrm{d} x^{26} \sqrt{-\operatorname{det} G} \mathrm{e}^{-2 \Phi}\left(R-\frac{1}{12} H_{\mu \nu \rho} H^{\mu \nu \rho}+4 \partial^{\mu} \Phi \partial_{\mu} \Phi\right) .
$$

This is the string theory low-energy effective action. It encodes the low-energy physics of string theory viewed from the perspective of the background. Note that there are further corrections from curvature $(\kappa)$ and loops $\left(g_{\mathrm{s}}\right)$ not displayed here.

The anomaly equations have the trivial solution $G=\eta, B=0, \Phi=\Phi_{0}$ which describes a flat background. The solution equally applies to torus compactification to effectively reduce the number of dimensions.

# String Coupling. 
Suppose $\Phi=\Phi_{0}$ is constant, then the dilaton coupling term is topological

$$
\int \mathrm{d} \xi^{2} \sqrt{-\operatorname{det} g} R[g] \sim \chi .
$$

It measures the [[Euler characteristic]] $\chi=2 h-2$ of [[worldsheet]].

Set $g_{\mathrm{s}}=e^{i \Phi_{0}}$. Then the generating functional yields precisely $\chi$ factors of $g_{\mathrm{s}}$.

$$
\mathrm{e}^{i S} \simeq \mathrm{e}^{i \Phi_{0} \chi}=g_{\mathrm{s}}^{\chi} .
$$

The expansion in this $g_{\mathrm{s}}$ thus corresponds to an expansion in [[worldsheet]] topology

![](https://cdn.mathpix.com/cropped/2022_01_21_6a05ef3b6320b8a7606bg-05.jpg?height=108&width=644&top_left_y=1103&top_left_x=295)

For general curved backgrounds, the string coupling $g_{\mathrm{s}}$ is determined by the asymptotic behaviour of the background, namely the asymptotic value $\Phi_{0}$ of dilaton field $\Phi$.

# String Frame. 
Notice the unusual factor of $\exp (-2 \Phi)$ in the above effective action $S$.

The scalar degrees of freedom can mix with the gravitational degrees of freedom. We may as well define a rescaled metric

$$
G_{\mu \nu}^{\prime}=f(\Phi) G_{\mu \nu} .
$$

With a suitable choice of $f$ we can remove the factor $\exp (-2 \Phi)$. We can go from the so-called string frame with $\exp (-2 \Phi)$ to the so-called Einstein frame where we recover the canonical kinetic term for each field. Non-Critical Strings. We have seen earlier that $D \neq 26$ breaks [[Weyl invariance|Weyl symmetry]] of the string action. Furthermore it is broken by the above anomalies. Therefore both anomalies should appear in the same place. In fact, $D$ enters in the effective action as a cosmological constant

$$
S=\ldots\left(R-\frac{1}{12} H_{\mu \nu \rho} H^{\mu \nu \rho}+4 \partial^{\mu} \Phi \partial_{\mu} \Phi-\frac{2}{3} \kappa^{-2}(D-26)\right)
$$

This implies that we can have $D<26$, but it requires a spacetime curvature at the Planck scale.

# Dilaton Scaling. 
We note two further peculiarities: The dilaton coupling to the [[worldsheet]] is not [[Weyl invariance|Weyl invariant]] and it has an unconventional power of $\kappa$.

The factor of $\kappa$ moves the classical Weyl breakdown effectively to one loop. There it can cancel against the quantum anomalies of other fields. Together this furnishes a consistent choice of normalisation.