We could now proceed and quantise the [[Higgs Mechanism#^8dcf8d|SQED Lagrangian]] . The model includes a massive vector field whose propagator is
$$
G^{\mu v}(p)=\frac{\eta^{\mu v}+p^{\mu} p^{v} / m^{2}}{p^{2}+m^{2}}
$$
The trouble with this massive vector field propagator is that for large momenta $p$ it approaches a finite value rather than decaying quadratically. This makes the UV-behaviour far worse than for an ordinary gauge field. Moreover, the appearance of the inverse of the mass spoils power counting. This **generically renders the model non-renormalisable.**

Now **the above [[Higgs Mechanism#^8dcf8d|SQED Lagrangian]] is very special, and the UV-divergences in fact cancel such that the model remains renormalisable**. This nice behaviour evidently is due to gauge symmetry in the original model: One could argue that the model with spontaneous symmetry breaking is really just the same as the model where gauge symmetry is intact; **the choice of the ground state should make no difference concerning renormalisability.**

More practically one can argue that renormalisability is a question of the UV. When momenta are reasonably large, the mass terms are insignificant, it does not matter whether $\mu^{2}$ is positive or negative.
A rigorous approach to show renormalisability explicitly is given by the so-called $R_{\xi}$-gauges. It is analogous to [[gauge fixing action for EM|gauge fixing]] by the [[Faddeev-Popov ghosts|Faddeev-Popov]] method. Let us therefore discuss this method.

We return to the [[Higgs Mechanism#^f9e5b8|first parametrisation]] of the complex scalar field $\phi$ where the momentum terms read 
![[Higgs Mechanism#^891e65]]

Now we need to take care of the off-diagonal quadratic term between $A$ and $\rho$. In [[Higgs Mechanism]] we have used a [[Higgs Mechanism#^36ff46|gauge transformation]] to remove it. Here this is achieved by adding an extra term to the gauge fixing functional $G[A, \Omega]$
$$
G=\partial^{\mu} A_{\mu}-\Omega-\xi q v \rho .
$$
Next we insert a delta-functional together with a compensating functional determinant into the path integral
$$
\int \operatorname{D} \alpha \operatorname{Det}\left(\delta G^{\prime} / \delta \alpha\right) \Delta\left[G^{\prime}\right] \text {. }
$$
We then eliminate the delta-functional by integrating over the auxiliary field $\Omega$ with Gaussian weight $S_{\Omega}=-\frac{1}{2} \xi^{-1} \int \mathrm{d} x^{4} \Omega^{2}$. This leads to a gauge fixing term
$$
\mathcal{L}_{\mathrm{gf}}=-\frac{1}{2} \xi^{-1}(\partial \cdot A)^{2}-\frac{1}{2} \xi q^{2} v^{2} \rho^{2}+q v \partial^{\mu} A_{\mu} \rho
$$

The argument of the functional determinant is given by the gauge variation of $G$
$$
\delta G=\partial^{2} \delta \alpha-\xi q^{2} v(v+\eta) \delta \alpha .
$$
**As opposed to the case of plain QED, this does depend on the fields, and therefore cannot be disregarded**. As for the non-abelian gauge field, we replace the functional determinant by the introduction of the fermionic [[Faddeev-Popov ghosts|ghost]] fields $C, \bar{C}$. Their Lagrangian reads
$$
\mathcal{L}_{\mathrm{gh}}=\bar{C}\left(\partial^{2}-\xi q^{2} v^{2}-\xi q^{2} v \eta\right) C .
$$
Collecting the various Lagrangians, we find the kinetic terms
$$
\begin{aligned}
\mathcal{L}=& \mathcal{L}_{\mathrm{SQED}}+\mathcal{L}_{\mathrm{gf}}+\mathcal{L}_{\mathrm{gh}} \\
=&-\frac{1}{2}\left(\partial^{\mu} A^{v}\right)\left(\partial_{\mu} A_{v}\right)+\frac{1}{2}\left(1-\xi^{-1}\right)(\partial \cdot A)^{2}-\frac{1}{2} q^{2} v^{2} A^{2} \\
&-\frac{1}{2}(\partial \eta)^{2}-\frac{1}{4} \lambda v^{2} \eta^{2} \\
&-\frac{1}{2}(\partial \rho)^{2}-\frac{1}{2} \xi q^{2} v^{2} \rho^{2}-\partial^{\mu} \bar{C} \partial_{\mu} C-\xi q^{2} v^{2} \bar{C} C \\
&+\text { interactions. }
\end{aligned}
$$
The gauge field needs further scrutiny, let us write its propagator
$$
G^{\mu v}(p)=\frac{1}{p^{2}+q^{2} v^{2}}\left(\eta^{\mu v}-(1-\xi) \frac{p^{\mu} p^{v}}{p^{2}+\xi q^{2} v^{2}}\right) .
$$
This propagator has several interesting features:
- For large momenta it decays quadratically.
- No mass scale appears in the denominator on its own.
- For $\xi \rightarrow \infty$ it approaches the propagator of a massive vector field.
- The 3 transverse modes have mass $q v$.
- The longitudinal mode has mass $\sqrt{\xi} q v$ as can be seen from the expression
$$
p_{\mu} G^{\mu v}(p)=\frac{\xi p^{v}}{p^{2}+\xi q^{2} v^{2}} .
$$

This means we have the following particles:
- a massive vector particle $A_{\mu}$ of mass $q v$.
- a scalar Higgs particle $\eta$ with mass $\sqrt{\lambda / 2} v$,
- the longitudinal mode of $A_{\mu}$ of mass $\sqrt{\xi} q v$.
- a scalar particle $\rho$ of mass $\sqrt{\xi} q v$,
- a pair of [[Faddeev-Popov ghosts|ghost]] and anti-[[Faddeev-Popov ghosts|ghost]] particles $C, \bar{C}$ of mass $\sqrt{\xi} q v$,

The former two are the physical particles of the model. The latter four are unphysical excitations, two bosons and two fermions, all with the same mass. Just as in the case of [[Faddeev-Popov ghosts|Faddeev-Popov]] gauge fixing, their contributions conspire to cancel out from all physical processes.

Moreover it can be shown that all physical processes are independent of the gauge fixing parameter $\xi$. Several particular values of $\xi$ are relevant:

- In the limit of $\xi \rightarrow \infty$ we recover the [[Higgs Mechanism#Alternative parametrisation|second parametrisation]] of the Lagrangian discussed above. In that case all the additional unphysical excitations become infinitely massive and decouple from physics. In the limit $\xi \rightarrow \infty$ the model is perfectly unitary. However, the standard massive vector field renders the theory superficially non-renormalisable.
- For finite values of $\xi$ the model is perfectly renormalisable. However, it contains 4 additional excitation modes which are partially non-unitary. Unitarity is recovered only in the sector of physical states. The discussion is analogous to the case of unbroken gauge symmetry.
- The value $\xi=1$ is convenient for computations since the unphysical particles have the same mass as the vector field, and since the vector field propagator has a plain constant numerator.