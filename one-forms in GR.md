---
alias:
- covector
- covectors
- cotangent vector
- cotangent vectors
- covariant vector
- covariant vectors
- one form
- one forms
- one-form
- one-forms
- covariant vector field
- covariant vector fields
tag: GR physics
---

A [[one-forms in GR|cotangent vector]] $V$ to a point $p\in \mathcal{M}$ is a vector in the [[cotangent space]]  $\mathcal{T}^*_p \mathcal{M}$. Under a [[general coordinate transformation]]:![[general coordinate transformation#^coordTrans]]The components $U_\mu$ of $U=U_\mu\dd{x^\mu}$ in the coordinate basis $\{\dd{x^\mu}\}$ of $\mathcal{T}^*_p \mathcal{M}$ transform [[covariantly]]:
$$U_\mu\rightarrow(U_\mu)'=U_\rho\pdv{x^\rho}{x'^\mu}$$
This is so that the change of basis still works: $\int Uf=\int U_\mu \dd{x^\mu}  f\stackrel{!}{=}\int U_\mu \pdv{x^\rho}{x'^\mu} \dd{x'^\mu}  f$. Now the collection of all [[one-forms in GR|cotangent vectors]] at all points of $\mathcal{M}$ is called the [[cotangent bundle]]. And we thus define  [[one-forms in GR|one-forms]] as maps (or more precisely sections) from [[spacetime]] (manifold) to the [[cotangent bundle]], associating to every point $p$ in [[spacetime]] (manifold) $\mathcal{M}$ a vector in $\mathcal{T}_p \mathcal{M}$:
$$\begin{align}
U:\mathcal{M} &\rightarrow \mathcal{T} \mathcal{M}\\
p&\mapsto U(p)
\end{align}$$

Now the components $U_\mu(p)$ change in the exact same way as $U_\mu$ but we write it a bit differently:

$$U_\mu(x)\rightarrow U_\mu(x')=U_\rho(x)\pdv{x^\rho}{x'^\mu}$$

