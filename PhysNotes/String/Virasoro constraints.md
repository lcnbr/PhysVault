# Virasoro constraints


$$
T_{\tau \sigma}=\dot{X} \cdot X^{\prime}=0, \quad T_{\tau \tau}=T_{\sigma \sigma}=\dot{X} \cdot \dot{X}+X^{\prime} \cdot X^{\prime}=0
$$
The first constraint demands the lines of constant $\tau$ to be orthogonal to lines of constant $\sigma$. This means, the [[Strings|string]] can move perpendicular to the direction it is stretched out^[[[broedela-3 Classical Bosonic String#^673caf]]. In other words, there are no longitudinal waves allowed, as already noted above: the [[Strings|string]] does not have an inner structure!^[[[broedela-3 Classical Bosonic String#^2bf2c3]]].
Let's try to get some intuition for these constraints. There is a simple meaning of the first constraint ($\dot{X} \cdot X^{\prime}$): we must choose our parameterization such that lines of constant $\sigma$ are perpendicular to the lines of constant $\tau$.

But we can do better. To gain more physical insight, we need to make use of the fact that we haven't quite exhausted our [[../QFTII/gauge symmetry]], there is enough remnant [[../QFTII/gauge symmetry]] to allow us to go to [[Temporal Gauge]],
$$
X^{0} \equiv t=R \tau
$$
so that $\left(X^{0}\right)^{\prime}=0$ and $\dot{X}^{0}=R$, where $R$ is a constant that is needed on dimensional grounds. The interpretation of this constant will become clear shortly. Then, writing $X^{\mu}=(t, \vec{x})$, the equation of motion for spatial components is the free wave equation,
$$
\ddot{\vec{x}}-\vec{x}^{\prime \prime}=0
$$
while the constraints become
$$
\begin{aligned}
\dot{\vec{x}} \cdot \vec{x}^{\prime} &=0 \\
\dot{\vec{x}}^{2}+\vec{x}^{\prime 2} &=R^{2}
\end{aligned}
$$

^660906

The first constraint tells us that the motion of the [[Strings|string]] must be perpendicular to the [[Strings|string]] itself. In other words, the physical modes of the [[Strings|string]] are transverse oscillations. There is no longitudinal mode. We'll also see this again in Section 2.2.

From the second constraint, we can understand the meaning of the constant $R$ : it is related to the length of the [[Strings|string]] when $\dot{\vec{x}}=0$,
$$
\int d \sigma \sqrt{(d \vec{x} / d \sigma)^{2}}=2 \pi R
$$
Of course, if we have a stretched [[Strings|string]] with $\dot{\vec{x}}=0$ at one moment of time, then it won't stay like that for long. It will contract under its own tension. As this happens, the second constraint equation relates the length of the [[Strings|string]] to the instantaneous velocity of the [[Strings|string]].

# In [[light cone coordinates#In the worldsheet]]
$$\left(\partial_{\mathrm{L} / \mathrm{R}} X_{\mathrm{L} / \mathrm{R}}^{\mu}\right)^{2}=0$$ ^800683

## For the [[closed string]]

This leads to [[Virasoro modes]]

## In [[light cone coordinates#In embedding space ambient space]]
Since in [[Light Cone Gauge]], 
$$
X_{\mathrm{L} / \mathrm{R}}^{+}=x_{\mathrm{L} / \mathrm{R}}^{+}+\frac{1}{2} \kappa^{2} p_{\mathrm{L} / \mathrm{R}}^{+} \xi^{\mathrm{L} / \mathrm{R}}
\implies \partial_{\mathrm{L} / \mathrm{R}} X_{\mathrm{L} / \mathrm{R}}^{+}=\frac{1}{2} \kappa^{2}p_{\mathrm{L}/\mathrm{R}}^{+}$$
Thus from [[#^800683]], and [[light cone coordinates#^a95469]] we have:
$$\left(\partial_{\mathrm{L} / \mathrm{R}} X_{\mathrm{L} / \mathrm{R}}^{\mu}\right)\cdot\left(\partial_{\mathrm{L} / \mathrm{R}} X_{\mathrm{L} / \mathrm{R}}^{\mu}\right)=-2\left(\partial_{\mathrm{L} / \mathrm{R}} X_{\mathrm{L} / \mathrm{R}}^{+}\right)\left(\partial_{\mathrm{L} / \mathrm{R}} X_{\mathrm{L} / \mathrm{R}}^{-}\right)+\left(\partial_{\mathrm{L} / \mathrm{R}} \vec{X}_{\mathrm{L}/\mathrm{R}}\right)^2$$

And the [[.md|Virasoro constraints]] become:
$$\left(\partial_{\mathrm{L} / \mathrm{R}} \vec{X}_{\mathrm{L} / \mathrm{R}}\right)^{2}-\kappa^{2} p_{\mathrm{L} / \mathrm{R}}^{+} \partial_{\mathrm{L} / \mathrm{R}} X_{\mathrm{L} / \mathrm{R}}^{-}=0$$