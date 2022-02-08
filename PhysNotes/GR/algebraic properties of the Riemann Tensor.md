---
alias:
- algebraic properties
tag: GR physics
---
# Algebraic properties


The [[Riemann curvature tensor|Riemann tensor]] is given by
$$
R^\mu{}_{\nu \rho \sigma}=\frac{\partial \Gamma^\mu{}_{\nu \rho}}{\partial x^{\sigma}}+\Gamma^\alpha{}_{\nu \rho} \Gamma^\mu{}_{\alpha\sigma}-\frac{\partial \Gamma^\mu{}_{\nu\sigma}}{\partial x^{\rho}}-\Gamma^\alpha{}_{\nu \sigma} \Gamma^\mu{}_{\alpha \rho},
$$
where the [[affine connection]] is given by
$$
\Gamma^\mu{}_{\nu \rho}=g^{\mu \alpha} \Gamma_{\alpha \nu \rho} $$
and
$$ \Gamma_{\alpha \nu \rho}=\frac{1}{2}\left[\frac{\partial g_{\alpha \nu}}{\partial x^{\rho}}+\frac{\partial g_{\alpha \rho}}{\partial x^{\nu}}-\frac{\partial g_{\nu \rho}}{\partial x^{\alpha}}\right]
$$
Let us lower the first index
$$
R_{\mu \nu \rho \sigma}=g_{\mu \alpha} R^\alpha{}_{\nu \rho \sigma} .
$$
After some straightforward algebra, using that
$$
0=\frac{\partial \delta^{\mu}{ }_{\beta}}{\partial x^{\sigma}}=\frac{\partial}{\partial x^{\sigma}}\left(g^{\mu \alpha} g_{\alpha \beta}\right) \rightarrow g_{\alpha \beta} \frac{\partial}{\partial x^{\sigma}} g^{\mu \alpha}=-g^{\mu \alpha} \frac{\partial}{\partial x^{\sigma}} g_{\alpha \beta}
$$
we find
$$
R_{\mu \nu \rho \sigma}=\frac{\partial \Gamma_{\mu \nu \rho}}{\partial x^{\sigma}}-\frac{\partial \Gamma_{\mu \nu \sigma}}{\partial x^{\rho}}+\Gamma^\beta{}_{\nu \rho} \Gamma_{\beta \mu \sigma}-\Gamma^\beta{}_{\nu \sigma} \Gamma_{\beta \mu \rho}
$$
or, more explicitly,

$$
R_{\mu \nu \rho \sigma}=\frac{1}{2}\left[
\frac{\partial^{2} g_{\mu \rho}}{\partial x^{\nu} \partial x^{\sigma}}
+\frac{\partial^{2} g_{\nu \sigma}}{\partial x^{\mu} \partial x^{\rho}}
-\frac{\partial^{2} g_{\nu \rho}}{\partial x^{\mu} \partial x^{\sigma}}
-\frac{\partial^{2} g_{\mu \sigma}}{\partial x^{\nu} \partial x^{\rho}}\right]+g_{\alpha \beta} \Gamma^\alpha{}_{\mu \sigma} \Gamma^\beta{}_{\nu \rho}-g_{\alpha \beta} \Gamma^\alpha{}_{\mu \rho} \Gamma^\beta{}_{\nu \sigma}
$$

^RiemannTensorDown

Remember the original [[Riemann curvature tensor#^RiemannTensor|Riemann tensor]]

We then find the following properties
## Symmetry
$$
R_{\mu \nu \rho \sigma}=R_{\rho \sigma \mu \nu}
$$
## Antisymmetry
$$
\begin{aligned}
&R_{\mu \nu \rho \sigma}=-R_{\mu \nu \sigma \rho} \\
&R_{\mu \nu \rho \sigma}=-R_{\nu \mu \rho \sigma}
\end{aligned}
$$
From the above it also follows that
$$
R_{\mu \nu \rho \sigma}=R_{\nu \mu \sigma \rho}
$$
## Cyclicity
$$
R^\mu{}_{\nu \rho \sigma}
+R^\mu{}_{\sigma \nu \rho}
+R^\mu{}_{\rho \sigma \nu}=0
$$