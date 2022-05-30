---
alias:
- weight
- weights
- conformal weights
---
# Conformal weight
Most [[local operator]]s (notable exception: $X$ ) are classified by their weights $(h, \bar{h})$. Considering a [[conformal group#Wick rotation In conformal field theory CFT Wick rotated|scaling/rotation]], one finds for $s,\epsilon \in \mathbb{C}$:

$$
\begin{aligned}
\mathcal{O}^{\prime}(z, \bar{z}) &=s^{h} \bar{s}^{\bar{h}} \mathcal{O}(s z, \bar{s} \bar{z}), \\
\delta \mathcal{O} &=\epsilon(h \mathcal{O}+z \partial \mathcal{O})+\bar{\epsilon}(\bar{h} \mathcal{O}+\bar{z} \bar{\partial} \mathcal{O}) .
\end{aligned}
$$
The terms $\partial \mathcal{O}$ in this expression would be there for any operator. They simply come from expanding $\mathcal{O}(z-\epsilon z, \bar{z}-\bar{\epsilon} \bar{z})$. The terms $h \mathcal{O}$ and $\bar{h} \mathcal{O}$ are special to operators which are eigenstates of dilatations and rotations. Some comments:
- Both $h$ and $\bar{h}$ are real numbers. 
- The weights are not as unfamiliar as they appear. They simply tell us how operators transform under rotations and scalings.  

    - The eigenvalue under rotation is usually called the *conformal spin*, $s$, and is given in terms of the weights as$$s=h-\bar{h}$$
    
    ^confspin
    - Meanwhile, the *scaling dimension* $\Delta$ of an operator is $$\Delta=h+\bar{h}$$ ^scaleingdim


# [[Unitary]] [[7 CFT/conformal field theory|CFT]]
For a unitary [[7 CFT/conformal field theory|CFT]] (physical, as the probabilistic interpretation yields conserved probabilities and add up to one), both $h$ and $\bar{h}$ have to be real and non-negative. Here are two examples of weights for some fields:
- $\partial X \rightarrow(1,0)$ 
- $(\partial X)^{2} \rightarrow(2,0)$. 
- The field $X$ does not have proper weights.

# Product
[[.md|Weight]] of the products of [[local operator]]s $\mathcal{O}=\mathcal{O}_{1} \mathcal{O}_{2}$ will be:

- In classical theory, the sum of individual weights. 
- In a quantum theory, weights are usually not additive, due to implicit normal ordering.

# From [[operator product expansion|OPE]]

We use the same trick as for any [[local operator#From the operator product expansion OPE|local operator]]. Using [[local operator#^d9edcd|Ward, residue]] and [[local operator#^d590f3|expanding the general TO OPE]] but considering a [[conformal group#Wick rotation In conformal field theory CFT Wick rotated|scaling]]  $\delta z=\epsilon z, \delta \mathcal{O}=\epsilon(h \mathcal{O}+z \partial \mathcal{O})$ we have:$$\epsilon(h \mathcal{O}+z \partial \mathcal{O})=\delta \mathcal{O} = \mathrm{Res}[\epsilon zT(z)\mathcal{O}]=\mathrm{Res}[\epsilon \sum\limits_i \frac{\mathcal{O}_i}{(z-w)^{i-1}}]=\epsilon \mathcal{O}_2$$nthus one needs to require at least a second order pole:

$$
T(z) \mathcal{O}(w, \bar{w})=\sum\limits_{i\in \mathbb{Z}} \frac{\mathcal{O}_i}{(z-w)^i}=\frac{h \mathcal{O}(w, \bar{w})}{(z-w)^{2}}+\frac{\partial \mathcal{O}(w, \bar{w})}{z-w}+\sum\limits_{i\neq2} \frac{\mathcal{O}_i}{(z-w)^i}
$$

Additionally we have the first order pole is necessarily the one we already have (c.f. [[local operator#^2456a9]]) thus: 

$$
T(z) \mathcal{O}(w, \bar{w})=\frac{h \mathcal{O}(w, \bar{w})}{(z-w)^{2}}+\frac{\partial \mathcal{O}(w, \bar{w})}{z-w}+\sum\limits_{i\neq\{1,2\}} \frac{\mathcal{O}_i}{(z-w)^i}
$$

^70ef67

The [[.md|conformal weight]] can be read off the [[stress-energy tensor#Stress-Energy operator product expansion OPE|T OPE]]'s second order pole!