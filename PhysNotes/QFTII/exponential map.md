---
alias:
tags:
- qftII
---
# Exponential Map.

Define a smooth map $\exp$ from a neighbourhood of $0$ in $\mathfrak{g}$ to a neighbourhood of $1$ in $\text{G}$
^[[../math/Lie theory|It can be extended to the whole [Lie theory]] $\mathfrak{g}$ and the connected component $\text{G}_0$ of the Lie group $\text{G}$ which includes the identity element $1$.]such that ^[For a map $f$ between two manifolds $f:A\to B$, its derivative $\der f$ at a point $a$ is a linear map between the corresponding tangent spaces $\der f(a):\mathrm{T}_aA\to \mathrm{T}_{f(a)}B$. In this case the derivative $\der\exp$ is defined as the identity map $\id$ on $\mathrm{T}_0\mathfrak{g}=\mathfrak{g}=\mathrm{T}_1\text{G}$.]
$$
\exp(0)=1,
\quad
\dd\exp(0)=\text{id},
\quad
\exp(na)=\exp(a)^n.
$$
This map is called the [[.md|exponential map]]. We can construct the exponential map as the limit
^[This is commonly achieved by transport via a particular vector field.]
$$
\exp(a)=\lim_{n\to\infty} \pqty{1+\frac{a}{n}}^n.
$$
Here $1+a/n$ is understood as an element of the [[../math/Lie group]] in the neighbourhood of $1$ and raising it to some power is achieved by group multiplication. Evidently, the definition makes sense only for sufficiently large $n$, hence the limit.