# Supersymmetry

String theory does contain spin-2-particles, which can be identified with [[graviton]]s. A fermionic extension of string theory will likely include spin- $\frac{3}{2}$ particles, which will be called gravitini. Gravitini can only exist in a supergravity theory, a supersymmetric version of a gravitational gauge theory. In those field thoeries, spacetime symmetries are extended by supersymmetry.

![[Pasted image 20220123215407.png]]

# Super-Poincaré Algebra.
The super-Poincaré algebra is an extension of the Poincaré algebra. While the Poincaré algebar consists of Lorentz rotations $M_{\mu \nu}$ and translations $P_{\mu}$,

$$
[M, M] \sim M, \quad[M, P] \sim P, \quad[P, P]=0
$$

The super-Poincaré algebra has additional generators, the so-called supercharges $Q_{m}^{I}$. They transform in spinor representations of the Lorentz algebra ( $m$ is a spinor index), and they are odd generators whose [[Lie bracket|Lie brackets]] are symmetric rather than anti-symmetric

$$
[M, Q] \sim Q, \quad[Q, P]=0, \quad\left\{Q_{m}^{I}, Q_{n}^{J}\right\} \sim \delta^{I J} \gamma_{m n}^{\mu} P_{\mu} .
$$

Furthermore, $\mathcal{N}$ is the rank of supersymmetry $I=1, \ldots, \mathcal{N}$. The supercharges $Q$ relate particles of different spin and different statistics, which are equal otherwise. Thus, supersymmetry can be considered as a symmetry relating "forces" and "matter".

# Wess-Zumino Model. 
Let us discuss a simple example of a supersymmetric field theory in $D=4$ dimensions. It consists of a complex scalar field $\phi$ and a chiral $^{1}$ fermion $\psi_{m}$ with Lagrangian

$$
\begin{aligned}
\mathcal{L}=&-\partial^{\mu} \bar{\phi} \partial_{\mu} \phi-\bar{m} m \bar{\phi} \phi \\
&-i \sigma_{\mu}^{n \dot{m}} \bar{\psi}_{\dot{m}} \partial^{\mu} \psi_{n}-\frac{1}{2} m \varepsilon^{m n} \psi_{m} \psi_{n}+\frac{1}{2} \bar{m} \varepsilon^{\dot{m} \dot{n}} \bar{\psi}_{\dot{m}} \bar{\psi}_{\dot{n}} \\
&-\frac{1}{2} \bar{g} m \bar{\phi}^{2} \phi-\frac{1}{2} g \bar{m} \bar{\phi} \phi^{2}-\frac{1}{4} g \bar{g} \bar{\phi}^{2} \phi^{2} \\
&-\frac{1}{2} g \varepsilon^{m n} \phi \psi_{m} \psi_{n}+\frac{1}{2} \bar{g} \varepsilon^{\dot{m} \dot{n}} \bar{\phi} \bar{\psi}_{\dot{m}} \bar{\psi}_{\dot{n}} .
\end{aligned}
$$

The fields both have mass $|m|$ and their scalar and Yukawa interactions are governed by a complex coupling constant $g$. The $2 \times 2$ matrices $\sigma_{\mu}$ are a generalisation of the Pauli matrices to chiral spinors in $D=(3,1)$. The $2 \times 2$ matrices $\varepsilon$ are anti-symmetric with $\varepsilon^{12}=\varepsilon_{12}=+1$.

Evidently, this model is Poincaré-invariant. In addition it has an invariance parametrised by a constant fermionic chiral spinor $\delta \epsilon_{m}$

$$
\begin{aligned}
\delta \phi &=\varepsilon^{m n} \delta \epsilon_{m} \psi_{n}, \\
\delta \bar{\phi} &=-\varepsilon^{\dot{m} \dot{n}} \delta \bar{\epsilon}_{\dot{m}} \bar{\psi}_{\dot{n}}, \\
\delta \psi_{m} &=-i \varepsilon_{m n} \sigma_{\mu}^{n \dot{\rho}} \delta \bar{\epsilon}_{\dot{p}} \partial^{\mu} \phi-\delta \epsilon_{m}\left(\bar{m} \bar{\phi}+\frac{1}{2} \bar{g} \bar{\phi}^{2}\right), \\
\delta \bar{\psi}_{\dot{m}} &=+i \varepsilon_{\dot{m} \dot{n}} \sigma_{\mu}^{p \dot{n}} \delta \epsilon_{p} \partial^{\mu} \bar{\phi}-\delta \bar{\epsilon}_{\dot{m}}\left(m \phi+\frac{1}{2} g \phi^{2}\right) .
\end{aligned}
$$

