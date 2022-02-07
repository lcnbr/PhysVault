---
alias:
 - averaging
 - gauge fixing
tags:
- qftII
---
# Averaging. 
Now we must somehow implement the [[gauge fixing for EM#Delta functional|gauge-fixing delta functional]] in the path integral. One option would be to solve for one component of $A_{\mu}$, e.g. $A_{0}$. Doing so would violate Lorentz invariance. Preserving Lorentz symmetry is one of the aims of the path integral formalism.

An alternative is to employ another trick, and integrate out $\Omega$ with a Gaußian potential
$$
S_{\Omega}[\Omega]=-\frac{1}{2 \xi} \int \mathrm{d} x^{4} \Omega^{2}, \quad \int \mathrm{D} \Omega \exp \left(i S_{\Omega}[\Omega]\right)=\text { const. }
$$

^4fe3a4

Since $Z[J]$ only formally depends on $\Omega$ this merely introduces another constant factor into the original [[gauge fixing for EM#^20dd2a|path integral]]
$$
Z[J] \sim \int \mathrm{D} \Omega \,\mathrm{D} A \,\Delta\left[G\left[A, {\Omega}\right]\right] \exp \left(i S_{\mathrm{EM}}[A, J]+i S_{\Omega}[\Omega]\right) .
$$
We now use the delta-functional (whose argument in linear in $\Omega$ ) to perform the path integral over $\Omega$ by substituting $\Omega=\partial \cdot A$ and obtain
$$
\mathrm{Z}[J] \sim \int \mathrm{D} A \exp \left(iS_{\mathrm{EM}}[A, J]+i S_{\mathrm{gf}}[A]\right)
$$
with an additional contribution to the action
$$
S_{\mathrm{gf}}[A]=-\frac{1}{2 \xi} \int \mathrm{d} x^{4}(\partial \cdot A)^{2} .
$$

^e09c3f

Where we implemented the [[gauge fixing for EM#^946f67|gauge-fixing functional]]