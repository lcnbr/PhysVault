---
alias:
- invariant bilinear form
tags:
- qftII
---
Consider a [[simple Lie group|simple]] (finite-dimensional) [[Lie theory]] $\mathfrak{g}$. Up to rescaling it has a unique invariant [[bilinear form#^symmetric|symmetric]] [[bilinear form]] $K: \mathfrak{g} \times \mathfrak{g} \rightarrow \mathbb{K}$ known as the [[Killing form]] $(\mathbb{K}=\mathbb{R}, \mathbb{C}$ denotes the number field over which the [[Lie algebras|Lie algebra]] $\mathfrak{g}$ is defined). Symmetry and invariance means that for all $a, b, c \in \mathfrak{g}$
$$
K(a, b)=K(b, a), \quad K([\![ c, a ]\!], b)+K(a, [\![ c, b ]\!])=0 .
$$


# From a [[lie algebra representation]]
A form with this property can be constructed easily using some [[lie algebra representation|representation]] $R$
$$
\operatorname{Tr} R(a) R(b)=B^{R} K(a, b) .
$$
Symmetry and invariance follow from cyclicity of the trace. Due to uniqueness of $K$ in a [[simple Lie group|simple]] [[Lie algebras|Lie algebra]], all these forms must be equivalent up to a factor of proportionality $B^{R}$ which depends on the particular representation $R$. Note that it also depends on the normalisation of $K$ as we shall discuss later.