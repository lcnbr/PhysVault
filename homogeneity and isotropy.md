---
alias:
tag: GR physics
---

# Homogeneity
A metric space is *homogeneous* if any given point $X$ can be transformed to any other point in its vicinity without changing the metric

$$
    X_\mu\to X\ind{\prime}{\mu} = X_\mu + \varepsilon_\mu.
$$

^transToPoint

The generic form of the transformation is given through the [[symmetries in GR#^killingVec|Killing vectors]] as 
$$
    x_\mu\to x\ind{\prime}{\mu} = x_\mu + \varepsilon_{(n)}\xi^{(n)}_\mu(x,X).
$$
To satisfy [[#^transToPoint]] we can choose $D=4$ [[symmetries in GR#^killingVec|Killing vectors]] with

$$
    \xi^{(n)}_\mu(X,X) = \delta\ind{n}{\mu}.
$$

^HomoKilling

The [[symmetries in GR#^killingVec|Killing vectors]] are linearly independent. If they were not there should exist a nontrivial relation 
$$
\begin{split}
    c_n\xi^{(n)}_\mu(x,X) &= 0 \\
    \Rightarrow\ c_N\xi^{(n)}_\mu(X,X) &= 0 \\
    c_n\delta\ind{n}{\mu} &= 0 \ \Rightarrow\ c_\mu =0.
\end{split}
$$
The above shows that it cannot exist.

# Isotropy

A metric space is *isotropic* about a point $X$ if an [[symmetries in GR#^isometryCond|isometry]] transformation
$$
    x_\mu \to x\ind{\prime}{\mu} = x_\mu + \varepsilon\xi_\mu(x,X),
$$
keeps $X$ fixed $X\ind{\prime}{\mu}=X_\mu$, while it can transform all other points in the vicinity.  [[symmetries in GR#^dcca41|Generally]]
$$
    \xi_\mu(x,X) = \alpha\ind{\rho}{\mu}(x,X)\xi_\rho(X,X) + \beta\ind{\nu\rho}{\mu}(x,X)\xi_{\nu;\rho}(X,X),
$$
with
$$
    \alpha\ind{\rho}{\mu}(X,X) = \delta\ind{\rho}{\mu}\ \& \ \beta\ind{\nu\rho}{\mu}(X,X) =0.
$$
From $\xi_\mu(X,X)=0$ it follows that (using [[symmetries in GR#^killingVec|Killing vector antisym under]] [[covariant divergence]])
$$
    \xi_\mu(x,X) = \beta\ind{\nu\rho}{\mu}(x,X)\underbrace{\xi_{\nu;\rho}(X,X)}_{\mathrm{antisymmetric}}.
$$
We can choose $\frac{D(D-1)}{2}=6$ [[symmetries in GR#^killingVec|Killing vectors]] such that

$$
    \xi^{(n,m)}_\mu(X,X) =0,
$$
and
$$
    \xi^{(n,m)}_{\nu;\rho}(X,X) = \delta\ind{n}{\nu}\delta\ind{m}{\rho}-\delta\ind{n}{\rho}\delta\ind{m}{\nu}.
$$

^IsoKilling

Then, indeed $X$ is not shifted. The [[symmetries in GR#^killingVec|Killing vectors]] are then antisymmetric
$$
    \xi^{(n,m)}_{\mu}(x,X) = \beta\ind{\nu\rho}{\mu}(x,X)\xi^{(n,m)}_{\nu;\rho}(X,X) = \beta\ind{nm}{\mu}-\beta\ind{mn}{\mu} = -\xi^{(m,n)}_\mu(x,X).
$$
They are also linearly independent. We have
$$
\begin{split}
    c_{nm}\xi^{(n,m)}_\mu(x,X) &= 0 \quad (c_{nm}=-c_{mn}) \\
    \Rightarrow\ c_{nm}\xi^{(n,m)}_{\mu;\nu}(x,X) &= 0 \\
    c_{nm}\left(\delta\ind{n}{\mu}\delta\ind{m}{\nu}-\delta\ind{n}{\nu}\delta\ind{m}{\mu}\right) &= 0 \\
    \Rightarrow\ c_{nm}-c_{mn} =0\ \ \Rightarrow\ c_{nm} &= 0.
\end{split}
$$

# Metric space isotropic about every point

Let us choose two points $X$ and $X+\dd{X}$. There are [[symmetries in GR#^killingVec|Killing vectors]] $\xi^{(n,m)}_\lambda(x,X)$ and $\xi^{(n,m)}_\lambda(x,X+\dd{X})$ which satisfy
$$
\begin{split}
    \xi^{(n,m)}_\lambda(X,X) &= \xi^{(n,m)}_\lambda(X+\dd{X},X+\dd{X}) = 0 \\
    \xi^{(n,m)}_\lambda(x,X) &= -\xi^{{(n,m)}}_\lambda(x,X) \\
    \xi^{(n,m)}_{\lambda;\rho} &= \left[\frac{\partial}{\partial x^\rho}\xi^{(n,m)}_\lambda(x,X)+\Gamma\underbracket{\xi(x,X)}_{=0 \text{ at }x=X}\right]_{x=X} \\
    &= \left[\frac{\partial}{\partial x^\rho}\xi^{(n,m)}_\lambda(x,X)\right]_{x=X} = \delta\ind{n}{\lambda}\delta\ind{m}{\rho}-\delta\ind{n}{\rho}\delta\ind{m}{\lambda},
\end{split}
$$
and exactly the same result for $X+\dd{X}$. The difference of the two [[symmetries in GR#^killingVec|Killing vectors]] will also be a [[symmetries in GR#^killingVec|Killing vector]]. Thus
$$
    \xi^{(n,m)}_\lambda(x,X+\dd{X})-\xi^{(n,m)}_\lambda(x,X) \stackrel{\text{taylor exp.}}{=} \frac{\partial\xi^{(n,m)}_\lambda(x,X)}{\partial X^\rho}\dd{X}^\rho,
$$
is a [[symmetries in GR#^killingVec|Killing vector]]. As $\dd{X}^\rho$ are chosen arbitrarily, we have that $\frac{\partial\xi^{(n,m)}_\lambda(x,X)}{\partial X^\rho}$ is a [[symmetries in GR#^killingVec|Killing vector]] of the metric. We now need to evaluate it at $x=X$. To compute this we recall that
$$
\begin{split}
    \xi^{(n,m)}_\lambda(X,X) &= 0 \\
    \Rightarrow\ \frac{\partial}{\partial X^\rho}\xi^{(n,m)}_\lambda(X,X) &= 0 \\
    \Rightarrow\ \left[\frac{\partial}{\partial x^\rho}\xi^{(n,m)}_\lambda(x,X)\right]_{x=X} + \left[\frac{\partial}{\partial X^\rho}\xi^{(n,m)}_\lambda(x,X)\right]_{x=X} &= 0 \\
    \left[\frac{\partial}{\partial X^\rho}\xi^{(n,m)}_\lambda(x,X)\right]_{x=X} = -\left.\xi^{(n,m)}_{\lambda;\rho}(x,X)\right|_{x=X} &= -(\delta\ind{n}{\lambda}\delta\ind{m}{\rho}-\delta\ind{n}{\rho}\delta\ind{m}{\lambda}).
\end{split}
$$
We have now a few "too many" [[symmetries in GR#^killingVec|Killing vectors]] at our disposal, so not all of them can be linearly independent. Let us look at a subset of them setting $n=\rho$. We have
$$
\begin{split}
    \left[\frac{\partial}{\partial X^\rho}\xi^{(\rho ,m)}_\lambda(x,X)\right]_{x=X} = -(\delta\ind{\rho}{\lambda}\delta\ind{m}{\rho}-\delta\ind{\rho}{\rho}\delta\ind{m}{\lambda}) &= (D-1)\delta\ind{m}{\lambda} \\
    \Rightarrow\ \left.\frac{1}{D-1}\frac{\partial}{\partial X^\rho}\xi^{(\rho,m)}_\lambda(x,X)\right|_{x=X} &= \delta\ind{m}{\lambda}.
\end{split}
$$
At $x=X$ this has the properties of a [[#^HomoKilling|Killing vectors in a homogeneous space]]. Our set of [[symmetries in GR#^killingVec|Killing vectors]] can be chosen as $\frac{D(D-1)}{2}$ [[#^IsoKilling|isotropy killing vectors]]
$$
    \xi^{(n,m)}_\lambda(x,X),
$$
with $\xi^{(n,m)}_{\lambda;\rho}(X,X) = -\xi^{(m,n)}_{\lambda;\rho}(X,X) = \delta\ind{n}{\lambda}\delta\ind{m}{\rho}-\delta\ind{n}{\rho}\delta\ind{m}{\lambda}$ and $D$ [[#^HomoKilling|homogeneity killing vectors]]:
$$
    \xi^{(\mu)}_\lambda(x,X) = \frac{1}{D-1}\frac{\partial}{\partial x^\rho}\xi^{(\rho,\mu)}_\lambda(x,X),
$$
with $\xi^{(\mu)}_\lambda(X,X) = \delta\ind{\mu}{\lambda}$.

This set saturated the maximum number of possible independent [[symmetries in GR#^killingVec|Killing vectors]]. Is it truly independent though? Yes. Consider a linear combination
$$
    c_\mu\xi^{(\mu)}_\lambda(x,X) + c_{\mu\nu}\xi^{(n,m)}_\lambda(x,X) =0.
$$
For $x=X$ we have $\xi^{(n,m)}_\lambda(X,X)=0$ and then 
$$
    c_\mu\xi^{(\mu)}_\lambda(X,X) =0\ \Rightarrow\ c_\mu\delta\ind{\mu}{\lambda} =0\ \Rightarrow\ c_\lambda=0.
$$
Now by differentiation with $x$ we have
$$
    \underbracket{c_\mu}_{=0}\left.\xi^{(\mu)}_{\lambda;\rho}(x,X)\right|_{x=X} + c_{\mu\nu}\eval{\xi^{(n,m)}_{\lambda;\rho}(x,X)}_{x=X} = 0\ \Rightarrow\ \cdots\ \Rightarrow\ c_{\mu\nu}=0.
$$
A metric space with $\frac{D(D+1)}{2}$ independent [[symmetries in GR#^killingVec|Killing vectors]] is called **maximally symmetric**. We have just shown that a space which is isotropic about every point and thus also homogeneous, is maximally symmetric. We can now show the converse. A maximally symmetric space is necessarily homogeneous and isotropic about any point.


*Example:* Consider a flat spacetime for which the Riemann tensor vanishes. We have that a [[symmetries in GR|Killing vector]] satisfies
$$
\begin{split}
    \xi_{\mu;\alpha;\beta} & = -\underbracket{R\ind{\rho}{\beta\alpha\mu}}_{=0}\xi_\rho \\
    \Rightarrow\ \frac{\partial^2\xi_\mu}{\partial x^\alpha\partial x^\beta} &= 0\ \Rightarrow\ \xi_\mu(x) = a_\mu + b_{\mu\rho}x^\rho\ \  \text{(linear in coords).}
\end{split}
$$
From $\xi_{\mu;\nu}=-\xi_{\nu;\mu}$ we have that $b_{\mu\nu}=-b_{\nu\mu}$. We can then define $\frac{D(D+1)}{2}$ independent [[symmetries in GR#^killingVec|Killing vectors]] as
$$
    \xi_\mu^{(\nu)}(x) = \delta\ind{\nu}{\mu},
$$
and
$$
    \xi_\mu^{(\nu\rho)}(x) = \frac{1}{2}\left(\delta\ind{\nu}{\mu}x^\rho-\delta\ind{\rho}{\mu}x^\nu\right).
$$
A generic [[symmetries in GR|Killing vector]] is decomposed as
$$
\begin{split}
    \xi(x) &= a_\nu\xi_\mu^{(\nu)} + b_{\nu\rho}\xi_\mu^{\nu\rho}(x) \\
    &= a_\nu\delta\ind{\nu}{\mu} + \frac{b_{\nu\rho}}{2}\left(\delta\ind{\nu}{\mu}x^\rho-\delta\ind{\rho}{\mu}x^\nu\right) \\
    &= a_\mu + \frac{1}{2}\left(b_{\mu\rho}x^\rho-b_{\nu\mu}x^\nu\right) \\
    &= a_\mu + \frac{b_{\mu\rho}-b_{\rho\mu}}{2}x^\rho.
\end{split}
$$
The space is homogeneous and isotropic about every point. 

Returning back to our general discussion, we remark that the number of [[symmetries in GR#^killingVec|Killing vectors]] does not depend on the choice of coordinates. If we have [[symmetries in GR#^killingVec|Killing vectors]] $\xi_\mu^{(n)},\,n=1,\cdots M$ in one coordinate system, we will have $M$ [[symmetries in GR#^killingVec|Killing vectors]]
$$
    \xi_\mu^{(n)}\equiv\frac{\partial x^\rho}{\partial x^{\prime\mu}}\xi_\rho^{(n)},
$$
under a transformation $x\to x^\prime$.
