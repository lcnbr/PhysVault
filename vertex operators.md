# Vertex Operators

The dictionary between particular string states and vertex operators is provided by the [[state-operator map]]. While it is clear, that each string state should correspond to a particular operator, the operator needs to be parametrized by the momentum and needs to carry information about the mode of the string it shall represent. It turns out that the simplest operator serving the purpose reads

$$
\mathcal{O}[q]=: \exp \left(i q_{\mu} X^{\mu}\right):
$$

This operator is a momentum eigenstate, which receives a phase $\exp \left(i q_{\mu} \epsilon^{\mu}\right)$ for the translation $X \rightarrow X+\epsilon$

$$
\mathcal{O}[q] \mapsto \exp \left(i q_{\mu} \epsilon^{\mu}\right) \mathcal{O}[q] .
$$

## String Vacuum. 
Calculating the OPE with the stress-energy tensor $T$

$$
T(z) \mathcal{O}[q](w, \bar{w})=\frac{\frac{1}{4} \kappa^{2} q^{2} \mathcal{O}[q](w, \bar{w})}{(z-w)^{2}}+\frac{\partial \mathcal{O}[q](w, \bar{w})}{z-w}+\ldots
$$
(Exercise 8.1) singles out a [[primary operator#From OPE]] with [[conformal weight#From operator product expansion OPE|weights]] $\left(\frac{1}{4} \kappa^{2} q^{2}, \frac{1}{4} \kappa^{2} q^{2}\right)$.

As discussed in the last chapter, $X$ itself is not a primary field. However, putting $X$ in the exponent makes an actual difference! The observed weight is non-trivial and non-integer. It is a quantum effect $\sim \kappa^{2}$.

Consider the two-point correlator

$$
\left\langle\mathcal{O}_{1}\left[q_{1}\right] \mathcal{O}_{2}\left[q_{2}\right]\right\rangle \simeq\left|z_{1}-z_{2}\right|^{\kappa^{2}\left(q_{1} \cdot q_{2}\right)}
$$

When actually performing this calculation, the zero mode $X^{\mu}=x^{\mu}+\ldots$ contributes an extra factor which is not obvious at first sight, but required for consistency ^e06534

$$
\int \mathrm{d} x^{D} \exp \left(i q_{1} \cdot x+i q_{2} \cdot x\right) \sim \delta^{D}\left(q_{1}+q_{2}\right) .
$$

Plugging $q_{1}=-q_{2}$ leads to the known form of a [[CFT 2-correlator|two-point function]] of [[primary operator|primary operators]] of [[conformal weight|weight]] $\left(\frac{1}{4} \kappa^{2} q^{2}, \frac{1}{4} \kappa^{2} q^{2}\right)$

$$
\left\langle\mathcal{O}_{1}\left[q_{1}\right] \mathcal{O}_{2}\left[q_{2}\right]\right\rangle \simeq \frac{\delta^{D}\left(q_{1}+q_{2}\right)}{\left|z_{1}-z_{2}\right|^{\kappa^{2} q_{1}^{2}}}
$$

The operator $\mathcal{O}[q](z, \bar{z})$ creates a string state at the [[worldsheet]] location $(z, \bar{z})$. The [[worldsheet]] location is unphysical, hence integrate over all potential insertion points:

$$
V[q]=g_{\mathrm{s}} \int \mathrm{d} z^{2} \mathcal{O}[q](z, \bar{z})
$$

Importantly, one can only integrate weight- $(1,1)$ primary operators: a scaling transformation of the integration variables needs to be compensated by a scaling transformation of the primary operator. Unless the two resulting factors compensate, the integral must be zero or ill-defined.

Correspondingly:

- Mass is determined $M^{2}=-q^{2}=-4 / \kappa^{2} ;$ The state describes the string tachyon!

- Intercept $a=\bar{a}=1$ determined by [[worldsheet]] integration.

# Excited Strings. 
What about excited strings? A level-1 state corresponds to

$$
V^{\mu \nu}[q]=g_{\mathrm{s}} \int \mathrm{d} z^{2} \partial X^{\mu} \bar{\partial} X^{\nu} \mathcal{O}[q] .
$$

- Weight is $\left(1+\frac{1}{4} \kappa^{2} q^{2}, 1+\frac{1}{4} \kappa^{2} q^{2}\right)=(1,1)$ for massless $q$.

- Primary condition removes unphysical polarisations, e.g.

$$
T(z) \partial X^{\mu}(w) \mathcal{O}[q](w, \bar{w}) \sim \frac{q^{\mu} \mathcal{O}[q]}{(z-w)^{3}}+\ldots
$$

- Gauge d.o.f. are total derivatives

$$
q_{\nu} V^{\mu \nu}[q]=-i g_{\mathrm{s}} \int \mathrm{d} z^{2} \bar{\partial}\left(\partial X^{\mu} \mathcal{O}[q]\right)=0
$$

We obtain the following vertex operator picture:

- CFT vacuum is empty [[worldsheet]] (genus 0 , no punctures).

- $\int \mathrm{d} z^{2} \mathcal{O}[q](z, \bar{z})$ is string vacuum $|0 ; q\rangle$ (add puncture).

- $\int \mathrm{d} z^{2} \ldots \mathcal{O}[q](z, \bar{z})$ are excited string states.

- Insertions of $\partial^{n} X^{\mu}$ correspond to string oscillators $\alpha_{n}^{\mu}$; insertions of $\bar{\partial}^{n} X^{\mu}$ correspond to $\bar{\alpha}_{n}^{\mu}$.
![](https://cdn.mathpix.com/cropped/2022_01_21_c033a2aa489843817853g-3.jpg?height=166&width=424&top_left_y=608&top_left_x=404)