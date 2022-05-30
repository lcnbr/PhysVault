---
alias:
tags:
- qftII
---
Consider the [[equations of motion for quantum fields]], 
the first term in the brackets generates the [[../AnalyticalMech/Euler-Lagrange equations]], the second one is usually removed by setting $J=0$ in the end. 
# In terms of [[graph generating functional]]
In terms of the [[graph generating functional]] this identity is known as the [[.md|Schwinger-Dyson equation]]
$$
\frac{\delta S}{\delta \Psi(x)}\left[-i \frac{\delta}{\delta J}\right] Z[J]=-J(x) Z[J]
$$
For example this implies the [[graph generating functional#time-ordered two-point correlator|expectation value]] of the classical equation of motion to hold
$$
\langle\delta S[\Psi] / \delta \Psi(x)\rangle=Z[J]^{-1}\eval*{\frac{\delta S}{\delta \Psi(x)}\left[-i \frac{\delta}{\delta J}\right] Z[J]}_{J=0}=Z[J]^{-1}\eval*{\pqty{-J(x)Z[J]}}_{J=0}=0
$$
In the presence of some other operator(s) $O[\Psi]$ in the correlator some more care is needed because the functional derivatives in the operator can remove the source $J$ before it is set to zero
$$
\begin{aligned}
\langle O[\Psi] \delta S / \delta \Psi(x)\rangle &=\left.Z[J]^{-1} O\left[-i \frac{\delta}{\delta J}\right] \frac{\delta S}{\delta \Psi(x)}\left[-i \frac{\delta}{\delta J}\right] Z[J]\right|_{J=0} \\
\>D_{e q} &=-\left.Z[J]^{-1} O\left[-i \frac{\delta}{\delta J}\right] J(x) Z[J]\right|_{J=0} \\
&=\left.i Z[J]^{-1} \frac{\delta O}{\delta \Psi(x)}\left[-i \frac{\delta}{\delta J}\right] Z[J]\right|_{J=0} \\
&=i\langle\delta O / \delta \Psi(x)\rangle
\end{aligned}
$$
Here, one of the fields $\Psi \simeq-i \delta / \delta J$ must act on the free $J(x)$, the other fields in $O$ amount to $\delta O / \delta \Psi(x)$ and act on $Z[J]$. This result shows that the equations of motion are satisfied in time-ordered correlators unless there are other fields present at the same point of spacetime.

# In terms of [[connected graph generating functional|connected generating functional]]


For the connected graphs one finds
$$
\frac{\delta S}{\delta \Psi(x)}\left[-i \hbar \frac{\delta}{\delta J}+\frac{\delta W}{\delta J}\right]=-J(x)
$$
Curiously, the generating functional now appears in the argument of the variation of the action.^[This is due  to  $\exp (-b(x)) a( \frac{\partial}{ \partial x}) \exp (b(x))=a\left(\frac{\partial }{ \partial x}+b^{\prime}(x)\right)$] Note that the functional derivative $\delta / \delta J$ in the argument of $\delta S / \delta \Psi$ can act only on the other argument $\delta W / \delta J$. 


# For the [[effective action]]
The Schwinger-Dyson equation for the [[effective action]] takes a rather implicit form
$$
\frac{\delta S}{\delta \Psi(x)}\left[\Psi+i \hbar\left(\frac{\delta^{2} G}{\delta \Psi^{2}}\right)^{-1} \frac{\delta}{\delta \Psi}\right]=\frac{\delta G}{\delta \Psi(x)}
$$
We observe that setting $\hbar=0$ implies that the leading order of the effective action $G$ coincides with the classical action $S$ (up to a constant shift).

# Correlator form
The [[.md|Schwinger-Dyson equation]] is the quantum analogue to the classical [[../AnalyticalMech/Euler-Lagrange equations]]

A convenient form of the Schwinger-Dyson equation uses correlators in the presence of sources $J$ (c.f. [[effective field functional]])
$$
\langle\delta S[\Psi] / \delta \Psi(x)+J(x)\rangle_{J}=0
$$
This is precisely the expectation value of the [[../AnalyticalMech/Euler-Lagrange equations]] in the presence of (arbitrary) sources. 

Commonly, the generating functional $Z[[graph generating functional|J]]. . Alternatively the generating functional can be viewed as the solution to the Schwinger-Dyson differential equation which is formulated in terms of the action $S$.




# In [[Feynman graphical notation]]
It is instructive to see how the Schwinger-Dyson equation acts on Feynman diagrams. To that end we split up the variation of the action into free and interacting parts $\delta S_{0} / \delta \Psi(x)$ and $\delta S_{\text {int }} / \delta \Psi(x)$. The free action grabs one end of a Feynman propagator, and converts it to a delta-function. The other end of the propagator may be attached to a vertex or to an operator in the correlator. The contribution from the first case is cancelled precisely by the interacting part of the action. The contribution from the second case corresponds to varying the operator by the field.
![[Pasted image 20220126092848.png|500]]