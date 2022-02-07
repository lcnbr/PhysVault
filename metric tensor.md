---
alias: 
- metric
tags: GR physics math
---
Following the [[principle of equivalence|PoE]] discussion we introduced the metric tensor:

![[principle of equivalence#^metric|PoE]]

and in terms of the [[infinitesimal proper time interval in SR|proper time]]:

![[principle of equivalence#^prorTimeGeneric|PoE]]


# Inverse
If the [[general coordinate transformation|coordinate transform]] $\xi^{\alpha} \rightarrow x^{\alpha}$ can be inverted, which is what one expects physically, then the metric has an inverse
$$
g^{\mu \nu} \equiv \eta^{\rho \sigma} \frac{\partial x^{\mu}}{\partial \xi^{\rho}} \frac{\partial x^{\nu}}{\partial \xi^{\sigma}}
$$
Indeed,
$$
\begin{aligned}
g^{\mu \rho} g_{\rho \nu} &=\left(\eta^{\alpha \beta} \frac{\partial x^{\mu}}{\partial \xi^{\alpha}} \frac{\partial x^{\rho}}{\partial \xi^{\beta}}\right)\left(\eta_{\gamma \delta} \frac{\partial \xi^{\gamma}}{\partial x^{\rho}} \frac{\partial \xi^{\delta}}{\partial x^{\nu}}\right) \\
&=\eta^{\alpha \beta} \eta_{\gamma \delta} \frac{\partial x^{\mu}}{\partial \xi^{\alpha}} \frac{\partial \xi^{\delta}}{\partial x^{\nu}} \underbrace{\frac{\partial x^{\rho}}{\partial \xi^{\beta}} \frac{\partial \xi^{\gamma}}{\partial x^{\rho}}}_{=\frac{\partial \xi^{\gamma}}{\partial \xi^{\beta}}=\delta^{\gamma}{ }_{\beta}} \\
&=\cdots=\delta_{\nu}^{\mu}, \quad
\end{aligned}
$$
where the dots signify only the contractions done in the missing steps. In particular these are, in order, metric with Kronecker delta, metric with metric, the resulting delta with $\xi$ differential and the derivatives with each other.