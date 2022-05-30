# Stress-Energy Tensor

Is defined as the matrix of [[conserved currents]] which arise from translational invariance,
$$
\delta \xi^{\alpha}=\epsilon^{\alpha} .
$$
In [[Minkowski space|flat spacetime]], a translation is a special case of a [[conformal group|conformal transformation]]. Suppose for the moment that we are in flat space $g_{\alpha \beta}=\eta_{\alpha \beta}$. Recall that we can usually derive conserved currents by promoting the constant parameter $\epsilon$ that appears in the symmetry to a function of the spacetime coordinates. The change in the action must then be of the form,
$$
\delta S=\int d^{2} \sigma J^{\alpha} \partial_{\alpha} \epsilon
$$
for some function of the fields, $J^{\alpha}$. This ensures that the variation of the action vanishes when $\epsilon$ is constant, which is of course the definition of a symmetry. But when the equations of motion are satisfied, we must have $\delta S=0$ for all variations $\epsilon(\sigma)$, not just constant $\epsilon$. This means that when the equations of motion are obeyed, $J^{\alpha}$ must satisfy
$$
\partial_{\alpha} J^{\alpha}=0
$$
The function $J^{\alpha}$ is our conserved current.
Let's see how this works for translational invariance. If we promote $\epsilon$ to a function of the [[worldsheet]] variables, the change of the action must be of the form (4.3). But what is $J^{\alpha}$ ? At this point we do the cute thing. Consider the same theory, but now coupled to a dynamical background metric $g_{\alpha \beta}(\sigma)$. In other words, coupled to gravity. Then we could view the transformation
$$
\delta \sigma^{\alpha}=\epsilon^{\alpha}(\sigma)
$$
as a diffeomorphism and we know that the theory is invariant as long as we make the corresponding change to the metric
$$
\delta g_{\alpha \beta}=\partial_{\alpha} \epsilon_{\beta}+\partial_{\beta} \epsilon_{\alpha} .
$$
This means that if we just make the transformation of the coordinates in our original theory, then the change in the action must be the opposite of what we get if we just transform the metric. (Because doing both together leaves the action invariant). So we have
$$
\delta S=-\int d^{2} \sigma \frac{\partial S}{\partial g_{\alpha \beta}} \delta g_{\alpha \beta}=-2 \int d^{2} \sigma \frac{\partial S}{\partial g_{\alpha \beta}} \partial_{\alpha} \epsilon_{\beta}
$$
Note that $\partial S / \partial g_{\alpha \beta}$ in this expression is really a functional derivatives but we won't be careful about using notation to indicate this. We now have the conserved current arising from translational invariance. We will add a normalization constant which is standard in string theory (although not necessarily in other areas) and define the stress-energy tensor to be
$$
T_{\alpha \beta}=-\frac{4 \pi}{\sqrt{g}} \frac{\partial S}{\partial g^{\alpha \beta}}
$$

^4db480

If we have a flat [[worldsheet]], we evaluate $T_{\alpha \beta}$ on $g_{\alpha \beta}=\delta_{\alpha \beta}$ and the resulting expression obeys $\partial^{\alpha} T_{\alpha \beta}=0$. If we're working on a curved [[worldsheet]], then the energy-momentum tensor is covariantly conserved, $\nabla^{\alpha} T_{\alpha \beta}=0$.

The Noether currents for spacetime symmetries are encoded in the conserved stress-energy tensor $T_{\alpha \beta}$

$$
T_{\alpha \beta}=-\frac{1}{4 \pi \kappa^{2}}\left(\left(\partial_{\alpha} X\right) \cdot\left(\partial_{\beta} X\right)-\frac{1}{2} \eta_{\alpha \beta} \eta^{\gamma \delta}\left(\partial_{\gamma} X\right) \cdot\left(\partial_{\delta} X\right)\right)
$$

