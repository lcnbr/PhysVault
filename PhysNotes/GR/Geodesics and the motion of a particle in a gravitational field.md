---
alias:
tag: GR physics
---
We have derived the equations of motion of a particle in the gravitational field by means of the [[principle of equivalence]]:![[principle of equivalence#^eomGeneric]]
with ![[principle of equivalence#^prorTimeGeneric]]
and ![[affine connection#^affineconnectionFromMetric]]

We will now show that the equations of motion describe a "geodesic" in spacetime. Namely, the trajectory minimizes the [[infinitesimal proper time interval in SR|proper time]] interval for the transition among any two points.
$$
\begin{aligned}
\delta \int_{\tau_{A}}^{\tau_{B}} \dd{\tau} 
&=\delta \int_{\tau_{A}}^{\tau_{B}} \sqrt{g_{\mu \nu}(x)  \dd{x^{\mu}}  \dd{x^{\nu}}} \\

&=\delta \int_{p_{A}}^{p_{B}}  \dd{p} \sqrt{g_{\mu \nu}(x) \dv{ x^{\mu}}{ p} \dv{ x^{\nu}}{ p}} \quad(p: \text { parameter describing the trajectory) }\\

\text{variational chain rule:}
&=\int_{p_{A}}^{p_{B}} \frac{\dd{ p}}{2}\underbracket{\pqty{g_{\mu \nu}(x) \dv{ x^{\mu}}{ p} \dv{ x^{\nu}}{ p}}^{-1 / 2}}_{\dv{ p}{ \tau}}
\left(\pdv{ g_{\mu \nu}}{ x^{\alpha}} \delta x^{\alpha} \dv{ x^{\mu}}{ p} \dv{ x^{\nu}}{ p}
+2 g_{\mu \nu} \dv{ x^{\mu}}{ p} \dv{ \delta x^{\nu}}{ p}\right) \\

&=\int_{p_{A}}^{p_{B}} \frac{\bcancel{\dd{ p}}}{2}\cancel{\left(\dv{ p}{ \tau}\right)}
\left[\pdv{ g_{\mu \nu}}{ x^{\alpha}} \dv{ x^{\mu}}{ \tau} \dv{ x^{\nu}}{ \tau} \delta x^{\alpha}
+2 g_{\mu \nu} \dv{ x^{\mu}}{ \tau} \dv{ \delta x^{\nu}}{ \tau}\right]\left(\frac{ \dd{\tau}}{ \bcancel{\dd{p}}}\right)^{\cancel{2}} \\

&=\int_{\tau_{A}}^{\tau_{B}} \dd{\tau}
\left[\frac{1}{2} \pdv{ g_{\mu \nu}}{ x^{\alpha}} \dv{ x^{\mu}}{ \tau} \dv{ x^{\nu}}{ \tau} \delta x^{\alpha}
-\dv{}{ \tau}\left(g_{\mu \alpha} \dv{ x^{\mu}}{ \tau}\right) \delta x^{\alpha}\right] \\

&=\int_{\tau_{A}}^{\tau_{B}} \dd{\tau}
\left[\frac{1}{2} \pdv{ g_{\mu \nu}}{ x^{\alpha}} \dv{ x^{\mu}}{ \tau} \dv{ x^{\nu}}{ \tau} 
-\underbracket{\pdv{ g_{\mu \alpha}}{ x^{\nu}} \dv{ x^{\mu}}{ \tau} \dv{ x^{\nu}}{\tau}}_{\text{split and exchange } \mu \text{ and } \nu}
-g_{\mu \alpha} \dv[2]{ x^{\mu}}{ \tau}\right] \delta x^{\alpha} \\

&=\int_{\tau_{A}}^{\tau_{B}} \dd{\tau}
\left[
\left(
\frac{1}{2} \pdv{ g_{\mu \nu}}{ x^{\alpha}}
-\frac{1}{2} \pdv{ g_{\mu \alpha}}{ x^{\nu}}
-\frac{1}{2} \pdv{ g_{\nu \alpha}}{ x^{\mu}}
\right) 
\dv{ x^{\mu}}{ \tau} \dv{ x^{\nu}}{ \tau}
+g_{\mu \alpha} \Gamma^{\mu}{ }_{\nu \beta} \dv{ x^{\nu}}{ \tau} \dv{ x^{\beta}}{ \tau}
\right] \delta x^{\alpha}
\end{aligned}
$$
The bracket above vanishes, leading to
$$
\delta \int_{\tau_{A}}^{\tau_{B}} \dd{\tau}=0
$$
Alternatively, instead of using the [[principle of equivalence|equivalence principle]], we could have used the variational principle in order to derive our equations of motion.

Let us now make a remark about how we can set the boundary conditions for solving the equations of motion of a particle moving inside the gravitational field with a known metric $g_{\mu \nu}$. The system of differential equations that we must solve is

![[principle of equivalence#^eomGeneric]] ^eom

and the [[principle of equivalence#^prorTimeGeneric|generic proper time]] or in a different form:

$$
g_{\mu \nu} \dv{ x^{\mu}}{ \tau} \dv{ x^{\nu}}{ \tau}=1
$$

^propTimeDiffEq


To satisfy [[#^propTimeDiffEq]] we need only to make sure that it is satisfied at an initial [[infinitesimal proper time interval in SR|proper time]] $\tau_{0}$ by choosing appropriate boundary conditions. Then it will keep being satisfied for arbitrary proper times due to [[principle of equivalence#^eomGeneric]]. Indeed, we have that

$$
\begin{aligned}
\dv{}{ \tau}\left(g_{\mu \nu} \dv{ x^{\mu}}{ \tau} \dv{ x^{\nu}}{ \tau}\right) 
&=2 g_{\mu \nu} \dv{^{2} x^{\mu}}{ \tau^{2}} \dv{ x^{\nu}}{ \tau}+\left(\dv{}{ \tau} g_{\mu \nu}\right) \dv{ x^{\mu}}{ \tau} \dv{ x^{\nu}}{ \tau} \\

\text{eom:}&=2 g_{\mu \nu}\left(-\Gamma_{\rho \sigma}^{\mu} \dv{ x^{\rho}}{ \tau} \dv{ x^{\sigma}}{ \tau}\right) \dv{ x^{\nu}}{ \tau}+\pdv{ g_{\rho \nu}}{ x^{\sigma}} \dv{ x^{\rho}}{ \tau} \dv{ x^{\sigma}}{ \tau} \dv{ x^{\nu}}{ \tau} \\

&=[-\underbracket{g_{\mu \nu} g^{\mu \delta}}_{\delta^{\delta}{ }_{\nu}}\left(\pdv{ g_{\sigma \delta}}{ x^{\rho}}+\pdv{ g_{\rho \delta}}{ x^{\sigma}}-\pdv{ g_{\rho \sigma}}{ x^{\delta}}\right)+\pdv{ g_{\rho \nu}}{ x^{\sigma}}] \dv{ x^{\rho}}{ \tau} \dv{ x^{\sigma}}{ \tau} \dv{ x^{\nu}}{ \tau} \\

&=\left[-\pdv{ g_{\sigma \nu}}{ x^{\rho}}-\cancel{\pdv{ g_{\rho \nu}}{ x^{\sigma}}}+\pdv{ g_{\rho \sigma}}{ x^{\nu}}+\cancel{\pdv{ g_{\rho \nu}}{ x^{\sigma}}}\right] \dv{ x^{\rho}}{ \tau} \dv{ x^{\sigma}}{ \tau} \dv{ x^{\nu}}{ \tau} \\

\text{swapping } \nu \text{ and } \rho \text{ on the second term}&=\left[-\pdv{ g_{\sigma \nu}}{ x^{\rho}}+\pdv{ g_{\sigma \nu}}{ x^{\rho}}\right] \dv{ x^{\rho}}{ \tau} \dv{ x^{\sigma}}{ \tau} \dv{ x^{\nu}}{ \tau}=0 .
\end{aligned}
$$
We can thus focus our attention on solving [[principle of equivalence#^eomGeneric]].