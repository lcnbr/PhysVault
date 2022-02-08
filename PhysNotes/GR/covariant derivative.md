---
alias:
- covariant differentiation
tag: GR
---
> In mathematics, the **covariant derivative** is a way of specifying a derivative along tangent vectors of a manifold. Alternatively, the covariant derivative is a way of introducing and working with a connection on a manifold by means of a differential operator, to be contrasted with the approach given by a principal connection on the frame bundle – see [[affine connection]]. In the special case of a manifold isometrically embedded into a higher-dimensional Euclidean space, the covariant derivative can be viewed as the orthogonal projection of the Euclidean directional derivative onto the manifold's tangent space. In this case the Euclidean derivative is broken into two parts, the extrinsic normal component (dependent on the embedding) and the intrinsic covariant derivative component.
>
> The name is motivated by the importance of changes of coordinate in physics: the covariant derivative transforms covariantly under a [[general coordinate transformation]], that is, linearly via the [[Jacobian]] matrix of the transformation.This article presents an introduction to the covariant derivative of a vector field with respect to a vector field, both in a coordinate free language and using a local coordinate system and the traditional index notation. The covariant derivative of a [[tensor fields in GR|tensor]] field is presented as an extension of the same concept. The covariant derivative generalizes straightforwardly to a notion of differentiation associated to a connection on a vector bundle, also known as a Koszul connection.
>
> [Wikipedia](https://en.wikipedia.org/wiki/Covariant%20derivative)



Let us now look at the derivative of a covariant vector
$$
\begin{aligned}
\frac{\partial V^{\alpha}}{\partial x^{\mu}} \rightarrow \frac{\partial (V^{ \alpha})'}{\partial x^{\prime \mu}} &=\frac{\partial}{\partial x^{\prime \mu}}\left(\frac{\partial x^{\prime \alpha}}{\partial x^{\gamma}} V^{\gamma}\right) \\
&=\underbracket{\frac{\partial x^{\beta}}{\partial x^{\prime \mu}} \frac{\partial^{2} x \prime \alpha}{\partial x^{\beta} \partial x^{\gamma}}}_{\text {non-tensorial }} V^{\gamma}+\frac{\partial x^{\prime \alpha}}{\partial x^{\gamma}} \frac{\partial x^{\beta}}{\partial x^{\prime \mu}} \frac{\partial V^{\gamma}}{\partial x^{\beta}}
\end{aligned}
$$
Then we define

$$
\boxed{\nabla_\mu V^\alpha=V^\alpha{}_{; \mu} \equiv \frac{\partial V^{\alpha}}{\partial x^{\mu}}+\Gamma^\alpha{}_{\mu \nu} V^{\nu}}
$$

^covDerivativeVector

which transforms as a [[tensor fields in GR|tensor]] as the non tensoral part of $\pdv{(V^\alpha)'}{x'^\mu}$ cancels the non-tensoral part in the [[transformation of the affine connection#^Vectorcontraction|transformation]] of  the [[affine connection]] contracted to a [[vector fields in GR|vector]]: 
$$
(V^\alpha{}_{; \mu})'=\frac{\partial x^{\prime \alpha}}{\partial x^{\beta}} \frac{\partial x^{\gamma}}{\partial x^{\prime \mu}} V^\beta{}_{; \gamma}
$$

This is a covariant derivative of a contravariant vector. 

# Covariant derivative of a [[one-forms in GR|covector]]
For a [[one-forms in GR|covariant vector]], we can find an analogous definition. Starting from
$$
\begin{aligned}
\frac{\partial U_{\alpha}}{\partial x^{\mu}} \rightarrow \frac{\partial (U_{\alpha})^{\prime}}{\partial x^{\prime \mu}} &=\frac{\partial}{\partial x^{\prime \mu}}\left(\frac{\partial x^{\beta}}{\partial x^{\prime \mu}} U_{\beta}\right) \\
&=\frac{\partial x^{\beta}}{\partial x^{\prime \alpha}} \frac{\partial x^{\gamma}}{\partial x^{\prime \mu}} \frac{\partial U_{\beta}}{\partial x^{\gamma}}+\frac{\partial^{2} x^{\beta}}{\partial x^{\prime \alpha} \partial x^{\prime \mu}} U_{\beta}
\end{aligned}
$$
We then use [[transformation of the affine connection#^covectorContraction]] to define:

$$
U_{\alpha ; \mu} \equiv \frac{\partial U_{\alpha}}{\partial x^{\mu}}-\Gamma^\delta{}_{\alpha \mu} U_{\delta}
$$

^covDerCovector

which transforms as a [[tensor fields in GR|tensor]].


# Covariant derivative of a [[tensor fields in GR|tensor]]
For a [[tensor fields in GR|tensor]], we can analogously construct a covariant derivative
$$
T^\alpha{}_{\beta \gamma ; \mu}=\frac{\partial}{\partial x^{\mu}} T^\alpha{}_{\beta \gamma}-\Gamma^\rho{}_{\beta \mu} T^\alpha{}_{\rho \gamma}-\Gamma^\rho{}_{\gamma \mu} T^\alpha{}_{\beta \rho}+\Gamma^\alpha{}_{\mu \rho} T^\rho{}_{\beta \gamma} .
$$

^covDerTensor

# Properties:

## Linear

The covariant derivative of a linear combination of [[tensor fields in GR|tensors]] (with constant coefficients) is the same linear combination of the covariant derivatives. For instance if $\alpha$ and $\beta$ are constants, then
$$
\left(\alpha A^\mu{}_{\nu}+\beta B^\mu{}_{\nu}\right)_{; \lambda}=\alpha A^\mu{}_{\nu ; \lambda}+\beta B^\mu{}_{\nu ; \lambda}
$$

## Leibniz rule
The covariant derivative of a direct product of [[tensor fields in GR|tensors]] obeys the Leibniz rule. For instance,
$$
\left(A^\mu{}_{\nu} B^{\lambda}\right)_{; \rho}=A^\mu{}_{\nu ; \lambda} B^{\lambda}+A^\mu{}_{\nu} B^\lambda{}_{; \rho}
$$

## Contraction
The covariant derivative of a contracted [[tensor fields in GR|tensor]] is the contraction of the covariant derivative. For instance, setting $\sigma=\lambda$ in [[#^covDerTensor]] gives
$$
\begin{aligned}
T^\alpha{}_{\beta \alpha ; \mu}&=\frac{\partial}{\partial x^{\mu}} T^\alpha{}_{\beta \alpha}-\Gamma^\rho{}_{\beta \mu} T^\alpha{}_{\rho \alpha}-\cancel{\Gamma^\rho{}_{\alpha \mu} T^\alpha{}_{\beta \rho}}+\cancel{\Gamma^\alpha{}_{\mu \rho} T^\rho{}_{\beta \alpha}} \\
&=\frac{\partial}{\partial x^{\mu}} T^\alpha{}_{\beta \alpha}-\Gamma^\rho{}_{\beta \mu} T^\alpha{}_{\rho \alpha} .
\end{aligned}
$$
## Raising and lowering indices
We also note that the covariant derivative of the metric [[tensor fields in GR|tensor]] is zero, because it vanishes in locally inertial coordinates where $\Gamma^\mu{}_{\nu \lambda}$ and $\partial g_{\mu \nu} / \partial x^{\lambda}$ vanish, and a [[tensor fields in GR|tensor]], zero in one coordinate system, is zero in all systems. The same result can also be obtained directly.

$$
g_{\mu \nu ; \lambda}=0
$$

^covDerMetric

We can also show in the same way that the covariant derivatives of the other forms of the metric tensor also vanish, that is,
 
$$

g_{; \lambda}^{\mu \nu} =0 
$$

^CovDerInv

$$
\delta_{\nu ; \lambda}^{\mu} =0

$$

^CovDerId

It follows that the operations of covariant differentiation and raising and lowering indices commute; for example,
$$
\left(g^{\mu \nu} V_{\nu}\right)_{; \lambda}=g^{\mu \nu} V_{\nu ; \lambda}
$$

Note that this implies a non trivial identity, if we equate [[#^covDerivativeVector]] to $g^{\mu \alpha }\cdot$[[#^covDerCovector]]:

$$
\begin{align}

g^{\mu \nu} V_{\nu;\lambda}&=g^{\mu \nu}\pqty{\pdv{V_\nu}{x^\lambda}-\Gamma^\beta{}_{\lambda \nu}V_\beta}\\
&=g^{\mu \nu}\pqty{\pdv{}{x^\lambda}(g_{\nu \alpha}V^\alpha)-\Gamma^\beta{}_{\lambda \nu}g_{\beta \alpha}V^\alpha}\\
&=\delta^\mu_\nu \pdv{V^\alpha}{x^\lambda}+V^\alpha\pqty{g^{\mu \nu} \pdv{g_{\nu \alpha}}{x^\lambda}-\Gamma^\beta{}_{\lambda \nu}g^{\mu \nu}g_{\beta \alpha}}\\
&\stackrel{!}{=}V^\mu{}_{;\lambda}=\pdv{V^\mu}{x^\lambda}+\Gamma^\mu{}_{\lambda \alpha}V^\alpha

\end{align}

$$

$$\implies \Gamma^\mu{}_{\lambda \alpha}=g^{\mu \nu} \pdv{g_{\nu \alpha}}{x^\lambda}-\Gamma^\beta{}_{\lambda \nu}g^{\mu \nu}g_{\beta \alpha}$$

# Importance
The importance of covariant differentiation arises from two of its properties: It converts [[tensor fields in GR|tensors]] to other [[tensor fields in GR|tensors]], and it reduces to ordinary differentiation in the absence of gravitation, that is, when $\Gamma_{v \lambda}^{\mu}=0$. These properties suggest the following algorithm for assessing the effects of gravitation on physical systems:

Write the appropriate special-relativistic equations that hold in the absence of gravitation, replace $\eta_{\mu \nu}$ with $g_{\mu v}$, and replace all derivatives with covariant derivatives. The resulting equations will be generally invariant and true in the absence of gravitation, and therefore, according to the [[principle of equivalence|equivalence principle]], they will be true in the presence of gravitational fields, provided always that we work on a space-time scale sufficiently small compared with the scale of the gravitational field.

# Derived quantites

We can define:

- [[covariant curl]]
- [[covariant divergence]]


# Along a curve:

![[Pasted image 20220205161318.png#leftwrap|300]]Often we are interested in the properties of particles that are moving along a trajectoy in spacetime, which will then only be defined along this curve. Therefore, we want a covariant derivative for [[tensor fields in GR|tensors]] defined only on a curve, as opposed to everywhere in space.
For example, consider a quantity $\Pi^{\mu \nu \rho}(x(\tau))$ which is defined on a trajectory $x(\tau)$ through spacetime. How would we compute its derivative?
In classical mechanics we worked with $\vec{x}(t), \frac{\vec{x}(t+\delta t)-\vec{x}(t)}{\delta t}$, or in [[special relativity]] with $\vec{x}(\tau), t(\tau)$. An appropriate derivative for a vector $V^{\mu}\left(x^{\alpha}(\tau)\right)$ living on the trajectory was then
$$
\frac{\mathrm{d} V^{\mu}(\tau)}{\mathrm{d} \tau}
$$
Problem: This is not covariant!
We thus introduce the covariant derivative along a curve
$$
\frac{\mathrm{D} A^{\mu}}{\mathrm{D} \tau} \equiv \frac{\mathrm{d} A^{\mu}}{\mathrm{d} \tau}+\Gamma^\mu{}_{\nu \lambda} \frac{\mathrm{d} x^{\lambda}}{\mathrm{d} \tau} A^{\nu}(\tau)
$$

Similarly, we have
$$
\frac{\mathrm{D} A_{\mu}}{\mathrm{D} \tau} \equiv \frac{\mathrm{d} A_{\mu}}{\mathrm{d} \tau}-\Gamma^\lambda{}_{\mu \nu} \frac{\mathrm{d} x^{\nu}}{\mathrm{d} \tau} A_{\lambda}
$$
for a contravariant vector. The generalizations to covariant and contravariant indices on [[tensor fields in GR|tensors]] are analogous to the normal covariant derivative.
Exercise: Check that $\frac{\mathrm{d} A^{\mu}}{\mathrm{d} \tau}$ and $\frac{\mathrm{d} A_{\mu}}{\mathrm{d} \tau}$ are not vectors, but that $\frac{\mathrm{D} A^{\mu}}{\mathrm{D} \tau}$ is.

In general the **directional covariant derivative** is given by: 

$$\frac{D}{\dd{\lambda}}=\dv{x^\mu}{\lambda}\nabla_\mu$$