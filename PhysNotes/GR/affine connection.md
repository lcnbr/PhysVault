---
alias: 
tag: GR physics math
---
Note it is not a [[tensor fields in GR|tensor]]!

Following the discussion in [[principle of equivalence|PoE]] we obtained a generalisation of eoms to arbitrary coordinates in an arbitrary gravitational field:

![[principle of equivalence#^eomGeneric]]
where 
![[principle of equivalence#^affineConnection|PoE]]

# Physical intuition
Physically, it can be viewed as the Newtonian analogue of the gravitational force/acceleration. This can be seen better in the [[instantaneous rest frame]] of the particle, where
$$
\dv{ x^\mu}{ \tau}=\left(\dv{ t}{ \tau}, \cancel{\dv{ \vec{x}}{ \tau}}\right)=\left(\dv{ t}{ \tau}, \vec{0}\right)
$$
Then the [[principle of equivalence#^eomGeneric|eom for an arbitrary gravitational field and an arbitrary coordinate system]] gives
$$
\begin{aligned}
\dv[2]{x^\alpha}{\tau}+\Gamma^\alpha{}_{00}\left(\dv{t}{ \tau}\right)^{2} &=0 \\
\dv[2]{x^\alpha}{t}\left(\dv{ t}{ \tau}\right)^{2}+\Gamma_{00}^\alpha\left(\dv{t}{\tau}\right)^{2} &=0 \\
\left(\dv{t}{\tau}\right)^{-2}\cdot\implies \dv[2]{ x^\alpha}{ t} &=-\Gamma_{00}^\alpha
\end{aligned}
$$

For $\alpha=1,2,3$ we get an analogous equation to $$ \dv[2]{ \vec{x}}{ t}=\vec{F}_{\text {grav }} / m . $$

# From [[metric tensor|metric]]

it can be derived from the metric as

$$
\boxed{\Gamma^\alpha{}_{\mu \nu}=
\frac{1}{2} g^{\alpha \rho}
\bqty{
    \pdv{ g_{\rho \nu}}{ x^{\mu}}
    +\pdv{ g_{\rho \mu}}{ x^{\nu}}
    -\pdv{ g_{\mu \nu}}{ x^{\rho}}
}}

$$

^affineconnectionFromMetric

Proof:
We write
$$
\begin{aligned}
\pdv{ g_{\alpha \beta}}{ x^{\gamma}} &=\pdv{}{ x^{\gamma}}\left[\eta_{\mu \nu} \pdv{ \xi^{\mu}}{ x^{\alpha}} \pdv{ \xi^{\nu}}{ x^{\beta}}\right] \\
&=\langle\alpha \gamma \mid \beta\rangle+\langle\alpha \beta \mid \gamma\rangle,
\end{aligned}
$$

with
$$
\langle\alpha \beta \mid \gamma\rangle \equiv \pdv{^{2} \xi^{\mu}}{ x^{\alpha}  x^{\beta}} \pdv{ \xi^{\nu}}{ x^{\gamma}} \eta_{\mu \nu}
$$
Then
$$
\begin{aligned}
\pdv{ g_{\rho \mu}}{ x^{\nu}}+\pdv{ g_{\rho \nu}}{ x^{\mu}}-\pdv{ g_{\mu \nu}}{ x^{\rho}} &=\cancel{\ip{\rho \nu}{\mu}} + \ip{\mu \nu}{\rho}+ \bcancel{\ip{\rho \mu}{\nu}}+ \ip{\mu \nu }{\rho}-\bcancel{\ip{\rho \mu}{\nu}}-\cancel{\ip{\rho \nu}{\mu}}\\
&=2 \ip{\mu \nu}{\rho}
\end{aligned}
$$
Thus
$$
\begin{aligned}
\frac{1}{2} g^{\alpha \rho}\left\{\pdv{ g_{\rho \nu}}{ x^{\mu}}+\pdv{ g_{\rho \mu}}{ x^{\nu}}-\pdv{ g_{\mu \nu}}{ x^{\rho}}\right\} &=\frac{1}{2} 2\ip{\mu \nu}{\rho} g^{\alpha \rho} \\
&=g^{\alpha \rho} \pdv{ \xi^{\beta}}{ x^{\mu}}{  x^{\nu}} \pdv{ \xi^{\gamma}}{ x^{\rho}} \eta_{\beta \gamma} \\
&=\eta^{\varepsilon \delta} \pdv{ x^{\alpha}}{ \xi^{\varepsilon}} \pdv{ x^{\rho}}{ \xi^{\delta}} \pdv{ \xi^{\beta}}{ x^{\mu}}{  x^{\nu}} \pdv{ \xi^{\gamma}}{ x^{\rho}} \eta_{\beta \gamma} \\
&=\eta^{\varepsilon \delta} \pdv{ x^{\alpha}}{ \xi^{\varepsilon}} \pdv{\xi^{\beta}}{ x^{\mu} }{ x^{\nu}} \delta^{\gamma}{ }_{\delta} \eta_{\beta \gamma} \\
&=\pdv{ x^{\alpha}}{ \xi^{\beta}} \pdv{ \xi^{\beta}}{ x^{\mu}  }{x^{\nu}}=\Gamma^\alpha{}_{\mu \nu}
\end{aligned}
$$


# Contraction:


The contracted affine connection is given by
$$
\Gamma^\mu{}_{\mu \rho}=\frac{1}{2} g^{\mu \alpha}\left(\frac{\partial g_{\mu \alpha}}{\partial x^{\rho}}+\cancel{\frac{\partial g_{\rho \alpha}}{\partial x^{\mu}}}-\cancel{\frac{\partial g_{\mu \rho}}{\partial x^{\alpha}}}\right)=\frac{1}{2} g^{\mu \alpha} \frac{\partial g_{\mu \alpha}}{\partial x^{\rho}} .
$$

^contractedConn

With some linear algebra we can show that
$$
\Gamma^\mu{}_{\mu \rho}=\frac{1}{2} \frac{\partial}{\partial x^{\rho}} \log \left(\operatorname{det} g_{\mu \nu}\right)
$$
Proof: Let us start with a matrix $M(x)$ and assume a variation $x \rightarrow \delta x$,
$$
\begin{aligned}
\delta \log \operatorname{det} M(x) &=\log (\operatorname{det} M(x+\delta x))-\log \operatorname{det} M(x) \\
&=\log \frac{\operatorname{det}(M(x+\delta x))}{\operatorname{det} M(x)}=\log \operatorname{det}\left(M^{-1}(x) M(x+\delta x)\right) \\
&=\operatorname{Tr}\left(\log \left(M^{-1}(x) M(x+\delta x)\right)\right) \\
&=\operatorname{Tr}\left(\log \left(M^{-1}(x)\left(M(x)+\frac{\partial M(x)}{\partial x} \delta x+\cdots\right)\right)\right) \\
&=\operatorname{Tr}\left(\log \left(1+M^{-1}(x) \frac{\partial M(x)}{\partial x} \delta x\right)\right) \\
&=\operatorname{Tr}\left(M^{-1}(x) \frac{\partial M(x)}{\partial x}\right) \delta x .
\end{aligned}
$$
The left-hand-side is also using the functional chain rule
$$
\begin{aligned}
\delta \log \operatorname{det}(M(x)) &=\frac{\partial}{\partial x} \bqty{\log \operatorname{det}(M(x))} \delta x \\
&=\frac{1}{\operatorname{det} M(x)} \frac{\partial}{\partial x}(\operatorname{det} M(x)) \delta x
\end{aligned}
$$
Thus,
$$
\operatorname{det}\left(M^{-1}(x)\right) \frac{\partial}{\partial x} \operatorname{det}(M(x))=-\operatorname{Tr}\left(M^{-1}(x) \frac{\partial}{\partial x} M(x)\right)
$$

For the metric matrix $g_{\mu \nu}(x)$ the inverse is $g^{\mu \nu}(x)$. For $M \equiv$ metric, we have

$$

\operatorname{det} g^{\mu \nu} \frac{\partial}{\partial x^{\rho}} \operatorname{det}\left(g_{\mu \nu}\right) =g^{\mu \alpha} \frac{\partial}{\partial x^{\rho}} g_{\alpha \mu} 
$$

^TraceMetric

Thus [[#^contractedConn]] becomes
$$
\Rightarrow \Gamma^{\mu}{ }_{\mu \rho}=\frac{1}{2} g^{\mu \alpha} \frac{\partial}{\partial x^{\rho}} g_{\alpha \mu} =\frac{1}{\operatorname{det} g_{\mu \nu}} \frac{\partial}{\partial x^{\rho}} \operatorname{det} g_{\mu \nu}=\frac{1}{\sqrt{g}} \frac{\partial}{\partial x^{\rho}} \sqrt{g}

$$

^DetContraction



where $g \equiv-\operatorname{det} g_{\mu \nu}$.


# Transformation

See [[transformation of the affine connection]] to see how it transforms and motivates the [[covariant derivative]]

# Weak field approx
Let us now compute the limit of weak gravitational fields. We can decompose $g_{\mu \nu} \approx \eta_{\mu \nu}+h_{\mu \nu}$ with a small $h_{\mu \nu}$. Then the [[affine connection#From metric tensor metric|affine connection]] is
$$
\Gamma^{\mu}{ }_{\nu \rho} \approx \frac{1}{2} \eta^{\mu \alpha}\left[\frac{\partial h_{\alpha \nu}}{\partial x^{\rho}}+\frac{\partial h_{\alpha \rho}}{\partial x^{\nu}}-\frac{\partial h_{\nu \rho}}{\partial x^{\alpha}}\right] \sim \mathcal{O}(h) .
$$

^36c7d0
