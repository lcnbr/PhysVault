---
alias:
tags:
- qftII
---
A distinguished representation of any [[Lie theory]] $\mathfrak{g}$ is the [[adjoint representation]] on the [[Lie theory]] itself
$$
\mathrm{ad}: \mathfrak{g} \rightarrow \operatorname{End}(\mathfrak{g}), \quad \operatorname{ad}(a) b:=[\![ a, b ]\!] .
$$
The [[Lie bracket#^jacobi|Jacobi identity]] ensures that $\text{ad}$ is a proper representation since it guarantees that for any $a, b \in \mathfrak{g}$
$$
\operatorname{ad}([\![ a, b ]\!])=[\operatorname{ad}(a), \operatorname{ad}(b)] .
$$
This becomes clear once applied to some $c \in \mathfrak{g}$ and using antisymmetry of the [[Lie bracket|Lie brackets]]
$$
\begin{aligned}
\operatorname{ad}([\![ a, b ]\!]) c &=[\![ [\![ a, b ]\!], c ]\!], \\
-\operatorname{ad}(a) \operatorname{ad}(b) c &=-[\![ a, [\![ b, c ]\!] ]\!]=[\![ [\![ b, c ]\!], a ]\!], \\
+\operatorname{ad}(b) \operatorname{ad}(a) c &=+[\![ b, [\![ a, c ]\!] ]\!]=[\![ [\![ c, a ]\!], b ]\!] .
\end{aligned}
$$
**The vector gauge potentials in [[N QED fields|Yang-Mills]] theory always belong to the [[Lie theory]] of the gauge group, and they transform in the adjoint representation.**


The adjoint representation for the Lie group reads^[Here the product $b^{\prime}=h b h^{-1}$ of group and algebra elements can be understood in terms of the group product $h(1+\epsilon b) h^{-1}=\left(1+\epsilon b^{\prime}\right)$ with the middle factor in the neighbourhood of 1 .]
$$
\text { Ad }: G \rightarrow \operatorname{Aut}(\mathfrak{g}), \quad \operatorname{Ad}(h) b:=h b h^{-1}
$$
