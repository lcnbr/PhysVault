---
alias:
- general coordinate transformations
- generalized coordinate transformations
- generalized coordinate transformation
- coordinate transform
- coordinate transforms
tag: GR physics
---

$$x^\mu \rightarrow x'^\mu(x)$$

^coordTrans

Note that mathematically the coordinates are functions, part of the chart from $U\subset \mathcal{M}$ of our ([[../QFTII/spacetime]]) manifold  $\mathcal{M}$ , to $\mathbb{R}^n$: 

$$\begin{align}
\phi: U &\rightarrow \mathbb{R}^n\\
p&\mapsto(x^1(p), x^2(p),\dots,x^n(p))
\end{align}$$

Unfortunately when changing coordinates we often talk about everything locally, i.e. at the point  $p$, and write $x^\mu$ or $x$ when we really mean $p$ (an example is at the top of the page, we should in fact write $x^\mu \rightarrow x'^\mu(p)$). However the point $p$ definitely doesn't care about what chart it is put through to spit out its coordinates and does not change under coordinate transforms (as meaningless as that statement is). 

The objects localized at (or attached to) $p$ similarly don't change based on how we label things in $\mathcal{M}$, however we can characterize them based on how *their* labels (coordinates ^[[#^coordTrans|not the same as the one from the chart, but the coordinates in the basis of whatever space they live in]]. There are [[scalar fields in GR|scalars]] which do not have coordinates, and thus cannot change. [[vector fields in GR|Tangent vectors]] that live in the [[tangent space]] at $p$: $\mathcal{T}_p \mathcal{M}$ whose coordinates change [[contravariance and covariance#^contra|contravariantly]] and whose basis changes [[contravariance and covariance#^cov|covariantly]] with [[#^coordTrans]], and we abusively call them [[vector fields in GR|contravariant vectors]] or just [[vector fields in GR|vectors]]. Dual to that are [[one-forms in GR|cotangent vectors]], or [[one-forms in GR|covectors]] living in the dual to $\mathcal{T}_p \mathcal{M}$: the [[../math/cotangent space]]: $\mathcal{T}^*_p \mathcal{M}$. Their coordinates change [[contravariance and covariance#^cov|covariantly]] and their basis changes [[contravariance and covariance#^contra|contravariantly]], we thus also abusively call them [[one-forms in GR|covariant vectors]]. These can be combined and generalized to [[tensor fields in GR|tensors]] living in the tensor product space $\mathcal{T}^{r,s}_p \mathcal{M}$. 

The picture is in fact more rich than this, since $p$ is generic, it can be viewed as a dynamical variable. Thus [[scalar fields in GR|scalars]] become [[scalar fields in GR|scalar fields]], [[vector fields in GR|vectors]] become [[vector fields in GR|vector fields]], [[one-forms in GR|covectors]] become, wait for it, [[one-forms in GR|one forms]] (or [[one-forms in GR|covector fields]]) and [[tensor fields in GR|tensors]] become [[tensor fields in GR|tensor fields]]. However, except for [[one-forms in GR|one forms]] we usually instead call them by the same name as their fixed point cousins and forget to add 'fields'. 


# A note on notation:
As with $p$, we never actually write down the invariant (under coordinate transformations) objects living in e.g. $V\in\mathcal{T}_p \mathcal{M}$, or $U \in \mathcal{T}^*_p \mathcal{M}$  (except in a coordinate free treatment of GR) and instead write their coordinates $V^\mu$ and $U_\mu$ and call *those* the [[vector fields in GR|vectors]] and [[one-forms in GR|covectors]]. Thus we chose to write the change in *coordinates* of $V^\mu$ as $(V^\mu)'$ since the object that is $V$ that we call $V^\mu$ does not change. We do not write $\cancel{V'^\mu}$. However if we talk about the basis in $\mathcal{T}_p \mathcal{M}$ associated to the coordinates $x^\mu$, the *coordinate basis* $\partial_\mu=\pdv{}{x^\mu}$ we write its change: $\partial'_\mu=\pdv{}{x'^\mu}$, since the object naturally depends on the coordinates. Now once we consider these objects as fields, $V\rightarrow V(p)$, most books again just write $V^\mu(x)$ when talking about the object $V(p)$. To avoid crowding primes we choose to write the change in coordinates  $V^\mu(x^\mu)$ of  $V(p)$ as $V^\mu(x')$ or $(V^\mu)'(p)$, but we'll prefer the first notation, where the parenthesis denotes dependence on the chart not the point.