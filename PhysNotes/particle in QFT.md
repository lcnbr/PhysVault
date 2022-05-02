https://physics.stackexchange.com/questions/163691/the-concept-of-particle-in-qft/163705#163705

Somewhat surprisingly, the "generic" particle of QFT is in fact totally delocalized.
More precisely, particles are thought to come from the mode expansion of free fields. Since every free relativistic field $\phi$ fulfills the Klein-Gordon equation $\left(\partial^{\mu} \partial_{\mu}-m^{2}\right) \phi=0$, a Fourier transform shows that it can be expanded as
$$
\phi(x)=\int \frac{\mathrm{d}^{3} p}{(2 \pi)^{3}} \frac{1}{\sqrt{2 p^{0}}}\left(a(\vec{p}) \mathrm{e}^{\mathrm{i} p x}+a^{\dagger}(\vec{p}) \mathrm{e}^{-\mathrm{i} p x}\right)
$$
where Lorentz invariance is not manifest, but can nevertheless be shown. A quantum field is operator-valued, and the operator valued objects $a(\vec{p}), a^{\dagger}(\vec{p})$ fulfill exactly the correct commutation relations to be interpreted as creation and annihilation operators. The $n$-particle state of particles that are associated with the field $\phi$ is now defined as
$$
\left|n ; p_{1}, \ldots, p_{n}\right\rangle:=a^{\dagger}\left(p_{1}\right) \ldots a^{\dagger}\left(p_{n}\right)|\Omega\rangle
$$
where $|\Omega\rangle$ is the (mostly) unique vacuum state. In this way, you first create all particle states that are sharply localized in momentum space (and hence completely delocalized in position space) and you can build localized particle states by the usual building of "wavepackets" with fuzzy momentum out of the sharp momentum states:

A QM wavepacket of width $\sigma_{x}$ localized at $x_{0}$ is constructed out of the pure momentum states $|\vec{p}\rangle$ as something like
$$
\left|x_{0}, \sigma_{x}\right\rangle=\int \frac{\mathrm{d}^{3} p}{(2 \pi)^{3}} \mathrm{e}^{2 \mathrm{i} \sigma_{x}^{2}\left(\mathrm{x}-\mathrm{x}_{0}\right)^{2}}|p\rangle
$$
It works exactly the same for localized QFT particles, except that one should multiply the measure with $\frac{1}{\sqrt{2 p^{0}}}$ to have a Lorentz invariant integration, and, of course, $|p\rangle=a^{\dagger}(p)|\Omega\rangle$.

The idea that "particles are local excitations of the fields" comes from the observation that this mode expansion is almost completely analogous to a classical field fulfilling a wave equation like the Klein-Gordon equation, where the $a(\vec{p}), a^{\dagger}(\vec{p})$ would directly represent an excitation of the field of wavenumber $\vec{p}$. It cannot be made precise in the context of QFT because the quantum field is operator-valued and has no definite values, so it is wholly unclear what rigorous sense could be given to it being "excited". It is a nice picture, but nothing you should take too literally.

Also, take note that this is for the free field. The true interacting field of a QFT cannot be mode expanded in this way, and particle states are (through the LSZ formalism) only obtained in the asymptotic past and future (when they were far enough apart for interactions to be effectively nonexistent) of the theory - the Hilbert space (and hence any states you could or could not identify as particles) of interacting QFTs is essentially unkown.

Furthermore, more mathematical methods of constructing QFTs often first construct the $a, a^{\dagger}$ and the Fock space of particle states, and then define the field out of it - then, the roles of particle and field as "fundamental" and "derived" are somewhat reversed.