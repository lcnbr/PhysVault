---
alias:
- 1PI generating function
tags:
- qftII
---
We have seen that the [[tree graph generating functional|tree functional]] $T[J]$
is the classical limit of the [[connected graph generating functional|connected functional]] [$W$](connected%20graph%20generating%20functional.md).
Furthermore, $T[J]$ is the [[Legendre transform]] of the [[action as a generating functional]] $S[\Psi]$.
It therefore makes sense to consider also the [[Legendre transform]]
of [$W$](connected%20graph%20generating%20functional.md). This functional is called the effective action $G[\Psi]$.
^[It is also denoted by $\Gamma$. Its argument sometimes takes a
different symbol to clearly distinguish it from the quantum field $\Psi$. However, there is no danger of confusion, and we shall use the same symbol.]
# Definition
We use the [[effective field functional]] to define the effective action is then defined as

$$
G[\Psi]:=W[J[\Psi]]-\int \dd[D]{x} J[\Psi](x)  \, \Psi(x).
$$

It turns out to generate
amputated one-particle irreducible (1PI) Feynman graphs.
These are precisely the graphs where cutting a single
line will never split the graph into two components.

At least two cuts are required to split any graph.
Moreover, the external fields $\Psi$ are directly connected
to the vertices of the graph without Feynman propagators.



How can this be seen? We know that the Legendre transformation
switches between [[action as a generating functional|vertices]] ($S[\Psi]$)
and [[tree graph generating functional|connected tree graphs made from these vertices]] ($T[J]$).
Here the starting point is
the [[connected graph generating functional|generating functional of connected graphs]] [$W$](connected%20graph%20generating%20functional.md) with loops.
**We view the connected graphs as trees made from some effective vertices**.

**How to describe these effective vertices?**
A defining property of trees is that cutting any line splits
a tree into two trees.
Therefore we iteratively split a graph in [$W$](connected%20graph%20generating%20functional.md) into subgraphs by cutting lines
such that each cut splits the graph into two components.
At the end of the procedure the graph is decomposed into
*effective vertices*.
^[Clearly, this procedure is finite and leads to a unique decomposition of the graph.]
These effective vertices have the
property that cutting any single line does not split the vertex.
Hence $G[\Psi]$ encodes precisely the 1PI graphs.
^[This is is qualitative argument. For a quantitative argument one would need to show that the correct prefactors of the graphs are produced. This turns out to work nicely if the prefactors are given by the natural symmetry factors.]



The effective vertices in $G[\Psi]$ certainly
contain the elementary vertices in the original action $S[\Psi]$.
This is evident since $T[J]$ is the classical limit of [$W$](connected%20graph%20generating%20functional.md),
consequently **$S[\Psi]$ must be the classical limit of $G[\Psi]$**.
The higher contributions are amputated loop graphs:

![|400](file:///C:/Users/Lucien/Documents/UNI/images/image156.png)
![|400](file:///C:/Users/Lucien/Documents/UNI/images/image155.png)


This generating functional comprises a small subset of all graphs.
Any connected graph can easily be reassembled as a tree graph
consisting of the vertices encoded by the effective action
![|400](file:///C:/Users/Lucien/Documents/UNI/images/image158.png)


We assume that the effective vertices labelled $\iunit G$
have at least three legs.
The *effective propagator* marked by $\ast$
represents a linear sequence
of effective two-point vertices $G'_2$
of arbitrary length

![|400](file:///C:/Users/Lucien/Documents/UNI/images/image157.png)

Here, $G'_2=G_2-S_0$ are those effective two-point vertices
which are not already in the kinetic term of the free action $S_0$.
^[The free action defines the Feynman propagator and therefore it never appears as an interaction vertex.]
Summing up the geometric series
shows that the effective propagator marked by $\ast$
is minus the inverse of the two-point effective vertex $G_2$

![|350](file:///C:/Users/Lucien/Documents/UNI/images/image154.png)


Note that the above relationship uses the fact
that the inverse of the Feynman propagator
is minus the free action $S_0$

![|200](file:///C:/Users/Lucien/Documents/UNI/images/image153.png)

The reason for calling $G[\Psi]$ the (quantum) effective action is as follows:

- Quantisation of a classical action $S[\Psi]$ yields the functional $Z[J]=\exp(\iunit W[J])$. We may thus say (define) that quantum physics of the classical model described by $S[\Psi]$ is given by $Z[J]$.
- The corresponding classical functional is the exponential $\exp(\iunit T[J])$ of the [[tree graph generating functional|tree functional]] $T[J]$. We note that the latter is the [[Legendre transform]] of $S[\Psi]$. Therefore we can say that **classical physics is given by exponentiation of the [[Legendre transform]] of $S[\Psi]$.**


Noting further that the [[connected graph generating functional|connected functional]] [$W$](connected%20graph%20generating%20functional.md)
is the [[Legendre transform]] of $G[\Psi]$,
we can thus say that quantum physics $Z[J]$
is equivalently described by:

- properly quantising a classical action $S[J]$ or
- taking classical physics of a hypothetical classical model described by the effective action $G[\Psi]$.
 

The effective action therefore encodes all quantum effects of the model
and lets us treat it as a hypothetical classical model based
on the quantum effective action $G[\Psi]$ as its action.
\footnote{Note that the quantum effective action
is intrinsically non-local and complex due to its loop diagrams,
while the classical action is local and real by construction.
Therefore a hypothetical action $G[\Psi]$ would violate
some of the fundamental requirements for a reasonable physical model.
However, the latter does not need to stop us from performing calculations.}

Importantly, the effective action encodes all loop effects,
and no loops have to be closed to recover the full
generating functional $Z[J]$ from $G[\Psi]$.
The latter property is particularly useful for renormalisation purposes
because finiteness of $G[\Psi]$ is equivalent to finiteness of $Z[J]$.





