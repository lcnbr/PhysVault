# Conformal Transformations

Conformal transformations are coordinate transformations preserving the angles locally, but allowing for changes in the definition of length. They preserve the metric up to a scale:

$$
g_{\mu^{\prime} \nu^{\prime}}^{\prime}\left(x^{\prime}\right)=\frac{\mathrm{d} x^{\mu}}{\mathrm{d} x^{\prime \mu^{\prime}}} \frac{\mathrm{d} x^{\nu}}{\mathrm{d} x^{\prime \nu^{\prime}}} g_{\mu \nu}(x) \stackrel{!}{=} f(x) g_{\mu^{\prime} \nu^{\prime}}(x) .
$$
 [[conformal transformations]] are the coordiante transform version of  [[Weyl invariance|weyl transformations]]
# Action on Coordinates. 
![[conformal group]]

# Action on Fields. 
Consider a free [[Field#Scalar Field|scalar]] with action

$$
S \sim \int \mathrm{d} x^{D} \frac{1}{2} \partial_{\mu} \Phi(x) \partial^{\mu} \Phi(x) .
$$

In order for the action to be invariant under the [[conformal group]], the [[Field#Scalar Field|scalar]] must
- transform under [[conformal group#^2426d1|Lorentz rotations]] and [[conformal group#^7e1b95|translations]] as
$$\Phi^{\prime}(x)=\Phi(\Lambda x+a) .$$


- Invariance under a [[conformal group#^8c03fe|scaling]] $x^{\prime}=s x$ requires
$$
\Phi^{\prime}(x)=s^{(D-2) / 2} \Phi(s x),
$$

^25c485

- while invariance under [[conformal group#^cd9a43|inversions]] translates into
$$
\Phi^{\prime}(x)=\left(x^{2}\right)^{-(D-2) / 2} \Phi(1 / x) .
$$


In the same way one can derive similar, but more complicated rules for

- a scalar field $\phi(x)$ with different scaling $\phi^{\prime}(x)=s^{\Delta} \phi(s x)$, ^9a696d
- spinning fields $\rho_{\mu}, \ldots$,
- derivatives $\partial_{\mu} \Phi, \partial_{\mu} \partial_{\nu} \Phi, \partial^{2} \Phi, \ldots$

# 2D Conformal Symmetries. 
In comparison to other dimensions, QFT's in 2D are rather tractable. [[conformal field theory|CFT]]'s in 2D are especially simple. The [[conformal group]] splits: [[conformal group#In 2D]]

The generators of the algebra underlying the group $\operatorname{SL}(2, \mathbb{R})_{\mathrm{L} / \mathrm{R}}$ can be supplemented by further generators to yield the infinite-dimensional Virasoro algebra. Infinitesimal transformations are then given by

$$
\delta \xi^{\mathrm{L} / \mathrm{R}}=\epsilon^{\mathrm{L} / \mathrm{R}}\left(\xi^{\mathrm{L} / \mathrm{R}}\right)=\sum_{n} \epsilon_{n}^{\mathrm{L} / \mathrm{R}}\left(\xi^{\mathrm{L} / \mathrm{R}}\right)^{1-n},
$$

where the values $n=-1, n=0$ and $n=1$ correspond to the generators of $\operatorname{SL}(2, \mathbb{R})_{\mathrm{L} / \mathrm{R}}$. The boundaries are typically distorted by Virasoro transformations, only a subalgebra preserves them, e.g. $\operatorname{SL}(2, \mathbb{R})$.