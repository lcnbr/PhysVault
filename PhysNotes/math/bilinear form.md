---
alias:
- bilinear
- nondegenerate
- symmetric bilinear form
- alternating
- anti-symmetric bilinear form
- skew-symmetric

tags:
- qftII
---

Let $V$ be a vector space over a field $\mathbb{K}$.  An [[bilinear form]] (in the most general, possibly indefinite, sense) on $V$ is a function
$$
B: V \times V \rightarrow K
$$
that is (1-3) bilinear:
1. $B( 0, x)=0$ and $B( x, 0)=0$;
^1
1. $B( x+y, z)=B( x, z)+B( y, z)$ and $B( x, y+z)=B( x, y)+B( x, z)$;
^2
1. $B( c x, y)={c}B( x, y)$ and $B( x, c y)=cB( x, y)$;
^3
# Properties
- $B(-,-)$ is **nondegenerate** if $B( v,w) = 0$ for all $w$ implies $v=0$. ^nondegenerate
-    **symmetric** if $B( v, w) = B( w, v)$ for all $v, w$ in $V$, see [[symmetric bilinear form]]; ^symmetric
-   **alternating** if $B( v, v) = 0$ for all $v$ in $V$;  ^alternating
-   **skew-symmetric** or **antisymmetric** if $B( v, w) = −B( w, v)$ for all $v, w$ in $V$; ^antisym
    
Note: Every alternating form is skew-symmetric (expand $B(\mathbf{v}+\mathbf{w}, \mathbf{v}+\mathbf{w})$).
If the characteristic of $K$ is not 2 then the converse is also true: every skew-symmetric form is alternating. If, however, char $(K)=2$ then a skew-symmetric form is the same as a symmetric form and there exist symmetric/skew-symmetric forms that are not alternating.


# Associated matrix

If $V$ is a finite-dimensional vector space, then relative to any basis $\left\{e_{i}\right\}_{i}=\mathcal{B}$ of $V$, a [[bilinear form]] $B$ is represented by a matrix $[B]$,
$$
B(\vec{v},\vec{w})=B(v^ie_{(i)},w^je_{(j)})=v^iw^j B (e_{(i)},e_{(j)})=[B]_{\mathcal{B}\mathcal{B}}[v]^\mathcal{B}[w]^\mathcal{B}=[B]^\mathcal{B}{}_\mathcal{B}[v^\top]_\mathcal{B}[w]^\mathcal{B}=[v^\top][B][w]
$$
The components of $B$ are given by $[B]_{i j}:=B\left(e_{i}, e_{j}\right)$.

A bilinear form has different matrices on different bases. However, the matrices of a bilinear form on different bases are all congruent.

## Induced properties

In general, the associated matrix can be any matrix, any element of $\operatorname{Mat}_{n\times n}$. However if it is:

- [[#^nondegenerate]]  $\iff$ the matrix must have full rank
- [[#^symmetric]] $\iff$ the matrix must be symmetric
- [[#^alternating]] $\iff$ the matrix is skew-symmetric and has only $0$ along the diagonal (implied by skew-symmetry if $\operatorname{Char}(\mathbb{K})\neq2$)
- [[#^antisym]] $\iff$ the matrix is skew-symmetric

