---
alias:
- tensor
- tensors
- tensor field
- tensor fields
tag: GR physics
---
Just as we can see elements ([[one-forms in GR|covectors]]) in the dual tangent space (the cotangent space $T^*_p \mathcal{M}$) as linear maps from $T_p \mathcal{M}\rightarrow \mathbb{R}$ we can see elements of $T_p \mathcal{M}$ as linear maps from $T^*_p  \mathcal{M} \rightarrow \mathbb{R}$. Now consider a *multilinear* map: $${\large\stackrel{r}{\cross}}\,T^*_p \mathcal{M} \times{\large \stackrel{s}{\cross}}T_p\mathcal{M}\longrightarrow \mathbb{R}$$

This is what we call an $(r,s)$ tensor at $p$, where $r+s$ is the rank of the tensor. Now the transformation properties of a [[.md|tensor]] under a  [[general coordinate transformation]] comes directly from the transformation properties of [[vector fields in GR|vectors]] and [[one-forms in GR|covectors]]: 

Let $T$ be a $(r,s)$ tensor, we write it in the coordinate basis:

$$
T= T^{\alpha_1\cdots \alpha_r}{}_{\beta_1\cdots \beta_s}\,\partial_{\alpha_1}\otimes\cdots \otimes\partial_{\alpha_r}\otimes \dd{x^{\beta_1}}\otimes\cdots \otimes\dd{x^{\beta_s}}
$$

