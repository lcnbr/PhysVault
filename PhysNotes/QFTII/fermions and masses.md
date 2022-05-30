A peculiar feature of the electroweak interactions for the fermionic matter fields is that they are **chiral; they are not invariant under spacetime parity transformations**. Chiral couplings of spinors to a vector field are modelled by the axial current $\bar{\psi} \gamma^{5} \gamma^{\mu} \psi$ instead of the more familiar vector current $\bar{\psi} \gamma^{\mu} \psi$. The matrix $\gamma^{5}$ receives an extra sign under parity transformations because it is based on the totally antisymmetric tensor $\varepsilon^{\mu \nu \rho \sigma}$.

Superficially one could combine vector and axial couplings. In nature, however, it was found that the vector and axial couplings have exactly the same strength. This finding is in line with theory: Couplings to vector fields should arise only by means of some [[YM covariant derivative|covariant derivative]]. In other words, the form of the Dirac equation typically predicts vector couplings. However, we can split up the Dirac spinor into two chiral spinors,
$$
\psi=\psi_{\mathrm{L}}+\psi_{\mathrm{R}}, \quad \psi_{\mathrm{L} / \mathrm{R}}=\frac{1}{2}\left(1 \pm \gamma^{5}\right) \psi .
$$
Then the derivative terms for the two components decouple entirely ^[[2N). However, in many models this group splits into U(N)L ⇥ U(N)R (left/right or vector/axial) by mass terms or other interactions. For example in the standard model, the complex conjugate of a right-handed quark transforming as a 3 of SU(3) is a left-handed quark transforming in the [conjugate representation](../math/defining representation of su(n|Note that the complex conjugate of a right-handed spinor is left-handed. Therefore, every model can be represented by left-handed spinors only. The maximal symmetry acting on N Dirac spinors therefore is U(2N). However, in many models this group splits into U(N)L ⇥ U(N)R (left/right or vector/axial) by mass terms or other interactions. For example in the standard model, the complex conjugate of a right-handed quark transforming as a 3 of SU(3) is a left-handed quark transforming in the [conjugate representation]].md)  ̄ 3 of SU(3). The latter is different from what is commonly called the lefthanded quarks which transform as a 3 of SU(3). ]^[ In dimensional regularisation it is difficult to represent $\gamma^5$, and it should be avoided in the kinetic terms. A single chiral spinor should be supplemented by a spinor of opposite chirality which does not interact with any other field. In that way all matrices $\gamma^5$ can be shifted to the interactions.
]
$$
\bar{\psi} \gamma^{\mu} \partial_{\mu} \psi=\bar{\psi}_{\mathrm{L}} \gamma^{\mu} \partial_{\mu} \psi_{\mathrm{L}}+\bar{\psi}_{\mathrm{R}} \gamma^{\mu} \partial_{\mu} \psi_{\mathrm{R}} .
$$
If we let the left and right components transform in different representations of the gauge group, we naturally obtain chiral couplings
$$
\begin{aligned}
& \bar{\psi}_{\mathrm{L}} \gamma^{\mu} D_{\mu}^{\mathrm{L}} \psi_{\mathrm{L}}+\bar{\psi}_{\mathrm{R}} \gamma^{\mu} D_{\mu}^{\mathrm{R}} \psi_{\mathrm{R}} \\
=& \bar{\psi} \gamma^{\mu}\left(\partial_{\mu}+\frac{1}{2} g A_{\mu}^{a}\left(T_{a}^{\mathrm{L}}+T_{a}^{\mathrm{R}}\right)\right) \psi-\frac{1}{2} g A_{\mu}^{a} \bar{\psi} \gamma^{5} \gamma^{\mu}\left(T_{a}^{\mathrm{R}}-T_{a}^{\mathrm{L}}\right) \psi .
\end{aligned}
$$
Since the choice of representation in compact groups is typically discrete, there are only discrete choices for the vector and axial couplings. For example, when one of the representations is trivial, the vector and axial couplings have equal magnitude.

