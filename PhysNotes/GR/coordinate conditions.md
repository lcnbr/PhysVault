---
alias:
- harmonic coordinate conditions
tag: GR physics
---


The [[metric tensor|metric]] $g_{\mu \nu}(x)$ is a symmetric $4 \times 4$ matrix and contains ten independent elements. [[Einstein's field equations|Einstein's equations]]
$$
R_{\mu \nu}-\frac{g_{\mu \nu}}{2} R+\Lambda g_{\mu \nu}+8 \pi G T_{\mu \nu}=0,
$$
are also ten in number, however four of them are not independent, due to four [[Bianchi identities]]
$$
\left(R^{\mu \nu}-g^{\mu \nu} R+\Lambda g^{\mu \nu}-8 \pi G T^{\mu \nu}\right)_{; \mu}=0 .
$$
This means that the Einstein equation suffice to determine only $6$ out of $10$ components of $g_{\mu \nu}(x)$. 

## Gauge freedom in [[electrodynamics in GR|electrodynamics]]
This is an analogous situation to [[electrodynamics in GR|Maxwell's equations]] (in [[special relativity]]). [[electrodynamics in GR#^PotMax|They]] read

$$
\left(\partial^{2} g_{\mu \nu}-\partial_{\mu} \partial_{\nu}\right) A^{\nu}=0 .
$$

If $A_{\text{sol}}^{\nu}(x)$ is a solution of the above, then so is
$$
A_{\mathrm{sol}}^{\prime \nu}(x)=A_{\mathrm{sol}}^{\nu}(x)+\partial^{\nu} f(x) \text {. }
$$
We can write this as a pseudo [[Bianchi identities|Bianchi identity]]
$$
\frac{\partial}{\partial x^{\mu}}\left[\partial^{2} g^{\mu \nu}-\partial^{\mu} \partial^{\nu}\right] A_{\nu}=\left(\partial^{2} \partial^{\nu}-\partial^{2} \partial^{\nu}\right) A_{\nu}=0 .
$$
In [[electrodynamics in GR|electrodynamics]] we remove this ambiguity in the solutions by "fixing the gauge" with an additional gauge-fixing condition. For example, if we find a solution $A_{\text {sol }}^{\nu}(x)$, we can always construct an $A_{\text {sol }}^{\prime\nu}(x)$ solution which satisfies the **Lorenz gauge condition**

$$
\partial_{\nu} A_{\mathrm{sol}}^{\prime \nu}=0,
$$

^lorenzGauge

by using as $f(x)$ a solution of the differential equation

$$
\partial^{2} f(x)=-\partial_{\nu} A_{\mathrm{sol}}^{\nu}(x) .
$$

^lorenzGaugeTrans

# Harmonic coordinate conditions
Let us now return to General Relativity and [[Einstein's field equations|Einstein's equations]]. Also for them we need to "fix the gauge" in order to render the solutions of [[Einstein's field equations|Einstein's equations]] unique.
One possible way to do this is by imposing the so called harmonic coordinate conditions, which demand a vanishing contraction of the  [[affine connection#From metric tensor metric|affine connection]]

$$
\Gamma^{\lambda} \equiv \Gamma^{\lambda}{ }_{\mu \nu} g^{\mu \nu}=0 .
$$

^harmCoordCond

Let us work out the left-hand side of this equation
$$
\begin{aligned}
\Gamma^{\lambda} &
=\frac{g^{\mu \nu} g^{\lambda \alpha}}{2}
\left[
    \frac{\partial g_{\nu \alpha}}{\partial x^{\mu}}
    +\frac{\partial g_{\mu \alpha}}{\partial x^{\nu}}
    -\frac{\partial g_{\mu \nu}}{\partial x^{\alpha}}
\right] \\

&=g^{\mu \nu} g^{\lambda \alpha} \frac{\partial g_{\mu \alpha}}{\partial x^{\nu}}
-g^{\lambda \alpha}\left(
    \frac{1}{2} g^{\mu \nu} \frac{\partial g_{\mu \nu}}{\partial x^{\alpha}}
\right) \\

&=g^{\mu \nu}\left(
    -g_{\mu \alpha}\frac{\partial g^{\lambda \alpha}}{\partial x^{\nu}} 
\right)
-g^{\lambda \alpha} \frac{1}{\sqrt{g}} \frac{\partial \sqrt{g}}{\partial x^{\alpha}} \\

&=-\frac{\partial g^{\lambda \alpha}}{\partial x^{\alpha}}-\frac{1}{\sqrt{g}} g^{\lambda \alpha} \frac{\partial \sqrt{g}}{\partial x^{\alpha}} \\

&=-\frac{1}{\sqrt{g}} \frac{\partial}{\partial x^{\alpha}}\left(\sqrt{g} g^{\lambda \alpha}\right) .
\end{aligned}
$$

where we used [[affine connection#Contraction]], and thus the harmonic coordinate condition results to

$$
\frac{\partial}{\partial x^{\alpha}}\left(\sqrt{g} g^{\alpha \lambda}\right)=0 .
$$

^HarmCoorCondsqrt

(You can compare it to [[.md#^lorenzGauge]] .) 

We now have to show that it is possible to satisfy the harmonic coordinate condition. Suppose that we find a solution of [[Einstein's field equations#^EinsteinEqWithoutR|Einstein's equations]] for the metric $g_{\mu \nu}(x)$ with $\Gamma^{\lambda} \equiv \Gamma^\lambda{}_{\mu \nu} g^{\mu \nu}$ which do not satisfy the harmonic coordinate condition $\Gamma^{\lambda}=0$. All it takes to construct a solution which does satisfy the condition is a coordinate transformation. Indeed, under a transform $x^{\mu} \rightarrow x^{\prime \mu}=x^{\prime \mu}(x)$, we have, using [[transformation of the affine connection#^altTrans]]
$$
\begin{aligned}
\Gamma^{\prime \lambda} &=(g^{ \mu \nu})^\prime \Gamma^{\prime \lambda}{ }_{\mu \nu} \\
&=\frac{\partial x^{\prime \mu}}{\partial x^{\rho}} \frac{\partial x^{\prime \nu}}{\partial x^{\sigma}} g^{\rho \sigma}\left[\frac{\partial x^{\prime \lambda}}{\partial x^{\alpha}} \frac{\partial x^{\beta}}{\partial x^{\prime \mu}} \frac{\partial x^{\gamma}}{\partial x^{\prime \nu}} \Gamma^{\alpha}{ }_{\beta \gamma}-\frac{\partial x^{\alpha}}{\partial x^{\prime \mu}} \frac{\partial x^{\beta}}{\partial x^{\prime \nu}} \frac{\partial^{2} x^{\prime \lambda}}{\partial x^{\rho} \partial x^{\sigma}}\right] \\
&=\frac{\partial x^{\prime \lambda}}{\partial x^{\alpha}} \Gamma^{\alpha}-\frac{\partial^{2} x^{\prime \lambda}}{\partial x^{\rho} \partial x^{\sigma}} g^{\rho \sigma} .
\end{aligned}
$$
To get to $\Gamma^{\prime \lambda}=0$, our coordinate transformation needs to satisfy the following differential equation
$$
\frac{\partial^{2} x^{\prime \lambda}}{\partial x^{\rho} \partial x^{\sigma}} g^{\rho \sigma}-\frac{\partial x^{\prime \lambda}}{\partial x^{\alpha}} \Gamma^{\alpha}=0 .
$$
(compare to [[.md#^lorenzGaugeTrans]]). This can be rewritten in terms of the [[D'Alambert operator in GR|D'Alembert operator]] as:

$$
\square^2 x^{\prime \lambda}(x)=0,
$$
which justifies the name of harmonic coordinate conditions.
