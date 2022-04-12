---
---

So far I've shown that if $\mathscr{L}^{\prime}$ is chosen to be gauge invariant, that has the desirable effect of preserving the gauge invariance of massless electrodynamics, and if we break the gauge invariance just by adding a photon mass term, we obtain a massive vector meson coupled to a conserved current. Now I will tackle the problem of constructing a Lagrangian invariant under the gauge transformation (27.12). The key to the construction is a prescription, called minimal coupling, that will generate extra terms, such that the resulting Lagrangian will automatically be gauge invariant. These terms will not involve the derivatives of $A_{\mu}$, but only $A_{\mu}$ itself. I'll explain at the end where the word "minimal" comes from. The prescription is a machine, but it is not universally applicable. You give me a Lagrangian for matter (or whatever you want to call it) without electromagnetism, and, provided one condition is met, I'll generate the Lagrangian including the interactions with electromagnetism.

The necessary condition is that the matter Lagrangian $\mathscr{L}_{m}\left(\phi, \partial^{\mu} \phi\right)$ describing a set of fields - scalar, spinor, vector, whatever, but not including $A_{\mu}$ itself-has a one-parameter group of internal symmetries of the sort we talked about earlier (in Chapter 6). Under this group, an infinitesimal transformation of $\phi$ is given by
$$\delta \phi=-i Q \phi \delta \lambda \quad$$where $Q$ is some matrix, and $\delta \lambda$ some parameter
or, for a finite transformation,
$$
\phi(x) \rightarrow \phi(x, \lambda)=e^{-i Q \lambda} \phi(x)
$$
If this transformation leaves $\mathscr{L}_{m}$ unchanged, under normal circumstances it would enable us to deduce the existence of a conserved current, $J^{\mu}$ :
$$
J^{\mu}=-i \pi^{\mu} Q \phi
$$
This seems a reasonable and necessary condition to get an interaction Lagrangian coupled to the photon. If the photon is coupled to the matter fields with a constant, say the electromagnetic coupling constant $e$, and if you have a conserved current when the photon is around, you can imagine it should stay conserved as $e \rightarrow 0$. So you want to start out with a theory that has a conserved current even before you include the photon. 

Then if we then promote the parameter $\lambda$ to an arbitrary function of spacetime, the infinitesimal transformation 
$$
\delta \phi=-i Q \phi \delta \lambda(x)
$$
is not an invariance of our Lagrangian, because if I compute $\delta\left(\partial^{\mu} \phi\right)$, I'll get two terms;
$$
\delta\left(\partial^{\mu} \phi\right)=\partial^{\mu}(\delta \phi)=\partial^{\mu}(-i Q \phi \delta \lambda(x))=-i Q\left(\partial^{\mu} \phi\right) \delta \lambda-i Q \phi\left(\partial^{\mu} \delta \lambda\right)
$$
The first term is hunky dory, no problem there. But the second term is a disaster. However we've also got the electromagnetic field involved, which under an infinitesimal gauge transformation ($\delta \chi$) obeys $\delta A_\mu=\partial_\mu \delta \chi$. Consider a combination of the ordinary derivative $\partial_{\mu}$ acting on $\phi$ with a product of the vector field $A_{\mu}$ times $\phi$ :
$$
D_{\mu} \phi=\partial_{\mu} \phi+i e A_{\mu} Q \phi
$$
This expression is called the covariant derivative. Its transformation $\delta\left(D_{\mu} \phi\right)$ looks like this:
$$
\begin{aligned}
\delta\left(D_{\mu} \phi\right) &=\delta\left(\partial_{\mu} \phi+i e A_{\mu} Q \phi\right)=\delta\left(\partial_{\mu} \phi\right)+i e\left(\delta A_{\mu}\right) Q \phi+i e A_{\mu} Q(\delta \phi) \\
&=-i Q\left(\partial^{\mu} \phi\right) \delta \lambda-i Q \phi\left(\partial^{\mu} \delta \lambda\right)+i e\left(\partial^{\mu} \delta \chi\right) Q \phi+i e A_{\mu} Q(-i Q \phi \delta \lambda)
\end{aligned}
$$
We can make the second and third terms cancel if we choose
$$
\delta \lambda=e \delta \chi
$$
in which case
$$
\delta\left(D_{\mu} \phi\right)=-i Q\left(\partial^{\mu} \phi+i e A_{\mu} Q \phi\right) \delta \lambda=-i Q\left(D_{\mu} \phi\right) \lambda
$$
The covariant derivative of $\phi$ transforms in exactly the same way as $\phi$, which is why it's called "covariant". 