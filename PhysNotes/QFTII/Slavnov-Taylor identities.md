---
alias:
- Slavnov-Taylor equation
- Slavnov-Taylor identity

tags:
- qftII
---


# In terms of [[graph generating functional]]
Multiplying the [[Schwinger-Dyson equation#In terms of graph generating functional]] by the field variation from [[Noether's theorem]] we find
$$
\underbrace{\pqty{\frac{\delta \Psi(x)}{\delta \alpha} \frac{\delta S}{\delta \Psi(x)}}}_{\partial_{\mu} N^{\mu}}\left[-i \frac{\delta}{\delta J}\right] Z[J]=-\frac{\delta \Psi(x)}{\delta \alpha}\left[-i \frac{\delta}{\delta J}\right] J(x) Z[J] .
$$
We obtain the [[Slavnov-Taylor identities|Slavnov-Taylor equation]]
$$
\partial_{\mu} N^{\mu}\left[-i \frac{\delta}{\delta J}\right](x) Z[J]=-\frac{\delta \Psi(x)}{\delta \alpha}\left[-i \frac{\delta}{\delta J}\right](J(x) Z[J])
$$
In the integral form the [[Noether's theorem|Noether current]] drops out
$$
\int \mathrm{d} x^{D} \frac{\delta \Psi(x)}{\delta \alpha}\left[-i \frac{\delta}{\delta J}\right](J(x) Z[J])=0
$$
The content of the above statements is clearer when expanding $\frac{\delta \Psi(x)}{\delta \alpha}$ in powers of $J$. Their expansion coefficients are identities between quantum correlation functions. For instance, the leading order of the differential form is the classical conservation law of the expectation value
$$
\langle\partial \cdot N(x)\rangle=0
$$
The term at first order in differential form reads
$$
\left\langle\Psi(y) \partial_{\mu} N^{\mu}(x)\right\rangle=i \delta^{D}(x-y)\langle\delta \Psi(x) / \delta \alpha\rangle .
$$
Here, the current is conserved unless there is another field at coincident location. Note that the extra term equals the symmetry variation of the other field. Therefore, one can view the current divergence $\partial \cdot N(x)$ to be a symmetry generator localised at $x$
After integration over $x$ we find the global field variation
$$
\langle\delta \Psi(y) / \delta \alpha\rangle=0
$$
In words it tells us that the expectation value of the change of $\Psi$ vanishes. This is obvious since the transformed field $\Psi^{\prime}$ is related to $\Psi$ by symmetry.
The same holds at second order
$$
\langle(\delta \Psi(y) / \delta \alpha) \Psi(z)\rangle+\langle\Psi(y)(\delta \Psi(z) / \delta \alpha)\rangle=0
$$
telling that the expectation value of the change of the product $\Psi(y) \Psi(z)$ vanishes.
# As a correlator

We can write  the Slavnov-Taylor equation in terms of a correlator in the presence of sources (c.f. [[effective field functional]])
$$
\left\langle\partial_{\mu} N^{\mu}(x)+(\delta \Psi(x) / \delta \alpha) J(x)\right\rangle_{J}=0
$$
The argument of the correlator is just the classical conservation of the [[Noether's theorem|Noether current]] when sources are included. The pleasant feature of this equation is that additional fields can be introduced into the correlator by means of the sources.

# Example

Example. Consider the interacting complex scalar field with Lagrangian
$$
\mathcal{L}=-\partial^{\mu} \phi^{*} \partial_{\mu} \phi-m^{2} \phi^{*} \phi-\frac{1}{4} \lambda\left(\phi^{*} \phi\right)^{2}
$$
Rotation of the fields by a phase $\delta \phi=i \delta \alpha \phi, \delta \phi^{*}=-i \delta \alpha \phi^{*}$ is a continuous global symmetry. We define the associated [[Noether's theorem|Noether current]] via
$$
i \phi \partial^{2} \phi^{*}-i \phi^{*} \partial^{2} \phi=\partial_{\mu} N^{\mu} \quad \Longrightarrow \quad N^{\mu}=i \phi \partial^{\mu} \phi^{*}-i \phi^{*} \partial^{\mu} \phi
$$
We can now write the above [[Slavnov-Taylor identities#As a correlator|Slavnov-Taylor equation]] 
$$
\left\langle\partial_{\mu} N^{\mu}(x)\right\rangle_{j, j^{*}}=-i\left\langle\phi(x) j(x)-\phi^{*}(x) j^{*}(x)\right\rangle_{j, j^{*}}
$$
Disabling the sources leads to the classical conservation law for the expectation value
$$
\left\langle\partial_{\mu} N^{\mu}(x)\right\rangle=0
$$
However, the conservation law is deformed when additional fields are inserted into the correlator via $\phi=-i \delta / \delta j$
$$
\left\langle\partial_{\mu} N^{\mu}(x) \phi(y)\right\rangle=-\delta^{D}(x-y)\langle\phi(y)\rangle
$$
Integration over $x$ yields the statement that the expectation value of a charged quantity vanishes
$$
\langle\phi(y)\rangle=0
$$
For the insertion of two fields we find
$$
\left\langle\partial_{\mu} N^{\mu}(x) \phi(y) \phi^{*}(z)\right\rangle=\left(\delta^{D}(x-z)-\delta^{D}(x-y)\right)\left\langle\phi(y) \phi^{*}(z)\right\rangle
$$
Note that this identity holds exactly even in the presence of interactions. Here the integration over $x$ yields a trivial statement. In other words, the symmetry permits a non-trivial expectation value of the uncharged correlator $\left\langle\phi(y) \phi^{*}(z)\right\rangle$.