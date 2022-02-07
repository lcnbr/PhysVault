---
alias:
tag: GR physics
---

We have already proven that the [[Riemann curvature tensor|Riemann tensor]] and its linear combinations are the only possible tensors where second derivatives of the [[metric tensor|metric]] enter linearly. One such possible linear combination is the Ricci tensor
$$
R_{\mu \nu} \equiv R^{\alpha}{ }_{\mu \alpha \nu}=g^{\alpha \beta} R_{\alpha \mu \beta \nu} .
$$

^cd7107

The Ricci tensor is the only second rank tensor that can be formed, due to the antisymmetry of the Riemann tensor. Indeed,
$$
\underbrace{g^{\alpha \beta}}_{\text {symm. }} \underbrace{R_{\alpha \beta \gamma \delta}}_{\text {antisymm. }}=0, \text { etc.. }
$$

# Explicit form


From [[Riemann curvature tensor#^RiemannTensor|Riemann tensor]] we have:

$$
R_{\mu \rho}=\frac{\partial \Gamma^{\beta}{ }_{\mu \beta}}{\partial x^{\rho}}
-\frac{\partial \Gamma^{\beta}{ }_{\mu \rho}}{\partial x^{\beta}}
-\Gamma^{\alpha}{ }_{\mu \rho} \Gamma^{\beta}{ }_{\alpha \beta}
+\Gamma^{\alpha}{ }_{\mu \beta} \Gamma^{\beta}{ }_{\alpha \rho},
$$


# weak field approximation



Let us now compute the limit of weak gravitational fields. We can decompose $g_{\mu \nu} \approx \eta_{\mu \nu}+h_{\mu \nu}$ with a small $h_{\mu \nu}$ and. Then using the [[affine connection#Weak field approx|affine connection]] we have

$$
\begin{split}
    R_{\mu\nu} &= \frac{\partial\Gamma\ind{\alpha}{\mu\alpha}}{\partial x^\nu} - \frac{\partial\Gamma\ind{\alpha}{\mu\nu}}{\partial x^\alpha} + \mathcal{O}(h^2) \\
    &= \frac{\eta^{\alpha\rho}}{2}\left[ \frac{\partial}{\partial x^\nu}\left(\cancel{\frac{\partial h_{\mu\rho}}{\partial x^\alpha}} +\frac{\partial h_{\rho\alpha}}{\partial x^\mu} - \frac{\partial h_{\mu\alpha}}{\partial x^\rho}\right) - \frac{\partial}{\partial x^\alpha}\left(\cancel{\frac{\partial h_{\mu\rho}}{\partial x^\nu}} + \frac{\partial h_{\nu\rho}}{\partial x^\mu} - \frac{\partial h_{\mu\nu}}{\partial x^\rho}\right) \right] +\mathcal{O}(h^2) \\
    
\end{split}
$$


$$
\implies R_{\mu \nu}  = \frac{\eta^{\alpha\rho}}{2}\left[ \frac{\partial^2 h_{\rho\alpha}}{\partial x^\mu\partial x^\nu} + \frac{\partial^2 h_{\mu\nu}}{\partial x^\rho\partial x^\alpha} - \frac{\partial^2 h_{\mu\alpha}}{\partial x^\rho\partial x^\nu} - \frac{\partial^2 h_{\nu\rho}}{\partial x^\mu\partial x^\alpha} \right] + \mathcal{O}(h^2)=R^{(1)}{}_{\mu \nu}+ \mathcal{O}(h^2)
$$

^weeakApprox

We represent the linear part $R^{(1)}{}_{\mu \nu}$ as:

![[Pasted image 20220206160122.png#center|400]]