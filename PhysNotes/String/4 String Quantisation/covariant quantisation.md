---
Alias:
- canonical quantisation
---
From the [[classical closed string in the Hamiltonian formalism]] we derived the [[../Poisson brackets]] for the [[../closed string]]: 
![[classical closed string in the Hamiltonian formalism#^b420f5]]
In [[.md|canonical quantisation]] this results in the following set of commutation relations of the corresponding quantum operators
$$
\begin{aligned}
\left[x^{\mu}, p^{\nu}\right] &=i \eta^{\mu \nu} \\
\left[\alpha_{m}^{\mathrm{L}, \mu}, \alpha_{n}^{\mathrm{L}, \nu}\right]=\left[\alpha_{m}^{\mathrm{R}, \mu}, \alpha_{n}^{\mathrm{R}, \nu}\right] &=m \eta^{\mu \nu} \delta_{m+n}
\end{aligned}
$$

^58ef6b

## Space of States. 
Compose the space of [[states]] from a [[quantum free particle]] and a set of [[../quantum harmonic oscillator]]s:
- momentum eigenstates for free particle $|q\rangle$,
- [[../quantum harmonic oscillator|HO]] vacuum $|0\rangle$ and excitations for each mode/orientation.

Define ![[../closed string vacuum state]] 
## Negative Norm States. 
One problem: we have states with negative norm
$$
\begin{aligned}
|n, \mu, \mathrm{L} / \mathrm{R} ; q\rangle &:=\alpha_{-n}^{\mathrm{L} / \mathrm{R}, \mu}|0 ; q\rangle \\
|n, \mu, \mathrm{L} / \mathrm{R} ; q|^{2} &=\left\langle 0 ; q\left|\alpha_{n}^{\mathrm{L} / \mathrm{R}, \mu} \alpha_{-n}^{\mathrm{L} / \mathrm{R}, \mu}\right| 0 ; q\right\rangle=n \eta^{\mu \mu}
\end{aligned}
$$
For $\mu=0$ this state has negative norm. In fact, it is not allowed by Virasoro constraints. General resolution of this problem: impose Virasoro constraints! All states obeying the Virasoro constraints have non-negative norm. This problem needs some care. We shall continue the covariant quantisation later.
