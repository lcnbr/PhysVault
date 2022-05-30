Finite-dimensional irreps of the unitary algebras $\mathfrak{s u}(N)$ have been classified and their tensor products are well understood. Useful tools in this regard are Young diagrams^[Young diagrams are called Young tableaux when filled with particular numbers
] and Dynkin labels. ^[This topic is far beyond the scope of this course, but a very nice topic of group theory and combinatorics, so let us give a flavour.
]
# Young diagrams
Young diagrams are heaps of boxes. They describe certain symmetrisation classes or equivalently representations of the symmetric group $S_{N}$. A single box corresponds to the [[../math/defining representation of su(n|defining representation]].md). The conjugate [[../math/defining representation of su(n|fundamental representation]].md) corresponds to a vertical stack of $N-1$ boxes. The adjoint representation adds a single box to the right of the topmost box. The trivial representation has no box which we denote by a dot. For example, for $N=5$
![[../math/Pasted image 20220126211352.png|500]]
Horizontal stacks of boxes correspond to symmetrisation; vertical stacks correspond to anti-symmetrisation. For example, the above decomposition of the tensor products of two defining representations can be expressed as follows
![[../math/Pasted image 20220126211411.png|200]]
Young diagrams are useful tools to work with representations of $\mathfrak{s u}(N)$. For instance, there are rules for computing the dimension of irreps and rules for the decomposition of tensor products.


# Dynkin labels
Dynkin labels are a convenient rewriting of the shape of Young diagram in terms of a set of non-negative integer numbers $l_{k}$. Suppose $n_{i}(i=1, \ldots, N)$ denotes the number of boxes in the $i$-th row of the Young diagram. Then the corresponding Dynkin labels are defined as
$$
\left[l_{1}, \ldots, l_{N-1}\right] \text { with } l_{k}:=n_{k+1}-n_{k} .
$$
For example, the elementary representations for $\mathfrak{s u}(N)$ are expressed in terms of $N-1$ Dynkin labels as
$$
\begin{aligned}
\text { triv } &=[00 \ldots 00], & \operatorname{def} &=[10 \ldots 00], \\
\mathrm{ad} &=[10 \ldots 01], & \overline{\mathrm{def}} &=[00 \ldots 01] .
\end{aligned}
$$
The Dynkin labels $l_{k}$ are associated to the nodes $k$ of the Dynkin diagram of the underlying algebra $\mathfrak{a}_{N-1}$
$$
\left[l_{1}, l_{2}, \ldots, l_{N-1}\right] \equiv \bigcirc^{l_{1}} \bigcirc_{2}^{l_{2}} \ldots \ldots-\bigcirc
$$
In that sense, the Dynkin labels are a natural means of describing representations in more general algebras.