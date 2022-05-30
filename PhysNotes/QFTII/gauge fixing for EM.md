---
alias:
- gauge-fixing delta functional
- gauge-fixing functional
- delta functional
- gauge-fixing delta functional for EM
- gauge-fixing functional for EM
- delta functional for EM
tags:
- qftII
---
---
# [[gauge fixing action for EM|Gauge fixing]] functional
Ideally, we should count each physical configuration only once. To this end we introduce a gauge-fixing condition $G[[x|A]]= 0$ where $G$ is some functional that is assumed to vanish for exactly one point in each gauge orbit. For example, we could use the functional map $G[[x|A]]=\partial^{\mu} A_{\mu}(x)$ which enforces the Lorenz gauge. ^[This condition almost fixes the gauge up to some residual gauge transformations. This particular deviation from the assumptions turns out to be okay.] In fact, we will use a slightly more general gauge condition ^[Other gauges are acceptable as well, but the following discussion may have to be adapted.] 


$$
G[[x|A, \Omega]]=\partial^{\mu} A_{\mu}(x)-\Omega(x) .
$$

^946f67

where $\Omega(x)$ is some function that defines the gauge. This generalisation is useful since we have already seen in QFT I that $\partial^{\mu} A_{\mu}$ does not identically vanish in the quantum theory.

# Delta functional
We would like to restrict the path integral by inserting a delta functional $\Delta$

$$
\int \mathrm{D} A \Delta[G[A, \Omega]] \exp \left(i S_{\mathrm{EM}}[A, J]\right) \text {. }
$$

^20dd2a


However, this insertion has the undesirable feature that it is not evidently related to the original [[graph generating functional|formulation]] of $Z[[../math/delta function#Composition with a function]] $\delta(f(x))=\delta\left(x-x_{0}\right) /\left|f^{\prime}\left(x_{0}\right)\right|$ where $f\left(x_{0}\right)=0$.]
Instead, we use the assumption that the functional $G\left[A^{\prime}, \Omega\right]$ vanishes precisely at one point of the gauge orbit, where $A^{\prime}$ is the gauge potential $A$ transformed by the field $\alpha$
$$
A_{\mu}^{\prime}=A_{\mu}+\left(\partial_{\mu} \alpha\right) .
$$
This implies the delta-functional identity^[The functional determinant Det is approximated by an ordinary determinant when the coordinates $x$ and $y$ are discretised.]
$$
1=\int \operatorname{D} \alpha \Delta\left[[\frac{\delta G\left[A^{\prime}, \Omega\right](x|G\left[A^{\prime}, \Omega\right]]}{\delta \alpha(y)}\right) \text {, }
$$
where the 1 on the l.h.s. represents the number of solutions of $G\left[A^{\prime}, \Omega\right]= 0$ over a gauge orbit.

A convenient feature of the above gauge-fixing functional map $G$ is that its functional derivative in the determinant is independent of $A, \Omega$ and $\alpha$. It simply reads
$$
\frac{\delta G\left[[x|A^{\prime}, \Omega\right]]}{\delta \alpha(y)}=\partial^{2} \delta(x-y) \text {. }
$$
Hence we can write the identity as
$$
1=\operatorname{Det}\left(\partial^{2}\right) \int \operatorname{D} \alpha \Delta\left[G\left[A^{\prime}, \Omega\right]\right] .
$$
The trick used by Faddeev and Popov is to insert the identity into the [[path integral for EM]]
$$
Z[J]=\operatorname{Det}\left(\partial^{2}\right) \int \operatorname{D} \alpha \mathrm{D} A \Delta\left[G\left[A^{\prime}, \Omega\right]\right] \exp \left(i S_{\mathrm{EM}}[A, J]\right) .
$$
We now perform a reparametrisation of the integration variable $A$ to transform $A^{\prime}$ to $A$. This reparametrisation is both a shift and a gauge transformation, hence $\mathrm{D} A$ and $S_{\mathrm{EM}}[A, J]$ remain unchanged

$$
Z[J]=\operatorname{Det}\left(\partial^{2}\right)\left(\int \mathrm{D} \alpha\right) \int \mathrm{D} A \Delta[G[A, \Omega]] \exp \left(i S_{\mathrm{EM}}[A, J]\right)
$$



**We have now separated the path integral over the gauge-fixed potential $A$ from a divergent prefactor which does not depend on $A$.**



