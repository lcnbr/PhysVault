---
alias:
tags:
- qftII
---
Yang-Mills theory is often explained in terms of $N\times N$ unitarity matrices. The latter form a Lie group. Let us therefore discuss [[Lie group]]s, [[Lie algebras]] and their relationship.
# Definition
The definition is given in : [[Lie group#Definition]]

## Example
The set of unitary matrices evidently defines a (compact) smooth manifold, and it is a group with a smooth composition rule.


## Properties
Lie groups can be distinguished by several useful properties:
- They can be [[simple Lie group|simple]], [[semi-simple Lie group|semi-simple]] or composite.
- They can be real or complex (as a manifold).
- They can be compact or non-compact (as a manifold).
- They can be [[simply connected]], [[connected topological space|connected]] or disconnected (as a manifold).
- They can be finite or infinite-dimensional (as a manifold).

# Composition

[[simple Lie group|Simple Lie group]]s serve as fundamental building blocks for more general Lie groups:

- [[semi-simple Lie group]]
- Composite Lie groups are direct or non-direct products of simple or abelian Lie groups.

#
Consider four groups of matrices which take one of the following block forms:

$$
\begin{array}{c@{\qquad}c@{\qquad}c@{\qquad}c}
\begin{pmatrix}{\Huge\ast\vphantom{$_{a}^{a}$}}\end{pmatrix}
&
\begin{pmatrix}\ast&0\\0&\ast\end{pmatrix}
&
\begin{pmatrix}\ast&\star\\0&1\end{pmatrix}
&
\begin{pmatrix}1&\star\\0&1\end{pmatrix}
\\[2.5ex]
\text{simple}
& \text{semi-simple}
& \text{composite}
& \text{abelian}
\\[0.5ex]
\text{SU}(4)
& \text{SU}(2)\times\text{SU}(2)
& \text{Poincaré}
& \text{translations}
\end{array}
$$

Suppose $\ast$ denotes (sub)matrices which from a [[simple Lie group]] and $\star$ denotes general matrices.



- The first group, e.g. $\text{SU}(4)$, is simple by definition (c.f. [[special unitary group]].
- The second, e.g. $\text{SU}(2)\times\text{SU}(2)$, is a [[direct product]] of [[simple Lie group|simple groups]], hence it is [[semi-simple Lie group|semi-simple]]. It is not [[simple Lie group|simple]] because it has [[normal sub-group]]s.
- The third group is not a direct product, hence it is not semi-simple. Furthermore it is not simple because it contains normal subgroups: One of them is composed from matrices where the upper-left submatrix $\ast$ is replaced by the unit matrix (fourth group). An example for groups of this form is the [[../String/Poincare invariance|Poincaré group]]. It can be written as $5\times 5$ matrices whose upper-left $4\times 4$ submatrix $\ast$ belongs to the [[Lorentz group]] and the upper-right $4\times 1$ submatrix $\star$ is a translation vector. The subgroup of translations is normal.


In Yang-Mills theory we will encounter mostly direct products of compact, finite-dimensional, simple or abelian, real Lie groups. Furthermore, most of the results presented below will apply only to particular types of Lie groups, in most cases at least to finite-dimensional, simple Lie groups.








