---
alias:
tag: GR physics
---

# Homogeneity
A metric space is *homogeneous* if any given point $X$ can be transformed to any other point in its vicinity
$$
    X_\mu\to X\ind{\prime}{\mu} = X_\mu + \varepsilon_\mu.
$$
The generic form of the transformation is given through the [[symmetries in GR#^killingVec|Killing vectors]] as 
$$
    x_\mu\to x\ind{\prime}{\mu} = x_\mu + \varepsilon_{(n)}\xi^{(n)}_\mu(x,X).
$$
To satisfy \eqref{eq:trafo of point X} we can choose $D=4$ [[symmetries in GR#^killingVec|Killing vectors]] with
$$
    \xi^{(n)}_\mu(X,X) = \delta\ind{n}{\mu}.
$$
The [[symmetries in GR#^killingVec|Killing vectors]] are linearly independent. If they were not there should exist a nontrivial relation 
$$
\begin{split}
    c_n\xi^{(n)}_\mu(x,X) &= 0 \\
    \Rightarrow\ c_N\xi^{(n)}_\mu(X,X) &= 0 \\
    c_n\delta\ind{n}{\mu} &= 0 \ \Rightarrow\ c_\mu =0.
\end{split}
$$
The above shows that it cannot exist.

\textbf{*2:}} A metric space is isotropic about a point $X$ if an isometry transformation
$$
    x_\mu \to x\ind{\prime}{\mu} = x_\mu + \varepsilon\xi_\mu(x,X),
$$
keeps $X$ fixed $X\ind{\prime}{\mu}=X_\mu$, while it can transform all other points in the vicinity. Generally 
$$
    \xi_\mu(x,X) = \alpha\ind{\rho}{\mu}(x,X)\xi_\rho(X,X) + \beta\ind{\nu\rho}{\mu}(x,X)\xi_{\nu;\rho}(X,X),
$$
with
$$
    \alpha\ind{\rho}{\mu}(X,X) = \delta\ind{\rho}{\mu}\ \& \ \beta\ind{\nu\rho}{\mu}(X,X) =0.
$$
From $\xi_\mu(X,X)=0$ it follows that
$$
    \xi_\mu(x,X) = \underbrace{\beta\ind{\nu\rho}{\mu}(x,X)}_{\mathrm{antisymmetric}}\xi_{\nu;\rho}(X,X).
$$
We can choose $\frac{D(D-1)}{2}=6$ [[symmetries in GR#^killingVec|Killing vectors]] such that
$$
    \xi^{(n,m)}_\mu(X,X) =0,
$$
and
$$
    \xi^{(n,m)}_{\nu;\rho}(X,X) = \delta\ind{n}{\nu}\delta\ind{m}{\rho}-\delta\ind{n}{\rho}\delta\ind{m}{\nu}.
$$
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

\textbf{*3:}} Metric space isotropic about every point

Let us choose two points $X$ and $X+\diff X$. There are [[symmetries in GR#^killingVec|Killing vectors]] $\xi^{\mu\nu}_\lambda(x,X)$ and $\xi^{(\mu\nu)}_\lambda(x,X+\diff X)$ which satisfy
$$
\begin{split}
    \xi^{(\mu\nu)}_\lambda(X,X) &= \xi^{(\mu\nu)}_\lambda(X+\diff X,X+\diff X) = 0 \\
    \xi^{(\mu\nu)}_\lambda(x,X) &= -\xi^{(\nu\mu)}_\lambda(x,X) \\
    \xi^{(\mu\nu)}_{\lambda;\rho} &= \left[\frac{\partial}{\partial x^\rho}\xi^{(\mu\nu)}_\lambda(x,X)+\Gamma\cancelto{0}{\xi(x,X)}\right]_{x=X} \\
    &= \left[\frac{\partial}{\partial x^\rho}\xi^{(\mu\nu)}_\lambda(x,X)\right]_{x=X} = \delta\ind{\mu}{\lambda}\delta\ind{\nu}{\rho}-\delta\ind{\mu}{\rho}\delta\ind{\nu}{\lambda},
\end{split}
$$
and exactly the same result for $X+\diff X$. The difference of the two [[symmetries in GR#^killingVec|Killing vectors]] will also be a [[symmetries in GR|Killing vector]]. Thus
$$
    \xi^{(\mu\nu)}_\lambda(x,X+\diff X)-\xi^{(\mu\nu)}_\lambda(x,X) = \frac{\partial\xi^{(\mu\nu)}_\lambda(x,X)}{\partial X^\rho}\diff X^\rho,
$$
is a [[symmetries in GR|Killing vector]]. As $\diff X^\rho$ are chosen arbitrarily, we have that $\frac{\partial\xi^{(\mu\nu)}_\lambda(x,X)}{\partial X^\rho}$ is a [[symmetries in GR|Killing vector]] of the metric. We now need to evaluate it at $x=X$. To compute this we recall that
$$
\begin{split}
    \xi^{(\mu\nu)}_\lambda(X,X) &= 0 \\
    \Rightarrow\ \frac{\partial}{\partial X^\rho}\xi^{(\mu\nu)}_\lambda(X,X) &= 0 \\
    \Rightarrow\ \left[\frac{\partial}{\partial x^\rho}\xi^{(\mu\nu)}_\lambda(x,X)\right]_{x=X} + \left[\frac{\partial}{\partial X^\rho}\xi^{(\mu\nu)}_\lambda(x,X)\right]_{x=X} &= 0 \\
    \left[\frac{\partial}{\partial X^\rho}\xi^{(\mu\nu)}_\lambda(x,X)\right]_{x=X} = -\left.\xi^{\mu\nu}_{\lambda;\rho}(x,X)\right|_{x=X} &= -(\delta\ind{\mu}{\lambda}\delta\ind{\nu}{\rho}-\delta\ind{\mu}{\rho}\delta\ind{\nu}{\lambda}).
\end{split}
$$
We have now a few "too many\grqq\, [[symmetries in GR#^killingVec|Killing vectors]] at our disposal, so not all of them can be linearly independent. Let us look at a subset of them setting $\mu=\rho$. We have
$$
\begin{split}
    \left[\frac{\partial}{\partial X^\rho}\xi^{(\rho\nu)}_\lambda(x,X)\right]_{x=X} = -(\delta\ind{\rho}{\lambda}\delta\ind{\nu}{\rho}-\delta\ind{\rho}{\rho}\delta\ind{\nu}{\lambda}) &= (D-1)\delta\ind{\nu}{\lambda} \\
    \Rightarrow\ \left.\frac{1}{D-1}\frac{\partial}{\partial X^\rho}\xi^{(\rho\nu)}_\lambda(x,X)\right|_{x=X} &= \delta\ind{\nu}{\lambda}.
\end{split}
$$
At $x=X$ this has the properties of a [[symmetries in GR|Killing vector]] in a homogeneous space. Our set of [[symmetries in GR#^killingVec|Killing vectors]] can be chosen as 
$$
    \xi^{(\mu\nu)}_\lambda(x,X),
$$
with $\xi^{(\mu\nu)}_{\lambda;\rho}(X,X) = -\xi^{(\nu\mu)}_{\lambda;\rho}(X,X) = \delta\ind{\mu}{\lambda}\delta\ind{\nu}{\rho}-\delta\ind{\mu}{\rho}\delta\ind{\nu}{\lambda}$ and
$$
    \xi^{(\mu)}_\lambda(x,X) = \frac{1}{D-1}\frac{\partial}{\partial x^\rho}\xi^{(\rho\mu)}_\lambda(x,X),
$$
with $\xi^{(\mu)}_\lambda(X,X) = \delta\ind{\mu}{\lambda}$.

This set saturated the maximum number of possible independent [[symmetries in GR#^killingVec|Killing vectors]]. Is it truly independent though? Yes. Consider a linear combination
$$
    c_\mu\xi^{(\mu)}_\lambda(x,X) + c_{\mu\nu}\xi^{(\mu\nu)}_\lambda(x,X) =0.
$$
For $x=X$ we have $\xi^{(\mu\nu)}_\lambda(X,X)=0$ and then 
$$
    c_\mu\xi^{(\mu)}_\lambda(X,X) =0\ \Rightarrow\ c_\mu\delta\ind{\mu}{\lambda} =0\ \Rightarrow\ c_\lambda=0.
$$
Now by differentiation with $x$ we have
$$
    \underbrace{c_\mu}_{=0}\left.\xi^{(\mu)}_{\lambda;\rho}(x,X)\right|_{x=X} + c_{\mu\nu}\xi^{(\mu\nu)}_{\lambda;\rho}(X,X) = 0\ \Rightarrow\ \cdots\ \Rightarrow\ c_{\mu\nu}=0.
$$
A metric space with $\frac{D(D+1)}{2}$ independent [[symmetries in GR#^killingVec|Killing vectors]] is called maximally symmetric. We have just shown that a space which is isotropic about every point and thus also homogeneous, is maximally symmetric. We can now show the converse. A maximally symmetric space is necessarily homogeneous and isotropic about any point.

*Proof:} For concreteness let us take $D=2$ dimensions and a metric space with $n=1,\cdots,\frac{D(D+1)}{2}=3$ *independent} [[symmetries in GR#^killingVec|Killing vectors]], $\xi^{1}_\mu(x),\,\xi^{2}_\mu(x),\,\xi^{3}_\mu(x)$. They of course take the form
$$
    \xi^{(n)}_\mu(x) = \alpha\ind{\rho}{\mu}(x)\xi^{(n)}_\rho(X) + \beta\ind{\rho\nu}{\mu}(x)\xi^{(n)}_{\rho;\nu}(X),
$$
where $\xi^{(n)}_{\rho;\nu}(X) = -\xi^{(n)}_{\nu;\rho}(X)$. Let us organize the constants $\xi^{(n)}_\rho(X)\,\&\,\xi^{(n)}_{\rho;\nu}(X)$ into a matrix
$$
    M = \begin{pmatrix}
    \xi_1^{(1)}(X) & \xi_2^{(1)}(X) & \xi_{1;2}^{(1)}(X) \\ 
    \xi_1^{(2)}(X) & \xi_2^{(2)}(X) & \xi_{1;2}^{(2)}(X) \\
    \xi_1^{(3)}(X) & \xi_2^{(3)}(X) & \xi_{1;2}^{(3)}(X)
    \end{pmatrix}.
$$
We must have that $\det M \neq0$. If $\det M =0$ then the system of equations
$$
    \vec{c}\cdot M =0,
$$
has a solution with
$$
    \vec{c} = (c_1,c_2,c_3) \neq0.
$$
Then we can have the solutions of the equations
$$
\begin{split}
    c_1\xi_1^{(1)}(X)+c_2\xi_1^{(2)}(X)+c_3\xi_1^{(3)}(X) &= 0 \\
    c_1\xi_2^{(1)}(X)+c_2\xi_2^{(2)}(X)+c_3\xi_2^{(3)}(X) &= 0 \\
    c_1\xi_{1;2}^{(1)}(X)+c_2\xi_{1;2}^{(2)}(X)+c_3\xi_{1;2}^{(3)}(X) &= 0,
\end{split}
$$
or, more compactly,
$$
    \sum_nc_n\xi_\rho^{(n)}(X) = 0\ \& \ \sum_n c_n\xi_{\rho;\nu}^{(n)}(X) =0,
$$
for some $\vec{c}=\lbrace c_n\rbrace$ which is $\vec{c}\neq0$. But then, for the same values of $\lbrace c_n\rbrace$ we will have
$$
    \sum_nc_n\xi_\mu^{(n)}(x) = \alpha\ind{\rho}{\mu}(x)\bigg(\underbrace{\sum_nc_n\xi_\rho^{(n)}(X)}_{=0}\bigg) + \beta\ind{\rho\nu}{\mu}(x)\bigg(\underbrace{\sum_nc_n\xi_{\rho;\nu}^{(n)}(X)}_{=0}\bigg) = 0,
$$
and the [[symmetries in GR#^killingVec|Killing vectors]] $\xi_\mu^{(n)}(x)$ would be linearly independent, contrary to our assumption. Given that $\det M\neq0$, the matrix $M$ has an inverse and the equation
$$
    \vec{D}\cdot M = \vec{A},
$$
with $\vec{D}=(d_1,d_2,d_3),\,\vec{A}=(q_1,q_2,b_{12})$, has a solution $\vec{D}=\vec{A}\cdot M^{-1}$ for any possible $\vec{A}$. Then, a superposition 
$$
\begin{split}
    \Tilde{\xi}_\mu(x) &= \sum_nd_n\xi_\mu^{(n)}(x) = \alpha\ind{\rho}{\mu}(x)\bigg(\sum_nc_n\xi_\rho^{(n)}(X)\bigg) + \beta\ind{\rho\nu}{\mu}(x)\bigg(\sum_nc_n\xi_{\rho;\nu}^{(n)}(X)\bigg) \\
    &= \alpha\ind{\rho}{\mu}(x)q_\rho + \beta\ind{\rho\nu}{\mu}(x)b_{\rho\nu},
\end{split}
$$
will have
\begin{equation*}
\begin{split}
    \Tilde{\xi}_\rho(X) &= q_\rho\quad\text{arbitrary (homogeneous space)} \\
    \Tilde{\xi}_{\rho;\nu}(X) &= b_{\rho\nu} = -b_{\nu\rho}\quad\text{arbitrary (homogeneous space).}
\end{split}
\end{equation*}
Therefore a maximally symmetric space is both homogeneous and isotropic about any point $X$.

*Example:} Consider a flat spacetime for which the Riemann tensor vanishes. We have that a [[symmetries in GR|Killing vector]] satisfies
$$
\begin{split}
    \xi_{\mu;\alpha;\beta} & = -\underbrace{R\ind{\rho}{\beta\alpha\mu}}_{=0}\xi_\rho \\
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
