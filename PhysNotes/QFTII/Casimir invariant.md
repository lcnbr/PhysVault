---
alias:
tags:
- qftII
---
The [[../math/Killing form]] of a [[../math/semi-simple Lie group|semi-simple]] [[../math/Lie algebras|Lie algebra]] is invertible. Therefore there is a corresponding invariant element $C_{2} \in \mathfrak{g} \otimes \mathfrak{g}$ called the Casimir invariant. Thought of as a matrix, $C_{2}$ is the inverse of the [[../math/Killing form]] $K \in \mathfrak{g}^{*} \otimes \mathfrak{g}^{*}$. It obeys the invariance property for all $a \in \mathfrak{g}$
$$
(\operatorname{ad}(a) \otimes \mathrm{id}+\mathrm{id} \otimes \operatorname{ad}(a)) C_{2}=0 .
$$
For example, for $\mathfrak{g}=\mathfrak{s u}(2)$ the Casimir invariant $C_{2}$ serves as the squared angular momentum operator. $\quad{J}^{2}$

The invariance property is particularly relevant for representations of $C_{2} \in \mathfrak{g} \otimes \mathfrak{g}$ which one typically defines as ^[The symbol $\dot{\otimes}$ here means that the a representations $R$ is applied to each tensor factor of $C_{2}$ and the resulting two matrices are joined by matrix multiplication. The meaning of this abstract definition may become clearer later when it is expanded in a basis of $\mathfrak{g}$.]
$$
R\left(C_{2}\right):=(R \dot{\otimes} R) C_{2}
$$
The above invariance condition then reads for all $a \in \mathfrak{g}$
$$
\left[R(a), R\left(C_{2}\right)\right]=0 .
$$
By a version of Schur's lemma for [[../math/Lie algebras]], this implies that **an irreducible representation of $C_{2}$ is necessarily proportional to the identity operator**
$$
R\left(C_{2}\right)=C_{2}^{R} \mathrm{id}^{R} .
$$
The eigenvalue $C_{2}^{R}$ is a characteristic quantity of the irreducible representation $R .$ For example, the constant $C_{2}^{j}$ for a spin- $j$ representation of $\mathfrak{s u}(2)$ evidently is proportional to $j(j+1)$.