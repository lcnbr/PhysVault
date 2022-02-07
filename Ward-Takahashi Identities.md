---
Alias:
- Ward-Takahashi identity
tags:
- qftII
---
QED is a gauge theory with one abelian [[gauge symmetry]]. In the quantisation process we have broken gauge invariance, but a global $\mathrm{U}(1)$ invariance remains. The [[Slavnov-Taylor identities|Slavnov-Taylor identity]] for the latter is called [[Ward-Takahashi Identities|Ward-Takahashi identity]]. **It guarantees consistent renormalisation of the coupling constant (charges).**


The gauge-fixed QED Lagrangian with sources has the following terms
$$
\begin{aligned}
\mathcal{L}_{\mathrm{QED}} &=\bar{\psi}\left(\gamma^{\mu} D_{\mu}-m\right) \psi-\frac{1}{4} F^{\mu v} F_{\mu v} \\
\mathcal{L}_{\mathrm{gf}} &=-\frac{1}{2} \xi^{-1}(\partial \cdot A)^{2} \\
\mathcal{L}_{\mathrm{src}} &=\bar{\psi} \rho+\bar{\rho} \psi-J^{\mu} A_{\mu} .
\end{aligned}
$$
Here the covariant derivatives are defined as
$$
D_{\mu} \psi=\left(\partial_{\mu}-i q A_{\mu}\right) \psi, \quad D_{\mu} \bar{\psi}=\left(\partial_{\mu}+i q A_{\mu}\right) \bar{\psi}
$$
We note that the global part of the gauge transformation acts as
$$
\delta \psi=i q \delta \alpha \psi, \quad \delta \bar{\psi}=-i q \delta \alpha \bar{\psi} .
$$
We construct the [[Noether's theorem|Noether current]] $N^{\mu}$ from the action via its divergence $\partial \cdot N$
$$
\partial_{\mu} N^{\mu}=-i q \bar{\psi} \gamma^{\mu}\left(D_{\mu} \psi\right)-i q\left(D_{\mu} \bar{\psi}\right) \gamma^{\mu} \psi
$$
This equation has the electromagnetic current of the spinor field as its solution
$$
N^{\mu}=-i q \bar{\psi} \gamma^{\mu} \psi
$$
The associated [[Slavnov-Taylor identities#As a correlator|Slavnov-Taylor identity]] reads 7
$$
\left\langle\partial_{\mu} N^{\mu}-i q \bar{\psi} \rho+i q \bar{\rho} \psi\right\rangle_{\rho, \bar{\rho}, J}=0 .
$$
This equation is one version of the Ward-Takahashi identity which involves the electromagnetic current.


The identity is usually expressed in terms of a gauge field which couples to the electromagnetic current. The current $N^{\mu}$ also appears in the equations of motion for the electromagnetic field, let us therefore consider its Schwinger-Dyson equation
$$
\left\langle-i q \bar{\psi} \gamma^{\mu} \psi-\partial_{\nu} F^{\mu \nu}+\xi^{-1} \partial^{\mu}(\partial \cdot A)-J^{\mu}\right\rangle_{\rho, \bar{\rho}, J}=0
$$
Assembling the two identities yields another version of the WardTakahashi identity
$$
\left\langle-\xi^{-1} \partial^{2}(\partial \cdot A)+\partial \cdot J-i q \bar{\psi} \rho+i q \bar{\rho} \psi\right\rangle_{\rho, \bar{\rho}, J}=0
$$
^ward

# Momentum Space. 

The identity is conventionally expressed in momentum space as follows: The first term picks a Feynman graph with an external photon line whose momentum is $k$ and whose polarisation index is $\mu$.

![[Pasted image 20220126125450.png|200]]

It multiplies the graph by $\xi^{-1} k^{2} k_{\mu}$. The external photon line connects to the remainder of the graph by the propagator
$$
G_{\mathrm{F}}^{\mu \nu}(k)=\frac{\eta^{\mu \nu}-(1-\xi) k^{\mu} k^{\nu} / k^{2}}{k^{2}-i \epsilon}
$$
Multiplied by the prefactor we obtain
$$
\xi^{-1} k^{2} k_{\mu} G_{\mathrm{F}}^{\mu v}(k)=k^{v}
$$
This means we actually consider a graph with one amputated photon line whose polarisation vector is contracted with $k$. Now there are two options:

![[Pasted image 20220126125527.png|300]]

- The other side of the photon propagator is connected to a source $J$, i.e. we consider a plain photon propagator (disconnected from the remainder of the graph). In this case we obtain $\partial \cdot J$ which cancels precisely the corresponding term in the Ward-Takahashi identity. This part of the identity is somewhat trivial as it concerns only a plain photon propagator.
- Otherwise, the photon line connects to a non-trivial (sub)graph. The remaining two terms involving spinors and sources must cancel this graph. They pick a spinor line of a graph with one fewer photon line. They shift the spinor momentum by $k$, and they multiply the graph by the charge $\pm q$ of the particle. The sum over all external spinor lines should then precisely cancel the sum over all photon insertions as explained above.
![[Pasted image 20220126125549.png|400]]
^wardloop
# Propagator

Let us consider two examples, a photon propagator and a spinor-photon vertex:

We have already seen that the plain photon propagator $G_{\mathrm{F}}^{\mu v}(k)$ satisfies the identity, and it absorbs the term $\partial \cdot J$ completely. How about the loop correction $M^{\mu v}(k)$ ? Consider the graph $\xi^{-1} k^{2} k_{\mu} M^{\mu v}(k)$ with one external photon line amputated and contracted with its own momentum. As there are no external spinor lines, this graph must vanish exactly. We learn that the loop corrections to the propagator must be exactly transversal
$$
M^{\mu v}(k) \sim \eta^{\mu v}-k^{\mu} k^{\nu} / k^{2} .
$$
The only violation of transversality originates from the [[gauge fixing action for EM|gauge fixing]] term in the plain propagator. This identity substantiates our earlier claim in the context of introduction of [[Faddeev-Popov ghosts|ghost]] fields.

Next, consider a quantum vertex $M_{\mu}\left(k, p, p^{\prime}\right)$ of two spinor fields and a photon where the photon line of momentum $k$ was already amputated. Denote by $M_{0}\left(p, p^{\prime}\right)$ the quantum propagator of the spinor field. The [[Ward-Takahashi Identities#^wardloop|Ward-Takahashi identity]] implies ${ }^{8}$
$$
-i k \cdot M\left(k, p, p^{\prime}\right)=i q M_{0}\left(p, p^{\prime}+k\right)-i q M_{0}\left(p+k, p^{\prime}\right)
$$

![[Pasted image 20220126125913.png|400]]