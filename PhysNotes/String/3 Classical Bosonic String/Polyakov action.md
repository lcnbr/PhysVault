# Polyakov Action^[[[broedela-3 Classical Bosonic String#^e76a0e]]] 
Is a polynomial action with an additional dynamical [[worldsheet]] metric $g_{\alpha \beta}$, the [[Strings|string]] analogue of the [[Polynomial (einbein) Action]]:

$$
S[X,g]=-\frac{1}{2 \pi \kappa^2} \int \mathrm{d} \xi^2 \sqrt{-\operatorname{det} g} \frac{1}{2} g^{\alpha \beta}\left(\partial_{\alpha} X\right) \cdot\left(\partial_{\beta} X\right)
$$

^2638f6

Where $g$ is the [[intrinsic worldsheet metric]]. The [[equations of motion|e.o.m.]] ofr the [[Field|field]] $X$ is the same as for the [[Nambu-Goto action]]^[[[broedela-3 Classical Bosonic String#^0ee739]]](with $\gamma$ replaced by $g$):
$$
\partial_{\alpha}\left(\sqrt{-\operatorname{det} g} ~g^{\alpha \beta} \partial_{\beta} X^{\mu}\right)=0
$$

^96acbc


The [[equations of motion|e.o.m.]] for the [[intrinsic worldsheet metric]] $g$ is^[[[broedela-3 Classical Bosonic String#^4cdcb4]]](by varying the action and thus $g$, c.f. [[intrinsic worldsheet metric#Varying the determinant]]): 
$$
\left(\partial_{\alpha} X\right) \cdot\left(\partial_{\beta} X\right)=\frac{1}{2} g_{\alpha \beta} g^{\gamma \delta}\left(\partial_{\gamma} X\right) \cdot\left(\partial_{\delta} X\right)
$$
Its solution is given by:

$$g_{\alpha \beta}=f(\xi)\left(\partial_{\alpha} X\right) \cdot\left(\partial_{\beta} X\right)=f(\xi) \gamma_{\alpha \beta}$$

And it relates the [[intrinsic worldsheet metric]] with the [[induced worldsheet metric]], where $f(\xi)$ is a local scale^[[[broedela-3 Classical Bosonic String#^80a893]]]. This scale nicely cancels in the [[#^2638f6|action]] and thus in the [[#^96acbc|field eom]]. This scaling freedom in fact has a name: *[[Weyl invariance]]* and is the analogue of the einbein freedom from the [[Polynomial (einbein) Action]]

# Symmerties

The [[Polyakov action]] carries over the [[Nambu-Goto action#Symmetries]] and adds [[Weyl invariance]]:
On the [[worldsheet]]
- [[reparametrisation invariance]]
- [[Weyl invariance]] 

On [[spacetime]]
- [[Poincare invariance]]

# Gauge choices


Since we have [[reparametrisation invariance]] and [[Weyl invariance]] we impose the [[conformal gauge]]. 

## Action in [[conformal gauge]]
The resulting action describes $D$ free massless scalar particles on the [[worldsheet]]
$$
S=-\frac{1}{2 \pi \kappa^2} \int \mathrm{d} \xi^2 \frac{1}{2} \eta^{\alpha \beta}\left(\partial_{\alpha} X\right) \cdot\left(\partial_{\beta} X\right)
=\int \mathrm{d} \tau L, \quad L=\frac{1}{2 \pi \kappa^{2}} \int \mathrm{d} \sigma \frac{1}{2}\left(\dot{X}^{2}-X^{\prime 2}\right)
$$

## [[equations of motion|e.o.m.]] in [[conformal gauge]]
The corresponding equation of motion for $X$ is simply the *[[harmonic wave equation]]*:^[[[broedela-3 Classical Bosonic String#^ad765e]]]
$$
\partial^2 X^{\mu}=0 \quad \text { or } \quad \ddot{X}=X^{\prime \prime}
$$

^583cf2

The equation of motion for the [[intrinsic worldsheet metric|worldsheet metric]]  $g$ (in [[conformal gauge]])^[[[broedela-3 Classical Bosonic String#^7f20e1]]]:
$$
T_{\alpha \beta}:=\left(\partial_{\alpha} X\right) \cdot\left(\partial_{\beta} X\right)-\frac{1}{2} \eta_{\alpha \beta} \eta^{\gamma \delta}\left(\partial_{\gamma} X\right) \cdot\left(\partial_{\delta} X\right)=0
$$
where $T_{\alpha \beta}$ is the [[energy-momentum tensor]] for $D$ scalar particles. The trace of the energy-momentum tensor vanishes by construction due to the [[Weyl invariance|conformal/Weyl symmetry]] ^[[[broedela-3 Classical Bosonic String#^57dd9e]]]$\left(T_{\alpha}^{\alpha}=0\right)$, while the two remaining e.o.m. are called [[Virasoro constraints]]

The [[energy-momentum tensor]] $T_{\alpha \beta}$ is conserved, it is sufficient to impose constraints on an initial time slice only.


# Solutions
We now need to solve the [[#^583cf2|e.o.m.s]] and [[Virasoro constraints]]
## In [[light cone coordinates#In the worldsheet]]

Using [[light cone coordinates#In the worldsheet]] the [[#^583cf2|e.o.m.s]] and [[Virasoro constraints]] read
$$
\partial_{\mathrm{L}} \partial_{\mathrm{R}} X^{\mu}=0, \quad\left(\partial_{\mathrm{L} / \mathrm{R}} X\right)^2=0
$$

^2cca81

The first equation can be solved by a simple separation of variables
$$
X^{\mu}\left(\xi^{\mathrm{L}}, \xi^{\mathrm{R}}\right)=X_{\mathrm{L}}^{\mu}\left(\xi^{\mathrm{L}}\right)+X_{\mathrm{R}}^{\mu}\left(\xi^{\mathrm{R}}\right)
$$

^b37d90

While there are $D$ left-movers $X_{\mathrm{L}}$ and $D$ right-movers $X_{\mathrm{R}}$ initially, the [[Virasoro constraints]] $\left(\partial X_{\mathrm{R}, \mathrm{L}}\right)^2=0$ remove one left- and one right-mover. Two reparametrisations remain:
- [[conformal transformations]]:
$$
\xi^{\mathrm{R}} \mapsto \xi^{\prime \mathrm{R}}\left(\xi^{\mathrm{R}}\right), \quad \xi^{\mathrm{L}} \mapsto \xi^{\mathrm{L}}\left(\xi^{\mathrm{L}}\right)
$$
In two dimensions (and only there), there are infinitely many [[conformal transformations]]. Those remove another left- and right-mover.
- constant shifts: between $X_{\mathrm{L}}^{\mu}$ and $X_{\mathrm{R}}^{\mu}$.

In summary, there are $(D-2)$ left- and right-movers remaining, which parametrise the transverse directions of the [[Strings|string]].

# Extent of [[Strings|string]]

So far we have not constrained the extent of the [[worldsheet]]s, they have extended infinitely   in [[spacetime]]. But we want confined spacial extent:

- For closed [[Strings|string]]: circular topology, identify $\sigma \equiv \sigma + 2 \pi$ (other choices are possible)
- For open [[Strings|string]]: interval topology, boundary conditions at $\sigma=0,\pi$ ([[Branes]])

## Solutions for the [[closed string]] 

^11dd41

### Covariant formulation

For the [[closed string]], the solution function $X=X_\mathrm{L}+X_\mathrm{R}$ to [[#^2cca81]] in [[light cone coordinates#In the worldsheet]] should be $2 \pi$-[[periodic]]^[[[broedela-3 Classical Bosonic String#^aa2a07]]]; this is most easily realised with a [[Fourier decomposition]]^[[[broedela-3 Classical Bosonic String#^aff9cb]]]:
$$
X_{\mathrm{L} / \mathrm{R}}^{\mu}=\frac{1}{2} x^{\mu}+\frac{1}{2} \kappa^2 p^{\mu} \xi^{\mathrm{L} / \mathrm{R}}+\sum_{n \neq 0} \frac{i \kappa}{\sqrt{2} n} \alpha_{n}^{\mathrm{L} / \mathrm{R}, \mu} \exp \left(-i n \xi^{\mathrm{L} / \mathrm{R}}\right)
$$

^83a903

To note:
- $x^\mu$ and $p^\mu$ are constants here, labeled suggestively. 
-   The coefficients $i \kappa / \sqrt{2} n$ are for convenience^[[[broedela-3 Classical Bosonic String#^d32b3c]]. 
-   Linear dependency on $\xi^{\mathrm{L} / \mathrm{R}}$ does not clash with the periodicity condition because after adding the left- and right-mover, the dependence on $\sigma$ drops out: $X^{\mu}=x^{\mu}+$ $\kappa^2 p^{\mu} \tau+\ldots$^[[[broedela-3 Classical Bosonic String#^a18e07]]]. 
-   Reality of the [[worldsheet#Embedding]] coordinate $X$ is ensured by demanding $\alpha_{-n}=\left(\alpha_{n}\right)^{*}$^[[[broedela-3 Classical Bosonic String#^12e07c]]].

The motion of the center of mass is described by the conjugate pair $x, p$ (conjugation involves an additional factor of $\kappa^2$ ), while the [[string modes]] $\alpha_{n}^{\mathrm{L} / \mathrm{R}, \mu}$ (left/right movers) describe the amplitudes of the oscillations on the [[Strings|string]].
Plugging the [[#^83a903|above]] into the [[Virasoro constraints#In light cone coordinates In the worldsheet]]  yields
$$
\kappa^2 \sum_{n} L_{n}^{\mathrm{L} / \mathrm{R}} \exp \left(-i n \xi^{\mathrm{L} / \mathrm{R}}\right)=0
$$

Where the $L_{n}^{\mathrm{L} / \mathrm{R}}$ are the [[Virasoro modes]].

Since all [[Virasoro constraints]] $L_{n}=0$ are conserved by the e.o.m.
$$
\dot{L}_{n}=i n L_{n},
$$
it is sufficient to impose them on an initial time slice only.
The [[Virasoro modes#Mass of the string|mass of a string]] depends on the mode amplitudes $\alpha$. If none of the modes is excited, the [[Strings|string]] behaves like a massless point particle. If there are only few and small excitations, one will encounter a light (or tiny) particle while large excitations can add up to yield a big and highly massive object.

Due to the [[Minkowski signature]] of the [[spacetime]], the [[time-like]] modes $\alpha^{0}$ contribute a negative $M^2$. If one, however, takes all [[Virasoro constraints]] into account, tachyons (particles with negative mass-squared) are excluded.



### [[Light Cone Gauge]] with [[light cone coordinates#In embedding space ambient space]]

The [[Virasoro constraints]] in their above form are complicated and non-linear. We can employ the [[Weyl invariance|conformal symmetry]] on the [[worldsheet]] in order to solve them. The connection between the [[Weyl invariance|conformal symmetry]] on the [[worldsheet]] and the ability to choose the particular gauge in [[light cone coordinates]] below can not spelled out here explicitly.

Changing to [[light cone coordinates#In embedding space ambient space]] and applying [[Light Cone Gauge]] ($X^+$depends on $\tau$ linearly, i.e. does not exhibit oscillator modes.)
This results in the gauge condition
$$
X_{\mathrm{L} / \mathrm{R}}^+=x_{\mathrm{L} / \mathrm{R}}^++\frac{1}{2} \kappa^2 p_{\mathrm{L} / \mathrm{R}}^+ \xi^{\mathrm{L} / \mathrm{R}}
$$
The [[Virasoro constraints#In light cone coordinates In embedding space ambient space]] is solved by
$$
X_{\mathrm{L} / \mathrm{R}}^-(\xi)=\frac{1}{\kappa^2 p_{\mathrm{L} / \mathrm{R}}^+} \int^{\xi} d \xi^{\prime}\left(\partial \vec{X}_{\mathrm{L} / \mathrm{R}}\left(\xi^{\prime}\right)\right)^2
$$
leaving $2(D-2)$ arbitrary functions $\vec{X}_{\mathrm{L} / \mathrm{R}}\left(\xi^{\mathrm{L} / \mathrm{R}}\right)$. These are the transverse modes of the [[Strings|string]].

Periodicity of $X^+$and $X^-$ requires
$$
p_{\mathrm{L}}^+=p_{\mathrm{R}}^+=p^+, \quad \int_{0}^{2 \pi} d \xi\left(\left(\partial \vec{X}_{\mathrm{R}}\right)^2-\left(\partial \vec{X}_{\mathrm{L}}\right)^2\right)=0
$$
In addition, there is the residual gauge freedom $\Delta X_{\mathrm{R}}^{\mu}\left(\xi^{\mathrm{R}}\right)=-\Delta X_{\mathrm{L}}^{\mu}\left(\xi^{\mathrm{L}}\right)=$ const., which corresponds to the residual constraints mentioned above.

![[Virasoro modes#In light cone coordinates In embedding space ambient space]]


In summary, the [[Light Cone Gauge]] comes with manifestly positive mass for all particles and is a very convenient way to get rid of almost all constraints. However, by introducing [[light cone coordinates]], we give up a manifestly Lorentz-invariant formulation.

## Summary
We have seen that the classical closed string is described by
- a bunch of harmonic oscillators $\alpha_{n}^{\mathrm{L} / \mathrm{R}}$ for the string modes;
- a relativistic particle $(x, p)$ describing the centre of mass.

Both systems are coupled via [[Virasoro constraints]].
We have derived two reasonable formulations:
- Covariant formulation
    - $D$ oscillators $\alpha_{n}^{\mu}$ per mode,
    - physical solutions must obey [[Virasoro constraints]] $L_{n}^{\mathrm{R}}=L_{n}^{\mathrm{L}}=0$,
    - [[Poincare invariance|Poincaré symmetry]] in spacetime manifest,
    - [[worldsheet]] theory has [[conformal invariance|conformal symmetry]] (later).
- Light cone formulation
    - $D-2$ oscillators $\vec{\alpha}_{n}$ per mode,
    - physical solutions must obey $L_{0}^{\mathrm{R}}=L_{0}^{\mathrm{L}}=0$ residual constraints,
    - [[Poincare invariance|Poincaré symmetry]] of spacetime partially manifest,
    - manifest [[Poincare invariance|Poincaré symmetry]] on [[worldsheet]].