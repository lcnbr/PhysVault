---
alias: 
- curvature tensor
- Riemann tensor
tag: GR physics
---

To generalise [[determining the metric#^poissonEq|the poisson equation]] we are searching for a tensor with a second derivative of the metric. One such [[tensor fields in GR|tensor]] emerges in the following commutator
$$
A_{\mu ; \nu ; \rho}-A_{\mu ; \rho ; \nu}
$$
where $A_{\mu}$ is a [[vector fields in GR|vector]]. We have
$$
\begin{aligned}
A_{\mu ; \nu ; \rho} &=\left(A_{\mu ; \nu}\right)_{ ; \rho}=
\frac{\partial}{\partial x^{\rho}} A_{\mu ; \nu}
-\Gamma^{\alpha}{ }_{\mu \rho} A_{\alpha ; \nu}
-\Gamma^{\alpha}{ }_{\nu \rho} A_{\mu ; \alpha} \\

&=\frac{\partial}{\partial x^{\rho}}\left(\frac{\partial A_{\mu}}{\partial x^{\nu}}
-\Gamma^{\beta}{ }_{\mu \nu} A_{\beta}\right)-\Gamma^{\alpha}{ }_{\mu \rho}\left(\frac{\partial A_{\alpha}}{\partial x^{\nu}}
-\Gamma^{\beta}{ }_{\alpha \nu} A_{\beta}\right)-\Gamma^{\alpha}{ }_{\nu \rho}\left(\frac{\partial A_{\mu}}{\partial x^{\alpha}}
-\Gamma^{\beta}{ }_{\mu \alpha} A_{\beta}\right) \\

&=\underbracket{\frac{\partial^{2} A_{\mu}}{\partial x^{\nu} \partial x^{\rho}}
-\Gamma^{\alpha}{ }_{\mu \nu} \frac{\partial A_{\alpha}}{\partial x^{\rho}}
-\Gamma^{\alpha}{ }_{\mu \rho} \frac{\partial A_{\alpha}}{\partial x^{\nu}}
-\Gamma^{\alpha}{ }_{\nu \rho} \frac{\partial A_{\mu}}{\partial x^{\alpha}}}_{\text{symmetric under exchange }\nu \leftrightarrow \rho}
 \\
&+\Gamma^{\alpha}{ }_{\nu \rho} \Gamma^{\beta}{ }_{\mu \alpha} A_{\beta}-\left(\frac{\partial \Gamma^{\beta}{ }_{\mu \nu}}{\partial x^{\rho}}
-\Gamma^{\alpha}{ }_{\mu \rho} \Gamma^{\beta}{ }_{\alpha \nu}\right) A_{\beta} .
\end{aligned}
$$

Taking the commutator we eliminate the symmetric part and obtain:

$$
A_{\mu ; \nu ; \rho}-A_{\mu ; \rho ; \nu}=-R_{\mu \nu \rho}^{\beta} A_{\beta},
$$

^RiemannComm

with


$$
R^\beta{}_{\mu \nu \rho} \equiv \frac{\partial \Gamma^{\beta}{ }_{\mu \nu}}{\partial x^{\rho}}-\frac{\partial \Gamma^{\beta}{ }_{\mu \rho}}{\partial x^{\nu}}-\Gamma^{\alpha}{ }_{\mu \rho} \Gamma^{\beta}{ }_{\alpha \nu}+\Gamma^{\alpha}{ }_{\mu \nu} \Gamma^{\beta}{ }_{\alpha \rho},
$$


^RiemannTensor


the so called [[Riemann curvature tensor]]. It is indeed a tensor, as the left-hand side of [[#^RiemannComm]] is a tensor and $A_{\beta}$ in the right-hand side is a vector. 
Similarly, we can find that
$$
V^\mu{}_{; \nu ; \rho}-V^\mu{}_{; \rho ; \nu}=R^\mu{}_{\beta \nu \rho} V^{\beta},
$$

and for tensors (as an example)
$$
T^\lambda{}_{\mu ; \nu ; \kappa}-T^\lambda{}_{\mu ; \kappa ; \nu}=R^\lambda{}_{\sigma \nu \kappa}T^\sigma{}_{\mu}-R^\sigma{}_{\mu \nu \kappa} T^\lambda{}_{\sigma} \text { etc.. }
$$

^9f35dc

**Thus the [[Riemann curvature tensor|curvature tensor]] measures the amount with which [[covariant derivative]]s don't commute! If it vanishes, then they do commute, which is the mark of flat space, i.e no curvature** 

The curvature tensor is very special. We will prove that it is unique, i.e it is the only tensor which can be constructed from the metric, its first and its second derivatives and it is linear in the second derivative of the metric $\left(\rightarrow\right.$ contains $\left.\nabla^{2} \phi\right)$ ! The [[uniqueness of the Riemann curvature tensor|uniqueness of the Riemann tensor]] will be essential for generalizing the Poisson equation of Newtonian mechanics to the field equations of Einstein. 

As stated above the [[Riemann curvature tensor|curvature tensor]] measures the deviation from flatness by seeing how much derivatives don't commute. But when can we be sure that space is in fact flat?:  [[when space is flat]]. 

The Riemann tensor has very nice [[algebraic properties of the Riemann Tensor|algebraic properties]], and thus give rise to two important objects as linear combinations of the [[Riemann curvature tensor|Riemann tensor]]: 

- [[Ricci tensor]]
- [[Ricci scalar]]

Finally there are the [[Bianchi identities]]