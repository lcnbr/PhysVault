---
alias:
tags:
- qftII
---
# Basis
For non-abelian gauge theories it is convenient to choose some basis $T_{a}$ for the Lie algebra $\mathfrak{g}$. The elements $T_{a}$ are called generators of $\mathfrak{g}$. In quantum physics, the basis is typically chosen to be imaginary
$$
a=i a^{c} T_{c} \in \mathfrak{g}
$$
One the one hand, this choice usually makes the representation of $T_{a}$ hermitian which is convenient because it guarantees real eigenvalues. On the other hand, it introduces several unnecessary factors of i. For instance, a group element $h$ is typically parametrised via the exponential map as
$$
h=\exp \left(i a^{c} T_{c}\right) \in \mathrm{G} .
$$

# [[Lie bracket]] of basis
Now that we have a basis, we can expand the [[Lie bracket|Lie brackets]] in terms of the structure constants $f_{a b}{ }^{c}$
$$
[\![ T_{a}, T_{b} ]\!]=i f_{a b}^{c} T_{c} .
$$

^fe8a1f

**For a real algebra, the structure constants $f_{a b}{ }^{c}$ must be real.**

# Killing form in basis
Furthermore we expand the [[Killing form|invariant bilinear form]] in this basis as

$$
K\left(T_{a}, T_{b}\right)=k_{a b}
$$
For a real, [[compact]], [[simple Lie group|simple]] [[Lie algebras|Lie algebra]], the matrix $k_{a b}$ is [[(semi|positive definite]]definiteness.md). By a suitable choice of (orthonormal) basis $T_{a}$ we can adjust $k_{a b}$ to be the unit matrix $k_{a b}=\delta_{a b}$. It may be convenient to make this assumption, but we shall keep the notation $k_{a b}$ to remain general and introduce $k^{a b}$ as its inverse.

For semi-simple Lie algebras the matrix $k_{a b}$ is [[bilinear form#^nondegenerate|non-degenerate]]. It can be **used to raise and lower indices**. For instance we can uniformise the indices of the structure constants
$$
f_{a b c}:=f_{a b}^{d} k_{d c} .
$$
These structure constants are totally anti-symmetric in all three indices
$$
f_{a b c}=-f_{b a c}=-f_{a c b} .
$$
Anti-symmetry of the former two indices follows by definition. Antisymmetry of the latter indices follows from invariance of $K$
$$
0=K\left([\![ T_{c}, T_{a} ]\!], T_{b}\right)+K\left(T_{a}, [\![ T_{c}, T_{b} ]\!]\right)=i f_{c a b}+i f_{c b a}
$$
Now we can also consider a representation $T_{a}^{R}$ of the basis $T_{a}$, namely
$$
T_{a}^{R}:=R\left(T_{a}\right) .
$$
[[#^fe8a1f|Evidently]] the matrices $T_{a}^{R}$ obey the commutator identity
$$
\left[T_{a}, T_{b}^{R}\right]=i f_{a b}^{c} T_{c}^{R} .
$$

A special case is the [[adjoint representation]]
$$
T_{a}^{\mathrm{ad}} T_{b}=\operatorname{ad}\left(T_{a}\right) T_{b}=[\![ T_{a}, T_{b} ]\!]=i f_{a b}^{c} T_{c} .
$$
Therefore, the [[adjoint representation]] $T_{a}^{\mathrm{ad}}$ is a matrix whose elements are the structure constants
$$
\left(T_{a}^{\mathrm{ad}}\right)_{b}^{c}=i f_{a b}^{c} .
$$
# [[Killing form]] and [[../QFTII/Casimir invariant]] in basis
Let us briefly discuss the expansion of the [[Killing form]] and [[../QFTII/Casimir invariant]] in term of the basis $T_{a}$ of generators. For an [[decomposition of representations|irreducible representation]] $R$ we know that the trace of two representation matrices yields the [[Killing form]]
$$
\operatorname{Tr}\left(T_{a}^{R} T_{b}^{R}\right)=B^{R} k_{a b}
$$
A representation of the quadratic [[../QFTII/Casimir invariant]] $C_{2}$ now takes the form
$$
R\left(C_{2}\right)=k^{a b} T_{a}^{R} T_{b}^{R} .
$$
For the [[adjoint representation]] we can write the above relation in terms of structure constants
$$
-f_{a c}^{d} f_{b d}^{c}=B^{\mathrm{ad}} k_{a b}=C_{2}^{\mathrm{ad}} k_{a b} .
$$
This relationship allows to compute the matrix $k_{a b}$ from the structure constants.
# Scaling
Finally, note that there is some arbitrariness in the definition of the generators $T^{a}$. We can simultaneously rescale all of them as well as the structure constants $f_{a b}^{c}$ by a common factor of $\alpha$
$$
T_{a} \rightarrow \alpha T_{a}, \quad f_{a b}^{c} \rightarrow \alpha f_{a b}^{c} .
$$
This transformation does not change any of the above relations. However, the matrix $k_{a b}$ related to the invariants and its inverse $k^{a b}$ must rescale as
$$
k_{a b} \rightarrow \alpha^{2} \beta k_{a b}, \quad k^{a b} \rightarrow \alpha^{-2} \beta^{-1} k^{a b},
$$
where $\beta$ is the rescaling of $K(a, b) \rightarrow \beta K(a, b)$ discussed earlier. This adds further arbitrariness to the various normalisations.