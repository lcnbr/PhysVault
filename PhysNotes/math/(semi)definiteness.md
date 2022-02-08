---
alias:
- positive semidefinite
- positive
- definite
- positive definite
- negative definite
- negative semidefinite
- indefinite
- complete
---
Consider an [[inner product space]] $(V;\langle\cdot,\cdot\rangle)$. We define a function $\|-\|^{2}: V \rightarrow \mathbb{C}$ by $\|x\|^{2}=\langle x, x\rangle ;$ in fact, $\|-\|^{2}$ takes only real values, by [[inner product#^4]].
* The [[inner product]] is **positive semidefinite**, or simply **positive**, if $\|x\|^{2} \geq 0$ always. ^possemidef
*  Notice that (by [[inner product#^1]] ), $\|x\|^{2}=0$ if $x=0$; the [[inner product]] is **definite** if the converse holds. ^def
*  An [[inner product]] is **positive definite** if it is both [[(semi)definiteness#^possemidef|positive]] and [[(semi)definiteness#^def|definite]]. ^posdef
*  As an aside, there are also **negative (semi)definite** inner products, which are slightly less convenient but not really different. An [[inner product]] is **indefinite** if some $\|x\|^{2}$ are positive and some are negative; these have a very different flavour. ^indef
* The [[inner product]] is **complete** if, given any infinite sequence $\left(v_{1}, v_{2}, \ldots\right)$ such that
$$
\lim _{m, n \rightarrow \infty}\left\|\sum_{i=m}^{m+n} v_{i}\right\|^{2}=0
$$
there exists a (necessarily unique) $\operatorname{sum} S$ such that
$$
\lim _{n \rightarrow \infty}\left\|S-\sum_{i=1}^{n} v_{i}\right\|^{2}=0 .
$$
If the [[inner product]] is definite, then this sum, if it exists, must be unique, and we write
$$
S=\sum_{i=1}^{\infty} v_{i}
$$
(with the right-hand side undefined if no such sum exists). ^complete

# From [[signature]]

We can identify the [[(semi)definiteness]] of the form from the [[signature]] of the matrix representation.
If the signature is:

- $(m,n,0)$ the [[bilinear form]] is **[[(semi)definiteness#^possemidef|positive semidefinite]]**^signPosSemi
- $(0,n,0)$ the [[bilinear form]] is **[[(semi)definiteness#^posdef|positive definite]]**^signPosDef
- $(m,0,n)$ the [[bilinear form]] is **[[(semi)definiteness#^indef|negative semidefinite]]**^signNegSemiDef
- $(0,0,n)$ the [[bilinear form]] is **[[(semi)definiteness#^indef|negative definite]]**^signNegDef
- $(0,p,q)$  the [[bilinear form]] is **[[(semi)definiteness#^def|definite]]** or nondegenerate ^signNondeg