In the electroweak model, the representations for the spinor fields follow a particular pattern: 
- The left-handed components transform in isospin- $1 / 2$ representations of $\mathrm{SU}(2)$ which unite two types of fields: electrons and neutrinos as well as up and down quarks. 
- Conversely, the right-handed components form (two) singlets. The $U(1)$ hypercharges are arranged such that the electromagnetic charges fit the observed values. The following tables list the representations of the particles in terms of third component of isospin $I_{3}$, hypercharge $Y$ as well as multiplicity in terms of colour within QCD

| field | $I_3$ |   Y   |  C  |
|:-----:|:-----:|:-----:|:---:|
| $v_R$ |   $0$   |   $0$   |  $3$  |
| $e_R$ |   $0$   |  $-1$   |  $3$  |
| $u_R$ |   $0$   | $\frac{+2}{3}$ |  $3$  |
| $d_R$ |   $0$   | $\frac{-1}{3}$ |  $3$  |

^a5b73b

|                                           field                                           |                           $I_3$                          |        Y         |  C  |
|:-----------------------------------------------------------------------------------------:|:---------------------------------------------------------:|:----------------:|:---:|
| $L_{\mathrm{L}}=\left(\begin{array}{l}v_{\mathrm{L}} \\ e_{\mathrm{L}}\end{array}\right)$ | $\left(\begin{array}{l}+1 / 2 \\-1 / 2\end{array}\right)$ | $-\frac{1 }{ 2}$ | $1$ |
| $Q_{\mathrm{L}}=\left(\begin{array}{l}u_{\mathrm{L}} \\d_{\mathrm{L}}\end{array}\right)$  | $\left(\begin{array}{l}+1 / 2 \\-1 / 2\end{array}\right)$ |  $\frac{+1}{6}$  |  3  |

^42a589

We shall consider only the first of the three generations of spinor fields. The other two families have analogous properties in all aspects that we will discuss


An interesting result of symmetry breaking is that while the coupling to all vector fields of $\operatorname{SU}(2) \times U(1)$ violates parity strongly, the coupling to the resulting electromagnetic field is via the usual vector current $\bar{\psi} \gamma^{\mu} \psi$. This may appear surprising, but it is a consequence of current conservation: After **symmetry breaking, the spinor fields are massive (see below) which violates conservation of the axial currents, but a remaining gauge symmetry can only couple to conserved currents.**

A consequence of unequal representations for the chiral components is that the usual Dirac mass term is not allowed
$$
\bar{\psi} \psi=\bar{\psi}_{\mathrm{R}} \psi_{\mathrm{L}}+\bar{\psi}_{\mathrm{L}} \psi_{\mathrm{R}} .
$$
For instance, it would break conservation of axial currents, and thus violate the gauge symmetry. There is another type of mass term for Dirac fields, called a Majorana mass, but it is allowed only for real representations. All representations in the standard model, however, are complex, except for a right-handed neutrino which is a singlet. 

Just like the vector particles, the fermions can only acquire masses by means of the Higgs field which has the following charges:

|                           field                           |                           $I_3$                           |   Y   |  C  |
|:---------------------------------------------------------:|:---------------------------------------------------------:|:-----:|:---:|
| $H=\left(\begin{array}{c}H^{+} \\H^{0}\end{array}\right)$ | $\left(\begin{array}{l}+1 / 2 \\-1 / 2\end{array}\right)$ | $\frac{+1}{2}$ |  $1$ |


The Higgs field can couple via Yukawa interactions to the spinor fields. There are 4 gauge-invariant couplings
$$
\bar{\nu}_{\mathrm{R}} H^{\top} \varepsilon L_{\mathrm{L}}, \quad \bar{e}_{\mathrm{R}} H^{\dagger} L_{\mathrm{L}}, \quad \bar{u}_{\mathrm{R}} H^{\top} \varepsilon Q_{\mathrm{L}}, \quad \bar{d}_{\mathrm{R}} H^{\dagger} Q_{\mathrm{L}},
$$
where $\varepsilon$ is the $2 \times 2$ antisymmetric matrix. The vacuum expectation value of the Higgs field then generates a mass term for each of the particle species: neutrinos, electrons, up and down quarks. ${ }^{11}$