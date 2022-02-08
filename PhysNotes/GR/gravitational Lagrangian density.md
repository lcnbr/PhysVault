---
alias:
tag: GR physics
---


We focus first on the gravitational term $\L_G$, ignoring (or setting to zero) the energy-momentum tensor. To maintain coordinate transformation invariance, $\L_G$ must be a scalar
$$
    \L_G\xrightarrow{x\to x^\prime}\L_G^\prime = \L_G.
$$
An one of a kind scalar that we know of is the curvature scalar. Let us take then 
$$
\begin{split}
    S_G &= \int\dd[4]{x}\sqrt{g}\mathcal{L} \\
    &= const. \int\dd[4]{x}\sqrt{g}R \\
    &= const. \int\dd[4]{x}\sqrt{g}g^{\alpha\beta}R_{\alpha\beta}.
\end{split}
$$
We require that the action is stationary under variations of the metric field
$$
    g_{\mu\nu}\to g_{\mu\nu}+\delta g_{\mu\nu}.
$$
We have

$$
    \delta S_G = const. \int\dd[4]{x}\,\delta(\sqrt{g}R),
$$

^variationAction

with
$$
\begin{split}
    \delta(\sqrt{g}R) &= (\delta\sqrt{g})R+\sqrt{g}\delta(g^{\alpha\beta}R_{\alpha\beta}) \\
    &= R\delta\sqrt{g} + \sqrt{g}(\delta g^{\alpha\beta})R_{\alpha\beta} + \sqrt{g}g^{\alpha\beta}\delta R_{\alpha\beta},
\end{split}

$$
where $g=-\det(g_{\mu\nu})$. Let us consider the variation
$$
\begin{split}
    \delta\log g &= \delta\log(-\det(g_{\mu\nu})) \\
    &= \log(-\det(g_{\mu\nu}+\delta g_{\mu\nu})) - \log(-\det(g_{\mu\nu})) \\
    &= \log(\frac{\det(g_{\mu\nu}+\delta g_{\mu\nu})}{\det(g_{\mu\nu})}) = \log(\det(g^{\mu\rho}(g_{\rho\nu}+\delta g_{\rho\nu}))) \\
    &= \log(\det(\delta\ind{\mu}{\nu}+g^{\rho\mu}\delta g_{\rho\nu})) = \log(\Tr(\delta\ind{\mu}{\nu}+g^{\rho\mu}\delta g_{\rho\nu})) \\
    &= \log(1+\Tr(g^{\rho\mu}\delta g_{\rho\nu})) +\mathcal{O}(\delta g^2) \\
    &= \log(1+g^{\mu\rho}\delta g_{\mu\rho}) +\mathcal{O}(\delta g^2)\\
    &= g^{\mu\rho}\delta g_{\mu\rho} + \mathcal{O}(\delta g^2).
