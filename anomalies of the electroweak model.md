---
alias:
tags:
- qftII
---
The electroweak theory involves chiral couplings of a gauge field to fermions. This interaction is a potentially dangerous since it can lead to gauge [[anomalies]]. However, the charges of the spinors are arranged in a particular pattern that avoids the anomalies.

![[fermions and masses#^a5b73b]]
![[fermions and masses#^42a589]]

Let us briefly discuss these consistency conditions.
Chiral anomalies in four dimensions can arise only for chiral couplings to spinors, i.e. for the electroweak groups $\mathrm{SU}(2)$ and $\mathrm{U}(1)$. The anomaly originates from a triangle diagram
![[Pasted image 20220126174120.png|200]]
which is proportional to some symmetric structure $d^{a b c}$ of the three involved gauge fields. However, there is no anomaly for $\mathrm{SU}(2)$ alone because there are no symmetric structure constants $d^{a b c}$ in this group. The symmetric structure $d^{a b c}$ trivially exists only for the abelian group $U(1)$. Moreover, there are anomalies for combined groups. Here, one of the indices of $d^{a b c}$ belongs to $U(1)$, the other two to the symmetric invariant form $k^{b c}$ of $\mathrm{SU}(2)$. These mixed anomalies can arise for $U(1) \times S U(2)$ and for $U(1) \times S U(3)$. Finally, there a mixed anomaly between $U(1)$ and gravity. If any of these anomalies is realised, one of the involved gauge symmetries would be badly broken in the quantum theory.
# U(1)
Consider first the pure $U(1)$ anomaly. We have to sum over all spinors propagating in the loop. At each coupling a factor of the hypercharge is inserted. Hence the overall contribution to the anomaly is proportional to
$$
A_{\mathrm{U}(1)} \sim \operatorname{Tr}_{\mathrm{L}} Y^{3}-\operatorname{Tr}_{\mathrm{R}} Y^{3} .
$$
This combination surprisingly equals zero
$$2 \cdot 1(-1 / 2)^{3}+2 \cdot 3(+1 / 6)^{3}-(0)^{3}-(-1)^{3}-3(+2 / 3)^{3}-3(-1 / 3)^{3}=0 .$$

# U(1) x SU(2)
The next anomaly mixes $\mathrm{U}(1)$ and $\mathrm{SU}(2)$. Only the left-handed lepton and quark doublets couple to $\mathrm{SU}(2)$, and they couple with the same strength. The third coupling is the hypercharge, hence the anomaly is proportional to
$$
A_{\mathrm{U}(1) \times \mathrm{SU}(2)} \sim \operatorname{Tr}_{\mathrm{L}} Y
$$

Here we find zero
$$
(-1 / 2)+3(+1 / 6)=0
$$

# U(1) x SU(3)
There is a mixed anomaly of $U(1)$ and the $S U(3)$ of quantum chromodynamics. This one involves only the quarks. Since the quarks all transform in the same [[defining representation of su(n)|fundamental representation]], we only need to sum over the hypercharges
$$
A_{\mathrm{U}(1) \times \mathrm{SU}(3)} \sim \operatorname{Tr}_{\mathrm{Q}, \mathrm{L}} Y-\operatorname{Tr}_{\mathrm{Q}, \mathrm{R}} Y
$$
Again, this combination equals zero
$$
2(+1 / 6)-(+2 / 3)-(-1 / 3)=0 .
$$

# mixed gravity
Finally, there is a potential mixed gravitational anomaly. Gravity is not part of the electroweak theory or the standard model, so we need not pay attention to this anomaly. Nevertheless, let us investigate it. Gravity couples to all particles with equal strength, so here we find
$$
A_{\mathrm{U}(1) \times \text { gravity }} \sim \operatorname{Tr}_{\mathrm{L}} Y-\operatorname{Tr}_{\mathrm{R}} Y
$$
This equals
$$
2(-1 / 2)+2 \cdot 3(-1 / 2)-(0)-(-1)-3(+2 / 3)-3(-1 / 3)=0 
$$
It is interesting to observe that there is no gravitational anomaly. Hence, the electroweak theory can be consistently coupled to nontrivial gravitational backgrounds or even to quantum gravity (as far as that makes sense on its own).

The anomaly cancellations are rather curious. They could be interpreted in several ways:
- The structure of the standard model is actually constrained much more than it may seem at first sight. In particular, the fact that there are three colours for the strong nuclear interactions does play a significant role. ${ }^{12}$
- The standard model may be embedded into some theory with a larger symmetry group at higher energies, a so-called grand unified theory, where the anomaly cancellations are more evident.

