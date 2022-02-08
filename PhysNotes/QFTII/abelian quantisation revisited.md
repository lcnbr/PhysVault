---
alias:
tags:
- qftII
---
Before we can quantise the [[N QED fields|Yang-Mills]] theory, we should first discuss the path integral formulation of electrodynamics. In QFT I, we have noticed that gauge invariance makes the naive vector field propagator ill-defined. The solution was to break gauge invariance by adding a gauge-fixing term. We will now consider how to achieve this in the path integral formulation.



[[path integral for EM]]
[[gauge fixing for EM]]
[[gauge fixing action for EM]]

# Discussion. 

Finally, we have recovered the Lagrangian of the electromagnetic field with the [[gauge fixing action for EM#^e09c3f|standard Lorenz gauge-fixing term]]. Up to some infinite but constant prefactors the new path integral is equal to the original [[path integral for EM]]
$$
\begin{aligned}
Z[J] &=\int \mathrm{D} A \exp \left(i {S_{\mathrm{EM}}}[A, J]\right) \\
&=\text { const } \cdot \int \mathrm{D} A \exp \left(i S_{\mathrm{EM}}[A, J]+i S_{\mathrm{gf}}[A]\right)
\end{aligned}
$$
Since all constant prefactors drop out of correlation functions, we can use the action with gauge-fixing term as the starting point for quantising electrodynamics.

Note, however, that the path integrals are only equivalent when the source field $J$ is conserved. Therefore, only correlation functions of gauge invariant combinations of the fields are meaningful in the gauge-fixed form. ^[Of course we may also compute more general correlation functions, but these are potentially unrelated to the original path integral and thus meaningless.]

We have used a modified Lorenz gauge condition $\partial \cdot A=\Omega$ where $\Omega$ is an auxiliary dynamical field. This field is governed by a [[gauge fixing action for EM#^4fe3a4|free Lagrangian]] without derivative terms which essentially force it (quantum mechanically close) to zero. This resulting gauge fixing of the electrodynamics Lagrangian is also known as $R_{\xi}$ - gauge. The parameter $\xi$ can be fixed at will, and no physical, gauge-invariant quantities may depend on it. A convenient choice is $\xi=1$ for Feynman gauge or the limit $\xi \rightarrow 0$ (after quantisation) for Landau gauge.

The resulting Feynman propagator for the vector field in momentum space is (c.f. [[Free Scalar Field]])
$$
\left(G_{\mathrm{F}}\right)_{\mu \nu}(p)=\frac{\eta_{\mu \nu}-(1-\xi) p_{\mu} p_{\nu} / p^{2}}{p^{2}-i \epsilon}
$$
Note that this propagator does not respect the strict Lorenz gauge as can be seen by contracting the propagator with $p^{\mu}$
$$
p^{\mu}\left(G_{\mathrm{F}}\right)_{\mu \nu}(p)=\frac{\xi p_{v}}{p^{2}-i \epsilon} .
$$
This term would have to be zero in a strict Lorenz gauge, nevertheless it is acceptable because the result is proportional $p_{v}$. The above relationship can be understood better when formulated in position space
$$
i\left\langle\partial \cdot A(x) A_{v}(x)\right\rangle=\xi \partial_{y, v} G_{\mathrm{F}}(x-y)=\partial_{v} \alpha_{x}(y) .
$$
The correlator of $\partial \cdot A$ with another gauge field yields a result which is proportional to a gauge transformation of the other gauge field by $\alpha_{x}(y)=\xi G_{\mathrm{F}}(x-y)$ which is effectively trivial. In practice, the nonvanishing term does not matter since the other side of the propagator should couple to a conserved current such as $J^{\mu}$.