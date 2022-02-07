---
alias: divergence
tag: GR physics
---

Consider a contravariant vector $V^{\mu}$. Its covariant divergence is
$$
V^\mu{}_{; \mu}=\frac{\partial V^{\mu}}{\partial x^{\mu}}+\Gamma^\mu{}_{\mu \rho} V^{\rho} .
$$

Using [[affine connection#^DetContraction|determinant form]] of the [[affine connection#Contraction]], thedivergence becomes:

$$
\begin{aligned}
V^\mu{}_{; \mu} &=\frac{\partial V^{\mu}}{\partial x^{\mu}}+\Gamma^\mu{}_{\mu \rho} V^{\rho} \\
&=\frac{\partial V^{\mu}}{\partial x^{\mu}}+\frac{1}{\sqrt{g}}\left(\frac{\partial}{\partial x^{\rho}} \sqrt{g}\right) V^{\rho} \\
\Rightarrow V^\mu{}_{; \mu} &=\frac{1}{\sqrt{g}} \frac{\partial}{\partial x^{\mu}}\left(\sqrt{g} V^{\mu}\right)
\end{aligned}
$$
We now can deduce a covariant form of Gauss's Theorem. If $V^{\mu}$ vanishes at infinity, we have
$$
\begin{aligned}
& \int \mathrm{d}^{4} x \partial_{\mu}\left(\sqrt{g} V^{\mu}\right)=0 \\
\Rightarrow & \int \underbracket{\mathrm{d}^{4} x \sqrt{g}}_{\text {invariant }} \underbracket{V^\mu{}_{; \mu}}_{\text {cov. deriv. }}=0
\end{aligned}
$$
Exercise: How does $V^\mu{}_{; \mu}$ transform under general coordinate transformations? Recall $\sqrt{g}$ is a [[densities|scalar density]] of weight $-1$, and reusing the determinant trick, we show that it is a [[scalar fields in GR|scalar]]!