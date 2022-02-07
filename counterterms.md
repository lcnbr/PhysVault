---
alias:
tags:
- qftII
---
Consider the dimensionally regulated [[massive scalar bubble]] integral
$$
I=\ldots+\frac{1}{32 \pi^{2}}\left(\frac{1}{\epsilon}-\gamma_{\mathrm{E}}+\log (4 \pi)+2-\log \frac{m^{2}}{\mu^{2}}\right)+\mathcal{O}(\epsilon) .
$$
In a scalar field theory with quartic interactions it can arise as the one-loop correction to the quartic interaction. When cubic interactions are included it also serves as a one-loop correction to the cubic interaction and to the kinetic term, specifically to the mass.

These three correction terms have a simple pole at $\epsilon=0$. We can remove the divergences by adding counterterms for the quartic interaction, the cubic interaction and the mass. Specifically, let us consider the quartic coupling and its divergent one-loop corrections in the [[effective action]] 
![[Pasted image 20220127081240.png|400]]
which yields
$$
-i \bar{\lambda}+i \bar{\lambda}^{2} I(s)+i \bar{\lambda}^{2} I(t)+i \bar{\lambda}^{2} I(u)+\ldots
$$
A suitable relationship between the renormalised quartic coupling constant $\lambda$ and the bare coupling $\bar{\lambda}=\bar{\lambda}_{\mathrm{MS}}$ is
$$
\bar{\lambda}_{\mathrm{MS}}=\lambda+\frac{3 \lambda^{2}}{32 \pi^{2} \epsilon}+\mathcal{O}\left(\lambda^{3}\right) .
$$
This counterterm removes precisely the $1 / \epsilon$ term in the above integral. Effectively, it changes the regularised integral to the subtracted integral $I_{\mathrm{MS}}=I-1 / 32 \pi^{2} \epsilon$
$$
I_{\mathrm{MS}}=\ldots+\frac{1}{32 \pi^{2}}\left(-\gamma_{\mathrm{E}}+\log (4 \pi)+2-\log \frac{m^{2}}{\mu^{2}}\right)+\mathcal{O}(\epsilon) .
$$
In terms of diagrams the divergent loop has a counterterm that makes it perfectly finite
![[Pasted image 20220127081528.png|300]]

This result can be generalised to a method of constructing minimal counterterms proportional to pole term $1 / \epsilon$. In the dimensionally regularised integrals this removes all corresponding poles $1 / \epsilon$ and makes them finite. The method is called the minimal subtraction (MS) scheme. At one loop it can be conveniently implemented at the level of regularised integrals by simply discarding the $1 / \epsilon$ terms.
Inspection of many cases makes obvious that each pole $1 / \epsilon$ is accompanied by an Euler constant $-\gamma_{\mathrm{E}}$ and a logarithm $\log (4 \pi)$. Importantly they all arise in the universal combination $1 / \epsilon-\gamma_{E}+\log (4 \pi) .$ It is therefore convenient to modify the scheme to that counterterms are proportional to this combination.
$$
\bar{\lambda}_{\overline{\mathrm{MS}}}=\lambda+3 \lambda^{2} \frac{1 / \epsilon-\gamma_{\mathrm{E}}+\log (4 \pi)}{32 \pi^{2}}+\mathcal{O}\left(\lambda^{3}\right) .
$$
This scheme is called MS-bar, and it is the scheme commonly applied in conjunction with dimensional regularisation. The subtraction of the above integral reads
$$
I_{\overline{\mathrm{MS}}}=\ldots+\frac{1}{32 \pi^{2}}\left(2-\log \frac{m^{2}}{\mu^{2}}\right)+\mathcal{O}(\epsilon)
$$
Finally, one could also choose to remove more terms of the integral such as the integer 2 or the term $\log \left(m^{2} / \mu^{2}\right)$. However, these terms are not universal in the sense that they may appear with different coefficients in different loop integrals. Note that the redefinition of the coupling constant must be independent of the momenta. In other words, merely shifts of the integrals are permissible, but the kinematical dependence (hidden in the above expressions) remains unchanged.

Another important observation is that the above choices of counterterms are related by a change of the renormalisation scale. For instance, using the renormalisation scale $\mu_{\overline{\mathrm{MS}}}$ in the MS scheme with
$$
\mu_{\overline{\mathrm{MS}}}=\frac{\exp \left(\frac{1}{2} \gamma_{\mathrm{E}}\right)}{\sqrt{4 \pi}} \mu
$$
is equivalent to the MS-bar scheme with renormalisation scale $\mu$. Hence, there is no physical significance to the constant $\mu$. Nevertheless, the operation of changing the renormalisation scale $\mu$ has important physical consequences as we shall discuss later.