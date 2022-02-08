---
alias:
- tensor densities
- tensor density
- scalar density
- scalar densities
- tensor density fields
- tensor density field
tag: GR physics
---
# Scalar Density #definition 
Consider the determinant of the metric
$$
g \equiv-\operatorname{det}\left(g_{\mu \nu}\right) .
$$
Under a [[general coordinate transformation]], it transforms as
$$
\begin{aligned}
g \rightarrow g^{\prime} &=-\operatorname{det}\left((g_{\mu \nu})'\right)=-\operatorname{det}\left(\frac{\partial x^{\rho}}{\partial x^{\prime \mu}} g_{\rho \sigma} \frac{\partial x^{\sigma}}{\partial x^{\prime \nu}}\right) \\
&=-\operatorname{det}\left(g_{\rho \sigma}\right) \operatorname{det}\left(\frac{\partial x^{\rho}}{\partial x^{\prime \mu}}\right)^{2}=g\vqty{\frac{\partial x}{\partial x^{\prime}}}^{2} \\
&=g\left|\frac{\partial x^{\prime}}{\partial x}\right|^{-2},
\end{aligned}
$$
where $\vqty{\frac{\partial x^{\prime}}{\partial x}}$ is the Jacobian of the [[general coordinate transformation|generalized coordinate transformation]] i.e. the determinant of the [[contravariance and covariance#^coordInv|inverse basis change matrix]]. Then the determinant of the metric is not a [[scalar fields in GR|scalar]]. A quantity which is transformed as a scalar but with extra factors of the Jacobian is called a **scalar density**. Generically, a scalar density $\Omega$ transforms as
$$
\Omega \rightarrow \Omega^{\prime}=\Omega\left|\frac{\partial x^{\prime}}{\partial x}\right|^{w},
$$
where the $w$-power is called the *weight* of the scalar density. 



## Volume element #example
We observe that the 4-dimensional volume element is a scalar density of weight 1. Indeed,
$$
\mathrm{d}^{4} x \equiv \mathrm{d} x^{0} \mathrm{~d} x^{1} \mathrm{~d} x^{2} \mathrm{~d} x^{3} \rightarrow \mathrm{d}^{4} x^{\prime}=\left|\frac{\partial x^{\prime}}{\partial x}\right| \mathrm{d}^{4} x
$$
The combination $\sqrt{g} \mathrm{~d}^{4} x$ is invariant under [[general coordinate transformation|general coordinate transformations]]. Indeed,
$$
\sqrt{g} \mathrm{~d}^{4} x \rightarrow \sqrt{g^{\prime}} \mathrm{d}^{4} x^{\prime}=\sqrt{g\left|\frac{\partial x^{\prime}}{\partial x}\right|^{-2}} \mathrm{~d}^{4} x\left|\frac{\partial x^{\prime}}{\partial x}\right|=\sqrt{g} \mathrm{~d}^{4} x .
$$


# Tensor density
Similarly, we find objects which transform as [[tensor fields in GR|tensors]] with extra factors of the Jacobian.
$$
\Omega^{\mu_{1} \cdots}{}_{\nu_{1} \cdots} \rightarrow (\Omega^{ \mu_{1} \cdots}{}_{\nu_{1} \cdots})'=\frac{\partial x^{\prime \mu_{1}}}{\partial x^{\alpha_{1}}} \cdots \frac{\partial x^{\beta_{1}}}{\partial x^{\prime \nu_{1}}} \cdots\left|\frac{\partial x^{\prime}}{\partial x}\right|^{w} \Omega^{\alpha_{1} \cdots}{}_{\beta_{1} \cdots}
$$
The above defines a *tensor density of weight $w$*. Notice that we can turn a tensor density into a normal [[tensor fields in GR|tensor]] by multiplying it with an appropriate power of the determinant of the metric. Concretely,
$$
\begin{aligned}
g^{w / 2} \Omega^{\mu_{1} \cdots}{}_{\nu_{1} \cdots} \rightarrow g^{\prime w / 2} &\pqty{\Omega^{ \mu_{1} \cdots}{ }_{\nu_{1} \cdots}}'  \\
&=g^{w / 2}\left(\left|\frac{\partial x^{\prime}}{\partial x}\right|^{-2}\right)^{w / 2} \Omega^{\alpha_{1} \cdots}{ }_{\beta_{1} \cdots}\left|\frac{\partial x^{\prime}}{\partial x}\right|^{w}\left(\frac{\partial x^{\prime \mu_{1}}}{\partial x^{\alpha_{1}}}\right) \cdots\left(\frac{\partial x^{\beta_{1}}}{\partial x^{\prime \nu_{1}}}\right) \cdots \\
&=g^{w / 2} \Omega_{\beta_{1} \cdots}^{\alpha_{1} \cdots}\left(\frac{\partial x^{\prime \mu_{1}}}{\partial x^{\alpha_{1}}}\right) \cdots\left(\frac{\partial x^{\beta_{1}}}{\partial x^{\prime \nu_{1}}}\right) \cdots
\end{aligned}
$$

## Levi-Civita symbol

The fully antisymmetric Levi-Civita symbol is a tensor density. Consider the quantity
$$
\varepsilon^{\alpha \beta \gamma \delta} \frac{\partial x^{\prime \mu}}{\partial x^{\alpha}} \frac{\partial x^{\prime \nu}}{\partial x^{\beta}} \frac{\partial x^{\prime \rho}}{\partial x^{\gamma}} \frac{\partial x^{\prime \sigma}}{\partial x^{\delta}}=\text { const. } \varepsilon^{\mu \nu \rho \sigma} .
$$
For $\mu \nu \rho \sigma=0,1,2,3$ we obtain
$$
\text { const. }=\varepsilon^{\alpha \beta \gamma \delta} \frac{\partial x^{0}}{\partial x^{\alpha}} \frac{\partial x^{\prime 1}}{\partial x^{\beta}} \frac{\partial x^{\prime 2}}{\partial x^{\gamma}} \frac{\partial x^{\prime 3}}{\partial x^{\delta}}=\operatorname{det}\left(\frac{\partial x^{\prime}}{\partial x}\right)=\left|\frac{\partial x^{\prime}}{\partial x}\right|
$$
Thus
$$
\varepsilon^{\alpha \beta \gamma \delta} \frac{\partial x^{\prime \mu}}{\partial x^{\alpha}} \frac{\partial x^{\prime \nu}}{\partial x^{\beta}} \frac{\partial x^{\prime \rho}}{\partial x^{\gamma}} \frac{\partial x^{\prime \sigma}}{\partial x^{\delta}}=\left|\frac{\partial x^{\prime}}{\partial x}\right| \varepsilon^{\mu \nu \rho \sigma} .
$$
From the above we conclude that the Levi-Civita symbol is a tensor density.
Exercise: Proof that $\sqrt{g} \varepsilon^{\mu \nu \rho \sigma}$ is a [[tensor fields in GR|tensor]].