---
alias:
tag: GR physics
---

Let us consider the [[covariant derivative]] of a [[symmetries in GR|Killing vector]], $\xi_{\mu;\nu}$, which,[[Riemann curvature tensor#^9f35dc| as every second rank tensor, satisfies]]

$$
    \left(\xi_{\mu;\nu}\right)_{;\rho;\sigma}-\left(\xi_{\mu;\nu}\right)_{;\sigma;\rho} = -R\ind{\lambda}{\mu\rho\sigma}\xi_{\lambda;\nu}-R\ind{\lambda}{\nu\rho\sigma}\xi_{\mu;\lambda}.

$$

^2DerTens


Recall also that

![[symmetries in GR#^2ndDerKilling]]
Then [[#^2DerTens]] becomes 

$$
\begin{split}
    \left(-R\ind{\lambda}{\rho\nu\mu}\xi_\lambda\right)_{;\sigma} - \left(-R\ind{\lambda}{\sigma\mu\nu}\xi_\lambda\right)_{;\rho} &= -R\ind{\lambda}{\mu\rho\sigma}\xi_{\lambda;\nu}-R\ind{\lambda}{\nu\rho\sigma}\xi_{\mu;\lambda} \\
    \Rightarrow\ \left(R\ind{\lambda}{\sigma\mu\nu;\rho}-R\ind{\lambda}{\rho\mu\nu;\sigma}\right)\xi_\lambda &= R\ind{\lambda}{\rho\nu\mu}\xi_{\lambda;\sigma}-R\ind{\lambda}{\sigma\mu\nu}\xi_{\lambda;\rho} - R\ind{\lambda}{\mu\rho\sigma}\xi_{\lambda;\nu}+R\ind{\lambda}{\nu\rho\sigma}\xi_{\lambda;\mu} \\
    \left(R\ind{\lambda}{\sigma\mu\nu;\rho}-R\ind{\lambda}{\rho\mu\nu;\sigma}\right)\xi_\lambda &= {Q\ind{\lambda}{\mu\nu\rho\sigma}}^\alpha\xi_{\lambda;\alpha}(x),
\end{split}
$$

^2DerKill

with
 $$
     {Q\ind{\lambda}{\mu\nu\rho\sigma}}^\alpha \equiv +R\ind{\lambda}{\nu\rho\sigma}\delta\ind{\alpha}{\mu} + R\ind{\lambda}{\rho\nu\mu}\delta\ind{\alpha}{\sigma} - R\ind{\lambda}{\sigma\mu\nu}\delta\ind{\alpha}{\rho} - R\ind{\lambda}{\mu\rho\sigma}\delta\ind{\alpha}{\nu}.
$$
[[#^2DerKill]] holds for every [[symmetries in GR|Killing vector]] at any point $x$ of our space. At any point $x$, there exist [[symmetries in GR|Killing vectors]] with $\xi_\lambda(x)=0$ and $\xi_{\lambda;\mu}(x)=-\xi_{\mu;\lambda}(x)$ ([[homogeneity and isotropy#^IsoKilling|isotropy]]). For them only the right-hand side of [[#^2DerKill]]  survives. As $\xi_{\lambda;\mu}(x)$ is arbitrary and antisymmetric, the antisymmetric part of the coefficient should vanish
$$
    {Q\ind{\lambda}{\sigma\mu\nu}}^\alpha = {Q\ind{\alpha}{\sigma\mu\nu}}^\lambda.
$$
Also, at every point $x$, we can find [[symmetries in GR|Killing vectors]] with $\xi_\lambda(x)$ arbitrary and $\xi_{\lambda;\mu}(x)=0$ ([[homogeneity and isotropy#^HomoKilling|homogeneity]]). Due to them, we must also have that 
$$
\begin{split}
    R\ind{\lambda}{\sigma\mu\nu;\rho}-R\ind{\lambda}{\rho\mu\nu;\sigma} &=0 \\
    {Q\ind{\lambda}{\sigma\mu\nu\rho}}^\alpha\delta\ind{\sigma}{\alpha} &= {Q\ind{\alpha}{\mu\nu\rho\sigma}}^\lambda\delta\ind{\sigma}{\alpha} \\
    {Q\ind{\lambda}{\mu\nu\rho\sigma}}^\sigma &= {Q\ind{\sigma}{\mu\nu\rho\sigma}}^\lambda.
\end{split}
$$
Performing the contractions and exploiting the  [[algebraic properties of the Riemann Tensor#Antisymmetry|antisymmetry properties]] of the [[Riemann curvature tensor|Riemann tensor]], we arrive at

$$
    (D-1)R_{\lambda\rho\sigma\nu}=R_{\rho\nu}g_{\lambda\sigma}-R_{\sigma\rho}g_{\lambda\nu}.
$$

^MaxSymRiemTens

But
$$
\begin{split}
    R_{\lambda\rho\sigma\nu} &= -R_{\rho\lambda\sigma\nu} \\
    R_{\rho\nu}g_{\lambda\sigma} - R_{\sigma\rho}g_{\lambda\nu} &= -R_{\lambda\nu}g_{\rho\sigma}+R_{\lambda\sigma}g_{\rho\nu} \\
    \overset{\times g^{\lambda\sigma}}{\Rightarrow}\ R_{\rho\nu}D-R_{\nu\rho} &= -R_{\rho\nu}+g_{\rho\nu}R \\
    \Rightarrow\ R_{\rho\nu} &= \frac{g_{\rho\nu}}{D}R.
\end{split}
$$
Then [[#^MaxSymRiemTens]] becomes
$$
\begin{split}
    (D-1)R_{\lambda\rho\sigma\nu} &= \frac{R}{D}\left[g_{\rho\nu}g_{\lambda\sigma}-g_{\rho\sigma}g_{\lambda\nu}\right] \\
    \Rightarrow\ R_{\mu\nu\rho\sigma} &= \frac{g_{\mu\rho}g_{\nu\sigma}-g_{\mu\sigma}g_{\nu\rho}}{D(D-1)}R.
\end{split}
$$
From the Bianchi identity
$$
\begin{split}
    \left(R^{\mu\nu}-\frac{g^{\mu\nu}}{2}R\right)_{;\mu} &=0 \\
    \left(\frac{g^{\mu\nu}}{D}-\frac{g^{\mu\nu}}{2}\right)R_{;\mu} &= 0 \\
    \Rightarrow\ (D-2)\frac{\partial R}{\partial x^\mu} &= 0.
\end{split}
$$
For $D\neq2$ it follows that $\frac{\partial R}{\partial x^\alpha}=0$ and thus 
$$
    R=constant\equiv -D(D-1)\kappa.
$$
$\kappa$ is known as the curvature constant. In terms of it, the [[Riemann curvature tensor|Riemann tensor]] is 
$$
    R_{\alpha\beta\gamma\delta} = +\kappa\left(g_{\alpha\delta}g_{\beta\gamma}-g_{\alpha\gamma}g_{\beta\delta}\right),
$$
and
$$
    R_{\alpha\beta} = -(D-1)\kappa g_{\alpha\beta}.
$$
**Theorem** (without proof, see Weinberg)

If two matrices, $g_{\mu\nu}$ and $\Theta\ind{\prime}{\mu\nu}$, satisfy the above equations and have the same number of positive and negative eigenvalues, then the two can be related with a coordinate transformation
$$
    g\ind{}{\mu\nu}(x') = \frac{\partial x^{\alpha}}{\partial x^{\prime\mu}}\frac{\partial x^\beta}{\partial x^{\prime\nu}}g_{\alpha\beta}(x),
$$
and, thus, they are physically equivalent.

**I.E the metric is unique!**
