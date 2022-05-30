---
alias:
- YM
- Yang-Mills
tags:
- qftII
---
# Gauge transformations of nQED
Based on [[spinor electrodynamics]] is it straightforward to enlarge the [[spinor electrodynamics#^gaugetransformations|local symmetries]] by adding additional fields. Suppose we have $N$ types of spinor fields $\psi^{i}, i=1, \ldots, N$, with equal masses $m$. Consider the mass term
$$
-m \bar{\psi}_{i} \psi^{i}
$$
It is not only invariant under $N$ copies of $U(1)$ transformations $\psi^{i} \rightarrow$ $\exp \left(i q \alpha_{i}\right) \psi^{i}$, but it rather has the larger symmetry
$$
\psi^{\prime i}=U^{i}{ }_{k} \psi^{k}, \quad \bar{\psi}_{i}^{\prime}=\left(U^{*}\right)_{i}^{k} \bar{\psi}_{k}=\bar{\psi}_{k}\left(U^{\dagger}\right)^{k}{ }_{i}
$$
where $U$ is an $N \times N$ matrix which must be unitary $U^{\dagger}=U^{-1}$ such that (using index-free vector and matrix notation)
$$
\bar{\psi}^{\prime} \psi^{\prime}=\bar{\psi} U^{\dagger} U \psi=\bar{\psi} U^{-1} U \psi=\bar{\psi} \psi
$$
The unitary matrices form the [[../math/Lie group]] called $\mathrm{U}(N)$.

# Non-Abelian Gauge Potential. 

We can now replace the transformation factor $\exp (i q \alpha(x))$ by $U(x)$ everywhere in [[spinor electrodynamics]]. We merely have to pay attention that, unlike the phase factor $\exp (i q \alpha)$, matrices do not commute in general. [[spinor electrodynamics#^gaugetransformations|field transformation rules]] become
$$
\psi^{\prime}(x)=U(x) \psi(x), \quad \bar{\psi}^{\prime}(x)=\bar{\psi}(x) U(x)^{-1}
$$

![[YM covariant derivative]]

![[YM gauge potential]]

# Non-Abelian Gauge Theory. 

![[Yang-Mills field strength]]

## Lagrangian
We are now in the position to write a Lagrangian which is manifestly invariant under [[#Gauge transformations of nQED|gauge transformations]]. First we need to find a suitable kinetic term for the gauge field. The usual term $F^{\mu v} F_{\mu v}$ is only [[Yang-Mills field strength#^67d8bd|gauge covariant]]; putting it inside a trace makes it properly invariant
$$
\mathcal{L}_{\mathrm{YM}}=-\frac{1}{2 g_{\mathrm{YM}}^{2}} \operatorname{Tr}{F^{\mu \nu}} F_{\mu \nu}
$$
Interestingly, this **model is interacting due to the extra non-linear terms in $A_{\mu}$ within $F_{\mu \nu}$**. This Lagrangian extends electromagnetism and the model is called Yang-Mills theory. The prefactor $g_{Y M}$ in fact serves as a coupling constant we shall see later. 

## 

The graphical representation for the interactions in pure Yang-Mills theory is a cubic and a quartic vertex between gauge fields. ^[The non-abelian gauge fields are often depicted by curly lines. Here we recycle the wiggly lines otherwise used for abelian photons.
]
![[Pasted image 20220126221154.png|200]]

# spinor matter coupling
The spinor matter sector for a non-abelian gauge theory (YangMills theory coupled to matter) takes precisely the same form as [[spinor electrodynamics|before]]
$$
\mathcal{L}_{\text {spinor }}=\bar{\psi}\left(\gamma^{\mu} D_{\mu}-m\right) \psi .
$$
Note that here $\psi$ and $\bar{\psi}$ are vectors and $D_{\mu}$ is a matrix in an $N$ dimensional space. The resulting vertex is analogous to the vertex in QED.
![[Pasted image 20220126221339.png|100]]

# Scalar matter
Scalar matter can just as well be coupled to the gauge field. For a vector of complex scalars we would write
$$
\mathcal{L}_{\text {scalar }}=-\left(\bar{D}^{\mu} \bar{\phi}\right)\left(D_{\mu} \phi\right)-m^{2} \bar{\phi} \phi .
$$
The kinetic term for the scalar field (dashed line) necessarily comes along with a cubic and a quartic vertex.

![[Pasted image 20220126222248.png|200]]