To show invariance under this transformation is tedious but straight-forward. 

# Supermultiplets. 
The classification of unitarity irreducible representations (UIR) of the Poincaré algebra distinguishes particles by their mass and spin (or helicity for massless particles). UIR's of the super-Poincaré algebra combine several UIR's of the ordinary Poincaré algebra into a supermultiplet. Let us discuss some features of supermultiplets.

The size and constituents of a supermultiplet depend strongly on:
- the number of dimensions $D$ 
-  the $\operatorname{rank}$ of supersymmetry $\mathcal{N}$. 
 - If $N$ denotes the number of supercharges in total, a minimal supermultiplet has $2^{N / 2}$ constituent fields.

For instance, the Wess-Zumino model has 4 on-shell degrees of freedom: a complex scalar $\phi$ and a chiral spinor $\psi$. It has the minimum amount of $\mathcal{N}=1$ supersymmetry which in $D=4$ amounts to $N=4$ supercharges. the fields $\phi$ and $\psi$ therefore form the minimal supermultiplet.

Note that in the massless case supermultiplets are typically much smaller. It can be shown that half of the supercharges generate states of zero norm. As usual, these states are irrelevant for physics and should be projected out. The resulting minimal supermultiplet then has only $2^{N / 4}$ states.



The above considerations also lead to an upper bound on the allowable number of supercharges in an interacting QFT: every positive supercharge increases the considered spin components by half a unit. Given $N$ supercharges, the spin component therefore increases by $N / 8$ units in total within the supermultiplet. Therefore the maximum total spin in a supermultiplet is at least $N / 16$. since the maximum spin must not exceed $1 / 2$ for matter fields, 1 for gauge fields and 2 for gravity, the maximum number of allowable supercharges equals 8,16 and 32 , respectively. 

# Superspace. 
Supersymmetry is not merely a curiosity of particular QFT's, it also has a geometric meaning: It is the translational symmetry of superspace which [[#Super-Poincaré Algebra|extends]] the ordinary Minkowski space coordinates $x^{\mu}$ by $N$ anti-commuting coordinates $\theta_{I}^{m}$. Fields on superspace can be expanded in $\theta$ to yield a finite collection of fields with various spin

$$
F(x, \theta)=F_{0}(x)+F_{m}^{I}(x) \theta_{I}^{m}+* \theta^{2}+\ldots+F_{N}(x) \theta^{N} .
$$

This allows to package a supermultiplet of particles into a single field on superspace.

# Spinors. 
Supersymmetry is based on spinor representations of the group $\operatorname{Spin}(D-1,1)$ which is a two-fold cover of the [[Lorentz group]] $\mathrm{SO}(D-1,1)$. Let us discuss spinor representations in various dimensions.

In $D=4$, the default (Dirac) spinor has 4 complex components, it belongs to the space $\mathbb{C}^{4}$. It can be split into two chiral spinors (Weyl): $\mathbb{C}^{2} \oplus \mathbb{C}^{2}$. Alternatively, a reality condition (Majorana) can be imposed: $\operatorname{Re}\left(\mathbb{C}^{4}\right)=\mathbb{R}^{4} \simeq \mathbb{C}^{2}=\operatorname{Re}\left(\mathbb{C}^{2} \oplus \mathbb{C}^{2}\right)$. Note that in $D=4$ the reality condition cannot be imposed on chiral spinors because complex conjugation flips chirality.

Let us now summarise the features on spinors in higher dimensions:

- The dimension of the Dirac spinor is multiplied by a factor of 2 for every step $D \rightarrow$ $D+2$.
- Chiral spinors (Weyl) exist only when $D$ is even.
- Real spinors (Majorana) exist for $D=0,1,2,3,4(\bmod 8)$.


The number of supercharges $N=\mathcal{N}\times \text{dim}_\text{spinor}$. This leads to a maximum rank of supersymmetry $\mathcal{N}$ in a given dimension $D$ and a maximum dimension $D$ for interacting supersymmetric QFT's:

- For $D=4$ the maximum rank is $\mathcal{N}=2,4,8$ for matter ($N=8$), gauge ($N=16$) and gravity theories ($N=32$), respectively.

- In $D=10$ $\implies \text{dim}_\text{dirac spinor}=2^{\frac{10}{2}=32}\implies\text{dim}_\text{chiral spinor}=16$ the minimum spinor is the real chiral spinor with 16 components. This is the dimensional bound for gauge theories.

- In $D=11$ the real spinor has 32 components. This is the dimensional bound for gravitational theories.