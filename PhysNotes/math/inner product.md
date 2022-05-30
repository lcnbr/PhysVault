---
alias:
- Hermitian inner product
- Hermitian form
---
Let $V$ be a vector space over the field of complex numbers. (One can generalise the choice of field somewhat.) An [[.md|inner product]] (in the most general, possibly indefinite, sense) on $V$ is a function
$$
\langle-,-\rangle: V \times V \rightarrow \mathbb{C}
$$
that is (1-3) [[sesquilinear form|sesquilinear]] and (4) [[sesquilinear form#^herm|conjugate symmetric]]; that is:
1. $\langle 0, x\rangle=0$ and $\langle x, 0\rangle=0$;
^1
1. $\langle x+y, z\rangle=\langle x, z\rangle+\langle y, z\rangle$ and $\langle x, y+z\rangle=\langle x, y\rangle+\langle x, z\rangle$;
^2
1. $\langle c x, y\rangle=\bar{c}\langle x, y\rangle$ and $\langle x, c y\rangle=c\langle x, y\rangle$;
^3
1. $\langle x, y\rangle=\overline{\langle y, x\rangle}$.^[Here we use the physicist's convention that the inner product is conjugate-linear in the first variable rather than in the second, rather than the mathematician's convention, which is the reverse. Note that we use the same field as values of the inner product as for scalars; the complex conjugation will be irrelevant for some choices of field most notably the reals.]
^4

The axiom list above is rather redundant. First of all, (1) follows from (3) by setting $c=0$; besides that, (1-3) come in pairs, only one of which is needed, since each half follows from the other using (4). It is even possible to derive (3) from (2) by supposing that $V$ is a topological vector space and that the inner product is continuous (which, as we will see, is always true anyway for a [[Hilbert space]]).


# Signature
A [[.md|inner product]] defines a [[quadratic form]], and one can thus define its signature, based on its [[sesquilinear form#Matrix form|matrix representation]] $[H]$:

Since $[[sesquilinear form#Induced properties]]), its eigenvalues are real, and thus $[[signature|H]]. We can identify the [[semi)definiteness]((semi|(semi)definiteness]]definiteness.md) of the form from the [[(semi]]definiteness.md#From%20signature%7Csignature)

