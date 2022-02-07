---
alias:
- physical state
- physical states
- closed state
- exact state
- closed states
- exact states

tags:
- qftII

---
The BRST [[BRST transformation|operator]] $Q$ squares to zero, $Q^{2}=0$, in close analogy to the exterior derivative $\mathrm{d}:=\mathrm{d} x^{\mu} \partial_{\mu} .$ Such operators define a cohomology which often encodes some important information. For example, the de Rham cohomology of the exterior derivative probes the global topology of differentiable manifolds. The BRST cohomology turns out to describe physical states and operators.
Suppose we go back to canonical quantisation with a Hilbert space $\mathbb{H}$. The [[BRST symmetry]] leads to an associated operator $Q$ acting on $\mathbb{H}$. There are two types of distinguished states:

- Closed states are annihilated by $Q$

$$
Q|\Psi\rangle=0 \quad \leftrightarrow \quad|\Psi\rangle \in \mathbb{H}_{\mathrm{cl}} .
$$

^closed

- Exact states are in the image of $Q$

$$
|\Psi\rangle=Q|\Omega\rangle \text { for some }|\Omega\rangle \in \mathbb{H} \quad \leftrightarrow \quad|\Psi\rangle \in \mathbb{H}_{\mathrm{ex}} .
$$

^exact

By construction exact states are also closed, but not necessarily vice versa, $\mathbb{H}_{\mathrm{ex}} \subset \mathbb{H}_{\mathrm{cl}}$. The BRST cohomology $\mathbb{H}_{\mathrm{phys}}$ is defined as the quotient space
$$
\mathbb{H}_{\text {phys }}=\mathbb{H}_{\mathrm{cl}} / \mathbb{H}_{\mathrm{ex}}
$$
^physical

This space (restricted to [[Faddeev-Popov ghosts|ghost]] number zero) turns out to define the physical states. In other words, physical states are defined as equivalence classes $|\Psi\rangle+Q \mathbb{H}$ of states in the original Hilbert space
$$
|\Psi\rangle \simeq|\Psi\rangle+Q|\Omega\rangle \quad \text { with } \quad Q|\Psi\rangle=0
$$
^phys

We have postulated that the BRST cohomology (of [[Faddeev-Popov ghosts|ghost]] number zero) defines physical states. This makes sense only if physical answers depend on equivalence classes but not on their representatives. The discussion is similar to the corresponding discussion of equivalence classes of the vector field in QFT I.
**The key insight is that the BRST operator is hermitian**
$$
Q^{\dagger}=Q
$$
This implies that exact states $|\Psi\rangle=Q|\Omega\rangle$ have zero overlap with closed states $|\Phi\rangle$
$$
\langle\Phi \mid \Psi\rangle=\langle\Phi|Q| \Omega\rangle=\left\langle\Phi\left|Q^{\dagger}\right| \Omega\right\rangle=0
$$
Therefore the scalar product is independent of the representative $\left|\Psi^{\prime}\right\rangle=|\Psi\rangle+Q|\Omega\rangle$ of an equivalence class
$$
\left\langle\Phi \mid \Psi^{\prime}\right\rangle=\langle\Phi \mid \Psi\rangle+\langle\Phi|Q| \Omega\rangle=\langle\Phi \mid \Psi\rangle
$$