The stress-energy tensor is an object of central importance for [[7 CFT/conformal field theory|CFT]] and its [[operator product expansion|OPE]] will allow to characterize operators.
# Tracelessness in a [[7 CFT/conformal field theory|CFT]]
The Stress-Energy Tensor is Traceless
In conformal theories, $T_{\alpha \beta}$ has a very important property: its trace vanishes. To see this, let's vary the action with respect to a [[conformal group#^8c03fe|scale transformation]] which is a special case of a [[conformal group|conformal transformation]],
$$
\delta g_{\alpha \beta}=\epsilon g_{\alpha \beta}
$$
Then we have using [[#^4db480]]
$$
\delta S=\int d^{2} \sigma \frac{\partial S}{\partial g_{\alpha \beta}} \delta g_{\alpha \beta}=-\frac{1}{4 \pi} \int d^{2} \sigma \sqrt{g} \epsilon T_{\alpha}^{\alpha}
$$
But this must vanish in a conformal theory because scaling transformations are a symmetry. So
$$
T_{\alpha}^{\alpha}=0
$$
This is the key feature of a conformal field theory in any dimension. Many theories have this feature at the classical level, including Maxwell theory and Yang-Mills theory in four-dimensions. However, it is much harder to preserve at the quantum level. (The weight of the world rests on the fact that Yang-Mills theory fails to be conformal at the quantum level). Technically the difficulty arises due to the need to introduce a scale when regulating the theories. Here we will be interested in two-dimensional theories which succeed in preserving the [[conformal invariance|conformal symmetry]] at the quantum level.

We know that the trace is exactly zero because of [[Weyl invariance|Weyl symmetry]]. On the [[worldsheet]], the two remaining components $T_{\mathrm{LL}}$ and $T_{\mathrm{RR}}$ translate into the euclidean quantities

$$
T=-\frac{1}{\kappa^{2}}(\partial X)^{2}, \quad \bar{T}=-\frac{1}{\kappa^{2}}(\bar{\partial} \bar{X})^{2} .
$$

(Let us ignore the string physical state condition which eventually sets them to zero, $T=\bar{T}=0$.)

# The Stress-Tensor in [[Wick rotation#In conformal field theory CFT|Complex Coordinates]]
In [[Wick rotation#In conformal field theory CFT|Complex Coordinates]], the vanishing of the trace $T_{\alpha}^{\alpha}=0$ becomes
$$
T_{z \bar{z}}=0
$$
Meanwhile, the conservation equation $\partial_{\alpha} T^{\alpha \beta}=0$ becomes $\partial T^{z z}=\bar{\partial} T^{z \bar{z}}=0$. Or, lowering the indices on $T$,
$$
\bar{\partial} T_{z z}=0 \quad \text { and } \quad \partial T_{\bar{z} \bar{z}}=0
$$
In other words, $T_{z z}=T_{z z}(z)$ is a holomorphic function while $T_{\bar{z} \bar{z}}=T_{\bar{z} \bar{z}}(\bar{z})$ is an antiholomorphic function. We will often use the simplified notation
$$
T_{z z}(z) \equiv T(z) \text { and } T_{\bar{z} \bar{z}}(\bar{z}) \equiv \bar{T}(\bar{z})
$$


# Noether Currents
The stress-energy tensor $T_{\alpha \beta}$ provides the Noether currents for translations. What are the currents associated to the other conformal transformations? Consider the infinitesimal change,
$$
z^{\prime}=z+\epsilon(z), \quad \bar{z}^{\prime}=\bar{z}+\bar{\epsilon}(\bar{z})
$$
where, making contact with the two examples above, constant $\epsilon$ corresponds to a translation while $\epsilon(z) \sim z$ corresponds to a rotation and dilatation. To compute the current, we'll use the same trick that we saw before: we promote the parameter $\epsilon$ to depend on the [[worldsheet]] coordinates. But it's already a function of half of the [[worldsheet]] coordinates, so this now means $\epsilon(z) \rightarrow \epsilon(z, \bar{z})$. Then we can compute the change in the action, again using the fact that we can make a compensating change in the metric,
$$
\begin{aligned}
\delta S &=-\int d^{2} \sigma \frac{\partial S}{\partial g^{\alpha \beta} \delta g^{\alpha \beta}} \\
&=\frac{1}{2 \pi} \int d^{2} \sigma T_{\alpha \beta}\left(\partial^{\alpha} \delta \sigma^{\beta}\right) \\
&=\frac{1}{2 \pi} \int d^{2} z \frac{1}{2}\left[T_{z z}\left(\partial^{z} \delta z\right)+T_{\bar{z} \bar{z}}\left(\partial^{\bar{z}} \delta \bar{z}\right)\right] \\
&=\frac{1}{2 \pi} \int d^{2} z\left[T_{z z} \partial_{\bar{z}} \epsilon+T_{\bar{z} \bar{z}} \partial_{z} \bar{\epsilon}\right]
\end{aligned}
$$

Firstly note that if $\epsilon$ is holomorphic and $\bar{\epsilon}$ is anti-holomorphic, then we immediately have $\delta S=0$. This, of course, is the statement that we have a symmetry on our hands. (You may wonder where in the above derivation we used the fact that the theory was conformal. It lies in the transition to the third line where we needed $\left.T_{z \bar{z}}=0\right)$.

At this stage, let's use the trick of treating $z$ and $\bar{z}$ as independent variables. We look at separate currents that come from shifts in $z$ and shifts $\bar{z}$. Let's first look at the symmetry
$$
\delta z=\epsilon(z) \quad, \quad \delta \bar{z}=0
$$
We can read off the conserved current from (4.6) by using the standard trick of letting the small parameter depend on position. Since $\epsilon(z)$ already depends on position, this means promoting $\epsilon \rightarrow \epsilon(z) f(\bar{z})$ for some function $f$ and then looking at the $\bar{\partial} f$ terms in (4.6). This gives us the current
$$
J^{z}=0 \quad \text { and } \quad J^{\bar{z}}=T_{z z}(z) \epsilon(z) \equiv T(z) \epsilon(z)
$$
Importantly, we find that the current itself is also holomorphic. We can check that this is indeed a conserved current: it should satisfy $\partial_{\alpha} J^{\alpha}=\partial_{z} J^{z}+\partial_{\bar{z}} J^{\bar{z}}=0 .$ But in fact it does so with room to spare: it satisfies the much stronger condition $\partial_{\bar{z}} J^{\bar{z}}=0$.

Similarly, we can look at transformations $\delta \bar{z}=\bar{\epsilon}(\bar{z})$ with $\delta z=0$. We get the antiholomorphic current $\bar{J}$,
$$
\bar{J}^{z}=\bar{T}(\bar{z}) \bar{\epsilon}(\bar{z}) \quad \text { and } \quad \bar{J}^{\bar{z}}=0
$$




# Conservation. 
The current $J(z)=\epsilon(z) T(z)$ corresponds to the infinitesimal transformation $\delta z=\epsilon(z)$. While classical conservation $\bar{\partial} J=0$ is ensured by means of the e.o.m., in quantum mechanics the conservation law is implied by the Ward identity:

$$
\bar{\partial} J(z) \mathcal{O}(w, \bar{w})=2 \pi \delta^{2}(z-w, \bar{z}-\bar{w}) \delta \mathcal{O}(w, \bar{w}) .
$$

Thus, the current $J(z)$ is conserved everywhere except at the operator locations.

In order to calculate the [[operator product expansion|OPE]] between the current and an operator, one has to capture the contribution from lack of conservation of the current at the operator location. This is implemented mathematically by integrating $z$ around a small circle centered at $w$ :

$$
\frac{1}{2 \pi} \int_{|z-w|<\epsilon} \mathrm{d} z^{2} \ldots
$$

In a first step, let us evaluate the integration over $\bar{z}\left(\int \mathrm{d} z^{2} \bar{\partial} \ldots=-i \int \mathrm{d} z \ldots\right)$ and obtain

$$
\begin{aligned}
\operatorname{Res}\left[J_{z} \mathcal{O}_{1}\right]=&\frac{1}{2 \pi i} \oint_{\partial \epsilon} \mathrm{d} z~ J_{z}(z) \mathcal{O}_{1}\left(\sigma_{1}\right)\\
=& \frac{1}{2 \pi i} \int_{|z-w|=\epsilon} \mathrm{d} z~ J(z) \mathcal{O}(w, \bar{w}) \\
=& \frac{1}{2 \pi i} \int_{|z-w|=\epsilon} \mathrm{d} z ~\ \epsilon(z) T(z) \mathcal{O}(w, \bar{w}) \\
=& \delta \mathcal{O}(w, \bar{w}) .
\end{aligned}
$$

^383bc0

In summary: [[conformal transformations]] are transformations $\delta z=\epsilon(z)$. The (holomorphic) function $\epsilon(z)$ gives rise to currents $J(z)=\epsilon(z) T(z)$ which are conserved except at the operator locations. At the operator locations, the failure of conservation of the current $J(z)$ quantifies the transformation properties of the respective operator. 

# Stress-Energy [[operator product expansion|OPE]]. 
In the last paragraph of this chapter, we would like to derive the [[operator product expansion|OPE]] of an [[local operator|operator]] $\mathcal{O}$ and the stress-energy tensor $T$. So let us consider the previous equation for several types of infinitesimal transformations.

- [[local operator#From the operator product expansion OPE|For any local operator we have]]:![[local operator#^2456a9]]
Further terms with higher poles and polynomials in "..." are unconstrained from considering just infinitesimal translations. 
- For an operator $\mathcal{O}$ of [[conformal weight|holomorphic weight]] $h$ [[conformal weight#From operator product expansion OPE|we have]]:![[conformal weight#^70ef67]]
- For a [[quasi-primary operator#From operator product expansion OPE]] we have:![[quasi-primary operator#^70ef67]]
- For a [[primary operator#From OPE|primary operator]] we have: ![[primary operator#^b8595a]]
- When there is a derivative acting on an operator, the poles are shifted by one order. Thus, [[../math/descendants]] are not ([[quasi-primary operator|quasi-]])[[primary operator]]s.

Let us state the [[operator product expansion|OPE]] of the stress-energy tensor. An explicit computation using [[Wick's theorem]] yields:

$$
T(z) T(w)=\frac{c / 2}{(z-w)^{4}}+\frac{2 T(w)}{(z-w)^{2}}+\frac{\partial T(w)}{z-w}+\ldots .
$$

This is a general result in [[7 CFT/conformal field theory|CFT]]'s. It encodes the Virasoro algebra! Let us note a couple of properties of the stress-energy tensor:

- $T$ is a [[local operator]],
- $T$ has holomorphic weight $h=2$ (classically),
- $T$ is [[quasi-primary operator|quasi-primary]],
- $T$ is not [[primary operator|primary]] (unless $c=0$ ),
- the quartic pole carries central charge $c=D$.

[[conformal transformations]] for the stress-energy tensor $T$ are almost primary:

$$
\begin{aligned}
\delta T &=\delta z \partial T+2 \partial \delta z T+\frac{c}{12} \partial^{3} \delta z, \\
T^{\prime}(z) &=\left(\frac{\mathrm{d} z^{\prime}}{\mathrm{d} z}\right)^{2}\left(T\left(z^{\prime}\right)+\frac{c}{12} S\left(z^{\prime}, z\right)\right), \\
S\left(z^{\prime}, z\right) &=\left(\frac{\mathrm{d}^{3} z^{\prime}}{\mathrm{d} z^{3}}\right)\left(\frac{\mathrm{d} z^{\prime}}{\mathrm{d} z}\right)^{-1}-\frac{3}{2}\left(\frac{\mathrm{d}^{2} z^{\prime}}{\mathrm{d} z^{2}}\right)^{2}\left(\frac{\mathrm{d} z^{\prime}}{\mathrm{d} z}\right)^{-2} .
\end{aligned}
$$

The additional term $S$ is the Schwarzian derivative, which vanishes for [[moebius transformation|Möbius transformations]].