Assume a scalar $\phi$ of dimension $\Delta$ (c.f. [[conformal transformations#^9a696d]]) and write the [[correlator]]
$$
\left\langle\phi\left(x_{1}\right) \phi\left(x_{2}\right)\right\rangle=F\left(x_{1}, x_{2}\right) .
$$

- The [[correlator]] should be invariant under [[conformal group#^7e1b95|translations]]
$$
F\left(x_{1}, x_{2}\right)=F\left(x_{1}-x_{2}\right)=: F\left(x_{12}\right),
$$
which means it should depend on the difference between the two points $x_{1}$ and $x_{2}$ only. 
- Invariance under [[conformal group#^2426d1|Lorentz rotations]] requires dependence on a Lorentz-scalar
$$
F\left(x_{12}\right)=F\left(x_{12}^{2}\right) .
$$
- Finally, [[conformal transformations#^9a696d|scaling invariance]] demands the following equality
$$
\left\langle\phi\left(x_{1}\right) \phi\left(x_{2}\right)\right\rangle \stackrel{!}{=}\left\langle\phi^{\prime}\left(x_{1}\right) \phi^{\prime}\left(x_{2}\right)\right\rangle=s^{2 \Delta}\left\langle\phi\left(s x_{1}\right) \phi\left(s x_{2}\right)\right\rangle,
$$
hence $F\left(x_{12}^{2}\right)=s^{2 \Delta} F\left(s^{2} x_{12}^{2}\right)$ and

$$
F\left(x_{12}^{2}\right)=\frac{N}{\left(x_{12}^{2}\right)^{\Delta}} .
$$

In summary, there is little freedom left. 
# Logarithmic Correlator. 
Remembering the [[conformal transformations#^25c485|vanishing scaling dimension]] $\Delta=(D-$ 2) $/ 2=0$ of a scalar, we would end up with a constant correlator $F\left(x_{1}, x_{2}\right)=N$. Fortunately this is not the complete truth: let us take the limit $D=2+2 \epsilon, N=N_{2} / \epsilon$ for small $\epsilon$

$$
F\left(x_{1}, x_{2}\right)=\frac{N_{2}}{\epsilon\left(x_{12}^{2}\right)^{\epsilon}} \rightarrow \frac{N_{2}}{\epsilon}-N_{2} \log x_{12}^{2}+\ldots
$$

Dropping the leading (divergent) term which is independent of the separation, the correlator can be logarithmic for $\epsilon=0(\Delta=0)$. Let us now consider the argument in [[light cone coordinates]]

$$
x_{12}^{2}=-x_{12}^{\mathrm{L}} x_{12}^{\mathrm{R}}
$$

and identify

$$
x^{\mathrm{L}}=\exp \left(i \xi^{\mathrm{L}}\right), \quad x^{\mathrm{R}}=\exp \left(i \xi^{\mathrm{R}}\right) .
$$

What is the motivation for this identification? It is a two-dimensional conformal transformation which incorporates the closed-string periodicity condition $\sigma \equiv \sigma+2 \pi$ automatically . Of course, one has to choose appropriate coordinates for boundaries in the new coordinates.

# $\tau$ dependence
So far, almost all conditions on the conformal correlator are taken care of. Only translational invariance is spoiled: the [[Polyakov action#Solutions for the closed string|string coordinates]] are functions of $x^{\mathrm{L} / \mathrm{R}}$ except for the linear dependence on $\tau=-\frac{i}{2} \log \left(x^{\mathrm{L}} x^{\mathrm{R}}\right)$. The solution to this problem is obvious: instead of choosing the field $X$ alone, take $\partial X^{\mu} / \partial x^{\mathrm{L} / \mathrm{R}}$ :

$$
\left\langle 0\left|\partial_{\mathrm{L}} X^{\nu}\left(x_{2}\right) \partial_{\mathrm{L}} X^{\mu}\left(x_{1}\right)\right| 0\right\rangle=\frac{-\frac{1}{2} \kappa^{2} \eta^{\mu \nu}}{\left(x_{2}^{\mathrm{L}}-x_{1}^{\mathrm{L}}\right)^{2}} .
$$

^191134

This is indeed closer to the expected form of a conformal correlator!