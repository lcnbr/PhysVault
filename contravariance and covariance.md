---
alias:
- contravariant
- covariant
- covariantly
- contravariantly
Tag: GR physics math
---
 ![](https://upload.wikimedia.org/wikipedia/commons/thumb/7/72/Covariantcomponents.gif/390px-Covariantcomponents.gif)
 Consider two bases or a vector space, $\qty{e_i}=\mathcal{B}$ and $\qty{e'_i}=\mathcal{B'}$, then an element $v$ of the vector space can be written out in components:
 $$v=[v]^{\mathcal{B}:i}[e_i]_\mathcal{B}=v^i e_{(i)}=[v]^{\mathcal{B'}:i}[e'_i]_\mathcal{B'}=(v^i)'e'_{(i)}
 $$

 Now if we denote the change of basis: $$[e'_i]_\mathcal{B'}= [\mathbb{1}]_\mathcal{B'}{}^\mathcal{B}[e_i]_\mathcal{B}$$
 Then the first equality becomes:
 
 $$[v]^{\mathcal{B}:i}[e_i]_\mathcal{B}=[v]^{\mathcal{B'}:i}[e'_i]_\mathcal{B'}=[v]^{\mathcal{B'}:i}[\mathbb{1}]_\mathcal{B'}{}^\mathcal{B}[e_i]_\mathcal{B}
 $$

 We cancel out $[e_i]_\mathcal{B}$ on both sides and multiply by the inverse of the change of basis: $[\mathbb{1}]^\mathcal{B'}{}_\mathcal{B}$:
 $$[\mathbb{1}]^\mathcal{B'}{}_\mathcal{B}[v]^{\mathcal{B}}=[v]^{\mathcal{B'}}
 $$

Now we say the components of $v$ are changing contravariantly. For a [[general coordinate transformation]], the change of basis is given by: 

$$\pdv{x^\mu}{x'^\rho}$$

^coordChang

and its inverse is :

$$\pdv{x'^\rho}{x^\mu}$$ 

^coordInv

Thus a contravariant object $V^\mu$ changes with the [[#^coordInv|inverse]] of the basis change under a [[general coordinate transformation]]:

$$V'^\mu =V^\rho\pdv{x'^\mu }{x^\rho}$$

^contra

For example the dual basis, the differentials/one-forms change in this way:
 
$$\dd{x^\mu}\rightarrow \dd{x'^\mu}=\pdv{x'^\mu}{x^\rho}\dd{x^\rho}$$
Now there always is an associated dual basis defined by:

 $$e^{i}e_j=\delta^i_j$$
 In component vectors this equality is:

 $$[e^i]^\mathcal{B}[e_j]_\mathcal{B}$$
 Now changing the basis we have:
 $$[e^i]^\mathcal{B}[\mathbb{1}]_\mathcal{B}{}^\mathcal{B'}[e'_j]_\mathcal{B'}$$
 Which implies that the dual basis changes as:

 $$[e'^i]^\mathcal{B'}=[e^i]^\mathcal{B}[\mathbb{1}]_\mathcal{B}{}^\mathcal{B'}=[\mathbb{1}]^\mathcal{B'}{}_\mathcal{B}[e^i]^\mathcal{B}$$

 An element of the dual space is written in components:
 $$\alpha=[\alpha]_{\mathcal{B}:i}[e^i]^\mathcal{B}=[\alpha]_{\mathcal{B'}:i}[e'^ i]^\mathcal{B'}$$
 An using the change of basis we have:

 $$\alpha=[\alpha]_{\mathcal{B}:i}[e^i]^\mathcal{B}=[\alpha]_{\mathcal{B'}:i}[e'^ i]^\mathcal{B'}=[\alpha]_{\mathcal{B'}:i}[\mathbb{1}]^\mathcal{B'}{}_\mathcal{B}[e^i]^\mathcal{B}$$

 As before, we cancel the $[e^i]^\mathcal{B}$ on both sides and multiply by the change of basis $[\mathbb{1}]_\mathcal{B'}{}^\mathcal{B}$:

 $$[\alpha]_{\mathcal{B'}}=[\mathbb{1}]_\mathcal{B'}{}^\mathcal{B}[\alpha]_\mathcal{B}$$

 An obvious example is the original basis $\qty{e_i}$! And the coordinate basis, the directional derivatives changes in this way: 

 $$\pdv{}{x^\mu}\rightarrow\pdv{}{x'^\mu}=\pdv{x^\rho}{x'^\mu}\pdv{}{x^\rho}$$

 Thus a covariant object $U_\mu$ changes with the [[#^coordChang|basis change]] under a [[general coordinate transformation]]:
 
$$U'_\mu =U_\rho\pdv{x^\rho }{x'^\mu}$$

^cov
