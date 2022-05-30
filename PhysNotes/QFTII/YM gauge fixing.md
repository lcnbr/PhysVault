---
alias:
tags:
- qftII
- YM
---
# Non-Abelian [[gauge fixing action for EM|Gauge Fixing]]. 
Let us now go through the [[abelian quantisation revisited|abelian quantisation]] procedure but with non-abelian fields. The action with source terms reads (compare to [[path integral for EM]])
$$
S_{\mathrm{YM}}[A, J]=-\frac{1}{2 g_{\mathrm{YM}}^{2}} \int \mathrm{d} x^{4} \operatorname{Tr} F_{\mu \nu} F^{\mu \nu}-\int \mathrm{d} x^{4} \operatorname{Tr} J^{\mu} A_{\mu}
$$
We can choose the same gauge-fixing function as [[gauge fixing for EM|before]]
$$
G[[x|A, \Omega]]=\partial^{\mu} A_{\mu}(x)-\Omega(x),
$$
and fix the gauge by means of the identity (compare to [[gauge fixing for EM#Delta functional|EM identity]])
$$
1=\int \operatorname{D} U \Delta\left[G\left[A^{\prime}, \Omega\right]\right] \operatorname{Det}_{(x a, y b)}\left(\frac{\delta G\left[A^{\prime}, \Omega\right]^{a}(x)}{\delta \alpha^{b}(y)}\right) .
$$
Here $U(x)$ is a group element, and the integration measure $D U$ is assumed to be invariant under group multiplication. In other words, for a fixed $V, \mathrm{D}(U V)=\mathrm{D} U=\mathrm{D}(V U)$. Moreover, the variation $\delta U$ of a group element $U$ is expressed through the [[../math/Unitary algebras|algebra]] element $\delta \alpha$ as, (c.f. [[infinitesimal YM gauge transformations]])
$$
\delta U=i \delta \alpha U .
$$
To compute the operator in the determinant, consider the transformation of the gauge potential
$$
A_{\mu}^{\prime}=U A_{\mu} U^{-1}+i U\left(\partial_{\mu} U^{-1}\right) .
$$
Its variation can be expressed as a [[YM covariant derivative|covariant derivative]] of $\delta \alpha$ (c.f. [[infinitesimal YM gauge transformations]])
$$
\delta A_{\mu}^{\prime}=\left(\partial_{\mu} \delta \alpha\right)-i\left[A_{\mu}^{\prime}, \delta \alpha\right]=\left[D_{\mu}^{\prime}, \delta \alpha\right]=\left(\left(D_{\mu}^{\prime}\right)^{\mathrm{ad}} \delta \alpha\right) .
$$
Hence we can write the identity as
$$
1=\int \operatorname{D} U \Delta\left[G\left[A^{\prime}, \Omega\right]\right] \operatorname{Det}\left(\partial^{\mu}\left(D_{\mu}^{\prime}\right)^{\operatorname{ad}}\right)
$$
**Note that the determinant now depends on $A^{\prime}$ and therefore it cannot be pulled out of the integral.** (compare to [[gauge fixing for EM]])
^7ceeb2

We insert the identity into the [[graph generating functional|path integral]] with [[N QED fields#Lagrangian]] 
$$
\begin{gathered}
\mathrm{Z}[J]=\int \operatorname{D} U D A \Delta\left[G\left[A^{\prime}, \Omega\right]\right] \operatorname{Det}\left(\partial^{\mu}\left(D_{\mu}^{\prime}\right)^{\operatorname{ad}}\right) \\
\cdot \exp \left(i S_{\mathrm{YM}}[A, J]\right)
\end{gathered}
$$
Next we perform a gauge transformation by $U^{-1}$ to bring all gauge potentials to the original form. ^[Strictly speaking the source term is not invariant under gauge transformations. However, it is effectively invariant as long as we extract only gaugeinvariant correlation functions from the generating functional $Z[J]$. When the source $J$ is viewed as representing gauge-invariant couplings to matter fields, the gauge transformation of the matter fields induces the desired transformation for $J$.]


$$
\begin{gathered}
\mathrm{Z}[J]=\left(\int \mathrm{D} U\right) \int \mathrm{D} A \Delta[G[A, \Omega]] \operatorname{Det}\left(\partial^{\mu} D_{\mu}^{\mathrm{ad}}\right) \\
\cdot \exp \left(i S_{\mathrm{YM}}[A, J]\right)
\end{gathered}
$$

^1e83f9


Now the integral over the gauge orbit is isolated and can be dropped.