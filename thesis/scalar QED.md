---
alias:
tag:
---

Using the [[minimal coupling prescription]]^[[[@colemanQUANTUMFIELDTHEORY2018#27 2 The minimal coupling prescription zotero open-pdf 0_4E7XKTS3 625]] with $Q=\text{diag}(q_1,q_2)$]. We want to couple a set of massive scalar fields to electromagnetism. The minimal coupling prescription works provided that our base mass lagrangian admits a conserved current.
Our base mass lagrangian is: 

$$\mathcal{L}_m=\sum\limits_{i=1}^2 \partial_\mu \phi_i^\dagger\,\partial^\mu \phi_i - m_i^2 \phi^\dagger_i \phi_i$$
Notice that under the following transformation:

$$\begin{aligned}
\phi_i(x) &\rightarrow e^{-\iunit q_i \lambda} \phi_i(x) \\
\phi_i^{\dagger}(x) &\rightarrow e^{\iunit q_i \lambda} \phi_i^\dagger(x) \\
\end{aligned}$$
or infinitesimally:
$$\begin{aligned}
\delta\phi_i &= -\iunit  \phi_i q_i \delta\lambda \\
\delta\phi_i^{\dagger} &= \iunit  \phi_i^\dagger q_i\delta \lambda\\
\end{aligned}$$
the above Lagrangian is unchanged. Note the sign of the transformation is important. If we upgrade the parameter $\lambda$ to a spacetime function $\lambda(x)$, the Lagrangian is not invariant anymore (c.f [[minimal coupling prescription]]) and invariance is restored if we replace all the derivatives $\partial_\mu$ with the [[gauge covariant derivative|covariant derivative]] $D_\mu$, i.e. if along with the transformation above, we perform a gauge transformation of the photon field:

$$A_\mu\rightarrow A_\mu + \frac{1}{e} \partial_\mu \lambda$$

or infinitesimally

$$\delta A_\mu = \frac{1}{e} \partial_\mu \delta \lambda$$
then the whole lagrangian: 

$$\mathcal{L}_{ED}+\mathcal{L}_{m}(\phi_i,\partial_\mu \phi_i)\rightarrow \mathcal{L}_{ED}+\mathcal{L}_{m}(\phi_i,D_\mu \phi_i)$$
is invariant under the above defined gauge transformation, with the [[gauge covariant derivative|covariant derivative]] defined as:

$$D_\mu=\partial_\mu+\iunit \,e\,q_i\,A_\mu$$




