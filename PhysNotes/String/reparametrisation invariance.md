---
Alias:
- reparametrisation invariant
- diffeomorphism invariance
- diffeomorphism invariant
---
If a space is paramatrised by some coordinates $\xi$, such as [[worldsheet#worldsheet coordinates]] then [[.md|reparametrisation invariance]] is the freedom to choose any monotonic function of the $\xi$s , then the object in question stays the same. 

We call a local diffeomorphism invariance, when the object is invariant under^[[[broedela-3 Classical Bosonic String#^b320ec]]]: 
$$\xi^{\alpha} \mapsto \tilde{\xi}^{\alpha}=\xi^{\alpha}-\epsilon^{\alpha}(\xi)$$

Reparameterization invariance, also known as diffeomorphisms. This is a [[../QFTII/gauge symmetry]] on the [[worldsheet]]. We may redefine the [[worldsheet]] coordinates as $\xi^{\alpha} \rightarrow \tilde{\xi}^{\alpha}(\xi)$. The fields $X^{\mu}$ transform as [[worldsheet]] scalars, while $g_{\alpha \beta}$ transforms in the manner appropriate for a $2 \mathrm{~d}$ metric.
$$
\begin{aligned}
&X^{\mu}(\xi) \rightarrow \tilde{X}^{\mu}(\tilde{\xi})=X^{\mu}(\xi) \\
&g_{\alpha \beta}(\xi) \rightarrow \tilde{g}_{\alpha \beta}(\tilde{\xi})=\frac{\partial \xi^{\gamma}}{\partial \tilde{\xi}^{\alpha}} \frac{\partial \xi^{\delta}}{\partial \tilde{\xi}^{\beta}} g_{\gamma \delta}(\xi)
\end{aligned}
$$
It will sometimes be useful to work infinitesimally. If we make the coordinate change $\xi^{\alpha} \rightarrow \tilde{\xi}^{\alpha}=\xi^{\alpha}-\eta^{\alpha}(\xi)$, for some small $\eta$. The transformations of the fields then become,
$$
\begin{aligned}
&\delta X^{\mu}(\xi)=\eta^{\alpha} \partial_{\alpha} X^{\mu} \\
&\delta g_{\alpha \beta}(\xi)=\nabla_{\alpha} \eta_{\beta}+\nabla_{\beta} \eta_{\alpha}
\end{aligned}
$$
where the [[../GR/covariant derivative]] is defined by $\nabla_{\alpha} \eta_{\beta}=\partial_{\alpha} \eta_{\beta}-\Gamma_{\alpha \beta}^{\xi} \eta_{\xi}$ with the [[Levi-Civita connection]] associated to the [[worldsheet]] metric given by the usual expression,
$$
\Gamma_{\alpha \beta}^{\xi}=\frac{1}{2} g^{\xi \rho}\left(\partial_{\alpha} g_{\beta \rho}+\partial_{\beta} g_{\rho \alpha}-\partial_{\rho} g_{\alpha \beta}\right)
$$