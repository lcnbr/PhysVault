The [[Callan-Symanzik equation]] is particularly strong and easiest to interpret for a two-point function $G_{2}$ which depends on a single momentum scale $p$ only. Equivalently we can consider a higher-point function $G$ for a particular momentum configuration which is governed by a single overall momentum scale $p$. The [[Callan-Symanzik equation]] thus reads
$$
\left(p \frac{\partial}{\partial p}-\beta(\lambda) \frac{\partial}{\partial \lambda}-n d-n \gamma(\lambda)\right) G(p, \lambda, \mu)=0 .
$$
Let us introduce the running coupling function $\tilde{\lambda}(z, \lambda)$ with $z=p / \mu$ which is defined by a differential equation and an initial condition
$$
\left(p \frac{\partial}{\partial p}-\beta(\lambda) \frac{\partial}{\partial \lambda}\right) \tilde{\lambda}(p / \mu, \lambda)=0, \quad \tilde{\lambda}(1, \lambda)=\lambda .
$$
Furthermore we make an ansatz depending on the running coupling with appropriate overall scaling
$$
G(p, \lambda, \mu)=p^{n d} \tilde{G}(p / \mu, \tilde{\lambda}(p / \mu, \lambda)) .
$$
It simplifies the [[Callan-Symanzik equation]] as follows
$$
\left(z \frac{\partial}{\partial z}-n \gamma(\lambda(z, \tilde{\lambda}))\right) \tilde{G}(z, \tilde{\lambda})=0,
$$
where $\lambda(z, \tilde{\lambda})$ is the inverse function of $\tilde{\lambda}(z, \lambda)$. This equation is now easy enough to solve as
$$
\tilde{G}(z, \tilde{\lambda})=\exp \left(\int_{1}^{z} \frac{\mathrm{d} z^{\prime}}{z^{\prime}} n \gamma\left(\lambda\left(z^{\prime}, \tilde{\lambda}\right)\right)\right) \tilde{F}(\tilde{\lambda})
$$
with a function $\tilde{F}(\tilde{\lambda})$ to be determined by the dynamics of the QFT.
The running coupling constant $\tilde{\lambda}$ depends on the (relative) momentum scale $p / \mu$. However, since several particles are involved in each interaction, which momentum does $p$ refer to? The momentum dependence can be interpreted in several ways:
- The elementary interaction of QED involves a single photon line. One could argue that $p$ is an (approximate) measure of the virtuality of this photon. For example, consider $W^{\pm}$pair production at a particle collider with intermediate photons. Its virtuality (centre-of-mass energy) in the electroweak regime (100 GeV) determines the effective coupling strength of the electromagnetic field. Here the effective fine structure constant is significantly different than for everyday electromagnetic processes (including production of electron-positron pairs).
In non-abelian gauge theories, the association of energy to a specific particle is not as straight-forward since the cubic gauge vertex makes no distinction between the three contributing gluons.
- More accurately, the above equations hold when all the momenta involved in the process are rescaled by exactly the same amount. Here the equations predict the shift of the coupling due to the scaling factor.
- To understand the precise dependence on all involved momenta, one must calculate the actual loop integrals.