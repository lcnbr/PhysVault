From Poisson brackets to anticommutators ^e8071f

Look at the classical [[../Strings|string]] in the [[../../AnalyticalMech/Hamiltonian]] formalism. We would like to derive the [[../Poisson brackets]] for the variables $x, p, \alpha_{n}$.

Let us start with the [[../3 Classical Bosonic String/Polyakov action#Action in conformal gauge]] in [[../3 Classical Bosonic String/conformal gauge]] for a [[../closed string]]
$$
S=\int \mathrm{d} \tau L, \quad L=\frac{1}{2 \pi \kappa^{2}} \int_{0}^{2 \pi} \mathrm{d} \sigma \frac{1}{2}\left(\dot{X}^{2}-X^{\prime 2}\right)
$$
and substitute the closed-string mode expansion (with free time dependence)
$$
X^{\mu}=\kappa \sum_{n} \beta_{n}^{\mu}(\tau) \exp (-i n \sigma) .
$$
Now calculate the derivatives and perform the integration over $\sigma$ in order to obtain a tower of independent harmonic oscillators (here $\beta_{0}$ is the free particle):
$$
L=\frac{1}{2} \sum_{n}\left(\dot{\beta}_{n} \cdot \dot{\beta}_{-n}-n^{2} \beta_{n} \cdot \beta_{-n}\right) .
$$
The [[../Poisson brackets|Poisson bracket]] between canonical momentum and $\beta$ reads:
$$
\pi_{n}=\dot{\beta}_{n}, \quad\left\{\beta_{m}^{\mu}, \pi_{n}^{\nu}\right\}=\eta^{\mu \nu} \delta_{m+n} .
$$
Matching $X$ with the [[../3 Classical Bosonic String/Polyakov action#^83a903|previous classical solution]] at $\tau=0$
$$
x^{\mu}=\kappa \beta_{0}^{\mu}, \quad p^{\mu}=\frac{\pi_{0}^{\mu}}{\kappa}, \quad \alpha_{n}^{\mathrm{L} / \mathrm{R}, \mu}=\frac{n \beta_{\mp n}^{\mu}}{i \sqrt{2}}+\frac{\pi_{\mp n}^{\mu}}{\sqrt{2}}
$$

### [[../Poisson brackets]]
leads to the following non-trivial [[../Poisson brackets]] in the original variables
$$
\left\{x^{\mu}, p^{\nu}\right\}=\eta^{\mu \nu}, \quad\left\{\alpha_{m}^{\mathrm{L}, \mu}, \alpha_{n}^{\mathrm{L}, \nu}\right\}=\left\{\alpha_{m}^{\mathrm{R}, \mu}, \alpha_{n}^{\mathrm{R}, \nu}\right\}=-i m \eta^{\mu \nu} \delta_{m+n} .
$$

^b420f5

These can then be used in [[covariant quantisation|canonical quantisation]]

## Field theory approach
The same result could have been obtained borrowing some mathematical tools which are prominently used in quantum field theory. The [[../../AnalyticalMech/Conjugate momenta|conjugate momentum]] $\Pi^{\mu}$ and canonical [[../Poisson brackets]] read
$$
\Pi^{\mu}=\frac{1}{2 \pi \kappa^{2}} \dot{X}^{\mu}, \quad\left\{X^{\mu}(\sigma), \Pi^{\nu}\left(\sigma^{\prime}\right)\right\}=\eta^{\mu \nu} \delta\left(\sigma-\sigma^{\prime}\right)
$$

Now, given those basic relations, one can use and derive the following relations:
$$
\frac{1}{2 \pi} \int_{0}^{2 \pi} \mathrm{d} \sigma X^{\mu}(0, \sigma)=x^{\mu}, \quad \int_{0}^{2 \pi} \mathrm{d} \sigma \Pi^{\mu}(0, \sigma)=p^{\mu}
$$
as well as
$$
\begin{aligned}
\int_{0}^{2 \pi} \mathrm{d} \sigma X^{\mu}(0, \sigma) \exp (-i n \sigma) &=\frac{2 \pi i \kappa}{\sqrt{2} n}\left(\alpha_{n}^{\mathrm{L}, \mu}-\alpha_{-n}^{\mathrm{R}, \mu}\right) \\
\int_{0}^{2 \pi} \mathrm{d} \sigma \Pi^{\mu}(0, \sigma) \exp (-i n \sigma) &=\frac{1}{\sqrt{2} \kappa}\left(\alpha_{n}^{\mathrm{L}, \mu}+\alpha_{-n}^{\mathrm{R}, \mu}\right)
\end{aligned}
$$
where we have used the fundamental Fourier integral $(2 \pi)^{-1} \int \mathrm{d} \sigma \exp \left(i \sigma\left(n-n^{\prime}\right)\right)=2 \pi \delta_{n-n^{\prime}}$. Using linearity of the [[../Poisson brackets|Poisson bracket]], it is not too difficult to obtain the above [[../Poisson brackets]] of modes.
