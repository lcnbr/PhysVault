---
alias:
- covariant vector
- covariant vectors
- covariantly
tag: SR GR physics
---

Since the *components* $V^\mu$ under a specific basis $\{e_\mu\}_\mu=\mathcal{B}$: $V=[[\mu)}$  of [contravariant vectors](contravariant vectors in SR.md|V]] transform covariantly under a [[../String/Lorentz transformation]], we need to compensate such that:
    $$V=[V]^{\mathcal{B}:\mu}[e_\mu]=V^\mu e_{(\mu)}=[V]^{\mathcal{B}':\mu}[e'_\mu]=(V^\nu)'e'_{(\nu)}=\Lambda^\nu{}_\mu V^\mu e'_{(\nu)}$$

Thus we need that $e_{(\mu)}= \Lambda^\nu{}_\mu e'_{(\nu)}$ which when multiplying by the [[../String/Lorentz transformation#Inverse]] $\Lambda_\alpha{}^\mu$ yields:

$$\Lambda_\alpha{}^\mu e_{(\mu)}= e'_{(\alpha)}$$
This gives us our definition for [[.md|covariant vectors]]: as any object whose components transform under a [[../String/Lorentz transformation]] like:

$$U_\mu \rightarrow (U_\mu)'=\Lambda_\mu{}^\nu U_\nu $$

^definingProp

So, the covariant vectors transform with the inverse of a [[../String/Lorentz transformation]] (and with the basis thus *co*-variant). As an example consider the **spacetime derivative** , under a [[../String/Lorentz transformation]], changes as
$$
\pdv{}{ x^{\mu}} \rightarrow \pdv{}{ x^{\prime \mu}}=\pdv{ x^{\rho}}{ x^{\prime \mu}} \pdv{}{ x^{\rho}}=\Lambda_{\mu}{ }^{\rho} \pdv{}{ x^{\rho}}
$$
where we recognized that $\pdv{ x^{\rho}}{ x^{\prime \mu}}=\Lambda_{\mu}{ }^{\rho}$, the inverse of a [[../String/Lorentz transformation]]. Indeed, we have, using the chain rule
$$
\begin{aligned}
\delta_{\nu}^{\mu}&=\pdv{ x^{\prime \mu}}{ x^{\prime \nu}} =  \pdv{ x^{\prime \mu}}{ x^{\rho}} \pdv{ x^{\rho}}{ x^{\prime \nu}}=\Lambda^{\mu}{}_{\rho} \pdv{ x^{\rho}}{ x^{\prime \nu}} \\
\implies  & \Lambda^{\mu}{}_{\rho} \Lambda_{\mu}{}^{\sigma} \pdv{ x^{\rho}}{ x^{\prime \nu}}=\delta_{\nu}^{\mu} \Lambda_{\mu}{}^{\sigma} \\
\implies &\delta_{\rho}^{\sigma} \pdv{ x^{\rho}}{ x^{\prime \nu}} =\Lambda_{\nu}{}^{\sigma} \implies \pdv{ x^{\sigma}}{ x^{\prime \nu}}=\Lambda_{\nu}{}^{\sigma}
\end{aligned}
$$
