---
alias:
tags:
- qftII
---
A related issue is unitarity of the physical scattering matrix. The [[BRST symmetry|BRST operator]] is a symmetry; therefore it commutes with the Hamiltonian and with the S-matrix ${ }^{20}$
$$
[Q, S]=0
$$

^ae2739

Consider some [[BRST cohomology#^phys|physical initial state]]   $|\Psi\rangle$. It is scattered to a final state $S|\Psi\rangle$ which is closed
$$
Q S|\Psi\rangle=S Q|\Psi\rangle=0
$$
As expected, changing the representative of the initial state changes the representative of the final state
$$
S\left|\Psi^{\prime}\right\rangle=S|\Psi\rangle+S Q|\Omega\rangle=S|\Psi\rangle+Q S|\Omega\rangle
$$
We can now consider unitarity of the S-matrix $S^{\dagger} S=1$. Towards deducing the optical theorem we should insert the decomposition of unity between the S-matrices
$$
1=\sum_{\Omega}|\Omega\rangle\left\langle\Omega^{*}\right|
$$
where $\{|\Omega\rangle\}$ is some basis of the full Hilbert space $\mathbb{H}$ and $\left\{\left\langle\Omega^{*}\right|\right\}$ is the corresponding dual basis of $\mathbb{H}^{*}$ with $\left\langle\Omega^{*} \mid \Omega^{\prime}\right\rangle=\delta_{\Omega, \Omega^{\prime}}$. For our purposes it makes sense to pick a basis of physical, [[BRST cohomology|unphysical]] and [[BRST cohomology|exact states]]. This decomposition is not intuitive because the space $\mathbb{H}_{\mathrm{ex}}$ is null in the scalar product of states. Let us discuss the implications briefly:

Consider an [[BRST cohomology|exact state]] $|\Omega\rangle=Q|\Lambda\rangle$. By construction its overlap with the dual state $\left\langle\Omega^{*}\right|$ is non-zero
$$
0 \neq\left\langle\Omega^{*} \mid \Omega\right\rangle=\left\langle\Omega^{*}|Q| \Lambda\right\rangle .
$$
From this it follows that $\left\langle\Omega^{*}\right| Q$ cannot be trivial and therefore must be an unphysical costate. Similarly one can argue that 
$$
\begin{aligned}
\left(\mathbb{H}_{\mathrm{ex}}\right)^{*} &=\mathbb{H}_{\text {unphys }} \\
\left(\mathbb{H}_{\text {phys }}\right)^{*} &=\mathbb{H}_{\text {phys }} \\
\left(\mathbb{H}_{\text {unphys }}\right)^{*} &=\mathbb{H}_{\text {ex. }}
\end{aligned}
$$
The decomposition of unity can thus be written as 
$$
1=\sum_{\Omega \text { physical }}\ket{\Omega }\bra{\Omega}+\sum_{\bra{\Omega} \text { exact }}\ket{\Omega }\bra{\Omega^{*} }+\sum_{\bra{\Omega^{*} }\text { exact }} \ket{\Omega }\bra{\Omega^{*}}.
$$
Let us now turn to the formulation of the optical theorem by considering matrix elements of the unitarity statement for two [[BRST cohomology|physical states]]
$$
\left\langle\Phi\left|S^{\dagger} S\right| \Psi\right\rangle=\langle\Phi \mid \Psi\rangle
$$
The above decomposition of unity is very convenient because the [[BRST cohomology|exact states]] $|\Omega\rangle$ and $\left\langle\Omega^{*}\right|$ are cancelled in the combination $\left\langle\Phi\left|S^{\dagger}\right| \Omega\right\rangle$ and $\left\langle\Omega^{*}|S| \Psi\right\rangle$, respectively ([[#^ae2739]]). The optical theorem can thus be expressed as
$$
\left\langle\Phi\left|S^{\dagger} S\right| \Psi\right\rangle=\sum_{\Omega \text { physical }}\left\langle\Phi\left|S^{\dagger}\right| \Omega\right\rangle\langle\Omega|S| \Psi\rangle=\langle\Phi \mid \Psi\rangle .
$$
In the optical theorem one is therefore free to restrict the sum over intermediate states to physical intermediate states as desired (as long as the external states are physical). However, one can also perform the sum over all intermediate states including unphysical ones. The result was hown to be the same, therefore the contributions from unphysical gauge modes must cancel exactly against the contributions from [[Faddeev-Popov ghosts|ghost]] modes. The applicability of the full intermediate Hilbert space is crucial because unphysical gauge and [[Faddeev-Popov ghosts|ghost]] fields do propagate within loops.

In conclusion, **it is consistent to restrict the S-matrix to physical external states, even though loop amplitudes are computed using all the fields.**

Independence of [[gauge fixing action for EM|Gauge Fixing]]. 

Finally, let us consider the relevance of the gauge-fixing terms of the Lagrangian. From [[BRST transformation#^e15f52]] we have already seen that $\mathcal{L}_{\mathrm{BRST}}$ is exact, $\mathcal{L}_{\mathrm{BRST}}=Q K_{\mathrm{BRST}}$, while $\mathcal{L}_{Y M}$ is [[BRST cohomology#^physical|physical]] ([[BRST transformation#^f64663|closed]] but [[BRST transformation#^f33149|not exact]]). Both terms contribute to the Hamiltonian and therefore they govern the time-evolution and scattering of states.

Consider a [[BRST cohomology|physical state]] $|\Psi\rangle$ and act with $\mathcal{L}_{\mathrm{BRST}}$. It can be written as
$$
\mathcal{L}_{\text {BRST }}|\Psi\rangle=\left(Q K_{\text {BRST }}\right)|\Psi\rangle=Q\left(K_{\text {BRST }}|\Psi\rangle\right) .
$$
It shows that whenever the gauge-fixing term is applied to a [[BRST cohomology|physical state]], the result must be an [[BRST cohomology|exact state]] which is equivalent to the zero state.

**This sketch of an argument demonstrates that the precise formulation of the [[gauge fixing action for EM|gauge fixing]] does not influence the correlators of [[BRST cohomology|physical states]]. In particular all physical correlators are independent of the gauge-fixing parameter $\xi$**.