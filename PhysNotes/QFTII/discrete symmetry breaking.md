

We have discussed various kinds of interacting scalar field theories. The Lagrangian had the basic form
$$
\mathcal{L}=-\frac{1}{2}(\partial \phi)^{2}-\frac{1}{2} m^{2} \phi^{2}-\frac{1}{24} \lambda \phi^{4} \implies U(\phi)= \frac{1}{2} m^{2} \phi^{2}+\frac{1}{24} \lambda \phi^{4}
$$
We have dropped a potential cubic term in order to have a minimal amount of symmetry, namely the **global discrete $\mathbb{Z}_{2}$ symmetry $\phi \rightarrow$ $-\phi$.**

So far we have always assumed the mass squared $m^{2}$ to be either zero or positive in order to have a physical interpretation for the field excitations. **However, it is perfectly permissible to assume a negative value for $m^{2}$**. The point is that the potential is dominated by the quartic interaction $\phi^{4}$ for large $\phi$. Consequently, it is bounded from below (for positive $\lambda$ ) irrespectively of the magnitude or sign of the mass term. The [[../AnalyticalMech/Lagrangian|potential]] has one of the following shapes

![[Pasted image 20220126143541.png|500]]

Let us therefore consider the case of negative $m^{2}$ expressed as a positive $\mu^{2}=-m^{2}$
$$
\mathcal{L}=-\frac{1}{2}(\partial \phi)^{2}+\frac{1}{2} \mu^{2} \phi^{2}-\frac{1}{24} \lambda \phi^{4} \implies U(\phi)= -\frac{1}{2} \mu^{2} \phi^{2}+\frac{1}{24} \lambda \phi^{4}= \frac{1}{24} \lambda ( \phi^2-v^2)^2- \frac{3}{2} \frac{\mu^4}{\lambda}
$$
Evidently, the expansion of the field around a classical value $\phi=0$ leads to undesirable [[tachyon|tachyonic]] excitations. In other words, $\phi=0$ is a stationary point of the potential; it is however not a local minimum, but rather a local maximum.

Since the potential is bounded from below, there must be a minimum somewhere around which we can quantise the model. In fact, there are two local minima at
$$
\phi=\pm v, \quad v=\sqrt{6 \mu^{2} / \lambda}
$$

^b869b7

They are symmetric because of the invariance under the global reflection symmetry.
The constant field $\phi(x)=\pm v$ is a solution to the equation of motion. We can therefore expand the field $\phi$ around this solution
$$
\phi(x)=\pm v+\eta(x),
$$
where $\eta$ serves as the quantum field. The expectation value of the quantum field in the vacuum is defined to be zero, hence $v$ is the vacuum expectation value of $\phi(x)$
$$
\langle\phi(x)\rangle=\pm v .
$$
We obtain a new Lagrangian in the new field $\eta$
$$
\mathcal{L}=-\frac{1}{2}(\partial \eta)^{2}+ \frac{3}{2} \frac{\mu^4}{\lambda}-\mu^{2} \eta^{2} \mp \frac{\lambda v }{6} \eta^{3}-\frac{1}{24} \lambda \eta^{4} .
$$
This is again a Lagrangian in the same class of scalar field theories. Let us discuss the terms that arise:

- The derivative term and the quartic interactions have not changed.
- The constant term does not actually play a role, we can disregard it.
- The term linear in $\eta$ receives two contributions which cancel exactly. This is the condition of the minimum.
- We obtain a regular mass term with mass $m=\sqrt{2} \mu$.
- There is a new cubic term with coefficient fixed by the quartic coupling and mass term.

The cubic term evidently violates the $\mathbb{Z}_{2}$ symmetry $\eta \rightarrow-\eta$, but altogether the original symmetry is still present in the somewhat obscure form
$$
\eta \rightarrow \mp 2 v-\eta .
$$
**This symmetry survives quantisation, but it is not compatible with the vacuum expectation value of the fields. The symmetry is said to be spontaneously broken.** ^8e43ca

The model has two possible ground state configurations $\phi=\pm v$, both are global minima of the potential. Which one should we choose as the ground state? There is no criterion to prefer one state over the other. This is the generic situation for spontaneous symmetry breaking: Since symmetry does not leave the ground state invariant, it must map it to some other state. This state has equivalent properties and therefore is also a ground state. **Hence, spontaneous symmetry breaking implies degeneracy of the ground state.** Which one of the two we choose makes no difference since all physics is the same for both states. ^[One could also consider linear combinations of ground states. In our situation, however, the mixing is strongly discouraged because transitions between the ground states have infinite energy. ] We can thus set $\phi(x)=+v+\eta(x)$ without prejudice.^[Fixing one of the ground states may appear paradoxical in the path integral framework: It sums over all field configurations which appears to include all ground states, so how can we specialise to one? In fact we should specify some boundary conditions for the fields. The vacuum expectation value is thus implemented as the field value in asymptotic regions of spacetime.
]