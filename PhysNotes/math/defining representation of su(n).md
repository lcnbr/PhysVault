---
alias:
- defining representation
- fundamental representation
- conjugate defining representation
- conjugate representation


tags:
- qftII
---

Since the [[special unitary group|Lie group]] $\operatorname{SU}(N)$ and [[su(n)|algebra]] $\mathfrak{s u}(N)$ are both formulated in terms of matrices, we know that
$$
\mathfrak{s u}(N), \operatorname{SU}(N) \subset \operatorname{End}\left(\mathbb{C}^{N}\right)
$$
Therefore it is straight-forward to construct an $N$-dimensional representation, the so-called *defining or fundamental representation* ^[The notion of fundamental representation may include more than just the defining representation(s).
] (with $\left.v \in \mathbb{C}^{N}\right)^{17}$
$$
\operatorname{def}(A) v=A v, \quad \operatorname{def}(U) v=U v, \quad D^{\text {def }}=N
$$
$A\in\mathfrak{s u}(N)$ and $U\in\operatorname{SU}(N)$
# Conjugate rep.
There is in fact another $N$-dimensional [[lie group representation|representation]], the conjugate defining representation ^[ Note that there are some complications related to different number fields of representations in real algebras: For example, the direct sum def $\oplus \overline{\text { def }}$ of a complex representation def and its complex conjugate $\overline{\text { def }}$ can be given a real structure; it thus has real dimension $D^{\text {def } \oplus \overline{\operatorname{def}}}=2 N$. Put differently, the real representation $\operatorname{def} \oplus \overline{\operatorname{def}}$ is decomposable, but only over the complex numbers.]
$$
\overline{\operatorname{def}}(A) v=A^{*} v=-A^{\top} v, \quad \overline{\operatorname{def}}(U) v=U^{*} v, \quad D^{\overline{\operatorname{def}}}=N .
$$
Note: the [[adjoint representation]] is a representation on the $\left(N^{2}-1\right)$-dimensional space $\mathfrak{g}$^[ It is sometimes tempting to confuse the defining with the [[adjoint representation]] since both can be formulated simply in terms of the $N \times N$ matrix $A$. The distinction becomes clearer when viewing the representation space $\mathfrak{g}$ as an $\left(N^{2}-1\right)$-dimensional vector space rather than a subspace of matrices.
]^[The [[adjoint representation]] is real and its real dimension is $D^{\text {ad }}=N^{2}-1$.]
$$
\operatorname{ad}(A) B=[A, B], \quad \operatorname{Ad}(U) B=U B U^{-1}, \quad D^{\mathrm{ad}}=N^{2}-1 .
$$
So we know that the [[su(n)|special unitary algebras]] have at least four (irreducible) representations: [[trivial representation|trivial]], [[adjoint representation|adjoint]], [[defining representation of su(n)|defining]] and [[defining representation of su(n)#Conjugate rep|conjugate defining ]].

These [[lie group representation]] suffice to formulate chromodynamics and the standard model: In Yang-Mills theories, the gauge fields transform in the [[adjoint representation]] and thus belong to the gauge algebra. The matter fields such as the quarks typically transform in the [[defining representation of su(n)|defining representation]]s, and their conjugates in the [[defining representation of su(n)#Conjugate rep|conjugate defining representation]]s. They may also transform in [[trivial representation]]s in which case they do not couple to the corresponding gauge fields.