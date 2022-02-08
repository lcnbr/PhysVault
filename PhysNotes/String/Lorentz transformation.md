---
alias:
- Lorentz transformations
- boost
- spacetime interval
tag: GR SR
---
The [[Lorentz transformation]] are the group of transformations that leave the [[infinitesimal proper time interval in SR]] invariant:

![[infinitesimal proper time interval in SR#^BoostInvariance]]

They form a [[group]], the [[Lorentz group]], which when supplemented by translations $x'^\mu=x^\mu+\alpha^\mu$ becomes the [[Poincaré group]].
# The [[Lorentz transformation]]s are [[linear transformation]]s
[[infinitesimal proper time interval in SR#^BoostInvariance|Proper time invariance]] implies that the ([[Lorentz transformation|Lorentz]]) transformations $x \rightarrow x^{\prime}$ are [[linear transformation]]s. To show this, we take the derivative of the [[infinitesimal proper time interval in SR#^metricInvar|metric transformation rule]]:
$$
\begin{aligned}
0 &=\pdv{x^\alpha}\eta_{\rho \sigma}=\pdv{x^\alpha}\pqty{\eta_{\mu \nu}\pdv{x'^\mu}{x^\rho}\pdv{x'^\nu}{x^\sigma}}\\
&=\eta_{\mu \nu}\pdv{x'^\mu}{x^\rho}{x^\alpha}\pdv{x'^\nu}{x^\sigma}+\eta_{\mu \nu}\pdv{x'^\mu}{x^\rho}\pdv{x'^\nu}{x^\sigma}{x^\alpha}\\
&=\ip{\alpha \rho}{\sigma}+\ip{\alpha \sigma}{\rho}
\end{aligned}
$$
The sum of the permutations
$$
\left.\begin{array}{rl}
\cancel{\ip{\alpha \rho}{\sigma}} + \ip{\alpha \sigma}{\rho}& =0 \\
\bcancel{\ip{\sigma \rho}{\alpha}}+{\ip{\sigma \alpha}{\rho}}& =0 \\
-\pqty{\bcancel{\ip{\rho \sigma}{\alpha}}+\cancel{\ip{\rho \alpha}{\sigma}}}& =0
\end{array}\right\} \Rightarrow 2\ip{\alpha \sigma}{\rho}=0
$$
gives that
$$
\ip{\alpha \sigma}{\rho}=\eta_{\mu \nu}\pdv{x'^\mu}{x^\rho}\pdv{x'^\nu}{x^\sigma}{x^\alpha}=0
$$
We can get rid of the metric by multiplying with the inverse metric from the left and of the [[Jacobian]] of the transformation by multiplying its inverse $\frac{\partial x}{\partial x^{\prime}}$ from the right. The inverse exists, because physically the [[Lorentz group|Lorentz transformation]] must have an inverse. Thus, the second order derivative of the transformation must vanish
$$
\boxed{\frac{\partial^{2} x^{\prime \mu}}{\partial x^{\rho} \partial x^{\sigma}}=0}
$$

or, in other words, the transformation must be linear
$$
x^{\prime \mu}=\Lambda^{\mu}{ }_{\nu} x^{\nu}+\rho^{\mu} .
$$
It is called the [[Poincaré transformation]] or [[Poincaré transformation|inhomogeneous Lorentz transformation]].


# Matrix Properties

We can now rewrite the [[infinitesimal proper time interval in SR#^metricInvar|metric transformation rule]] as
$$
\Lambda^\nu{}_\sigma \Lambda^\mu{}_\rho \eta_{\mu \nu}=\eta_{\rho \sigma} .
$$

^definingProp

Where $\eta_{\mu \nu}$ is the [[Minkowski metric]]. Now consider the above equation in a [[matrix form from index notation|matrix form]] ($\Lambda^\mu{}_\rho \eta_{\mu \nu} \Lambda^\nu{}_\sigma= (\Lambda^\top)_\rho{}^\mu \eta_{\mu \nu}\Lambda^\nu{}_\sigma$)
$$
\begin{aligned}
\Lambda^{T} \eta \Lambda=\eta \Rightarrow \operatorname{det}\left(\Lambda^{T} \eta \Lambda\right) &=\operatorname{det}(\eta) \\
(\operatorname{det} \Lambda)^{2} \operatorname{det} \eta &=\operatorname{det} \eta \\
\operatorname{det} \Lambda &=\pm 1
\end{aligned}
$$
Also, for $\rho=\sigma=0$ the [[#^definingProp]] becomes
$$
\begin{gathered}
\Lambda_{0}^{\mu} \Lambda_{0}^{\nu} \eta_{\mu \nu}=1 \\
\rightarrow\left(\Lambda_{0}^{0}\right)^{2}-\sum_{i=3}^{3}\left(\Lambda_{0}^{i}\right)^{2}=1 \Rightarrow\left(\Lambda_{0}^{0}\right)^{2} \geq 1
\end{gathered}
$$
Thus, from the [[#^definingProp]]  we find that
- $\operatorname{det} \Lambda=\pm 1$,
- $\Lambda_{0}^{0} \geq+1$ or $\Lambda_{0}^{0} \leq-1 .$

This defines the [[Lorentz group]].

# Components from frame transformation
Let us assume that an observer $\mathcal{O}$ sees a particle at rest and that another inertial observer $\mathcal{O}'$ sees the same particle moving with the velocity $\vec{v}$. The two frames are related by a coordinate transformation: $$\qty(x^\mu)'=\Lambda^\mu{}_\nu x^{\nu}+a^{\mu}$$
![[Pasted image 20220131213217.png|400]]


and thus the **spacetime interval** $\dd{x}^\mu$ transforms as:
$$\dd{\qty(x^\mu)'}=\Lambda^\mu{}_\nu \dd{x^{\nu}}$$

^spacetimeIntTrans

Let us observe the particle (at rest) in the frame $\mathcal{O}$ in two spacetime points $x^{\mu}$ and $\vec{x}^{\mu}+\mathrm{d} x^{\mu}$. We have $\dd{x^i}=0$ since the particle is at rest, and $\dd{x^0}=\dd{t}\neq0$ since we can never stop the advancement of time with a [[Lorentz group|Lorentz transformation]] ($\Lambda^0{}_0\neq0$)
Now, in the frame $\mathcal{O}'$, we have
$$
\begin{aligned}
\dd{\pqty{x^0}}' &= \Lambda^0{}_\nu \dd {x^{\nu}}\overset{\dd{x^i}=0}{=} \Lambda^0{}_0 \dd{ x^{0}}=\Lambda^0{}_0 \dd {t} \\
\dd{\pqty{x^i}}' &=\Lambda^i{}_0 \dd {x^{0}}+\Lambda^i{}_j \,\underbracket{\dd{ x^{j}}}_{=0}=\Lambda^i{}_0 \dd{t}
\end{aligned}
$$
We thus define:
$$
\dv{\pqty{{ x}^i}'}{\pqty{{ x}^0}'}=\frac{\Lambda^i{}_0}{\Lambda^0{}_0}=v^i
$$

^velocity

where $\vec{v}$ is the velocity of the particle. The [[infinitesimal proper time interval in SR|proper time]] intervals in the two frames are the same (c.f. [[infinitesimal proper time interval in SR#^BoostInvariance|defining property]] of [[infinitesimal proper time interval in SR#with Minkowski metric|proper time]])
$$

\begin{aligned}
\dd{\tau}^2&=\eta_{\mu \nu} \dd{x^\mu} \dd{ x^\nu}\overset{\dd{x^i}=0}{=} \dd{t}^2\\
\dd{\tau'}^2&=\dd{t}^2+\dd{\qty(\vec{x})'}^2=(\Lambda^0{}_0)^2 \dd{t}^2 +(\Lambda^i{}_0)^2 \dd{t}^2\\
\end{aligned}
$$
$$
\begin{aligned}
&\implies 1=(\Lambda^0{}_0)^2 +(\Lambda^i{}_0)^2=(\Lambda^0{}_0)^2 +(\vec{v})^2(\Lambda^0{}_0)^2\\
&\implies (\Lambda^0{}_0)^2=\frac{1}{1-\vec{v}^2}
\end{aligned}
$$
We thus define:
$$
\gamma=\gamma(\vec{v}) \equiv \Lambda^{0}{}_{0}=\frac{1}{\sqrt{1-\vec{v}^{2}}}
$$

^gamma

Returning back to [[#^velocity]] yields
$$
\Lambda^i{}_0=\gamma v_{i}=\frac{v_{i}}{\sqrt{1-\vec{v}^{2}}}
$$
The remaining elements fo $\Lambda^\mu{}_{\nu}$ cannot be determined uniquely. The [[Lorentz group|proper orthochronous Lorentz group]] contains the subgroup of [[special orthogonal group|rotations]] 

$$
\Lambda^{\mu}{}_{\nu}=\left\{\begin{array}{lc}
\mu=\nu=0: & 1 \\
\mu=0 \text { or } \nu=0: & 0 \\
\mu=i, \nu=j: & R_{i j}
\end{array}\right.
$$
with $\operatorname{det} R=1$ and $R^{T} R=\mathbb{1}_{3 \times 3}$.
For coordinate systems with parallel axes we have
$$
\Lambda(\vec{v})=\left(\begin{array}{c|c}
\gamma & \gamma v_{i} \\
\hline \gamma v_{i} & \delta_{i j}+\frac{v_{i} v_{j}}{\vec{v}^{2}}(\gamma-1)
\end{array}\right)
$$

^boost

This is called a "boost" transformation, it includes relative velocities but no rotations.
Exercise: Check that $\Lambda(\vec{v})$ satisfies [[#^definingProp]].

# Inverse
From [[#^definingProp]] we can multipy by $\eta^{\sigma \alpha}$ the [[Minkowski metric#Inverse]]
$$\Lambda^\nu{}_\sigma \Lambda^\mu{}_\rho \eta_{\mu \nu}\eta^{\sigma \alpha}=\eta_{\rho \sigma}\eta^{\sigma \alpha} .$$Permuting terms and simultaneously raising and lowering $\rho$ and $\sigma$ and using [[Minkowski metric#^3bcf5d|inverse relation]] we obtain
$$\Lambda_\mu{}^\alpha \Lambda^\mu{}_\rho =\delta_{\rho }^{ \alpha} .$$

Thus we identify $\Lambda_\mu{}^\alpha=(\Lambda^{-1})^\alpha{}_\mu$ and in fact from [[matrix form from index notation|matrix form]] we also have that $(\Lambda^{-1})^\alpha{}_\mu=(\Lambda^{\top})^\alpha{}_\mu$.  Note that this does not mean $\bcancel{\cancel{\Lambda^{-1}=\Lambda^\top}}$ it in fact means:$$\Lambda^{-1}=\eta \Lambda^{T} \eta
$$