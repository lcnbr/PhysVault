---
alias:
tags:
- qftII
---
We have learned in QFT I that a massless Dirac spinor field has a chiral symmetry
$$
\psi \rightarrow \exp \left(-i \gamma^{5} \beta\right) \psi
$$
in addition to its usual electric charge symmetry $\psi \rightarrow \exp (i \alpha) \psi$. The associated [[Noether's theorem|Noether current]] is the axial current
$$
N_{\mathrm{A}}^{\mu}=-i \bar{\psi} \gamma^{5} \gamma^{\mu} \psi
$$
It is classically conserved, even in the presence of the electromagnetic field
$$
\partial \cdot N_{\mathrm{A}}=-i \bar{\psi} \gamma^{5} \gamma^{\mu}\left(D_{\mu} \psi\right)-i\left(D_{\mu} \bar{\psi}\right) \gamma^{5} \gamma^{\mu} \psi=0
$$
The naive [[Slavnov-Taylor identities#As a correlator|Slavnov-Taylor identity]] for the axial current thus reads
$$
\left\langle\partial_{\mu} N_{\mathrm{A}}^{\mu}-\imath \bar{\rho} \gamma^{5} \psi-i \bar{\psi} \gamma^{5} \rho\right\rangle_{\rho, \bar{\rho}, J}=0 .
$$

^c15399

Consider now the correlator of the axial current with two photons
$$
\left\langle\partial \cdot N_{\mathrm{A}}(x) F_{\mu \nu}(y) F_{\rho \sigma}(z)\right\rangle \stackrel{?}{=} 0 .
$$
By the above identity the correlator should be zero because there are no further fermions to which the extra terms in the identity could couple.


Let us discuss the two contributions from one-loop graphs

![[Pasted image 20220126130921.png|400]]

We define the corresponding loop integral in momentum space as
$$
L^{\mu \nu \rho}\left(p, p^{\prime}\right):=I^{\mu \nu \rho}\left(p, p^{\prime}\right)+I^{\nu \mu \rho}\left(p^{\prime}, p\right)
$$
with
$$
\begin{aligned}
I^{\mu v \rho}\left(p, p^{\prime}\right): &:=\int \frac{-i \mathrm{~d} \ell^{4}}{(2 \pi)^{4}} \operatorname{Tr}\left[\gamma^{5} \gamma^{\rho} \frac{\gamma \cdot(\ell-p)}{(\ell-p)^{2}} \gamma^{\mu} \frac{\gamma \cdot \ell}{\ell^{2}} \gamma^{\nu} \frac{\gamma \cdot\left(\ell+p^{\prime}\right)}{\left(\ell+p^{\prime}\right)^{2}}\right] \\

\end{aligned}
$$
![[Pasted image 20220126131003.png|200]]

The above correlator consists of the contraction $k_{\rho} L^{\mu v \rho}\left(p, p^{\prime}\right)$. Now write $k=-p-p^{\prime}=(\ell-p)-\left(\ell+p^{\prime}\right)$, split the integrand into two terms and permute one past $\gamma^{5}$. Each term then cancels one of the adjacent spinor propagators. Permuting another term past $\gamma^{5}$ yields
$$
k_{\rho} I^{\mu v \rho}=\int \frac{-i \mathrm{~d} \ell^{4}}{(2 \pi)^{4}} \operatorname{Tr}\left[\gamma^{5} \gamma^{\mu} \frac{\gamma \cdot \ell}{\ell^{2}} \gamma^{v}\left(\frac{\gamma \cdot\left(\ell+p^{\prime}\right)}{\left(\ell+p^{\prime}\right)^{2}}-\frac{\gamma \cdot(\ell-p)}{(\ell-p)^{2}}\right)\right]
$$
It is tempting to argue that this integral vanishes:

- The trace of gamma-matrices produces the anti-symmetric tensor $\varepsilon$ in four dimensions, $\operatorname{Tr} \gamma^{5} \gamma^{\mu} \gamma^{v} \gamma^{\rho} \gamma^{\sigma}=4 i \varepsilon^{\mu \nu \rho \sigma}$.
- When writing the expression as a difference of two integrals, each one should depend on either $p$ or $p^{\prime}$ but not on both.
- Altogether there are only three vectors or indices at our disposal: $\mu, \rho$ and either $p$ or $p^{\prime}$. There is nothing to act as the fourth index of $\varepsilon$.

This conclusion is however too naive: One must pay attention to the fact that the two above integrals are divergent. Subtracting two divergent integrals is an ambiguous operation. The result may in principle be adjusted to any desired value, be it zero, finite or infinite.
In fact, the original integral $I^{\mu \nu \rho}$ diverges linearly which implies that its value depends on the choice of integration boundary. In other words, a shift of the loop momentum $\ell$ by $\delta \ell$ is not trivial, but it changes the integral $I^{\mu \nu \rho}$ by a finite amount
$$
\delta I^{\mu v \rho}=-\frac{i}{8 \pi^{2}} \varepsilon^{\mu \nu \rho \sigma} \delta \ell_{\sigma} .
$$
Importantly, such a shift can modify the conservation of currents and therefore the integration boundary has to be defined carefully.

Even though there is some arbitrariness in the definition of $I^{\mu v \rho}$, it does obey some unambiguous relations, which can be seen as obstructions to symmetries. Concretely, the definition of the loop integral $I^{\mu v \rho}\left(p, p^{\prime}\right)$ is cyclically symmetric in its three legs, but only up to a shift of the integration variable. Non-triviality of the latter implies a non-trivial cyclic symmetry relationship
$$
\begin{aligned}
I^{\mu \nu \rho}\left(p, p^{\prime}\right) &=I^{\nu \rho \mu}\left(p^{\prime}, k\right)-\frac{i}{8 \pi^{2}} \varepsilon^{\mu \nu \rho \sigma} p_{\sigma}^{\prime} \\
&=I^{\rho \mu \nu}(k, p)+\frac{i}{8 \pi^{2}} \varepsilon^{\mu \nu \rho \sigma} p_{\sigma} .
\end{aligned}
$$
For the relevant symmetric combination $L^{\mu v \rho}$ this implies a relationship between the conservation of the axial and vector currents
$$
k_{\rho} L^{\mu \nu \rho}\left(p, p^{\prime}\right)=k_{\rho} L^{\rho \mu \nu}(k, p)+\frac{i}{4 \pi^{2}} \varepsilon^{\mu \nu \rho \sigma} p_{\rho} p_{\sigma}^{\prime} .
$$
By choosing the integration such that the vector current is exactly conserved, $k_{\rho} L^{\rho \mu \nu}(k, p)=0$, which is crucial for a consistent [[gauge symmetry]] in the quantum theory, we find that the axial current is not conserved
$$
k_{\rho} L^{\mu \nu \rho}\left(p, p^{\prime}\right)=\frac{i}{4 \pi^{2}} \varepsilon^{\mu \nu \rho \sigma} p_{\rho} p_{\sigma}^{\prime}
$$
The pitfall in the above considerations depends on the regularisation scheme. We have argued using a momentum cut-off. However the same conclusion can be reached in other schemes.

# In dimensional regularisation
the above derivation makes the mistake to assume that $\gamma^{5}$ anti-commutes with all $\gamma^{\mu}$. First of all $\gamma^{5}$ is a strictly 4-dimensional concept. One can still define an antisymmetric product of 4 gamma-matrices which imitates the behaviour of $\gamma^{5}$. However, there are discrepancies at $\mathcal{O}(\epsilon)$. For instance, it anticommutes with 4 gamma-matrices but it commutes with the remaining $(-2 \epsilon)$ ones.
$$
\gamma^{5} \gamma^{\mu} \neq-\gamma^{\mu} \gamma^{5}
$$
The resulting factor of $\epsilon$ is then cancelled by a factor of $1 / \epsilon$ from a divergent loop integral.

It is also instructive to investigate the integral $L^{\mu \nu \rho}$ in position space. The anomaly originates from a distributional contribution when taking a derivative at a singularity
$$
\begin{aligned}
& \frac{\partial}{\partial z^{\rho}} \operatorname{Tr}\left[\gamma^{5} \gamma^{\rho} \frac{\gamma \cdot(z-x)}{(z-x)^{4}} \gamma^{\mu} \frac{\gamma \cdot(x-y)}{(x-y)^{4}} \gamma^{v} \frac{\gamma \cdot(y-z)}{(y-z)^{4}}\right] \\
\sim & \varepsilon^{\mu v \rho \sigma} \partial_{\rho} \delta^{4}(z-x) \partial_{\sigma} \delta^{4}(z-y)
\end{aligned}
$$
which is analogous to the identity $\partial^{2} x^{-2} \sim \delta^{4}(x)$ required for the scalar propagator.


# Adler-Bell-Jackiw identity
Curiously, a careful evaluation in either scheme yields the same result. It can be summarised in the [[anomaly|anomalous]] [[Slavnov-Taylor identities|Slavnov-Taylor identity]] known as the Adler-Bell-Jackiw identity
$$
\left\langle\partial_{\mu} N_{\mathrm{A}}^{\mu}-i \bar{\rho} \gamma^{5} \psi-i \bar{\psi} \gamma^{5} \rho-q^{2}(4 \pi)^{-2} \varepsilon^{\mu v \rho \sigma} F_{\mu \nu} F_{\rho \sigma}\right\rangle_{\rho, \bar{\rho}, J}=0
$$
Adler and Bardeen showed that this identity is exact, there are no further corrections from higher loop orders.

Let us discuss the additional term in the Adler-Bell-Jackiw identity (compare to [[#^c15399]]). We note that it has a special form: it can be written as a total derivative of a local quantity. This allows to redefine the axial [[Noether's theorem|Noether current]] by a compensating local term involving the gauge fields
$$
N_{\mathrm{A}}^{\prime \mu}=N_{\mathrm{A}}^{\mu}-\frac{q^{2}}{8 \pi^{2}} \varepsilon^{\mu v \rho \sigma} A_{v} F_{\rho \sigma} .
$$
which obeys the ordinary Slavnov-Taylor identity. However, in contradistinction to $N_{\mathrm{A}}$, the redefined axial current is no longer gauge invariant due to the presence of a bare gauge potential $A$. This again points at a clash between axial and [[gauge symmetry]] in the quantum theory.

A related feature of the anomaly term $F \wedge F=\mathrm{d}(A \wedge F)$ is that its integral is topological; it does not depend on the local degrees of freedom of the gauge field. As the Slavnov-Taylor identity was derived in integral form while discarding all potential boundary contributions, it is perhaps not too surprising to observe that the anomaly term has such a structure.