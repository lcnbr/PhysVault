 Let us consider a simple quantum field theory for a single massless field $\phi$ with a single dimensionless coupling constant $\lambda$ and a regularisation scale $\mu .{ }^{20}$ For example, the latter can be a momentum cutoff scale or the scale parameter of dimensional regularisation. We shall be interested in $n$-point correlation functions $G_{n}$ in momentum space which depend on the momenta $p_{k}$, as well as $\lambda$ and $\mu$
$$
G_{n}\left(p_{k}, \lambda, \mu\right)
$$
All of the above quantities are considered after regularisation, renormalisation and subsequent removal of the regulator; in particular, they are finite. The regularisation scale $\mu$ is a remainder from the regularisation procedure, and we would like to understand how quantities depend on it.

Suppose we change the renormalisation scale by some amount. Then we should be able to compensate the change of any physical variable by a change of the coupling constant and the normalisation of the $n$ external fields
$$\frac{\partial G_{n}}{\partial \mu}+\frac{\partial \lambda}{\partial \mu} \frac{\partial G_{n}}{\partial \lambda}-\frac{n}{\phi} \frac{\partial \phi}{\partial \mu} G_{n}=0$$
It is called the Callan-Symanzik equation. It completely determines the dependence on the renormalisation scale $\mu$ and thus makes it an relevant parameter since every physical quantity can be computed the dependence on the renormalisation scale $\mu$ and thus makes it an irrelevant parameter since every physical quantity can be computed at arbitrary $\mu$.
The Callan-Symanzik equation has the general form
$$\left(\mu \frac{\partial}{\partial \mu}+\beta(\lambda) \frac{\partial}{\partial \lambda}+n \gamma(\lambda)\right) G_{n}\left(p_{k}, \lambda, \mu\right)=0$$
where we have introduced the conventional functions $\beta(\lambda)$ and $\gamma(\lambda)$
$$
\beta(\lambda)=\mu \frac{\delta \lambda}{\delta \mu}, \quad \gamma(\lambda)=-\frac{\mu}{\phi} \frac{\delta \phi}{\delta \mu} .
$$
These dimensionless functions are universally defined for the QFT model at hand independently of the particular observable one may be interested in. Therefore they cannot depend on the external momenta, and since they are dimensionless they must depend only on $\lambda$ which is the only universal dimensionless parameter of the model.
A useful alternative form of the Callan-Symanzik equation follows by a common rescaling of all the momenta, fields and the renormalisation scale. Such a rescaling is trivial since there are no other scales involved in the calculation
$$
\left(\sum_{k} p_{k} \frac{\partial}{\partial p_{k}}-n d+\mu \frac{\partial}{\partial \mu}\right) G_{n}=0
$$
Here $d$ represents the canonical mass dimension of the field $\phi(p)$. Combining this relationship with the Callan-Symanzik equation yields the equation $\Rightarrow$ cancel scale!
$$
\left(\sum_{k} p_{k} \frac{\partial}{\partial p_{k}}-\beta(\lambda) \frac{\partial}{\partial \lambda}-n(d+\gamma(\lambda))\right) G_{n}=0 .
$$

This form is useful since it tells that changing the scale of all external momenta is equivalent to
- a change of the coupling strength $\lambda$ together with a
- rescaling the external fields according to a deformed mass dimension $d+\gamma(\lambda)$.

This has some crucial physical consequences:
- The **strength of the coupling constant depends on the scale of the external momenta. This effect is called a [[running coupling]], and it is governed by the beta-function $\beta(\lambda)$.**
- The mass dimension of the field $\phi$ effectively departs from its canonical value $d$ to $d+\gamma(\lambda)$ when interactions are turned on. The coefficient $\gamma(\lambda)$ is called the **anomalous dimension** of the field $\phi$. It is governed by renormalisation of the kinetic term, also known as wave function renormalisation.
- The **running of the coupling constant can also be interpreted as an anomalous dimension of the coupling constant.** The coupling constant develops an effective mass dimension once interactions are turned on. This effect is called dimensional transmutation. It follows from the Callan-Symanzik equation which essentially relates the coupling constant to the renormalisation scale, and therefore allows us to remove the coupling constant $\lambda$ in favour of the scale $\mu$.
- The anomalous dimensions of the fields and the coupling constants are directly related to the UV-divergences in QFT: They would never arise in a naive treatment of QFT without regularisation and renormalisation. One could argue that, since anomalous dimensions are indeed physical phenomena, a naive treatment of QFT ends up producing infinities in response to this conflict.