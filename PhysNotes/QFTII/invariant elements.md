---
alias:
tags:
- qftII
---
We have a [[Killing form]] and [[Casimir invariant]], each defined up to a constant $B^R$ and $C^R_2$



The factors $B^{R}$ and $C_{2}^{R}$ (among others) can be used to characterise irreducible representations. They also appear as characteristic quantities in computations of Feynman diagrams. Let us therefore discuss them in more detail.

By taking the trace of the identity $R\left(C_{2}\right)=C_{2}^{R}$ id $^{R}$ on both sides we can establish a relationship between the constants $B^{R}$ and $C_{2}^{R}$
$$
C_{2}^{R} \operatorname{Tr} \mathrm{id}^{R}=\operatorname{Tr} R\left(C_{2}\right)=\operatorname{Tr}(R \dot{\otimes} R) C_{2}=B^{R} K\left(C_{2}\right) .
$$

The latter identity uses the [[Killing form#From a lie algebra representation]] $K$. Then $K\left(C_{2}\right)=\operatorname{Tr} i d^{\mathrm{ad}}=D^{\mathrm{ad}}=\operatorname{dim} \mathfrak{g}$ is the dimension of the algebra, ^[ Note that $C_{2}$ is the inverse of $K$ and their contraction yields the dimension of the space $\mathfrak{g}$.] and for the l.h.s. $\operatorname{Tr} \mathrm{id}^{R}=D^{R}$ is the dimension of the representation $R$. We thus find the relation
$$
D^{\mathrm{ad}} B^{R}=D^{R} C_{2}^{R} .
$$
Therefore **all the constants $B^{R}$ can be determined in terms of the constants $C_{2}^{R}$.** In particular, for the [[adjoint representation]] it implies the equality of the two constants
$$
B^{\mathrm{ad}}=C_{2}^{\mathrm{ad}} .
$$
Note that there is some arbitrariness in the definition of the [[Killing form]] and the above constants $B^{R}$ and $C_{n}^{R}$ : The common rescaling by factors of $\beta$
$$
K(a, b) \rightarrow \beta K(a, b), \quad B^{R} \rightarrow \beta^{-1} B^{R}, \quad C_{2}^{R} \rightarrow \beta^{-1} C_{2}^{R},
$$
leaves all above relationships intact. This result shows **that there is no universal definition for the $B^{R}$ and $C_{2}^{R}$. However, fixing one of them, fixes all the others.** A common normalisation of the [[Killing form]] is $K(a, b):=\operatorname{Tr} \operatorname{ad}(a) \operatorname{ad}(b)$, the constant for the adjoint then equals $B^{\mathrm{ad}}=C_{2}^{\mathrm{ad}}=1$. However, this may neither be a convenient normalisation nor the typical one used in physics in the case of $\mathfrak{s u}(N)$. We therefore will not fix the normalisation, allowing to easily adjust to one's favourite normalisation.


# totally symmetric invariant polynomials
For most Lie algebras, there are analogous totally symmetric invariant polynomials $C_{n} \in \mathfrak{g}^{\otimes n}$ of higher degree $n$. Which ones of these higher invariants exist depends on the Lie algebra. The quadratic invariant $C_{2}$ exists for every simple Lie algebra. For example, $\mathfrak{s u}(2)$ has only the quadratic invariant $C_{2}$, whereas $\mathfrak{s u}(3)$ also has a cubic invariant $C_{3}$. Also the higher invariants $C_{n}$ have eigenvalues $C_{n}^{R}$ on irreducible representations $R$
$$
R\left(C_{n}\right)=C_{n}^{R} \mathrm{id}^{R},
$$
thus offering a way to characterise irreps $R$ in terms of the values $C_{n}^{R}$.

# And topology
Finally, there is a curious relationship between the invariants of $\mathfrak{g}$ and the topology of the associated (compact, connected, universal covering) Lie group G: In terms of cohomology, the group manifold is equivalent to a product of odd-dimensional spheres
$$
\mathrm{G} \simeq \prod_{k} S^{2 n_{k}-1}
$$
For every independent invariant of degree $n_{k}$ there is a sphere of dimension $2 n_{k}-1$. For example we have
$$
\operatorname{SU}(2) \simeq S^{3}, \quad \operatorname{SU}(3) \simeq S^{3} \times S^{5}
$$
in agreement with their spectra of Casimir invariants.