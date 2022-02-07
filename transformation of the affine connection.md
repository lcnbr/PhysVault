The [[affine connection]] is given by

![[principle of equivalence#^affineConnection|PoE]]


Under a [[general coordinate transformation]] $x \rightarrow x^{\prime}$ we have
$$
\begin{aligned}
\Gamma_{\mu \nu}^{\prime \alpha} &=\pdv{ x^{\prime \alpha}}{ \xi^{\rho}} \pdv{ \xi^{\rho}}{ x^{\prime \mu} }{ x^{\prime \nu}}=\pdv{ x^{\prime \alpha}}{ \xi^{\rho}}\left[\pdv{}{ x^{\prime \mu}} \pdv{ \xi^{\rho}}{ x^{\prime \nu}}\right] \\
&=\pdv{ x^{\prime \alpha}}{ \xi^{\rho}}\left[\pdv{}{ x^{\prime \mu}}\left(\pdv{ x^{\beta}}{ x^{\prime \nu}} \pdv{ \xi^{\rho}}{ x^{\beta}}\right)\right] \\
&=\pdv{ x^{\prime \alpha}}{ \xi^{\rho}} \pdv{ x^{\beta}}{ x^{\prime \nu}} \pdv{}{ x^{\prime \mu}} \pdv{ \xi^{\rho}}{ x^{\beta}}+\pdv{ x^{\prime \alpha}}{ \xi^{\rho}} \pdv{ \xi^{\rho}}{ x^{\beta}} \pdv{ x^{\beta}}{ x^{\prime \mu}  }{x^{\prime \nu}} \\
&=\underbracket{\pdv{ x^{\delta}}{ \xi^{\rho}} \pdv{ \xi^{\rho}}{ x^{\gamma} }{ x^{\beta}}}_{=\Gamma^{\delta}{}_{\gamma \beta}} \underbracket{\pdv{ x^{\prime \alpha}}{ x^{\delta}} \pdv{ x^{\beta}}{ x^{\prime \nu}} \pdv{ x^{\gamma}}{ x^{\prime \mu}}}_{\text {tensor-like part }}+\underbracket{\pdv{ x^{\prime \alpha}}{ x^{\beta}} \pdv{ x^{\beta}}{ x^{\prime \mu}}{  x^{\prime \nu}}}_{\text {non tensor-like part}}
\end{aligned}
$$
So the [[affine connection]] is not a tensor. Under a [[general coordinate transformation]] it changes as

$$
\Gamma^{\alpha}{}_{\mu \nu} \rightarrow \Gamma^{\prime \alpha}{}_{\mu \nu}=\pdv{ x^{\prime \alpha}}{ x^{\rho}} \pdv{ x^{\beta}}{ x^{\prime \mu}} \pdv{ x^{\gamma}}{ x^{\prime \nu}} \Gamma^\rho{}_{\beta \gamma}+\pdv{ x^{\prime \alpha}}{ x^{\beta}} \pdv{x^{\beta}}{ x^{\prime \mu}}{x^{\prime \nu}}
$$

^trans

This non-tensorial transformation of the [[affine connection]] is needed in order to render the geodesic equation for a particle in a gravitational field generally invariant. Indeed, you can show the the combination
$$
\frac{\mathrm{d}^{2} x^{\mu}}{\mathrm{d} \tau^{2}}+\Gamma^\mu{}_{\alpha \beta} \frac{\mathrm{d} x^{\alpha}}{\mathrm{d} \tau} \frac{\mathrm{d} x^{\beta}}{\mathrm{d} \tau}
$$
transforms as a tensor! ( $\rightarrow$ Exercise)
It is easier to prove the above if we derive an equivalent formula for the transformation of the [[affine connection]]. We have
$$
\begin{aligned}
\pdv{ x^{\prime \alpha}}{ x^{\prime \mu}}=\delta_{\mu}^{\alpha} &=\pdv{ x^{\prime \alpha}}{ x^{\beta}} \pdv{ x^{\beta}}{ x^{\prime \mu}} \\
0=\pdv{}{ x^{\prime \nu}}\delta^\alpha_\mu= \pdv{}{ x^{\prime \nu}}\left(\pdv{ x^{\prime \alpha}}{ x^{\beta}} \pdv{ x^{\beta}}{ x^{\prime \mu}}\right) &=\pdv{x^{\prime \alpha}}{ x^{\beta}  }{x^{\gamma}} \pdv{ x^{\beta}}{ x^{\prime \mu}} \pdv{ x^{\gamma}}{ x^{\prime \nu}}+\pdv{ x^{\prime \alpha}}{ x^{\beta}} \pdv{ x^{\beta}}{ x^{\prime \mu}}{  x^{\prime \nu}} \\
\Rightarrow-\pdv{x^{\prime \alpha}}{ x^{\beta}}{  x^{\gamma}} \pdv{ x^{\beta}}{ x^{\prime \mu}} \pdv{ x^{\gamma}}{ x^{\prime \nu}} &=\pdv{ x^{\prime \alpha}}{ x^{\beta}} \pdv{ x^{\beta}}{ x^{\prime \mu}}{x^{\prime \nu}}
\end{aligned}
$$
and thus


$$
\Gamma^\alpha{}_{\mu \nu} \rightarrow \Gamma^{\prime \alpha}{}_{\mu \nu}=\pdv{ x^{\prime \alpha}}{ x^{\rho}} \pdv{ x^{\beta}}{ x^{\prime \mu}} \pdv{ x^{\gamma}}{ x^{\prime \nu}} \Gamma^\rho{}_{\beta \gamma}-\pdv{ x^{\beta}}{ x^{\prime \mu}} \pdv{ x^{\gamma}}{ x^{\prime \nu}} \pdv{x^{\prime \alpha}}{ x^{\beta}}{  x^{\gamma}}
$$

^altTrans

The contraction with a vector now has a simpler form:

$$
\begin{aligned}
\Gamma^\alpha{}_{\mu \nu} V^{\nu} \rightarrow \Gamma'^\alpha{}_{\mu \nu} (V^{\nu})'=& \pdv{ x^{\prime \alpha}}{ x^{\rho}} \pdv{ x^{\sigma}}{ x^{\prime \mu}} \Gamma^\rho{}_{\sigma \nu} V^{\nu}-\pdv{ x^{\beta}}{ x^{\prime \mu}} \pdv{ x^{\gamma}}{ x^{\prime \nu}} \pdv{^{2} x^{\prime \alpha}}{ x^{\beta}  x^{\gamma}} \pdv{ x^{\prime \nu}}{ x^{\delta}} V^{\delta} \\
&=\pdv{ x^{\prime \alpha}}{ x^{\rho}} \pdv{ x^{\sigma}}{ x^{\prime \mu}} \Gamma^\rho{}_{\sigma \nu} V^{\nu}-\underbracket{\pdv{ x^{\beta}}{ x^{\prime \mu}} \pdv{ x^{\prime \alpha}}{ x^{\beta}  }{x^{\gamma}} }_{\text{non-tensoral}}V^{\gamma}
\end{aligned}
$$

^Vectorcontraction

As with the transformation of the contraction of the vector with the [[affine connection]] is

$$
\begin{align}
\Gamma^\beta{}_{\alpha \mu} U_{\beta} \rightarrow \Gamma^{\prime \beta}{}_{\alpha \mu} (U_{\beta})^{\prime}&=\frac{\partial x^{\gamma}}{\partial x^{\prime \alpha}} \frac{\partial x^{\sigma}}{\partial x^{\prime \mu}} \Gamma^\delta{}_{\gamma \sigma} U_{\delta}+\frac{\partial x^{\prime \beta}}{\partial x^{\delta}} \frac{\partial^{2} x^{\delta}}{\partial x^{\prime \alpha} \partial x^{\prime \mu}} \frac{\partial x^{\rho}}{\partial x^{\prime \beta}} U_{\rho} \\
&=\frac{\partial x^{\gamma}}{\partial x^{\prime \alpha}} \frac{\partial x^{\sigma}}{\partial x^{\prime \mu}} \Gamma^\delta{}_{\gamma \sigma} U_{\delta}+\underbracket{ \frac{\partial^{2} x^{\delta}}{\partial x^{\prime \alpha} \partial x^{\prime \mu}}}_{\text{non-tensoral}}  U_{\delta} \\
\end{align}
$$

^covectorContraction

And allows us to define the [[covariant derivative]]