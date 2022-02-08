---
alias:
tags:
- qftII
---
Classification. Finite-dimensional, complex, simple [[Lie groups]] have been classified: There are four infinite families $\mathfrak{a}_{n}, \mathfrak{b}_{n}, \mathfrak{c}_{n}$ and $\mathfrak{d}_{n}$. They are related to the three main classes of matrix algebras

|        type        |  matrix algebra symbol  | matrix group name |
|:------------------:|:-----------------------:|:-----------------:|
| $\mathfrak{a}_{n}$ |  $\mathfrak{s l}(n+1)$  |  special linear   |
| $\mathfrak{b}_{n}$ | $\mathfrak{s o}(2 n+1)$ | orthogonal (odd)  |
| $\mathfrak{c}_{n}$ |  $\mathfrak{s p}(2 n)$  |    symplectic     |
| $\mathfrak{b}_{n}$ |  $\mathfrak{s o}(2 n)$  | orthogonal (even) |

Here, the index of the algebras denotes their rank, a characteristic number for simple [[Lie algebras]].

We define the [[Lie bracket]] as the commutator for matrices, thus the groups need to close under commutation.
The matrix algebras have particular properties which are stable under taking commutators
- The commutator of two $N \times N$ matrices is traceless. Hence, traceless matrices form the [[special linear Lie algebra]] $\mathfrak{s l}(N)$
$$
A \in \mathfrak{s l}(N): \quad \operatorname{Tr} A=0
$$
- Anti-symmetric $N \times N$ matrices w.r.t. an invertible symmetric metric $M$ (e.g. $M=1$ ) close under taking commutators. Therefore they form the [[orthogonal Lie algebra]] $\mathfrak{s o}(N)$
$$
A \in \mathfrak{s o}(N): \quad A^{\top}=-M A M^{-1}, \quad M^{\top}=M
$$
- Anti-symmetric $N \times N$ matrices w.r.t. an invertible anti-symmetric metric $E$ close under taking commutators. They form the [[symplectic Lie algebra]] $\mathfrak{s p}(N)$
$$
A \in \mathfrak{s p}(N): \quad A^{\top}=-E A E^{-1}, \quad E^{\top}=-E .
$$
- Furthermore, there are five exceptional simple [[Lie theory]] $\mathfrak{g}_{2}, \mathfrak{f}_{4}$, $\mathfrak{e}_{6}, \mathfrak{e}_{7}$ and $\mathfrak{e}_{8}$ which are related to octonionic numbers.

Many properties of these simple [[Lie algebras]] can be encoded into so-called Dynkin diagrams. A Dynkin diagram consists of a collection of dots connected by lines of various styles. The number of dots equals the rank of the algebra. The Dynkin diagrams of the simple finite-dimension [[Lie groups]] are as follows:

![[Pasted image 20220126183045.png|330]]
![[Pasted image 20220126183106.png|400]]

In analogy to simple [[Lie algebras]], also the irreducible representations can be classified. Note that for a given [[Lie theory]] there exists a particular set of irreducible representations which a characteristic spectrum of admissible dimensions.

A complex [[Lie theory]] may have several corresponding real forms. For example, the special unitary algebra $\mathfrak{s u}(N)$ is a real form of the complex special linear algebra $\mathfrak{s l}(N, \mathbb{C})=\mathfrak{a}_{N-1} .$