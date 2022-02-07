# Primary operators.
[[primary operator|^|]]s are a subclass of the [[quasi-primary operator]]s described above. An operator is called primary, if it satisfies the [[quasi-primary operator|quasi-primary]] conditions for all transformations

$$
(z, \bar{z}) \rightarrow\left(z^{\prime}(z), \bar{z}^{\prime}(\bar{z})\right) \quad \text { or } \quad(\delta z, \delta \bar{z})=(\epsilon(z), \bar{\epsilon}(\bar{z}))
$$

Infinitesimally, one finds

$$
\delta \mathcal{O}=(h \partial \epsilon \mathcal{O}+\epsilon \partial \mathcal{O})+(\bar{h} \bar{\partial} \bar{\epsilon} \mathcal{O}+\bar{\epsilon} \bar{\partial} \mathcal{O})
$$

Of course, the infinitesimal transformations above can be derived from the general rule here easily.

## [[Conformal Correlators]]

Correlators are locally [[conformal invariance|conformal invariant]]. Only a subclass of transformations (e.g. [[moebius transformation|Möbius]]) leaves the correlator globally invariant. As an example, consider

$$
\left\langle\mathcal{O}_{1}^{\mu} \mathcal{O}_{2}^{\nu}\right\rangle=\frac{-\frac{1}{2} \kappa^{2} \eta^{\mu \nu}}{\left(z_{1}-z_{2}\right)^{2}}
$$

built from the primary operator $\mathcal{O}^{\mu}=\partial X^{\mu}$ with [[conformal weight|weights]] $(h, \bar{h})=(1,0)$. The correlator is exactly invariant under the transformation $\delta z=z^{1-n}$, if $|n| \leq 1$ ([[moebius transformation]]), but invariant up to polynomials for $|n|>1$.

# From [[OPE]]

We use the same trick as for a [[local operator#From the operator product expansion OPE|local operator]], its [[conformal weight#From operator product expansion OPE|conformal weight]] and a [[quasi-primary operator#From operator product expansion OPE|quasi-primary operator]]. Using [[local operator#^d9edcd|Ward, residue]] and [[local operator#^d590f3|expanding the general TO OPE]] but considering  a general transformation $\epsilon(z)$ (thus $\delta \mathcal{O}=(h  \epsilon' \mathcal{O}+\epsilon \partial \mathcal{O})$), which we suppose has no poles and can be Taylor expanded: $\epsilon(z)=\epsilon(w)+\epsilon'(w)(z-w)+\dots$ we substitute: $$(h  \epsilon' \mathcal{O}+\epsilon \partial \mathcal{O})=\delta \mathcal{O} = \mathrm{Res}[\epsilon (z)T(z)\mathcal{O}]= \sum\limits_{n=0} \frac{\epsilon^{(n)}}{n!}\mathcal{O}_{n+1}$$ identifying terms on both sides we have $\partial \mathcal{O}=\mathcal{O}_1$, $h\mathcal{O}=\mathcal{O}_2$, $\mathcal{O}_j=0~\forall j>2$, i.e. we need to demand the absence of higher poles:

$$
T(z) \mathcal{O}(w, \bar{w})=\frac{h \mathcal{O}(w, \bar{w})}{(z-w)^{2}}+\frac{\partial \mathcal{O}(w, \bar{w})}{z-w}+\text{non singular}
$$

^b8595a