Then the coordinates under [[general coordinate transformation#^coordTrans]] transform as:

$$
(T^{\alpha_1\cdots \alpha_r}{}_{\beta_1\cdots \beta_s})'=\pdv{ x^{\prime \alpha_{1}}}{ x^{\rho_{1}}}\cdots \pdv{ x^{\prime \alpha_{r}}}{ x^{\rho_{r}}}  \pdv{ x^{\sigma_{1}}}{ x^{\prime \beta_{1}}} \cdots\pdv{ x^{\sigma_{s}}}{ x^{\prime \beta_{s}}}  T^{\rho_{1}\cdots \rho_{r} }{}_{\sigma_{1} \cdots \sigma_{s} }
$$


Special cases of type $(r, s)$ tensors include
1. $T_{p}^{0,1} \mathcal{M}=T_{p}^{*} \mathcal{M}$, [[one-forms in GR|covectors]] are type $(0,1)$ tensors
2. $T_{p}^{1,0} \mathcal{M}=\left(T_{p}^{*} \mathcal{M}\right)^{*} \cong T_{p} \mathcal{M}$, [[vector fields in GR|vectors]] are type $(1,0)$ tensors
3. $T_{p}^{r, 0} \mathcal{M}$ is called the space of $r$-contravariant tensors and $r$ is the **[[contravariance and covariance|contravariant]]** rank
4.  $T_{p}^{0, s} \mathcal{M}$ is called the space of $s$-covariant tensors, and $s$ is the **[[contravariance and covariance|covariant]]** rank


# Fields

 Now the collection of all type $(r,s)$ [[.md|tensors]] at all points of $\mathcal{M}$ is an associated bundle of the principal frame bundle of $\mathcal{M}$ known as the *bundle of tensors of contravariant rank $r$ and covariant rank $s$*: $\mathbf{B}[[.md|\otimes^{r,s}\mathbb{R}]] as maps (or more precisely sections) from [[../QFTII/spacetime]] (manifold) to this bundle, associating to every point $p$ in [[../QFTII/spacetime]] (manifold) $\mathcal{M}$ a [[.md|tensor]]:
$$\begin{align}
T:\mathcal{M} &\rightarrow \mathbf{B}[\otimes^{r,s}\mathbb{R}]\\
p&\mapsto T(p)
\end{align}$$

Now the components $T^{\alpha_1\cdots \alpha_r}{}_{\beta_1\cdots \beta_s}(p)$ change in the exact same way as $T^{\alpha_1\cdots \alpha_r}{}_{\beta_1\cdots \beta_s}$ but we write it a bit differently:

$$T^{\alpha_1\cdots \alpha_r}{}_{\beta_1\cdots \beta_s}(x)\rightarrow T^{\alpha_1\cdots \alpha_r}{}_{\beta_1\cdots \beta_s}(x')=\pdv{ x^{\prime \alpha_{1}}}{ x^{\rho_{1}}}\cdots \pdv{ x^{\prime \alpha_{r}}}{ x^{\rho_{r}}}  \pdv{ x^{\sigma_{1}}}{ x^{\prime \beta_{1}}} \cdots\pdv{ x^{\sigma_{s}}}{ x^{\prime \beta_{s}}}  T^{\rho_{1}\cdots \rho_{r} }{}_{\sigma_{1} \cdots \sigma_{s} }(x)$$

# Examples

## Inverse Metric

An example of a 2-contravariant  tensor is the inverse of the metric. It terms of coordinates in locally inertial frames postulated by the [[principle of equivalence]] $\{\xi\}$ and lab-frame variables $\{x\}$
$$
g^{\mu \nu}(x)=\eta^{\rho \sigma} \frac{\partial x^{\mu}}{\partial \xi^{\rho}} \frac{\partial x^{\nu}}{\partial \xi^{\sigma}}
$$
In a new coordinate system $\left\{x^{\prime}\right\}$ we write
$$
\begin{aligned}
g^{\mu \nu}\left(x^{\prime}\right) &=\eta^{\rho \sigma} \frac{\partial x^{\prime \mu}}{\partial \xi^{\rho}} \frac{\partial x^{\prime \nu}}{\partial \xi^{\sigma}}=\eta^{\rho \sigma}\left(\frac{\partial x^{\prime \mu}}{\partial x^{\alpha}} \frac{\partial x^{\alpha}}{\partial \xi^{\rho}}\right)\left(\frac{\partial x^{\prime \nu}}{\partial x^{\beta}} \frac{\partial x^{\beta}}{\partial \xi^{\sigma}}\right) \\
&=\left(\eta^{\rho \sigma} \frac{\partial x^{\alpha}}{\partial \xi^{\rho}} \frac{\partial x^{\beta}}{\partial \xi^{\sigma}}\right) \frac{\partial x^{\prime \mu}}{\partial x^{\alpha}} \frac{\partial x^{\prime \nu}}{\partial x^{\beta}} \\
&=g^{\alpha \beta}(x) \frac{\partial x^{\prime \mu}}{\partial x^{\alpha}} \frac{\partial x^{\prime \nu}}{\partial x^{\beta}}
\end{aligned}
$$

# Metric
An example of a 2-covariant  tensor is the metric
$$
g_{\mu \nu}(x)=\eta_{\alpha \beta} \frac{\partial \xi^{\alpha}}{\partial x^{\mu}} \frac{\partial \xi^{\beta}}{\partial x^{\nu}}
$$



In a new coordinate system, we have
$$
g_{\mu \nu}\left(x^{\prime}\right)=\eta_{\alpha \beta} \frac{\partial \xi^{\alpha}}{\partial x^{\prime \mu}} \frac{\partial \xi^{\beta}}{\partial x^{\prime \nu}}=\cdots=g_{\rho \sigma}(x) \frac{\partial x^{\rho}}{\partial x^{\prime \mu}} \frac{\partial x^{\sigma}}{\partial x^{\prime \nu}}
$$
following analogous steps as for the inverse metric. This result is as anticipated for a $2^{\text {nd }}$ rank covariant tensor.


# Kronecker delta
An example of a mixed rank-2 tensor is the Kronecker delta symbol. We can represent the Kronecker delta as
$$
\delta^{\mu}{ }_{\nu} \equiv \frac{\partial x^{\mu}}{\partial x^{\nu}}
$$
In a new coordinate system
$$
\delta^{\prime \mu}{}_{\nu}=\frac{\partial x^{\prime \mu}}{\partial x^{\prime \nu}}=\frac{\partial x^{\prime \mu}}{\partial x^{\rho}} \frac{\partial x^{\rho}}{\partial x^{\prime \nu}}=\delta^\rho{}_{\sigma} \frac{\partial x^{\prime \mu}}{\partial x^{\rho}} \frac{\partial x^{\sigma}}{\partial x^{\prime \nu}}
$$
It is of course a numerical equality that we obtain ${\delta^{\prime \mu}}_{\nu}=\delta^\mu{}_{\nu} .$ However, this numerical equality should not hide from our sight the transformation property which corresponds to a mixed rank-2 tensor (rather than that of a scalar).


# Contraction

We note that if we set an upper and a lower index equal, summing over their values, this operation is called contraction. Contractions give rise to a tensor which transforms as having a lower rank. Concretely, in the following example
$$
\begin{aligned}
T^{\mu \nu}{}_{\mu} \rightarrow (T^{ \mu \nu}{}_{\mu})' &=\frac{\partial x^{\prime \mu}}{\partial x^{\rho}} \frac{\partial x^{\prime \nu}}{\partial x^{\sigma}} \frac{\partial x^{\alpha}}{\partial x^{\prime \mu}} T^{\rho \sigma}{}_{\alpha} \\
&=\frac{\partial x^{\prime \nu}}{\partial x^{\sigma}}\left(\frac{\partial x^{\prime \mu}}{\partial x^{\rho}} \frac{\partial x^{\alpha}}{\partial x^{\prime \mu}}\right) T^{\rho \sigma}{}_{\alpha}=\frac{\partial x^{\prime \nu}}{\partial x^{\sigma}} \frac{\partial x^{\alpha}}{\partial x^{\rho}} T^{\rho \sigma}{}_{\alpha} \\
&=\frac{\partial x^{\nu}}{\partial x^{\sigma}} \delta_{\rho}^{\alpha} T^{\rho \sigma}{}_{\alpha}=\frac{\partial x^{\prime \nu}}{\partial x^{\sigma}} T^{\rho \sigma}{}_{\rho} .
\end{aligned}
$$
This is the transformation of a rank-1 tensor (a vector) rather than a rank-3 tensor.

# "Lowering" and" Raising" indices
Let us consider a [[vector fields in GR|contravariant vector]] $V^{\mu}$ which we multiply with the [[metric tensor|metric]] $g_{\rho \sigma} V^{\mu}$ and then contract the index ' $\mu$ ' of the vector with one of the indices of the metric. The result of the contraction is a [[one-forms in GR|covariant vector]]
$$
V_{\sigma}=g_{\mu \sigma} V^{\mu}
$$
with
$$
\begin{aligned}
(V_{\sigma})^{\prime} &=(g_{\mu \sigma})^{\prime} (V^{\mu})'=\left(g_{\rho \alpha} \frac{\partial x^{\rho}}{\partial x^{\prime \mu}} \frac{\partial x^{\alpha}}{\partial x^{\prime \sigma}}\right)\left(\frac{\partial x^{\prime \mu}}{\partial x^{\delta}} V^{\delta}\right) \\
&=g_{\rho \alpha} V^{\delta} \underbracket{\frac{\partial x^{\rho}}{\partial x^{\prime \mu}} \frac{\partial x^{\prime \mu}}{\partial x^{\delta}}}_{=\delta^{\rho}{ }_{\delta}} \frac{\partial x^{\alpha}}{\partial x^{\prime \sigma}}=g_{\rho \alpha} V^{\rho} \frac{\partial x^{\alpha}}{\partial x^{\prime \sigma}} \\
&=V_{\alpha} \frac{\partial x^{\alpha}}{\partial x^{\prime \sigma}}
\end{aligned}
$$
Similarly, we can contract a [[one-forms in GR|covariant vector]] with the [[metric tensor#Inverse|inverse of the metric]] in order to construct a [[vector fields in GR|contravariant  dual of the vector]].
$$
U^{\mu} \equiv g^{\mu \nu} U_{\nu}
$$
with
$$
\begin{aligned}
(U^{\mu})' &=(g^{ \mu \nu})' (U_{\nu})^{\prime}=g^{\rho \sigma} \frac{\partial x^{\prime \mu}}{\partial x^{\rho}} \frac{\partial x^{\prime \nu}}{\partial x^{\sigma}} \frac{\partial x^{\gamma}}{\partial x^{\prime \nu}} V_{\gamma} \\
&=g^{\rho \sigma} U_{\sigma} \frac{\partial x^{\prime \mu}}{\partial x^{\rho}}=U^{\rho} \frac{\partial x^{\prime \mu}}{\partial x^{\rho}}
\end{aligned}
$$
Finally, we remark that we can use the metric tensor or its inverse to lower or raise indices in arbitrary tensors. This modifies their transformation properties under [[general coordinate transformation|general coordinate transformations]]. But, it does not alter the physical content of the tensors. We call all $2^{N}$ possible manifestations of a $N$-rank tensor duals.
$$
T^{\alpha_{1}}{}_{\alpha_{2}}{}^{ \alpha_{3} \cdots} {}_{\cdots}, T^{\alpha_{1}}{}_{\alpha_{2}}{}_{ \alpha_{3}}{}^{ \cdots} {}_{\cdots},T_{\alpha_{1}}{}_{\alpha_{2}}{}^{ \alpha_{3} \cdots} {}_{\cdots},
$$