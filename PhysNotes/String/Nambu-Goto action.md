[[.md|Nambu-Goto action]] is the [[Strings|string]] generalization of the [[Worldline action for a relativistic point particle]]^[[[broedela-3 Classical Bosonic String#^8a2d52]]]. Since the [[Worldline action for a relativistic point particle|worldlone action]] was proportional to the proper time^[[[broedela-3 Classical Bosonic String#^b224fe]]], the [[.md|Nambu-Goto action]] will be simply the area of the [[worldsheet]]^[[[broedela-3 Classical Bosonic String#^65b741]]]:

- [[worldline]] $\rightarrow$ [[worldsheet]]
- [[../AnalyticalMech/Action|action]] $\approxeq$ 'length' $\rightarrow$ [[../AnalyticalMech/Action|action]] $\approxeq$ 'area'

## Area in [[embedding space]]
The area element in terms of the embedding coordinates $X^\mu$ in [[Euclidean space]] (using a [[Wick rotation]]) reads^[[[broedela-3 Classical Bosonic String#^00a026]]]:

$$
\begin{aligned}
\mathrm{d}^{2} A &=\mathrm{d} \tau \, \mathrm{d} \sigma\left|X^{\prime}\right||\dot{X}||\sin \theta| \\
&=\mathrm{d} \tau \,\mathrm{d} \sigma \,\sqrt{X^{\prime 2} \dot{X}^{2} \sin ^{2} \theta} \\
&=\mathrm{d} \tau \,\mathrm{d} \sigma \,\sqrt{X^{\prime 2} \dot{X}^{2}\left(1-\cos ^{2} \theta\right)} \\
&=\mathrm{d} \tau \,\mathrm{d} \sigma \,\sqrt{X^{\prime 2} \dot{X}^{2}-\left(X^{\prime} \cdot \dot{X}\right)^{2}} \\
&=\mathrm{d} \xi^{2} \,\sqrt{\operatorname{det} \gamma},
\end{aligned}
$$

Note we used [[worldsheet#Derivatives]], and $\gamma$ is the [[induced worldsheet metric]]. Undoing the [[Wick rotation]] in order to return to a [[worldsheet]] with [[Minkowski signature]] leads to (just adds a minus sign under the $\sqrt{\square}$):

$$
S=-\frac{1}{2 \pi \kappa^{2}} A=-\frac{1}{2 \pi \kappa^{2}} \int \! \mathrm{d} \xi^{2} \sqrt{-\operatorname{det} \gamma}
$$

Where $\frac{1}{2 \pi \kappa^{2}}=\frac{1}{2 \pi \alpha'} =T$ is the [[Strings#Tension|string tension]]

## [[../AnalyticalMech/equations of motion|e.o.m.]]

By varying the action (using the [[induced worldsheet metric#Variation of the determinant broedela-3 Classical Bosonic String 108f58|variation of the determinant of the induced worldsheet metric]]) we obtain the following [[../AnalyticalMech/equations of motion|e.o.m.]]:

$$
\partial_{\alpha}\left(\sqrt{-\operatorname{det} \gamma} \gamma^{\alpha \beta} \partial_{\beta} X^{\mu}\right)=0
$$

^f8e1a4

The [[induced worldsheet metric|metric]] contains the [[embedding space|embedding]], this equation is highly nonlinear. To simplify this, as was the case with the [[Worldline action for a relativistic point particle]], we are going to pass to a polynomial action: the [[3 Classical Bosonic String/Polyakov action]]

### Geometrically

Geometrically (in euclidean signature)? The stationary action demands a surface with minimal area, i.e. a static soap film. Thus, the mean curvature is zero everywhere which implies that every point of the surface is a saddle point.
(c.f. [[../math/saddle point approximation]])


## Symmetries
- As for the [[Worldline action for a relativistic point particle|worldline action]] the [[.md|Nambu-Goto action]] features [[reparametrisation invariance]]: $\xi^\alpha\rightarrow\tilde{\xi}^\alpha(\xi)$As for the [[Worldline action for a relativistic point particle|point particle]], this is a [[../QFTII/gauge symmetry]]. It reflects the fact that we have a redundancy in our description because the [[worldsheet#worldsheet coordinates]] have no physical meaning.
- [[Poincare invariance]] of the [[../QFTII/spacetime]]. This is a global symmetry from the perspective of the [[worldsheet]], meaning that the parameters $\Lambda^\mu_\nu$ and $c^\mu$ which label the symmetry transformation are constants and do not depend on [[worldsheet#worldsheet coordinates]]

