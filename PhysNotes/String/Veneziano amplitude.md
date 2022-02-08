# Veneziano amplitude

For a start, let us consider an $n$-point closed-string amplitude (with $\mathcal{O}_{k}=\mathcal{O}\left[q_{k}\right]\left(z_{k}, \bar{z}_{k}\right)$ )

$$
A_{n} \sim \frac{1}{g_{\mathrm{s}}^{2}}\left\langle V_{1} \ldots V_{n}\right\rangle \sim g_{\mathrm{s}}^{n-2} \int \mathrm{d} z^{2 n}\left\langle\mathcal{O}_{1} \ldots \mathcal{O}_{n}\right\rangle .
$$

The simplest amplitude occurs for tachyon scattering; amplitudes for other strings (e.g. gluons) contain additional fields whose presence complicates the calculation of the correlator. Performing [[Wick's theorem|Wick]] contractions and the [[vertex operators#^e06534|zero mode integration]] yields

$$
\left\langle\mathcal{O}_{1} \ldots \mathcal{O}_{n}\right\rangle \sim \delta^{D}(Q) \prod_{j<k}\left|z_{j}-z_{k}\right|^{\kappa^{2} q_{j} \cdot q_{k}} 
$$

The integral is invariant under [[moebius transformation|Möbius transformations]] (note that $q_{k}^{2}=4 / \kappa^{2}$ ). We map three punctures to fixed positions $z_{1}=\infty, z_{2}=0, z_{3}=1$ The remaining integral for $n=4$ external strings reads

$$
A_{4} \sim g_{\mathrm{s}}^{2} \delta^{D}(Q) \int \mathrm{d} z^{2}|z|^{\kappa^{2} q_{2} \cdot q_{4}}|1-z|^{\kappa^{2} q_{3} \cdot q_{4}}
$$

 In fact, this transformation amounts to a factor of the divergent integral $\int \mathrm{d} z_{1}^{2} \mathrm{~d} z_{2}^{2} \mathrm{~d} z_{3}^{2}$. This integral does not depend on any external data and should be factored out from any amplitude calculation. The 6 integrations correspond to the 6 [[conformal transformations|global conformal symmetries]]. The above four-point integral can be performed exactly and yields a combination of [[gamma function]]s (in fact, it can be expressed as a product of [[Euler Beta function]]s):

$$
A_{4} \sim g_{\mathrm{s}}^{2} \delta^{D}(Q) \frac{\Gamma\left(-1-\kappa^{2} s / 4\right) \Gamma\left(-1-\kappa^{2} t / 4\right) \Gamma\left(-1-\kappa^{2} u / 4\right)}{\Gamma\left(+2+\kappa^{2} s / 4\right) \Gamma\left(+2+\kappa^{2} t / 4\right) \Gamma\left(+2+\kappa^{2} u / 4\right)}
$$

in terms of the [[Mandelstam invariants]] $s, t, u$

$$
s=-\left(q_{1}+q_{2}\right)^{2}, \quad t=-\left(q_{1}+q_{4}\right)^{2}, \quad u=-\left(q_{1}+q_{3}\right)^{2},
$$

with the relation $s+t+u=-q_{1}^{2}-q_{2}^{2}-q_{3}^{2}-q_{4}^{2}=-16 / \kappa^{2}$.

This is the Virasoro-Shapiro amplitude for closed strings.

Repeating the four-point calculation for the open string, this time using the vertex operator

$$
V[q]=g_{\mathrm{s}}^{\mathrm{open}} \int \mathrm{d} z \mathcal{O}[q](z) .
$$

The four-point amplitude for open-string tachyons reads then

$$
A_{4} \sim g_{\mathrm{s}} \frac{\Gamma\left(-1-\kappa^{2} s\right) \Gamma\left(-1-\kappa^{2} t\right)}{\Gamma\left(+2+\kappa^{2} u\right)}
$$

It was proposed (not calculated) earlier by Veneziano demanding crossing symmetry. The advent of this expression for the four-point amplitude is considered the birth of string theory (back then: dual resonance model).

The open and closed four-point scattering amplitudes have many desirable features:

- Poles at $s, t, u=4(N-1) / \kappa^{2}$ or $s, t=(N-1) / \kappa^{2}$ correspond to an infinite tower of virtual particles exchanged. The mass spectrum coincides with [[closed string spectrum|closed]] and [[open string spectrum|open]] strings.

![](https://cdn.mathpix.com/cropped/2022_01_21_c033a2aa489843817853g-4.jpg?height=137&width=260&top_left_y=1060&top_left_x=526)

- Residues indicate spin $J=2 N$ or $J=N$ : behaviour follows [[closed string spectrum#Regge Trajectories|regge trajectories]]
- Soft behaviour at $s \rightarrow \infty$. Even for [[graviton|gravitons]]!
- Manifest crossing symmetry $s \leftrightarrow t \leftrightarrow u$ or $s \leftrightarrow t .$ Amazing!

Not possible to obtain such a result from QFT with finitely many particles.