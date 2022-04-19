---
alias:
- in state
- out state
tag:
- qft
---

Following [[@collinsNewApproachLSZ2019]] and [this PhysStacExchange answer](https://physics.stackexchange.com/questions/525800/the-use-of-a-dagger-mathbfk-i-int-d3x-eikx-stackrel-leftrightarro)


# Notation

A free klein gordon field is written:

$$\phi_{\text{free}}(x^\mu)=\int \dd{\Phi(k)}\bqty{a_{\mathbf{k},\text{free}}\,e^{-\iunit k_\mu x^\mu}+a^\dagger_{\mathbf{k},\text{free}}\,e^{\iunit k_\mu x^\mu}}$$
Where boldface symbols are spacial 3-vectors and we use the notation from [[Lorentz invariant measure#Different forms]]. This field is as usual in the [[Heisenberg picture]], as it is a solution to the [[Heisenberg EOM]].

 The ideal free theory and its fields are envisioned to live in Fock Hilbert spaces $\mathcal{H}_{\text {in }}$ and $\mathcal{H}_{\text {out }}$.
 
  Now we are interested in an interacting field theory with an interacting field $\phi_\text{int}(x)$ that lives in a Hilbert space $\mathcal{H}$.
  >NB: We emphasize that interactions are not turned off at asymptotic regions: the Lagrangian does not depend explicitly on spacetime!
  
For an interacting field $\phi_\text{int}(x)$, one can in principle still perform a spatial Fourier expansion at each time $t$, however the spatial Fourier transform can no longer be identified with annihilation and creation operators. Instead, we shall define so-called (time-dependent) asymptotic creation and annihilation operators $\hat{a}^{\dagger}(\mathbf{k}, t)$ and $\hat{a}(\mathbf{k}, t)$ by the Klein-Gordon (KG). inner product of eq. (5.2) [and the Hermitian conjugate eq.]. The definition is extended to an asymptotic creation operator $\hat{a}_{1}^{\dagger}(t) \equiv \hat{a}^{\dagger}\left(f_{1}, t\right)$ for a Gaussian wave packet in eq. (5.6).
5. We would like to identify the temporal asymptotic 1 -particle states in the interacting theory with the corresponding 1-particle states in the free theory. For this, we assume the existence of a translation-invariant vacuum state $|\Omega\rangle$ of the full theory, $$\hat{P}_{\mu}|\Omega\rangle=0, \quad\langle\Omega \mid \Omega\rangle=1$$ This implies that $$\left\langle\Omega\left|\partial_{\mu} \hat{\varphi}(x)\right| \Omega\right\rangle=i\left\langle\Omega\left|\left[\hat{\varphi}(x), \hat{P}_{\mu}\right]\right| \Omega\right\rangle=0$$ We assume the existence of 1 -particle states of the full theory
$$
\hat{\mathbf{P}}|\mathbf{p}\rangle=\mathbf{p}|\mathbf{p}\rangle, \quad \hat{\mathbf{H}}|\mathbf{p}\rangle=\omega_{\mathbf{p}}|\mathbf{p}\rangle, \quad\left\langle\mathbf{p} \mid \mathbf{p}^{\prime}\right\rangle=(2 \pi)^{3} 2 \omega_{\mathbf{p}} \delta^{3}\left(\mathbf{p}-\mathbf{p}^{\prime}\right)
$$
in the Heisenberg picture. (To avoid clutter of notation, let's assume only 1 species of particles for simplicity.) Let us also introduce a Gaussian wave packet
$$
\left|f_{1}\right\rangle \equiv \int d^{3} k f_{1}(\mathbf{p})|\mathbf{p}\rangle .
$$
- We should get rid of tadpoles
$$
\langle\Omega|\hat{\varphi}(x)| \Omega\rangle=0
$$
which causes transitions between the vacuum and 1-particle states. Then
$$
\left\langle\Omega\left|\hat{a}^{\dagger}(\mathbf{k}, t)\right| \Omega\right\rangle=0, \quad\left\langle\Omega\left|\hat{a}_{1}^{\dagger}(t)\right| \Omega\right\rangle=0
$$
- We should normalize 1-particle states
$$
\langle\mathbf{p}|\hat{\varphi}(x)| \Omega\rangle=\sqrt{Z} e^{-i p \cdot x}
$$
cf. the Källén-Lehmann spectral representation. (Refs. 1 \& 2 furthermore assume that $Z=1$.)
- One may show that
$$
\hat{a}^{\dagger}(\mathbf{p}, \pm \infty)|\Omega\rangle=|\mathbf{p}\rangle, \quad \hat{a}(\mathbf{p}, \pm \infty)|\Omega\rangle=0
$$
cf. e.g. this Phys.SE answer by user1379857. (A possible relative phase is conventionally set equal to 1.) Note that the normalization is $\langle\mathbf{p} \mid \mathbf{k}\rangle=Z(2 \pi)^{3} 2 \omega \delta^{3}(\mathbf{p}-\mathbf{k})$.

- Similarly, for fixed total 3 -momentum p, multi-particle states are more energetic than the 1-particle state $|\mathbf{p}\rangle$, and hence automatically suppressed for asymptotic times due to the Riemann-Lebesque Lemma.
8. Finally let us return to OP's main question. Eq. (5.10) is fine as it is because eq. (5.2) is valid for interacting fields. Alternatively, one can postpone the use of the fundamental theorem of calculus (FTC) to a later stage as follows:
$$
\begin{aligned}
\hat{a}_{1}^{\dagger}(\infty) &-\hat{a}_{1}^{\dagger}(-\infty) \\
&=\sqrt{Z}\left[\hat{a}_{1, \text { out }}^{\dagger}(\infty)-\hat{a}_{1, \text { in }}^{\dagger}(-\infty)\right] \\
& \stackrel{(5.2)}{=}-i \sqrt{Z} \int d^{3} k f_{1}(\mathbf{k}) \int d^{3} x\left[e^{i k \cdot x} \overleftrightarrow{\partial}_{0} \hat{\varphi}_{\text {out }}(\infty, \mathbf{x})-e^{i k \cdot x} \overleftrightarrow{\partial}_{0} \hat{\varphi}_{\text {in }}(-\infty, \mathbf{x})\right] \\
&=-i \int d^{3} k f_{1}(\mathbf{k}) \int d^{3} x\left[e^{i k \cdot x} \overleftrightarrow{\partial}_{0} \hat{\varphi}(\infty, \mathbf{x})-e^{i k \cdot x} \overleftrightarrow{\partial}_{0} \hat{\varphi}(-\infty, \mathbf{x})\right] \\
& \stackrel{\text { FTC }}{=}-i \int d^{3} k f_{1}(\mathbf{k}) \int d^{4} x \partial_{0}\left[e^{i k \cdot x} \overleftrightarrow{\partial}_{0} \hat{\varphi}(x)\right] \\
&=\ldots
\end{aligned}
$$


