---
alias: 
- uniqueness of the Riemann tensor
- uniqueness of the curvature tensor
tag: GR physics
---
# Uniqueness of the [[Riemann curvature tensor]]
Proof: Focus on one point $X$ and erect a [[principle of equivalence|locally inertial frame]]. The [[affine connection]] vanishes at $X$ but not its derivatives
$$
\Gamma^{\alpha}{ }_{\mu \nu}=0 \text {, but } \frac{\partial \Gamma^{\mu}{ }_{\nu \rho}}{\partial x^{\sigma}} \neq 0 \text { in general. }
$$

Now consider a coordinate system transformation $x^{\prime} \rightarrow x$ which leave the [[affine connection]] zero at the point $X$. This is a subset of coordinate transformations. The [[affine connection]] transforms as [[transformation of the affine connection#^trans]] or with primes interchanged:
$$
\Gamma^{\mu}{ }_{\nu \rho}=\frac{\partial x^{\mu}}{\partial x^{\prime \alpha}} \frac{\partial x^{\prime \beta}}{\partial x^{\nu}} \frac{\partial x^{\prime \gamma}}{\partial x^{\rho}} \Gamma^{\prime \alpha}{ }_{\beta \gamma}+\frac{\partial x^{\mu}}{\partial x^{\prime \beta}} \frac{\partial^{2} x^{\prime \beta}}{\partial x^{\nu} \partial x^{\rho}},
$$
for a generic coordinate transformation. For the special point where $\Gamma^{\prime}=\Gamma=0$, we have
$$
\left(\frac{\partial^{2} x^{\prime \beta}(x)}{\partial x^{\nu} \partial x^{\rho}}\right)_{x=X}=0 .
$$
The derivative of the [[affine connection]], under these specialized transformations, transforms as
$$
\frac{\partial \Gamma^{\mu}{ }_{\nu \rho}}{\partial x^{\sigma}}=\underbrace{\frac{\partial x^{\mu}}{\partial x^{\prime \alpha}} \frac{\partial x^{\prime \beta}}{\partial x^{\nu}} \frac{\partial x^{\prime \gamma}}{\partial x^{\rho}} \frac{\partial x^{\prime \delta}}{\partial x^{\sigma}} \frac{\partial \Gamma^{\prime \alpha}{ }_{\beta \gamma}}{\partial x^{\prime \delta}}}_{\text {tensor-like }}-\underbrace{\frac{\partial^{3} x^{\mu}}{\partial x^{\prime \alpha} \partial x^{\prime \beta} \partial x^{\prime \gamma}} \frac{\partial x^{\prime \alpha}}{\partial x^{\nu}} \frac{\partial x^{\prime \beta}}{\partial x^{\rho}} \frac{\partial x^{\prime \gamma}}{\partial x^{\sigma}}}_{\text {non-tensor-like }} .
$$
So the derivative of the [[affine connection]] is clearly not a tensor. Can we formulate an object which is linear in the second derivative of the metric and transforms as a tensor (at least, for our special coordinate transformations above)? As the [[affine connection]] vanishes, the only objects available to us are its derivatives. We can write
$$
T^{\mu}{ }_{\nu \rho \sigma}=a_{1} \frac{\partial \Gamma^{\mu}{ }_{\nu \rho}}{\partial x^{\sigma}}+a_{2} \frac{\partial \Gamma^{\mu}{ }_{\rho \sigma}}{\partial x^{\nu}}+a_{3} \frac{\partial \Gamma^{\mu}{ }_{\sigma \nu}}{\partial x^{\rho}},
$$
which will therefore transform as
$$
T^{\mu}{ }_{\nu \rho \sigma}=\frac{\partial x^{\mu}}{\partial x^{\prime \alpha}} \frac{\partial x^{\prime \beta}}{\partial x^{\nu}} \frac{\partial x^{\prime \gamma}}{\partial x^{\rho}} \frac{\partial x^{\prime \delta}}{\partial x^{\sigma}} T^{\prime \alpha}{ }_{\beta \gamma \delta}-\left.\left(a_{1}+a_{2}+a_{3}\right) \frac{\partial^{3} x^{\mu}}{\partial x^{\prime \alpha} \partial x^{\prime \beta} \partial x^{\prime \gamma}} \frac{\partial x^{\prime \alpha}}{\partial x^{\nu}} \frac{\partial x^{\prime \beta}}{\partial x^{\rho}} \frac{\partial x^{\prime \gamma}}{\partial x^{\sigma}}\right|_{x=X} \text {. }
$$
For the non-tensorial part to vanish we must have $a_{3}=-a_{1}-a_{2}$. So, the general form is
$$
\begin{aligned}
\left.T^\alpha{}_{\mu \nu \rho}\right|_{x=X} &=a_{1}\left(\frac{\partial \Gamma^{\mu}{ }_{\nu \rho}}{\partial x^{\sigma}}-\frac{\partial \Gamma^{\mu}{ }_{\nu \sigma}}{\partial x^{\rho}}\right)_{x=X}+a_{2}\left(\frac{\partial \Gamma^{\mu}{ }_{\sigma \rho}}{\partial x^{\nu}}-\frac{\partial \Gamma^{\mu}{ }_{\sigma \nu}}{\partial x^{\rho}}\right)_{x=X} \\
&=\left.a_{1} R^\mu{}_{\nu \rho \sigma}\right|_{x=X}+\left.a_{2} R^\mu{}_{\sigma \nu \nu}\right|_{x=X} .
\end{aligned}
$$

**So, at the point $\mathrm{X}$ in our locally inertial reference frame, the only object which we can construct to behave as a tensor under our special coordinate transformations is the Riemann tensor (or a superposition of Riemann tensors).** Suppose there exists a second type of tensor $B^{\mu}{ }_{\nu \rho \sigma}$ which also is linear is the second derivative of the metric. At $x=X$ in the coordinates of our locally inertial frame we must have
$$
B^{\mu}{ }_{\nu \rho \sigma}=R^\mu{}_{\nu \rho \sigma} .
$$
But this is an identity among tensors. Then it should be valid generally. This concludes the proof of the uniqueness of the Riemann tensor, as the only tensor linearly dependent on the second derivative of the metric.

From the Riemann tensor we can create superpositions. The following ones are very interesting in General Relativity:
- [[Ricci tensor]]: $R_{\mu \nu} \equiv R_{\mu \alpha \nu}^{\alpha}$,
- Curvature scalar: $R \equiv g^{\mu \nu} R_{\mu \nu}$.

These will enter [[Einstein's field equations]], as we will see later on.

The value of the [[Riemann curvature tensor|curvature tensor]] affects what happens to a [[parallel transport|parallel transported]] [[tensor fields in GR|tensor]] if it [[round trips by parallel transport|completes a loop]]. Its value also crucially controls the *curvature*: