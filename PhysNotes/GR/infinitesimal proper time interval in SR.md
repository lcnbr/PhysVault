---
alias: 
- proper time
- proper time intervals
- proper time interval
tag: SR GR
---
$\mathrm{d} \tau$ is the proper time interval between two infinitesimally close points
$$
        \mathrm{d} \tau^{2} \equiv c^{2} \mathrm{~d} t^{2}-\mathrm{d} \vec{x}^{2}=\eta_{\mu \nu} \dd{x^\mu}\dd{x^\nu}
$$
We have from [[special relativity|measuring the speed of light]] that $\mathrm{d} \tau^{2}=0$ for events marked by the propagation of light ($\dd{\tau}=0$) and invariant under change of inertial frames for . Assuming that spacetime is homogeneous and isotropic yields that $\mathrm{d} \tau^{2}$ for any type of event is the same in all inertial frames. 

To illustrate this assume $\tau$ does depend on [[../QFTII/spacetime]] and [[velocity]].
$$
\mathrm{d} \tau^{2}=\mathrm{d} \tau^{\prime 2} \lambda(\cdots),
$$
where the dots represent the spacetime and velocity dependencies of the factor $\lambda$ introduced by the transformation between inertial frames. Intuitively we argue that the spacetime dependencies are eliminated because of the homogeneity of spacetime and the velocity dependencies are eliminated because of the isotropy of spacetime. 
# Velocity dependence
To more explicitly see the independence of velocities consider transformations between three frames
![[Pasted image 20220130145959.png|200]]
The proper time intervals are related by
$$
\mathrm{d} \tau^{2}=\lambda\left(\vec{v}_{1}\right) \mathrm{d} \tau^{\prime 2}=\lambda\left(\vec{v}_{2}\right) \mathrm{d} \tau^{\prime \prime 2}, \quad \mathrm{~d} \tau^{\prime 2}=\lambda\left(\vec{v}_{21}\right) \mathrm{d} \tau^{\prime \prime 2},
$$
and thus
$$
\lambda\left(\vec{v}_{21}\right)=\frac{\lambda\left(\vec{v}_{2}\right)}{\lambda\left(\vec{v}_{1}\right)} .
$$
Because we assumed isotropy, this simplifies to an expression only dependent on the absolute values of the velocities
$$
\lambda\left(\left|\vec{v}_{21}\right|\right)=\frac{\lambda\left(\left|\vec{v}_{2}\right|\right)}{\lambda\left(\left|\vec{v}_{1}\right|\right)} .
$$

If $\vec{v}_{21} \approx \vec{v}_{2}-\vec{v}_{1}$, the absolute values of the velocities are related by
$$
\left|\vec{v}_{21}\right|^{2}=\left|\vec{v}_{1}\right|^{2}+\left|\vec{v}_{2}\right|^{2}-2\left|\vec{v}_{1}\right|\left|\vec{v}_{2}\right| \cos \theta
$$
Since the $\cos \theta$ term is not isotropic, $\lambda$ has to be a constant. Then using (1.7) we have $\lambda=\frac{\lambda}{\lambda}=1$. This means that the proper time intervals
$$
\mathrm{d} \tau^{2}=\mathrm{d} \tau^{\prime 2}
$$

^BoostInvariance

are preserved, with $\mathrm{d} \tau^{2}=\mathrm{d} \tau^{\prime 2}=c^{2} \mathrm{~d} t^{2}-\mathrm{d} \vec{x}^{2}$. 

# with [[Minkowski metric]]
From now on we will use units such that $c=1$. We can then write
$$
\mathrm{d} \tau^{2}=\mathrm{d} t^{2}-\mathrm{d} \vec{x}^{2}=\eta_{\mu \nu} \mathrm{d} x^{\mu} \mathrm{d} x^{\nu}
$$

^metricInterval

where $\eta_{\mu \nu}$ is the [[Minkowski metric]] and we employ the [[Einstein summation]] convention.  
Combining [[#^BoostInvariance]] and  [[#^metricInterval]] yields
$$
\eta_{\mu \nu} \mathrm{d} x^{\mu} \mathrm{d} x^{\nu}=\eta_{\mu \nu} \mathrm{d} x^{\prime \mu} \mathrm{d} x^{\prime \nu}=\eta_{\mu \nu} \frac{\partial x^{\prime \mu}}{\partial x^{\rho}} \frac{\partial x^{\prime \nu}}{\partial x^{\sigma}} \mathrm{d} x^{\rho} \mathrm{d} x^{\sigma}
$$
Therefore
$$
\boxed{\eta_{\rho \sigma}=\frac{\partial x^{\prime \mu}}{\partial x^{\rho}} \frac{\partial x^{\prime \nu}}{\partial x^{\sigma}} \eta_{\mu \nu}}
$$

^metricInvar

# [[../math/linear transformation]]

The transformation that we used in [[.md#^BoostInvariance|boost invariance]] is a part of a [[../math/group]] of transformations that all have this property: the [[../String/Lorentz transformation]]s

