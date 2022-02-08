---
alias:
tags:
- qftII
---
Expansion. Consider the standard massive scalar bubble integral
![[Pasted image 20220127075611.png|150]]
$$
\begin{aligned}
&=\frac{\mu^{2 \epsilon}}{2} \int \frac{-i \mathrm{~d} \ell^{D}}{(2 \pi)^{D}} \frac{1}{\ell^{2}+m^{2}-i \epsilon} \frac{1}{(p-\ell)^{2}+m^{2}-i \epsilon} \\
&=\frac{\mu^{2 \epsilon}}{2} \int_{0}^{1} \mathrm{~d} z \int \frac{-i \mathrm{~d} \ell^{D}}{(2 \pi)^{D}} \frac{1}{\left(\ell^{2}+z \bar{z} p^{2}+m^{2}-i \epsilon\right)^{2}} .
\end{aligned}
$$
In the second step we have combined the denominators and shifted the integration variable to centre the integrand. The integral has the desired form and we use the [[basic integral#^5ee300|dimensionally regularised expression]] with [[basic integral#^098603]] and  [[basic integral#^9eb6e0]]] and [[introducing a scale#^3e7665]]
$$
I=\frac{\Gamma(\epsilon)}{32 \pi^{2}} \int_{0}^{1} \mathrm{~d} z\left(\frac{z \bar{z} p^{2}+m^{2}-i \epsilon}{4 \pi \mu^{2}}\right)^{-\epsilon} .
$$
Next we expand the integrand in $\epsilon$
$$
I=\frac{1}{32 \pi^{2}} \int_{0}^{1} \mathrm{~d} z\left(\frac{1}{\epsilon}-\gamma_{\mathrm{E}}-\log \frac{z \bar{z} p^{2}+m^{2}-i \epsilon}{4 \pi \mu^{2}}+\mathcal{O}(\epsilon)\right)
$$
We have performed the relevant parts of this integral in QFT I, here we obtain
$$
\begin{aligned}
I=&-\frac{1}{16 \pi^{2}} \sqrt{\frac{p^{2}+4 m^{2}-i \epsilon}{-p^{2}}} \arctan \sqrt{\frac{-p^{2}}{p^{2}+4 m^{2}-i \epsilon}} \\
&+\frac{1}{32 \pi^{2}}\left(\frac{1}{\epsilon}-\gamma_{\mathrm{E}}+\log (4 \pi)+2-\log \frac{m^{2}}{\mu^{2}}\right)+\mathcal{O}(\epsilon) .
\end{aligned}
$$
The dimensional regularisation agrees with the cut-off scheme up to terms of order $\epsilon$ and up to some constant shifts. The constant shifts can actually be absorbed by an appropriate change of the renormalisation scale $\mu$. Alternatively, they can be cancelled directly by counterterms. One of these shift terms is a pole at $\epsilon=0$ which indicates the divergence in $D=4$. Such poles are typical for dimensional regularisation.

We have terminated the expansion at $\epsilon^{0}$. This makes sense since we are mainly interested in the physics in $D=4$. What about the terms at positive orders of $\epsilon$ ? Are they relevant? Yes and no!
- Some of the sub-leading terms in $\epsilon$ are required even at $D=4$. This is the case whenever there are divergences in the Feynman diagram that can undo the suppression of $\mathcal{O}(\epsilon)$ terms.
- The higher-order terms in $\epsilon$ typically have a more complicated structure which is reminiscent of higher-loop contributions. In fact they compete with higher-loop terms and all terms are necessary to construct a consistent final result.
- After all divergences have been removed, we will eventually set $\epsilon=0$ and thus drop these terms.
- **Note that setting $\epsilon=0$ too early may discard some essential terms from the final answer and make it inconsistent**. For example, the external states in a scattering process are usually defined in $D=4$. However, this may lead to violations of unitarity since it is conceivable that the corresponding integrals over the phase space of intermediate particles diverge. In those cases, the difference between a simplified phase space with $D=4$ and the actual phase space with $D=4-2 \epsilon$ may be important.