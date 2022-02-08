---
alias:
- effective field
tags:
- qftII
---
The effective field functional $\Psi[J]$
is the functional derivative of  [$W$](connected%20graph%20generating%20functional.md)

$$
\Psi[J] = \frac{\delta W}{\delta J}[J],
$$

and denote its inverse by $J[\Psi]$.
The field functional $\Psi[J]$ is related to the quantum field $\Psi$:
It is the vacuum expectation value of a single field $\Psi$
in the presence of a source $J$
^[In the presence of a source means promoting the source field $J$ from an auxiliary quantity to an honest constituent of the classical action. A time-ordered vacuum expectation value in the presence of $J$ thus takes the form $\vev{O}_J := Z[J]^{-1} O[ \iunit\hbar\delta/\delta J] Z[J]$.]

$$
\Psi[J](x)=\expval{\Psi(x)}_J := Z[J]^{-1} \frac{-\iunit\hbar\delta}{\delta J(x)} Z[J]
=\frac{\delta W}{\delta J(x)}[J].
$$