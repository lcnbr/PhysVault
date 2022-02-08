---
alias:
tags:
- qftII
---
Let us consider a simple QFT model in dimensional regularisation. For example, the Lagrangian of a scalar field with a quartic interaction reads
$$
\mathcal{L}=-\frac{1}{2}(\partial \phi)^{2}-\frac{1}{2} m^{2} \phi^{2}-\frac{1}{24} \lambda \phi^{4}
$$
Consider now the mass dimension. For $D=4, \phi, m, \partial$ all have unit mass dimension and $\lambda$ is a dimensionless quantity. All terms in the Lagrangian have mass dimension 4 so that the action is properly dimensionless.

In [[basic integral#^9eb6e0|dimensional]] regularisation there are two choices to obtain a dimensionless action $S=\int \mathrm{d} x^{D} \mathcal{L}$ :
- We can keep the dimension of all involved quantities fixed. Then we have to multiply the Lagrangian by some overall dimensionful factor
$$
\mathcal{L}=\mu^{-2 \epsilon}\left(-\frac{1}{2}(\partial \phi)^{2}-\frac{1}{2} m^{2} \phi^{2}-\frac{1}{24} \lambda \phi^{4}\right)
$$
Here $\mu$ is some regularisation constant with unit mass dimension. ^3e7665
- The alternative is to adjust the mass dimension of the field $\phi$ to $1-\epsilon$. Then the kinetic terms have the desired mass [[basic integral#^9eb6e0|dimension]] $4-2 \epsilon$. The interaction term, however, has mass dimension $4-$ $4 \epsilon$. We can compensate it either by attributing a mass dimension $2 \epsilon$ to $\lambda$, or by factoring out this mass dimension and keeping $\lambda$ dimensionless
$$
\mathcal{L}=-\frac{1}{2}(\partial \phi)^{2}-\frac{1}{2} m^{2} \phi^{2}-\frac{1}{24} \mu^{2 \epsilon} \lambda \phi^{4} .
$$
Note that both choices are equivalent up to a rescaling of the field $\phi$ by $\mu^{\epsilon}$.

In the first choice, $\mu^{-2 \epsilon}$ is an overall prefactor of the action. It acts like Planck's constant $1 / \hbar$ which we have already observed to count loops in Feynman graphs. A contribution at $L$ loops therefore comes along with a factor of
$$
\lambda^{L} \mu^{2 \epsilon L} .
$$
This is in fact the only place where the new scale can appear. The dependence on $\mu$ therefore is always very mild since its exponent $\epsilon$ is always very small. It is logarithmic rather than polynomial.