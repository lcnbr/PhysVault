---
alias:
- sesquilinear
- nondegenerate sesquilinear form
- conjugate symmetric
- alternating sesquilinear form
- anti-symmetric sesquilinear form
- skew-Hermitian sesquilinear form

tags:
- qftII
- LA
---
Let $V$ be a vector space over the field $\mathbb{C}$. (One can generalise the choice of field somewhat.) A [[.md|sesquilinear form]] (in the most general, possibly indefinite, sense) on $V$ is a function
$$
\phi: V \times V \rightarrow \mathbb{C}
$$
that is (1-3) sesquilinear:
1. $\phi( 0, x)=0$ and $\phi( x, 0)=0$;
^1
1. $\phi( x+y, z)=\phi( x, z)+\phi( y, z)$ and $\phi( x, y+z)=\phi( x, y)+\phi( x, z)$;
^2
1. $\phi( c x, y)=\bar{c}\phi( x, y)$ and $\phi( x, c y)=c\phi( x, y)$;
^3


# Properties
- $\phi(-,-)$ is **nondegenerate** if $\phi( v,w) = 0$ for all $w$ implies $v=0$. ^nondegenerate
-    **conjugate symmetric** or **Hermitian** if $\phi( v, w) = \overline{\phi( w, v)}$ for all $v, w$ in $V$ see [[inner product|Hermitian form]]; ^herm
-   **skew-Hermitian** or **antisymmetric** if $\phi( v, w) = −\overline{\phi( w, v)}$ for all $v, w$ in $V$; ^antisym


    
# Matrix form

If $V$ is a finite-dimensional complex vector space, then relative to any basis $\left\{e_{i}\right\}_{i}=\mathcal{B}$ of $V$, a [[.md|sesquilinear form]] $\phi$ is represented by a matrix $[\phi]$,
$$
\phi(\vec{w},\vec{z})=\phi(w^ie_{(i)},z^je_{(j)})=\overline{w^i}z^j \phi (e_{(i)},e_{(j)})=[\phi]_{\mathcal{B}\mathcal{B}}[\bar{w}]^\mathcal{B}[z]^\mathcal{B}=[\phi]^\mathcal{B}{}_\mathcal{B}[\bar{w}^\top]_\mathcal{B}[z]^\mathcal{B}=[\bar{w}^\top][\phi][z]
$$
The components of $\phi$ are given by $[\phi]_{i j}:=\phi\left(e_{i}, e_{j}\right)$.

## Induced properties

In general, the associated matrix can be any matrix, any element of $\operatorname{Mat}_{n\times n}$. However if it is:

- [[#^nondegenerate]]  $\iff$ the matrix must have full rank
- [[#^herm]] $\iff$ the matrix must be Hermitian
- [[#^antisym]] $\iff$ the matrix is skew-symmetric

