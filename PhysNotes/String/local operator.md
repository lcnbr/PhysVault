---
alias:
- local operators
- field
tag: ST 
---

Under shifts $(\delta z, \delta \bar{z})=(\epsilon, \bar{\epsilon})$, all [[local operator|local operators]] transform as

$$
\begin{aligned}
\mathcal{O}(z+\epsilon, \bar{z}+\bar{\epsilon}) &=\mathcal{O}(z, \bar{z})+\epsilon \partial \mathcal{O}+\bar{\epsilon} \bar{\partial} \mathcal{O} \\
\delta \mathcal{O} &=\epsilon \partial \mathcal{O}+\bar{\epsilon} \bar{\partial}\overline{\mathcal{O}} .
\end{aligned}
$$
Thus shifting, we obtain the [[descendants]] $\partial^n\bar{\partial}^\bar{n}\mathcal{O}$.

Let’s first describe what we mean by a [[local operator]] in a [[conformal field theory|CFT]]. We will also refer to these objects as [[Field|fields]]. There is a slight difference in terminology between [[conformal field theory|CFTs]] and more general quantum field theories. Usually in quantum field theory, one reserves the term "field" for the objects $\phi$ which sit in the [[Action]] and are integrated over in the [[path integral]]. In contrast, in [[conformal field theory|CFT]] the term "[[local operator|field]]" refers to any local expression that we can write down. This includes $\phi$, but also includes derivatives $\partial^{n} \phi$ or composite operators such as $e^{i \phi}$. All of these are thought of as different fields in a [[conformal field theory|CFT]]. It should be clear from this that the set of all "fields" in a CFT is always infinite even though, if you were used to working with quantum field theory, you would talk about only a finite number of fundamental objects $\phi$. Obviously, this is nothing to be scared about. It's just a change of language: it doesn't mean that our theory got harder.

$\mathcal{O}_{i}(z, \bar{z})$, which are built from products of fields $X$ and their derivatives $\partial^{n} \partial^{n} X$, all of them evaluated at the same point $(z, \bar{z})$ on the [[Wick rotation#In conformal field theory CFT|worldsheet]]. The [[normal ordering]] $\mathcal{O}_{i}=\therefore \ldots$ is implicit for [[Local Operators]], thus there are no self-correlations. 
Typical examples are:
- $\mathcal{O}_{1}=:(\partial X)^{2}:$ 
- $\mathcal{O}_{2}^{\mu \nu}=: X^{\mu} \partial X^{\nu}:-: X^{\nu} \partial X^{\mu}:$

# From the [[operator product expansion|OPE]]

From the [[Ward identity]] and the [[residue theorem]] we obtained [[stress-energy tensor#^383bc0]] i.e. considering $J(z)=\epsilon(z)T(z)$ is the [[conserved current]] for the infinitesimal transformation $\delta z= \epsilon(z)$ we have:

$$\delta\mathcal{O}=\mathrm{Res}[J\mathcal{O}]=\mathrm{Res}[\epsilon(z)T(z)\mathcal{O}]$$ ^d9edcd

Supposing we can write a general (and suggestive of poles) form of the [[stress-energy tensor]] [[operator product expansion|OPE]]: $T(z)\mathcal{O}(w,\bar{w})=\sum\limits_i \frac{\mathcal{O}_i}{(z-w)^i}$ and considering a simple translation $\delta z=\epsilon, \delta \mathcal{O}=\epsilon \partial \mathcal{O}$: ^d590f3

$$\epsilon \partial \mathcal{O}=\delta \mathcal{O} = \mathrm{Res}[\epsilon T(z)\mathcal{O}]=\epsilon \mathcal{O}_{1}$$

Thus any local operator has the following  [[descendants|descendent]] simple pole:

$$
T(z) \mathcal{O}(w, \bar{w})=\ldots+\frac{\partial \mathcal{O}(w, \bar{w})}{z-w}+\ldots
$$

^2456a9
