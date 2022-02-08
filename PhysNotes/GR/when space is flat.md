---
alias: 
tag: GR physics
---
# When is space flat?

In Minkowski spacetime, $g_{\mu \nu}(x)=\eta_{\mu \nu}$ and $\Gamma^\mu{}_{\nu \rho}=0$ everywhere, we have that the [[Riemann curvature tensor]] is zero. The opposite is also valid. One can show that
(i) if $R_{\mu \nu \rho}^{\alpha}=0$ and
(ii) the metric $g_{\mu \nu}(x)$ at a point $X$ has three negative and one positive eigenvalues (as $\eta_{\mu \nu}$ ), then the metric is the Minkowski metric everywhere, $g_{\mu \nu}(x)=\eta_{\mu \nu} \forall x$.

Proof: The [[metric tensor|metric]] [[matrix form from index notation|matrix]] is symmetric. We can always bring it to a diagonal form by finding an appropriate orthogonal matrix $O$, such as
$$
O \mathbf{g}O^{T}=D
$$
where $\mathbf{g}$ is the metric matrix and $D$ is diagonal. In components
$$
O^\alpha{}_{\mu} g^{\mu \nu} O^\beta{}_{\nu}=D^{\alpha \beta}=\left\{\begin{aligned}
D^{\alpha}, &\quad \alpha=\beta \\
0, &\quad \alpha \neq \beta
\end{aligned}\right.
$$
We have one positive and three negative eigenvalues. Let us then choose $D^{0}$ positive and $D^{1}, D^{2}, D^{3}$ negative. We can then normalize
$$
\begin{aligned}
&O^0{}_{\mu}=\sqrt{+D^{0}} d^0{}_{\mu} \\
&O^i{}_{\mu}=\sqrt{-D^{i}} d^i{}_{\mu}
\end{aligned}
$$
Then the diagonalization equation takes the form
$$
g^{\mu \nu}(x) d^\alpha{}_{\mu}(x) d^{\beta}{ }_{\nu}(x)=\eta^{\alpha \beta}
$$
Let us now define a quantity $D^\alpha{}_{\mu}(x)$ at an arbitrary point $x$ to satisfy (to have vanishing [[covariant derivative]], as [[one-forms in GR|covectors]] indexed by $\alpha$)
$$
\frac{\partial D^\alpha{}_{\mu}(x)}{\partial x^{\nu}}=\Gamma^\lambda{}_{\mu \nu}(x) D^\alpha{}_{\lambda}(x)
$$

with a boundary condition $D^\alpha{}_{\mu}(X)=d^\alpha{}_{\mu}$. Let us now consider the [[covariant derivative]]
$$
\left(g^{\mu \nu} D^\alpha{}_{\mu} D^\beta{}_{\nu}\right)_{; \lambda}=2 g^{\mu \nu} \underbrace{D^\alpha{}_{\mu ; \lambda}}_{=0} D^\beta{}_{\nu}=0 .
$$

Where we used [[covariant derivative#Leibniz rule]] and that $g^{\mu \nu}{}_{;\alpha}=0$
But $g^{\mu \nu} D^\alpha{}_{\mu} D^\beta{}_{\nu}$ is a [[scalar fields in GR|scalar]] since the metric is contracted, and the remaining indices run over constant eigenvalues. So, its [[covariant derivative]] equals its normal derivative. Thus we have shown that
$$
\begin{aligned}
\frac{\partial}{\partial x^{\lambda}}\left(g^{\mu \nu} D^\alpha{}_{\mu} D^\beta{}_{\nu}\right) &=0 \\
\Rightarrow g^{\mu \nu}(x) D^\alpha{}_{\mu}(x) D^\beta{}_{\nu}(x) &=g^{\mu \nu}(X) D^\alpha{}_{\mu}(X) D^\beta{}_{\nu}(X) \\
&=g^{\mu \nu}(X) d^\alpha{}_{\mu} d^{\beta}{ }_{\nu} \\
&=\eta^{\alpha \beta}
\end{aligned}
$$
Thus there is a coordinate transformation encoded in $D^\alpha{}_{\mu}(x)$ which rotates the metric to the Minkowskian metric. The appropiate coordinate transformation $(x \rightarrow \xi)$ is
$$
\frac{\partial \xi^{\alpha}}{\partial x^{\mu}}=D^\alpha{}_{\mu}
$$
Then
$$
g^{\mu \nu}(x) \frac{\partial \xi^{\alpha}}{\partial x^{\mu}} \frac{\partial \xi^{\beta}}{\partial x^{\nu}}=\eta^{\alpha \beta}
$$
which is the correct tensor transformation. In the above derivation we have made a crucial assumption. That is, that a solution of
$$
\frac{\partial D^\alpha{}_{\mu}}{\partial x^{\nu}}=\Gamma_{\mu \nu}^{\lambda} D_{\lambda}^{\alpha},
$$
does exist at every point in spacetime. We can guarantee that if $R^{\alpha}{ }_{\mu \nu \rho}=0$ .  Let us consider a general equation of this form
$$
\frac{\partial S_{\mu}(x)}{\partial x^{\nu}}=\Gamma_{\mu \nu}^{\lambda} S_{\lambda}(x),
$$
for a general vector field $S_{\mu}(x)$ defined everywhere in spacetime. Now let us consider an arbitrary curve $x^{\mu}(\tau)$. We can multiply with $\frac{\mathrm{d} x^{\nu}}{\mathrm{d} \tau}$ and then we obtain
$$
\begin{aligned}
\frac{\mathrm{d} S_{\mu}(x)}{\mathrm{d} x^{\nu}} \frac{\mathrm{d} x^{\nu}}{\mathrm{d} \tau} &=\Gamma_{\mu \nu}^{\lambda}(x) \frac{\mathrm{d} x^{\nu}}{\mathrm{d} \tau} S_{\lambda}(x) \\
\Leftrightarrow \frac{\mathrm{d} S_{\mu}}{\mathrm{d} \tau} &=\Gamma_{\mu \nu}^{\lambda}(x) \frac{\mathrm{d} x^{\nu}}{\mathrm{d} \tau} S_{\lambda}(x(\tau)) .
\end{aligned}
$$
This can be solved uniquely. If $S_{\mu}(x)$ exists we can obtain a unique solution $S_{\mu}(x)$ independent of how we choose to connect $X$ and $x$ since if the  [[Riemann curvature tensor|Riemann tensor]] vanishes, [[parallel transport]] is invariant of path c.f. [[round trips by parallel transport]].