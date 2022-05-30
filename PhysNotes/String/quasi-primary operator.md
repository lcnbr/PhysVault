---
alias:
- quasi-primary
- Quasi-Primary Operators
- quasi-primary operators
---
# Quasi-Primary Operators.
A [[local operator]] with [[conformal weight|weights]] $(h, \bar{h})$ is called quasi-primary if

$$
\mathcal{O}^{\prime}(z, \bar{z})=\left(\frac{\mathrm{d} z^{\prime}}{\mathrm{d} z}\right)^{h}\left(\frac{\mathrm{d} \bar{z}^{\prime}}{\mathrm{d} \bar{z}}\right)^{\bar{h}} \mathcal{O}\left(z^{\prime}, \bar{z}^{\prime}\right)
$$

for all [[moebius transformation|^|]]s


For infinitesimal boosts $\delta(z, \bar{z})=\left(\epsilon z^{2}, \bar{\epsilon} \bar{z}^{2}\right)$ it must satisfy

$$
\delta \mathcal{O}=\epsilon\left(2 h z \mathcal{O}+z^{2} \partial \mathcal{O}\right)+\bar{\epsilon}\left(2 \bar{h} \bar{z} \mathcal{O}+\bar{z}^{2} \bar{\partial} \mathcal{O}\right) .
$$

[[../math/descendants|^|]] of [[.md|quasi-primary operator]]s are not [[.md|quasi-primary]]. In a [[7 CFT/conformal field theory|CFT]] it is sufficient to deal with [[.md|quasi-primary operators]] only.


# From [[operator product expansion|OPE]]

We use the same trick as for a [[local operator#From the operator product expansion OPE|local operator]] and its [[conformal weight#From operator product expansion OPE|conformal weight]]. Using [[local operator#^d9edcd|Ward, residue]] and [[local operator#^d590f3|expanding the general TO OPE]] but considering  a [[conformal group#Wick rotation In conformal field theory CFT Wick rotated|boost]] $\delta z=\epsilon z^{2}, \delta \mathcal{O}=$ $\epsilon\left(2 h z \mathcal{O}+z^{2} \partial \mathcal{O}\right)$ and substituting:
$$\epsilon\left(2 h z \mathcal{O}+z^{2} \partial \mathcal{O}\right)=\delta \mathcal{O} = \mathrm{Res}[\epsilon z^2T(z)\mathcal{O}]=\mathrm{Res}[\epsilon \sum\limits_i \frac{\mathcal{O}_i}{(z-w)^{i-2}}]=\epsilon \mathcal{O}_3$$we need to require the absence of the cubic pole:

$$
T(z) \mathcal{O}(w, \bar{w})=\sum\limits_{i\in \mathbb{Z}} \frac{\mathcal{O}_i}{(z-w)^i}=\frac{0}{(z-w)^{3}}+\frac{2h \mathcal{O}(w, \bar{w})}{(z-w)^{2}}+\frac{\partial \mathcal{O}(w, \bar{w})}{z-w}+\sum\limits_{i\neq3} \frac{\mathcal{O}_i}{(z-w)^i}
$$


Additionally we have that the first and second pole are necessarily the ones we already have (c.f. [[local operator#^2456a9]] and [[conformal weight#^70ef67]]) thus: 

$$
T(z) \mathcal{O}(w, \bar{w})=\sum\limits_{i\neq3} \frac{\mathcal{O}_i}{(z-w)^i}=\ldots+\frac{0}{(z-w)^{3}}+\frac{h \mathcal{O}(w, \bar{w})}{(z-w)^{2}}+\frac{\partial \mathcal{O}(w, \bar{w})}{z-w}+\ldots
$$


^70ef67

A [[.md|quasi-primary operator]] is *characterised* by the absence of a third order pole in the [[OPE]] with the [[stress-energy tensor]].