\end{split}
$$
Thus 
$$
\begin{split}
    \delta\log g &= g^{\mu\rho}\delta g_{\mu\rho} \\
    \Rightarrow\ \delta g^{1/2} &=\delta(\exp(\log(g)\frac{1}{2})=\frac{1}{2}\exp(\log(g)\frac{1}{2})\delta(\log(g))= \frac{1}{2}\sqrt{g}\delta\log g \\
    \Rightarrow\ \delta\sqrt{g} &= \frac{1}{2}\sqrt{g}g^{\mu\rho}\delta g_{\mu\rho}.
\end{split}
$$
Also, from
$$
\begin{split}
    g^{\alpha\beta}g_{\beta\gamma} &= \delta\ind{\alpha}{\gamma} \\
    0 = \delta\left(g^{\alpha\beta}g_{\beta\gamma}\right) &= \left(\delta g^{\alpha\beta}\right)g_{\beta\gamma} + g^{\alpha\beta}\delta g_{\beta\gamma} \\
    \left(\delta g^{\alpha\beta}\right)g_{\beta\gamma} &= -\left(\delta g_{\beta\gamma}\right)g^{\alpha\beta} \\
    \left(\delta g^{\alpha\beta}\right)g_{\beta\gamma}g^{\gamma\delta} &= -\left(\delta g_{\beta\gamma}\right)g^{\alpha\beta}g^{\gamma\delta} \\
    \Rightarrow\ \delta g^{\alpha\beta} &= -g^{\alpha\beta}g^{\delta\gamma}\delta g_{\beta\gamma}.
\end{split}
$$
The final variation we require is of the [[Ricci tensor]]. Recall that
![[Ricci tensor#^4133de]]
To compute the variation of the Ricci tensor, we will require the variation of the [[affine connection]]. While the [[affine connection]] $\Gamma\ind{\alpha}{\mu\nu}$ is **not** a tensor, it turns out that its variation **is** a tensor. To show this let us look at the [[covariant derivative]] of the variation of the metric
$$
    \delta g_{\mu\nu;\rho} = \left(\delta g_{\mu\nu}\right)_{;\rho} = \frac{\partial\delta g_{\mu\nu}}{\partial x^\rho} - \Gamma\ind{\alpha}{\mu\rho}\delta g_{\alpha\nu}-\Gamma\ind{\alpha}{\nu\rho}\delta g_{\alpha\mu}.
$$
Then
$$
\begin{split}
    \delta g_{\mu\rho;\nu} + \delta g_{\nu\rho;\mu} - \delta g_{\mu\nu;\rho} &= \frac{\partial\delta g_{\mu\rho}}{\partial x^\nu} + \frac{\partial\delta g_{\nu\rho}}{\partial x^\mu} - \frac{\partial\delta g_{\mu\nu}}{\partial x^\rho} + \cancel{\Gamma\ind{\alpha}{\mu\rho}\delta g_{\alpha\nu}} + \bcancel{\Gamma\ind{\alpha}{\rho\nu}\delta g_{\alpha\mu}} \\
    &\hspace{1.5cm} - \Gamma\ind{\alpha}{\mu\nu}\delta g_{\alpha\rho} - \bcancel{\Gamma\ind{\alpha}{\rho\nu}\delta g_{\alpha\mu}} - \Gamma\ind{\alpha}{\mu\nu}\delta g_{\alpha\rho} - \cancel{\Gamma\ind{\alpha}{\rho\mu}\delta g_{\alpha\nu}} \\
    &= \frac{\partial\delta g_{\mu\rho}}{\partial x^\nu} + \frac{\partial\delta g_{\nu\rho}}{\partial x^\mu} - \frac{\partial\delta g_{\mu\nu}}{\partial x^\rho} - 2\Gamma\ind{\alpha}{\mu\nu}\delta g_{\alpha\rho} \\
    &= \delta\left(\frac{\partial g_{\mu\rho}}{\partial x^\nu} + \frac{\partial g_{\nu\rho}}{\partial x^\mu} - \frac{\partial g_{\mu\nu}}{\partial x^\rho}\right) - 2\delta\left(\Gamma\ind{\alpha}{\mu\nu}g_{\alpha\rho}\right) + g_{\alpha\rho}2\delta\Gamma\ind{\alpha}{\mu\nu}.
\end{split}
$$
We have that
$$
    \delta\left(\Gamma\ind{\alpha}{\mu\nu}g_{\alpha\rho}\right) = \delta\bigg(\underbrace{g_{\alpha\rho}g^{\alpha\lambda}}_{=\delta\ind{\lambda}{\rho}}\left(\frac{\partial g_{\lambda\mu}}{\partial x^\nu}+\frac{\partial g_{\lambda\nu}}{\partial x^\mu}-\frac{\partial g_{\mu\nu}}{\partial x^\lambda}\right)\bigg) = \delta\left(\frac{\partial g_{\rho\mu}}{\partial x^\nu}+\frac{\partial g_{\rho\nu}}{\partial x^\mu}-\frac{\partial g_{\mu\nu}}{\partial x^\rho}\right).
$$
Thus we have shown that
$$
\begin{split}
    2g_{\alpha\rho}\delta\Gamma\ind{\alpha}{\mu\nu} &= \delta g_{\mu\rho;\nu} + \delta g_{\nu\rho;\mu} - \delta g_{\mu\nu;\rho} \\
    \delta\Gamma\ind{\lambda}{\mu\nu} &= \frac{1}{2}g^{\lambda\rho}\left(\delta g_{\mu\rho;\nu} + \delta g_{\nu\rho;\mu} - \delta g_{\mu\nu;\rho}\right).
\end{split}
$$
Therefore, unlike the [[affine connection]] $\Gamma\ind{\alpha}{\mu\nu}$ which is **not** a tensor, its variation $\delta\Gamma\ind{\alpha}{\mu\nu}$ **is** a tensor. Now let us take the variation of the [[Ricci tensor#Explicit form]]
$$
\begin{split}
    \delta R_{\mu\nu} &= \frac{\partial\delta\Gamma\ind{\alpha}{\mu\alpha}}{\partial x^\nu} - \frac{\partial\delta\Gamma\ind{\alpha}{\mu\nu}}{\partial x^\alpha} + \left(\delta\Gamma\ind{\alpha}{\mu\beta}\right)\Gamma\ind{\beta}{\nu\alpha} + \Gamma\ind{\alpha}{\mu\beta}\delta\Gamma\ind{\beta}{\nu\alpha} - \left(\delta\Gamma\ind{\alpha}{\mu\nu}\right)\Gamma\ind{\beta}{\beta\alpha} - \Gamma\ind{\alpha}{\mu\nu}\delta\Gamma\ind{\beta}{\beta\alpha} \\
    &= \underbrace{\frac{\partial\delta\Gamma\ind{\alpha}{\mu\alpha}}{\partial x^\nu} - \Gamma\ind{\alpha}{\mu\nu}\delta\Gamma\ind{\beta}{\beta\alpha}}_{=(\delta\Gamma\ind{\alpha}{\mu\alpha})_{;\nu}} \underbrace{- \frac{\partial\delta\Gamma\ind{\alpha}{\mu\nu}}{\partial x^\alpha} + \left(\delta\Gamma\ind{\alpha}{\mu\beta}\right)\Gamma\ind{\beta}{\nu\alpha} + \Gamma\ind{\alpha}{\mu\beta}\delta\Gamma\ind{\beta}{\nu\alpha} - \left(\delta\Gamma\ind{\alpha}{\mu\nu}\right)\Gamma\ind{\beta}{\beta\alpha}}_{=-(\delta\Gamma\ind{\alpha}{\mu\nu})_{;\alpha}} \\
    &= \delta\Gamma\ind{\alpha}{\mu\alpha;\nu} - \delta\Gamma\ind{\alpha}{\mu\nu;\alpha}.
\end{split}
$$
The above is the so called **Palatini equation**. Here we have recognized the [[covariant derivative]]s of the variation of the [[affine connection]] (which is a tensor). Contracting with $g^{\mu\nu}$, we have
$$
\begin{split}
    g^{\mu\nu}\delta R_{\mu\nu} &= g^{\mu\nu}\delta\Gamma\ind{\alpha}{\mu\alpha;\nu} - g^{\mu\nu}\delta\Gamma\ind{\alpha}{\mu\nu;\alpha} \\
    &= \left(g^{\mu\nu}\delta\Gamma\ind{\alpha}{\mu\alpha}\right)_{;\nu} - \left(g^{\mu\nu}\delta\Gamma\ind{\alpha}{\mu\nu}\right)_{;\alpha},
\end{split}
$$
where we have used the [[covariant derivative]] of the metric vanishes $g\ind{\mu\nu}{;\lambda}=0$. Notice that the two terms in the above are [[covariant divergence]]s of a vector. Recall then that
![[covariant divergence#^d26365]]
Then we can rewrite the equation in the form
$$
\begin{split}
    g^{\mu\nu}\delta R_{\mu\nu} &= \frac{1}{\sqrt{g}}\left[\frac{\partial}{\partial x^\nu}\left(\sqrt{g}g^{\mu\nu}\delta\Gamma\ind{\alpha}{\mu\alpha}\right) - \frac{\partial}{\partial x^\alpha}\left(\sqrt{g}g^{\mu\nu}\delta\Gamma\ind{\alpha}{\mu\nu}\right)\right] \\
    \Rightarrow\ \sqrt{g}g^{\mu\nu}\delta R_{\mu\nu} &= \frac{\partial}{\partial x^\nu}\left(\sqrt{g}g^{\mu\nu}\delta\Gamma\ind{\alpha}{\mu\alpha}-\sqrt{g}g^{\mu\alpha}\delta\Gamma\ind{\nu}{\mu\alpha}\right),
\end{split}
$$
which is a total derivative. Let us now return to the action variation of [[#^variationAction]]. Collecting the three contributions together, we have
$$
\begin{split}
    \delta S_G &= const.\int\dd[4]{x}\,\left[(\delta\sqrt{g})R + \sqrt{g}(\delta g^{\mu\nu})R_{\mu\nu} + \sqrt{g}g^{\mu\nu}\delta R_{\mu\nu}\right] \\
    &= const.\int\dd[4]{x}\, \left[\frac{1}{2}\sqrt{g}g^{\mu\nu}\delta g_{\mu\nu}R - R_{\alpha\beta}\sqrt{g}g^{\alpha\mu}g^{\beta\nu}\delta g_{\mu\nu}\right] + \cancelto{0}{\int\dd[4]{x}\,\frac{\partial}{\partial x^\alpha}(\cdots)} \\
    &= const. \int\dd[4]{x}\,\left[\frac{g^{\mu\nu}}{2}R-R^{\mu\nu}\right]\sqrt{g}\delta g_{\mu\nu}.
\end{split}
$$
Clearly the variation of the $S_G$ part of the action gives the desired terms in the left-hand side of Einstein`s equations. To add a cosmological constant, we write
$$
    S_G = const.\int\dd[4]{x}\sqrt{g}(R-2\Lambda).
$$
Then
$$
\begin{split}
    \delta S_G &= const.\int\dd[4]{x}\sqrt{g}\left[\left(-R^{\mu\nu}+\frac{g^{\mu\nu}}{2}R\right)\sqrt{g}\delta g_{\mu\nu} - 2\Lambda\left(-\frac{1}{2}\sqrt{g}g^{\mu\nu}\delta g_{\mu\nu}\right)\right] \\
    &= -const.\int\dd[4]{x}\,\left[R^{\mu\nu}-\frac{g^{\mu\nu}}{2}R+\Lambda g^{\mu\nu}\right]\sqrt{g}\delta g_{\mu\nu}.
\end{split}
$$
