---
alias:
- energy-momentum tensor
tag: GR physics
---

We are looking for a relativistic generalization of Poisson's equation
$$
\nabla^{2} \phi(x)=4 \pi G \rho(x),
$$
of Newtonian mechanics. We made progress in realizing that the only tensor which contains the second derivative of the metric (which is the General Relativity analogue of the potential) is the Riemann tensor. We now turn our attention to the right-hand side of the above equation, where we encounter the mass density
$$
\rho(\vec{x}, t)=\sum_{n} m_{n} \delta^{(3)}\left(\vec{x}-\vec{x}_{n}(t)\right),
$$
where the sum ranges over all particles and the $\delta$-function defines their trajectories. The mass density is one of the components of the energy-momentum tensor which in [[energy-momentum tensor in SR|special relativity]] reads

![[energy-momentum tensor in SR#^integralForm|energy-momentum tensor]]
$$
T^{\mu \nu}(\vec{x}, t)=\sum_{n} P_{n}^{\mu} \frac{\mathrm{d} x_{n}^{\nu}}{\mathrm{d} t} \delta^{(3)}\left(\vec{x}-\vec{x}_{n}(t)\right)=\sum_{n} m_{n} \int \mathrm{d} \tau \frac{\mathrm{d} x_{n}^{\mu}}{\mathrm{d} \tau} \frac{\mathrm{d} x_{n}^{\nu}}{\mathrm{d} \tau} \delta\left(x-x_{n}(\tau)\right) .
$$
In [[energy-momentum tensor in SR|special relativity]] , the right-hand side of the above equation is manifestly a tensor since $\frac{\mathrm{d} x_{n}^{\mu}}{\mathrm{d} \tau}$ is a vector and the $\delta$-function is a scalar. In General Relativity the $\delta$-function is not a scalar but a scalar density. Consider a scalar field $\phi(x)$. This can be written as
$$
\begin{aligned}
\phi(x) &=\int \mathrm{d}^{4} y \delta(x-y) \phi(y) \\
\Rightarrow \underbrace{\phi(x)}_{\text {scalar }} &=\int \underbrace{\mathrm{d}^{4} y \sqrt{g}}_{\text {scalar }} \underbrace{\frac{\delta(x-y)}{\sqrt{g}}}_{\text {scalar }} \underbrace{\phi(x)}_{\text {scalar }} .
\end{aligned}
$$

For the above to be an invariant equation under general coordinate transformations, we must have that $\frac{\delta(x-y)}{\sqrt{g}}$ rather than $\delta(x-y)$ is a scalar. We can now write down an energymomentum tensor for matter in General Relativity. This reads
$$
T^{\mu \nu}(x)=\frac{1}{\sqrt{g(x)}} \sum_{n} m_{n} \int \mathrm{d} \tau \frac{\mathrm{d} x_{n}^{\mu}}{\mathrm{d} \tau} \frac{\mathrm{d} x_{n}^{\nu}}{\mathrm{d} \tau} \delta\left(x-x_{n}(\tau)\right)
$$

^e30c90

The [[energy-momentum tensor in SR|energy-momentum tensor]] of [[special relativity]] satisfies the continuity equation
![[energy-momentum tensor in SR#^contEq|energy-momentum tensor]]
where $G^{\nu}$ in the right-hand side is the force density. The generalization of this in General Relativity is

$$
T^{\mu \nu}{}_{; \mu}=G^{\nu},
$$

^contEq

where $G^{\nu}$ is an appropriate generalization of the force density (excluding the gravitational force). The effect of gravitation in [[#^contEq]] resides in the [[covariant derivative|covariant differentiation]]. Explicitly
$$
\begin{aligned}
T^{\mu \nu}{ }_{; \mu} &=\frac{\partial T^{\mu \nu}}{\partial x^{\mu}}+\Gamma^{\mu}{ }_{\mu \rho} T^{\rho \nu}+\Gamma^{\nu}{ }_{\mu \rho} T^{\mu \rho} \\
&=\frac{1}{\sqrt{g}} \frac{\partial}{\partial x^{\mu}}\left(\sqrt{g} T^{\mu \nu}\right)+\Gamma^{\nu}{ }_{\mu \rho} T^{\mu \rho} .
\end{aligned}
$$
Where we actually used [[covariant divergence]]
Thus [[#^contEq]] implies:
$$
\implies \frac{1}{\sqrt{g}} \frac{\partial}{\partial x^{\mu}}\left(\sqrt{g} T^{\mu \nu}\right)=G^{\nu}-\underbracket{\Gamma^{\nu}{ }_{\mu \rho} T^{\mu \rho}}_{\textclap{\small {gravitational "force density“ }}} .
$$