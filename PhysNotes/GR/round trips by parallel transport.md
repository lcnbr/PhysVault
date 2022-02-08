---
alias: 
- round trip
tag: GR physics
---

![[Pasted image 20220205191545.png#leftwrap|100]]

Let us now think of a closed trajectory (e.g. a gyroscope moving in orbit around the earth).
The question we would like to investigate is by how much the [[spin in GR|spin]]-vector (or any other [[parallel transport|parallely transported]] vector) will be changed after completing a full orbit, returning back to the same point. To start, we will consider small closed curves. The [[affine connection]] can be expanded as
$$
\Gamma^\mu{}_{\nu \rho}(x)=\Gamma^\mu{}_{\nu \rho}(X)+\left(x^{\alpha}-X^{\alpha}\right) \frac{\partial \Gamma^\mu{}_{\nu \rho}}{\partial x^{\alpha}}(X)+\cdots
$$
where $X^{\alpha} \equiv x^{\alpha}\left(\tau_{0}\right)$ is a point on the curve. The [[parallel transport#^diffEq|differential equation]]  for [[parallel transport]] gives
$$
\begin{aligned}
\frac{S_{\mu}(\tau)-S_{\mu}\left(\tau_{0}\right)}{\tau-\tau_{0}} & \simeq \Gamma^\alpha{}_{\mu\rho} \frac{x^{\rho}(\tau)-x^{\rho}\left(\tau_{0}\right)}{\tau-\tau_{0}} S_{\alpha}\left(\tau_{0}\right) \\
S_{\mu}(\tau) &=S_{\mu}\left(\tau_{0}\right)+\Gamma^\alpha{}_{\mu\rho}(X)\left(x^{\rho}(\tau)-X^{\rho}\right) S_{\alpha}\left(\tau_{0}\right)+\cdots
\end{aligned}
$$
This is an approximation. We can improve on it by one order. Let us return to the original differential equation
$$
\begin{aligned}
\frac{\mathrm{d} S_{\mu}}{\mathrm{d} \tau} &=\Gamma^\alpha{}_{\mu\rho} S_{\alpha} \frac{\mathrm{d} x^{\rho}}{\mathrm{d} \tau} \\

\int_{\tau_{0}}^{\tau} \mathrm{d} S_{\mu} &=\int_{\tau_{0}}^{\tau}\dd{\tau} \Gamma^\alpha{}_{\mu\rho} S_{\alpha} \frac{\mathrm{d} x^{\rho}}{\mathrm{d} \tau} \\

\Rightarrow S_{\mu}(\tau) &=S_{\mu}\left(\tau_{0}\right)+\int_{\tau_{0}}^{\tau}\dd{\tau} \Gamma^\alpha{}_{\mu\rho} S_{\alpha} \frac{\mathrm{d} x^{\rho}}{\mathrm{d} \tau} \\

& \approx S_{\mu}\left(\tau_{0}\right)+\int_{\tau_{0}}^{\tau}\dd{\tau}\left[\Gamma^\alpha{}_{\mu\rho}(X)+\frac{\partial \Gamma^\alpha{}_{\mu\rho}}{\partial x^{\beta}}(X)\left(x^{\beta}-X^{\beta}\right)+\cdots\right] \\

& \qquad\cdot\left[S_{\alpha}\left(\tau_{0}\right)+\Gamma^\gamma{}_{\alpha \delta}(X)\left(x^{\delta}-X^{\delta}\right) S_{\gamma}(x)+\cdots\right] \cdot \frac{\mathrm{d} x^{\rho}}{\mathrm{d} \tau}\\

& \approx S_{\mu}\left(\tau_{0}\right)+\Gamma^\alpha{}_{\mu\rho}(X) S_{\alpha}\left(\tau_{0}\right) \int_{\tau_{0}}^{\tau}\dd{\tau} \frac{\mathrm{d} x^{\rho}}{\mathrm{d} \tau} \\

&\qquad+\left[\frac{\partial \Gamma^\alpha{}_{\mu\rho}}{\partial x^{\beta}}(X) S_{\alpha}\left(\tau_{0}\right)+\Gamma^\omega{}_{\mu \rho}(X) \Gamma^\alpha{}_{\omega \beta}(X) S_{\alpha}\left(\tau_{0}\right)\right] \int_{\tau_{0}}^{\tau}\dd{\tau}\left(x^{\beta}-X^{\beta}\right) \frac{\mathrm{d} x^{\rho}}{\mathrm{d} \tau}
\end{aligned}
$$
For a closed loop
$$
\oint \mathrm{d} \tau \frac{\mathrm{d} x^{\rho}}{\mathrm{d} \tau}=0
$$
Thus, the change in the vector becomes
$$
\Delta S_{\mu}=\left[\frac{\partial \Gamma^\alpha{}_{\mu\rho}}{\partial x^{\beta}}(X)+\Gamma^\omega{}_{\mu \rho} \Gamma^\alpha{}_{\omega \beta}\right] \oint \mathrm{d} \tau \frac{\mathrm{d} x^{\rho}}{\mathrm{d} \tau} x^{\beta}
$$
Notice that the term in brackets resembles the [[Riemann curvature tensor#^RiemannTensor|Riemann tensor]] and that the integral is antisymmetric in $\rho \leftrightarrow \beta$. Indeed,
$$
\begin{aligned}
\oint \mathrm{d} \tau \frac{\mathrm{d} x^{\rho}}{\mathrm{d} \tau} x^{\beta} &=\oint \mathrm{d} \tau\left[\frac{\mathrm{d}}{\mathrm{d} \tau}\left(x^{\rho} x^{\beta}\right)-x^{\rho} \frac{\mathrm{d} x^{\beta}}{\mathrm{d} \tau}\right] \\
&=-\oint \mathrm{d} \tau x^{\rho} \frac{\mathrm{d} x^{\beta}}{\mathrm{d} \tau}
\end{aligned}
$$
We can then write, using antisymmetry,
$$
\Delta S_{\mu}=\frac{1}{2} R^\alpha{}_{\mu \rho \beta}(X) S_{\alpha}(X) \oint \mathrm{d} \tau \frac{\mathrm{d} x^{\rho}}{\mathrm{d} \tau} x^{\beta} .
$$

We conclude that if $R_{\mu \nu \rho}^{\alpha}=0 \Rightarrow \Delta S_{\mu}=0$, there is no change in the vector.
![[Pasted image 20220205193809.png#leftwrap|150]]We have worked with small closed curves. If the [[Riemann curvature tensor|Riemann tensor]] vanishes in a big region, we can split it up into smaller cells. As in the proof of Stokes theorem, the common contributions from neighbouring cells will cancel out, leaving only contributions from the external boundary. Thus, the vector will be unchanged in any full orbit over any closed loop.
![[Pasted image 20220205194247.png#leftwrap|150]]Consider now the transition from a point $x\left(\tau_{0}\right)$ to $x\left(\tau_{1}\right)$ via two different paths, if the [[Riemann curvature tensor|Riemann tensor]] vanishes, then the change of the vector will be independent of the path $\Delta S_{A}=\Delta S_{B}$ (green and blue arrow would coincide)