---
alias:
tags:
- qftII
---
Another main operation to combine representations is the tensor product. The tensor product representation $R_{1 \otimes 2}$ of an element $h \in \mathrm{G}$ of the group on the space $\mathbb{V}_{1 \otimes 2}=\mathbb{V}_{1} \otimes \mathbb{V}_{2}$ is defined as
$$
R_{1 \otimes 2}(h)=R_{1}(h) \otimes R_{2}(h),
$$
The definition for a [[Lie algebras|Lie algebra]] element $a \in \mathfrak{g}$ is slightly different
$$
R_{1 \otimes 2}(a)=R_{1}(a) \otimes \operatorname{id}+\operatorname{id} \otimes R_{2}(a) .
$$
Evidently, both definitions of $R_{1 \otimes 2}$ satisfy the axioms of representations provided that $R_{1}, R_{2}$ are proper representations.

Tensor products of two or more identical representations $R$ are special since their tensor product naturally decomposes into certain symmetric components. For example, for the tensor product $\mathbb{V} \otimes \mathbb{V}$ of two identical spaces $\mathbb{V}$ we can define a permutation operator $P \in$ $\operatorname{End}(\mathbb{V} \otimes \mathbb{V})$
$$
P\left(v_{1} \otimes v_{2}\right):=v_{2} \otimes v_{1} .
$$
It can be used to construct two projectors $P^{\pm}$onto the symmetric and anti-symmetric subspaces $\mathbb{V}^{\pm}$of $\mathbb{V} \otimes \mathbb{V}$
$$
P^{\pm}=\frac{1}{2}\left(\text { id } \pm P\right).
$$
where id is the identity acting on $\mathbb{V} \otimes \mathbb{V}$. Now the definitions of the tensor product representation $R^{\otimes 2}$ commute with the permutation operator $P$, and hence also with the projectors $P^{\pm}$. Therefore it will act as a [[direct sum of representations]] $R^{\pm}$on the subspaces $\mathbb{V}^{\pm}$
$$
R^{\otimes 2}=R^{+} \oplus R^{-}, \quad R^{\pm}=P^{\pm} R^{\otimes 2} .
$$
For more than two identical representations, tensor products will split into several components with particular permutation symmetries determined by representations of the discrete permutation group.