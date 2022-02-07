---
alias:
tag: GR physics
---

The [[Einstein's field equations|Einstein's equations]]
![[Einstein's field equations#^EinsteinfieldEq|Einstein's equation]]
or, equivalently,
![[Einstein's field equations#^EinsteinEqWithoutR|Einstein's equation]]
with $\Lambda=0$ admit wave solutions. We can see this by looking at these equations in the weak field approximation. Namely, we take the metric to be a Minkowskian background and a small perturbation
$$
    g_{\mu\nu} = \eta_{\mu\nu} + h_{\mu\nu},
$$
with $h_{\mu\nu}$ small. The [[Ricci tensor]] is
![[Ricci tensor#^weeakApprox]]
To fix the ambiguity of choosing a coordinate system ('gauge'), we impose the [[coordinate conditions#^harmCoordCond|harmonic coordinate conditions]]
$$
\begin{split}
    g^{\alpha\beta}\Gamma\ind{\mu}{\alpha\beta} &=0 \\
    (\eta^{\alpha\beta}+h^{\alpha\beta})\frac{1}{2}(\eta^{\mu\rho}+h^{\mu\rho})\left[\frac{\partial h_{\alpha\rho}}{\partial x^\beta}+\frac{\partial h_{\beta\rho}}{\partial x^\alpha}-\frac{\partial h_{\alpha\beta}}{\partial x^\rho}\right] &= 0 \\
    \eta^{\mu\rho}\eta^{\alpha\beta}\left[2\frac{\partial h_{\alpha\rho}}{\partial x^\beta}-\frac{\partial h_{\alpha\beta}}{\partial x^\rho}\right]+ \mathcal{O}(h^2)&= 0 \\
    \eta^{\alpha\beta}\frac{\partial h_{\alpha\rho}}{\partial x^\beta} &= \frac{1}{2}\frac{\partial h_{\alpha\beta}}{\partial x^\rho}\eta^{\alpha\beta} + \mathcal{O}(h^2).
\end{split}
$$
Thus
$$
    \eta^{\alpha\beta}\frac{\partial^2h_{\alpha\mu}}{\partial x^\nu\partial x^\beta} \approx \frac{1}{2}\frac{\partial^2h_{\alpha\beta}}{\partial x^\mu\partial x^\nu}\eta^{\alpha\beta},
$$
and
$$
    \eta^{\alpha\beta}\frac{\partial^2h_{\beta\nu}}{\partial x^\mu\partial x^\alpha} \approx \frac{1}{2}\frac{\partial^2h_{\alpha\beta}}{\partial x^\mu\partial x^\nu}.
$$
With these two relations the expression for the linearized Ricci tensor simplifies to
$$
    R^{(1)}{}_{\mu\nu} = \frac{1}{2}\eta^{\alpha\beta}\frac{\partial^2h_{\mu\nu}}{\partial x^\alpha\partial x^\beta} = \frac{1}{2}\Box_{SR} h_{\mu\nu}.
$$
For a system of harmonic coordinates, Einstein's linearized equations become

$$
\begin{align}
    \square_{SR} h_{\mu\nu} &= -16\pi G\overbracket{(T_{\mu\nu}-\frac{g_{\mu\nu}}{2}T\ind{\alpha}{\alpha})}^{S_{\mu \nu}}  \\
    \frac{\partial h\ind{\alpha}{\mu}}{\partial x^\alpha}&=\frac{1}{2}\frac{\partial h\ind{\alpha}{\alpha}}{\partial x^\mu}. 
\end{align}
$$
^linearizedEq

Where raising and lowering indices has been done with the [[Minkowski metric]]. Now we need to [[solutions of the linearized field equations|solve these equations]]


