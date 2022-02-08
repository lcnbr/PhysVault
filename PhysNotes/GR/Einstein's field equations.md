---
alias:
- Einstein's equation
- Einstein's equations
tag: GR physics

---

We now have all the ingredients to build the relativistic generalization of Newton's law [[determining the metric#^poissonEq|poisson equation]]: $\nabla^{2} \phi=4 \pi G \rho$. As $\nabla^{2} \phi$ is contained inside the [[Riemann curvature tensor|Riemann tensor]] and $\rho=T^{00}$ inside the [[energy-momentum tensor in GR|energy-momentum tensor]] we can write an Ansatz of the form
$$
G^{\mu \nu}=c_{0} T^{\mu \nu},
$$
where $G_{\mu \nu}$ can be in general formed from the [[Riemann curvature tensor|Riemann tensor]] and the metric. As $T^{\mu \nu}=T^{\nu \mu}$, we expect $G^{\mu \nu}$ to be symmetric. Also, taking the [[covariant divergence]] of both sides, we have that
$$
G^{\mu \nu}{ }_{; \mu}=c_{0} T_{; \mu}^{\mu \nu} .
$$
In the absence of [[energy-momentum tensor in GR#^contEq|forces other than gravity]], we have $T^{\mu \nu}{}_{; \mu}=0$ and thus we must also have
$$
G^{\mu \nu}{ }_{; \mu}=0 .
$$
We have seen that the combination
$$
R^{\mu \nu}-\frac{1}{2} g^{\mu \nu} R
$$

has a [[Bianchi identities|vanishing covariant divergence]]. So, the most general rank- 2 tensor we can write is
$$
G^{\mu \nu}=R^{\mu \nu}-\frac{1}{2} g^{\mu \nu} R+\Lambda g^{\mu \nu},
$$
with $G^{\mu \nu}{ }_{; \mu}=0$. We have arrived at the equation

$$
R^{\mu \nu}-\frac{1}{2} g^{\mu \nu} R+\Lambda g^{\mu \nu}=c_{0} T^{\mu \nu}
$$

^anstazUp

or, with lower indices

$$
R_{\mu \nu}-\frac{1}{2} g_{\mu \nu} R+\Lambda g_{\mu \nu}=c_{0} T_{\mu \nu} .
$$

^anstazLow



# [[Newtonian limit]]

Let us now compute the limit of weak, static gravitational fields and slow, non-relativistic particles. We can decompose $g_{\mu \nu} \approx \eta_{\mu \nu}+h_{\mu \nu}$ with a small $h_{\mu \nu}$ and $\frac{\partial h_{\mu \nu}}{\partial x^{0}} \approx 0$ (static field approximation). Then the [[affine connection#From metric tensor metric|affine connection]] is


![[affine connection#^36c7d0]]
Terms of the form $\Gamma^{\alpha}{ }_{\mu \nu} \Gamma^{\beta}{ }_{\rho \sigma} \sim \mathcal{O}\left(h^{2}\right)$ can be dropped in the linear approximation. The [[Ricci tensor#Explicit form|Ricci tensor]] is then
![[Ricci tensor#^weeakApprox]]
The $R_{00}$ component will be of special interest. Ignoring $\frac{\partial h_{\mu \nu}}{\partial x^{0}}$ terms, within the static approximation, we have
$$
R_{00} \approx \frac{\eta^{j k}}{2} \frac{\partial h_{00}}{\partial x^{j} \partial x^{k}}=-\frac{1}{2} \nabla^{2} h_{00} .
$$
Then the $00$ LHS component of [[#^anstazLow]] is
$$
G_{00} \equiv R_{00}-\frac{1}{2} g_{00} R \approx R_{00}-\frac{1}{2} \eta_{00} R=R_{00}-\frac{R}{2},
$$
and thus [[#^anstazLow]]$_{00}$

$$
R_{00}-\frac{R}{2} \approx c_{0} T_{00}=c_{0} \rho
$$

^anstazLow00

Let us now focus on the space-components. Due to $\frac{\mathrm{d} x^{i}}{\mathrm{~d} t} \rightarrow 0$ we have $T_{i j} \ll T_{00}$ (slow moving on [[energy-momentum tensor in GR#^e30c90|energy momentum tensor]]). This then implies that:
$$
\begin{aligned}
R_{i j}-\frac{\eta_{i j}}{2} R & \approx 0 \\
R_{i j} & \approx \frac{\eta_{i j}}{2} R \\
R_{k k} & \approx-\frac{3}{2} R .
\end{aligned}
$$

The [[Ricci scalar|curvature scalar]] can now be approximated
$$
\begin{aligned}
& R=g^{\mu \nu} R_{\mu \nu}=R_{00}-R_{k k}=R_{00}+\frac{3}{2} R \\
\Rightarrow & R \approx-2 R_{00} .
\end{aligned}
$$
Thus, [[#^anstazLow00]] becomes
$$
\begin{aligned}
R_{00}-\frac{1}{2} R &=c_{0} \rho \\
R_{00} &=\frac{c_{0}}{2} \rho \\
-\nabla^{2} h_{00} &=c_{0} \rho
\end{aligned}
$$
It now remains to identify the $h_{00}$ metric perturbation with the Newtonian potential. This we have already done by comparing the equation of motion in the [[Newtonian limit]]. We have found that $h_{00} \approx 2 \phi$. Substituting into the above equation we obtain
$$
\nabla^{2} \phi=-\frac{c_{0}}{2} \rho \text {. }
$$
Comparing with the [[determining the metric#^poissonEq|poisson equation]]$\nabla^{2} \phi=4 \pi G \rho$ we can identify
$$
c_{0}=-8 \pi G .
$$

# Equation
Einstein's equations then read

$$
\boxed{R_{\mu \nu}-\frac{g_{\mu \nu}}{2} R+\Lambda g_{\mu \nu}=-8 \pi G T_{\mu \nu}}
$$

^EinsteinfieldEq

The constant $\Lambda$ is the so called cosmological constant. It contains no derivatives and it must have units of inverse length squared
$$
\Lambda \sim \frac{1}{\text { Length }^{2}} .
$$
Its introduction implies the existence of a physical length which must be very large as we do not observe significant deviations from Newton's gravity description at small length scales. However, at large scales the cosmological constant plays an important role, as it affects, for example, the expansion rate of the universe.

We can now find an alternative form of Einstein's equations elimintating the  [[Ricci scalar]]. By contracting the $\mu$ and $\nu$ indices, we find
    $$g^{\mu \nu}\left(R_{\mu \nu}-\frac{1}{2} g_{\mu \nu} R+\Lambda g_{\mu \nu}\right)=-8 \pi G T^{\mu}{ }_{\mu}$$ 
    $$R-\frac{4}{2} R+4 \Lambda=-8 \pi G T^{\mu}{ }_{\mu}$$
    $$8 \pi G T^{\mu}{ }_{\mu}+4 \Lambda=R .$$ 
Then, substituting the above into [[#^EinsteinfieldEq]] we have $$R_{\mu \nu}-\frac{g_{\mu \nu}}{2}\left(8 \pi G T^{\alpha}{ }_{\alpha}+4 \Lambda\right)+\Lambda g_{\mu \nu}=-8 \pi G T_{\mu \nu}$$

$$\boxed{R_{\mu \nu}=-8 \pi G\left(T_{\mu \nu}-T^{\alpha}{ }_{\alpha} \frac{g_{\mu \nu}}{2}\right)+\Lambda g_{\mu \nu}} .$$

^EinsteinEqWithoutR