---
alias:
tag: GR physics
---


Often a space is not maximally symmetric, but it has subspaces which are. For example, the space of the universe is thought as (approximately) isotropic and homogeneous at any given time $t$. However, the full space time is not. Consider generically a space of dimensionality $D$ with a maximally symmetric subspace of dimensionality $M$. We parametrize the subspace with  $i=1\cdots m$ variables $u^i$. We also have  $v^\alpha,\,\alpha=1\cdots D-M$ variables, to complete the coverage of the full space.

Maximal symmetry of the $M$-dimensional subspace means that there exist $\frac{M(M+1)}{2}$ Killing vectors which transform 
$$
\begin{split}
    u^i&\to u^{\prime i} = u^i+\xi^i(u,v) \\
    v^\alpha&\to v^{\prime\alpha}=v^\alpha,
\end{split}
$$
which leave the metric of the full space form-invariant. Killing vectors satisfy the condition
$$
    \xi_{\mu;\nu}+\xi_{\nu;\mu} =0,
$$
or, in its original form,
$$
    g_{\mu\rho}\frac{\partial\xi^\rho}{\partial x^\nu} + g_{\rho\nu}\frac{\partial\xi^\rho}{\partial x^\mu} + \frac{\partial g_{\mu\nu}}{\partial x^\rho}\xi^\rho =0.
$$
For $\mu,\nu=i,j$ in the $M$-dimensional subspace we have (note $\xi^\rho\neq0$ only for $\rho\in\{1,...,m\}$)

$$
    g_{ik}\frac{\partial\xi^k}{\partial u^j} + g_{jk}\frac{\partial\xi^k}{\partial u^i} + \frac{\partial g_{ij}}{\partial u^k}\xi^k =0.

$$

^killingMM

For $\mu=i$ in the $M$-dimensional subspace and $\nu=\alpha$ spanning the $v$-variables we have

$$
    g_{ik}\frac{\partial\xi^k}{\partial v^\alpha} + g_{\alpha k}\frac{\partial\xi^k}{\partial u^i} + \frac{\partial g_{\alpha i}}{\partial u^k}\xi^k =0.

$$

^killingMD

For $\mu=\alpha,\,\nu=\beta$ spanning the $v$-variables we have

$$
    g_{\alpha k}\frac{\partial\xi^k}{\partial v^\beta} + g_{\beta k}\frac{  \partial\xi^k}{\partial v^\alpha} + \frac{\partial g_{\alpha\beta}}{\partial u^k}\xi^k =0.

$$

^killingDD

We can now simplify the metric by constraining new coordinates $u^{\prime i}$ in which 
$$
    (g\ind{}{i\alpha})'=0.
$$
Indeed, under a coordinate transformation
$$
\begin{split}
    u^i&\to u^{\prime i}=u^{\prime i}(u,v) \\
    v^\alpha&\to v^{\prime\alpha} = v^\alpha,
\end{split}
$$
the metric transforms as 
$$
\begin{split}
    g\ind{}{i\alpha}(u',v) &= \frac{\partial u^j}{\partial u^{\prime i}}\frac{\partial u^k}{\partial v^{\prime\alpha}}g_{jk} + \frac{\partial u^j}{\partial u^{\prime i}}\underbrace{\frac{\partial v^\beta}{\partial v^{\prime\alpha}}}_{=\delta\ind{\beta}{\alpha}}g_{j\beta} + \cancelto{0}{\frac{\partial v^i}{\partial u^{\prime i}}}\frac{\partial v^\beta}{\partial v^{\prime\alpha}}g_{i\beta} \\
    \Rightarrow g\ind{}{i\alpha}(u',v) &= \frac{\partial u^j}{\partial u^{\prime i}}\left(\frac{\partial u^k}{\partial v^{\prime\alpha}}g_{jk}+g_{j\alpha}\right).
\end{split}
$$
It can be proven (see Weinberg) that we can always find a solution of 
$$
    \frac{\partial u^k}{\partial v^{\prime\alpha}}g_{jk}+g_{j\alpha},
$$
and thus render the cross terms $g_{i\alpha}$ to vanish. In these coordinates the Killing vector conditions become
- [[#^killingMM]]$\to g_{ik}\frac{\partial\xi^k}{\partial v^\alpha} =0$
- [[#^killingMD]]$\to \frac{\partial g_{\alpha\beta}}{\partial u^k}\xi^k=0$
- [[#^killingDD]]$\to g_{ik}\frac{\partial\xi^k}{\partial u^j} + g_{jk}\frac{\partial\xi^k}{\partial u^i} + \frac{\partial g_{ij}}{\partial u^k}\xi^k =0.$
- 
From the first equation we get $\frac{\partial\xi^k}{\partial v^\alpha}(u,v)=0$ and thus $\xi^k\equiv\xi^k(u)$ a function of the subspace variables only.

From the second equation we get $g_{\alpha\beta}=g_{\alpha\beta}(v)$, i.e. independent of the subspace variables $u$. 

Let us now consider the metric $g_{ij}(u,v_0)$ at a fixed value $v=v_0$. This is a second rank tensor, which depends only on the $u$ variables. However, any tensor which is defined in terms of the $u$ variables only lives in the maximally symmetric $M$-dimensional subspace with metric $g_{ij}(u,v)$. For such tensors we have proven that
$$
\begin{split}
    T_{ij}(u) &= (const.)g_{ij}(u,v) \\
    \Rightarrow\ g_{ij}(u,v) &= f(v) g_{ij}(u,v_0).
\end{split}
$$
We then have that
$$
    g_{ij}(u,v) = f(v)\tilde{g}_{ij}(u).
$$
Thus, we have found the following general structure for a metric with a maximally symmetric subspace
$$
    \dd\tau^2 = g_{\alpha\beta}(v)\dd v^\alpha\dd v^\beta + f(v^2)\tilde{g}_{ij}(u)\dd u^i\dd u^j,
$$
where $\tilde{g}_{ij}(u)$ is the metric of a maximally symmetric spacetime. If this subspace does not include time (it is just space) we then have the more specific form
$$
    \dd{\tau^2} = g_{\alpha\beta}(v)\dd{ v^\alpha}\dd{v^\beta} - f(v^2)\left[\dd{\vec{u}^2}+\frac{\left(\vec{u}\cdot\dd{\vec{u}}\right)^2}{1-\kappa\vec{u}^2}\right],
$$
with $\kappa = +1,-1,0$. In case of a $3$-dimensional isotropic and homogeneous subspace in a $4$-dimensional space we have
$$
\begin{split}
    u^1 &= r\cos\theta \\
    u^2 &= r\sin\theta\cos\varphi \\
    u^3 &= r\sin\theta\sin\varphi.
\end{split}
$$
We also set
$$
    \dd t = \sqrt{g(u)}\dd u.
$$
The metric takes the form
$$
    \dd\tau^2 = \dd t^2 - R^2(t)\left[\frac{\dd r^2}{1-\kappa r^2}+r^2\left(\dd\theta^2+\sin^2\theta\dd\varphi^2\right)\right].
$$
This is the so-called Robertson-Walker metric. According to the cosmological principal, space in the universe is homogeneous and isotropic (up to small perturbations). The Robertson-Walker metric is the leading order approximation for the gravitational field. The time function $R(t)$ is related through the Einstein field equations to the energy and matter content of the universe.

