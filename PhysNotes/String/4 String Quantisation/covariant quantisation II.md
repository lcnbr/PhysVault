---
alias:
tags:
- stringTheory
---
# Covariant quantisation II
In [[light cone quantisation]], [[../Poincare invariance|Poincaré symmetry]] is subject to an [[../../QFTII/anomaly]]. One can as well keep [[../Poincare invariance|Poincaré symmetry]] manifest: this is known as covariant quantisation. First steps for covariant quantisation have been done in [[covariant quantisation]].

Let us see how the spectrum arises in covariant approach. For simplicity, consider only one set of $L$ or $R$ oscillators.

# Vacuum State. 
The vacuum state $|0 ; q\rangle$ is defined as before by $\alpha_{0}^{\mu}|0 ; q\rangle \sim \kappa q^{\mu}|0 ; q\rangle$, $\alpha_{n>0}^{\mu}|0 ; q\rangle=0$. It satisfies
$$
L_{n>0}|0 ; q\rangle=0 \quad \text { and } \quad L_{0}|0 ; q\rangle=\frac{\kappa^{2} q^{2}}{4}|0 ; q\rangle .
$$
The state is not annihilated by the negative Virasoro modes. Instead $\langle 0 ; q| L_{n<0}=0$ hence $\left\langle 0 ; q\left|\left(L_{n}-\delta_{n} a\right)\right| 0 ; q\right\rangle=0 .$

#  generic physical states
For generic physical states $|\Psi\rangle,\langle\Phi|$ we should impose the [[../Virasoro constraints]]
$$
\begin{array}{ll}
L_{n>0}|\Psi\rangle=0, & L_{0}|\Psi\rangle=a|\Psi\rangle, \\
\langle\Phi| L_{n<0}=0, & \left\langle\Phi\left|L_{0}=a\right| \Phi\right\rangle,
\end{array}
$$
such that we have
$$
\left\langle\Phi\left|\left(L_{n}-\delta_{n} a\right)\right| \Psi\right\rangle=0 .
$$

# Virasoro Algebra. 
The algebra of quantum charges $L_{n}$ reads
$$
\left[L_{m}, L_{n}\right]=(m-n) L_{m+n}+\frac{c}{12} m\left(m^{2}-1\right) \delta_{m+n} .
$$
This defines the Virasoro algebra. The latter term is the central charge $c$ of Virasoro algebras (rather its representation on fields), namely $c=D$ in our case. We are interested in primary states
$$
L_{n>0}|\Psi\rangle=0, \quad L_{0}|\Psi\rangle=a|\Psi\rangle .
$$
We can now apply representation theory of the Virasoro algebra $\Rightarrow 2 \mathrm{D}$ CFT.
A proper treatment (BRST) requires additional [[../../QFTII/Faddeev-Popov ghosts|ghost]] fields. Inclusion of [[../../QFTII/Faddeev-Popov ghosts|ghost]] fields recovers the classical conformal algebra precisely when $D=26$ and $a=1$
$$
\left[L_{m}, L_{n}\right]=(m-n) L_{m+n} .
$$
In covariant gauge, the conformal algebra is anomalous. In light cone gauge, however, the [[../../QFTII/anomaly]] is shifted to the Lorentz algebra. $^{7}$ The [[../../QFTII/anomaly]] is proportional to $D-26$ and $a-1$, i.e. it can be avoided for a very specific choice of parameters.
