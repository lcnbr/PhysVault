
---
alias:
- decomposable
- irreducible
- irreps
tags:
- qftII
---
The direct [[direct sum of representations|sum]] operation can be reversed to [[decomposition of representations|decompose]] representations to their building blocks. There are three cases to be distinguished:
- A representation is [[decomposition of representations|decomposable]] if it can be written as a [[direct sum of representations|direct sum]] of proper sub-representations. $R=R_{1} \oplus R_{2} \quad R_{1,2} \neq \varnothing$ ^decomp
- A representation is [[decomposition of representations|irreducible]] if it has no proper sub-representation. Such a representation is also called irrep for short. An irrep is indecomposable by definition, and it can be considered an elementary building block for representations. ^irrep
- (Un)fortunately, there is a third class of representations which are reducible but indecomposable. These have proper sub-presentations but cannot be written as a direct sum of such. Representations of this type can be written as upper-triangular block-matrices. ^indecomp

Gladly, the third case is not encountered for unitary representations which are most relevant to quantum mechanics, and in particular to Yang-Mills theory. **For our purposes we may assume representations to be either irreducible or fully decomposable (to irreps).**
One practical complication in decompositions is that one first has to identify appropriate subspaces $\mathbb{V}_{1}, \mathbb{V}_{2}$ of $\mathbb{V}$ such that the representation matrices take on a block-diagonal form. Two relevant concepts are conjugation and equivalence: 

A representation $R_{1}$ can be conjugated to a representation $R_{2}$ by applying one and the same similarity transformation $M: \mathbb{V}_{1} \rightarrow \mathbb{V}_{2}$ for all $g \in \mathrm{G}$ or all $a \in \mathfrak{g}$
$$
R_{2}=M R_{1} M^{-1} .
$$
Any two such representations are called equivalent. Classification of representations, particularly irreps, is normally considered modulo equivalence.

The [[adjoint representation]] in $\mathrm{U}(N)$ is decomposable into a [[trivial representation]] and an $\left(N^{2}-1\right)$-dimensional representation. The latter is essentially the [[adjoint representation]] of the subgroup $\operatorname{SU}(N)$. More generally, the [[adjoint representation]] is [[decomposition of representations#^irrep|irreducible]] if the underlying group or algebra is [[simple Lie group|simple]].