---
Alias:
- D'Alembertian
- D'Alembert operator
tag: GR physics
---

# D'Alambert operator in General Relativity
Consider a scalar $\phi(x)$. Its covariant derivative is
$$
\phi_{; \mu}=\frac{\partial \phi}{\partial x^{\mu}} .
$$
Taking one more covariant derivative we have
$$
\phi_{; \mu ; \nu}=\frac{\partial^{2} \phi}{\partial x^{\mu} \partial x^{\nu}}-\Gamma^{\alpha}{ }_{\mu \nu} \frac{\partial \phi}{\partial x^{\alpha}} .
$$
Multiplying with $g^{\mu \nu}$ yields
$$
g^{\mu \nu} \phi_{; \mu ; \nu}=g^{\mu \nu} \frac{\partial^{2} \phi}{\partial x^{\mu} \partial x^{\nu}}-g^{\mu \nu} \Gamma^{\alpha}{ }_{\mu \nu} \frac{\partial \phi}{\partial x^{\alpha}},
$$

or, using the definition of $\Gamma^{\lambda}$
$$
\square^2 \phi \equiv \phi^{\mu}{ }_{; \mu}=g^{\mu \nu} \frac{\partial^{2} \phi}{\partial x^{\mu} \partial x^{\nu}}-\Gamma^{\alpha} \frac{\partial \phi}{\partial x^{\alpha}}
$$
In the above we recognize a generalization of the D'Alambert operator:

$$
\square^2 \equiv g^{\mu \nu} \frac{\partial^{2}}{\partial x^{\mu} \partial x^{\nu}}-g^{\mu \nu} \Gamma_{\mu \nu}^{\alpha} \frac{\partial}{\partial x^{\alpha}}
$$

^Dal
