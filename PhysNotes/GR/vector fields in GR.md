---
alias:
- vector
- tangent vector
- tangent vectors
- vectors
- contravariant vector
- contravariant vectors
- vector field
- vector fields
- contravariant vector field
- contravariant vector fields
tag: GR physics
---

A [[vector fields in GR|tangent vector]] $V$ to a point $p\in \mathcal{M}$ is a vector in the [[tangent space]]  $\mathcal{T}_p \mathcal{M}$. Under a [[general coordinate transformation]]:![[general coordinate transformation#^coordTrans]]The components $V^\mu$ of $V=V^\mu\partial_\mu$ in the coordinate basis $\{\partial_\mu\}$ of $\mathcal{T}_p \mathcal{M}$ transform [[contravariance and covariance]]:
$$V^\mu\rightarrow(V^\mu)'=V^\rho\pdv{x'^\mu}{x^\rho}$$
This is so that the chain rule still works: $Vf=V^\mu\partial_\mu f\stackrel{!}{=}V^\mu\pdv{x'^\rho}{x^\mu}\partial'_\rho f$. Now the collection of all [[vector fields in GR|tangent vectors]] at all points of $\mathcal{M}$ is called the [[tangent bundle]]. And we thus define  [[vector fields in GR|vector fields]] as maps (or more precisely sections) from [[spacetime]] (manifold) to the [[tangent bundle]], associating to every point $p$ in [[spacetime]] (manifold) $\mathcal{M}$ a vector in $\mathcal{T}_p \mathcal{M}$:
$$\begin{align}
V:\mathcal{M} &\rightarrow \mathcal{T} \mathcal{M}\\
p&\mapsto V(p)
\end{align}$$

Now the components $V^\mu(p)$ change in the exact same way as $V^\mu$ but we write it a bit differently:

$$V^\mu(x)\rightarrow V^\mu(x')=V^\rho(x)\pdv{x'^\mu}{x^\rho}$$

