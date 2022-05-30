---
alias:
tags:
- qftII
---
The basic integral to consider in dimensional regularisation is
$$
I_{n}(X)=\int \frac{-i \mathrm{~d} \ell^{D}}{(2 \pi)^{D}} \frac{1}{\left(\ell^{2}+X-i \epsilon\right)^{n}} .
$$

^098603

For convenience, we first [[../String/Wick rotation]] the integral
$$
I_{n}(X)=\int \frac{\mathrm{d} \ell_{\mathrm{E}}^{D}}{(2 \pi)^{D}} \frac{1}{\left(\ell_{\mathrm{E}}^{2}+X-i \epsilon\right)^{n}} .
$$
Now the integrand is spherically symmetric, therefore we transform to spherical coordinates
$$
I_{n}(X)=\operatorname{Vol}\left(S^{D-1}\right) \int_{0}^{\infty} \frac{\mathrm{d} \ell_{\mathrm{E}}}{(2 \pi)^{D}} \frac{\ell_{\mathrm{E}}^{D-1}}{\left(\ell_{\mathrm{E}}^{2}+X-i \epsilon\right)^{n}} .
$$
The volume of a $(D-1)$-sphere equals $\operatorname{Vol}\left(S^{D-1}\right)=2 \pi^{D / 2} / \Gamma(D / 2)$. The remaining radial integral after a change of variables $\ell_{\mathrm{E}}^{2}=z$ is a [[../String/Euler Beta function]] in $D$
$$
\frac{1}{2} \int_{0}^{\infty} \frac{\mathrm{d} z}{(2 \pi)^{D}} \frac{z^{D / 2-1}}{(z+X-i \epsilon)^{n}}=\frac{\Gamma(D / 2) \Gamma(n-D / 2)}{2(2 \pi)^{D} \Gamma(n)(X-i \epsilon)^{n-D / 2}} .
$$
Altogether the integral reads
$$
I_{n}(X)=\frac{\Gamma(n-D / 2)}{(4 \pi)^{D / 2} \Gamma(n)} \frac{1}{(X-i \epsilon)^{n-D / 2}} .
$$

^5ee300

The resulting expression has the nice feature that it is defined not only for integer $D$, but also for continuous values of the dimensionality of spacetime. We may thus use the above formula as the **definition of the integral for continuous $D$**. We have seen in QFT I that all integrals arising from Feynman diagrams can be brought into this form. Hence the above formula defines an extrapolation of arbitrary Feynman diagrams to non-integer dimensions.

We observe an important feature: The Gamma-function in the numerator has poles for even integers $D \geq 2 n$. Indeed, the integral has a UV-divergence when $D \geq 2 n$. ${ }^{2}$ However, for non-integer values of $D$, the function is perfectly finite. So indeed we can use a continuous number of spacetime dimensions $D$ as a regulator for the integral. For four-dimensional theories, a convenient choice is to take $D$ slightly below 43 ^f2748b
$$
D=4-2 \epsilon
$$

^9eb6e0

Dimensional regularisation provides a finite result for arbitrary Feynman integrals at arbitrary number of loops (as long as $D$ is not rational). Moreover it does not need to introduce a preferred point or direction which would violate Poincaré symmetry.