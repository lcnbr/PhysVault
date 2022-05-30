---
aliases: 
tags: 
sources:
date created: Monday, May 23rd 2022, 11:07:54 am
date modified: Wednesday, May 25th 2022, 3:50:37 pm
---
$\newcommand{\rKernAA}[1]{\overline{\mathcal{I}_\text{r}'}(#1)}$
$\newcommand{\vKernAA}[1]{\overline{\mathcal{I}_\text{v}'}(#1)}$
$\newcommand{\cutint}{\mathrlap{\displaystyle\int\limits_X}\mathrlap{\textstyle\sum}\hspace{1em}}$
$\newcommand{\euler}{\mathsf{e}}$
$\newcommand{\elchrg}{e}$
Let us use the [[KMOC framework]] for [[scalar QED]] 

$$\Delta O=\AAngle{\int \d {\overline{\Psi}(\bar{q})}\exp\par[\big]{-\iunit\bar{q}^\mu b_\mu}\par[\Big]{\vKernAA{O}+\rKernAA{O}}}  $$

Let us take $p_\mu^1$ as the observable corresponding to the momentum of the first particle.

We then have:

$$
\begin{aligned}
\vKernAA{p_\mu^1}&=\hbar^2\iunit\,  q\, \mathcal{A}(p_1,p_2 \to p_1+\hbar \bar{q},p_2-\hbar \bar{q})\\
\rKernAA{p_\mu^1}&=\hbar^2\cutint\ddP[2+\abs{X}]{r_1,r_2,r_X}(r_1^\mu-p_1^\mu)\,\hat{\delta}^{(4)}\left(p_{1}+p_{2}-r_{1}-r_{2}-r_{X}\right) \\
&\times   \mathcal{A}\left(p_{1}, p_{2} \rightarrow r_{1}, r_{2}, r_{X}\right) \mathcal{A}^{*}\left(p_1+\hbar \bar{q},p_2-\hbar \bar{q} \rightarrow r_{1}, r_{2}, r_{X}\right)
\end{aligned}$$


We can extract $\hbar$ from $q$ and from the amplitude, by extracting each $e$ along with an $\frac{1}{\sqrt{\hbar}}$ , thus quartic vertices yield a factor of $\frac{e^2}{\hbar}$ whereas cubic ones yield $\frac{e}{\sqrt{\hbar}}$.  If we count the number $V_3$ of all cubic vertices, and $V_4$ the number of quartic vertices we have that the number of internal lines is $I=\frac{1}{2}(3V_3+4V_4-E)$. This is because we have $3V_3+4V_4$  lines to start with, out of which $E$ are chosen to be external. The remaining $(3V_3+4V_4-E)$ ones are contracted among themselves to form $I$ internal lines. In our case we have $E=4+M$ where $M=\abs{X}$ is the number of messenger particles. Using the argument from [[loop counting]] we have that the number of loops of our graph $L$ is given by:
$$
\begin{aligned}
        L=I-V+N=&\frac{1}{2}(3V_3+4V_4-4-M)-V_4-V_3+1\\
=&\frac{1}{2}(V_3+2V_4)-1-\frac{M}{2}
\end{aligned}
$$
where $N$ is the number of [[connected topological space|connected]] components ($=1$ in our case) . Thus we see that the amount of extracted $\hbar$s corresponds directly to the number of loops plus one! We can thus write the amplitude $\mathcal{A}$ as a sum over reduced $L$-loop amplitudes $\bar{\mathcal{A}}^{(L)}$:

$$\mathcal{A}(p_1,p_2\to r_1,r_2,X)=\sum\limits_{L=0}^\infty\par[\Big]{\frac{e^{2}}{\hbar}}^{(L+1+\frac{\abs{X}}{2})}\bar{\mathcal{A}}^{(L)}(p_1,p_2\to r_1,r_2,X)$$


Going back to the integrands we have:

$$\begin{aligned}
\vKernAA{p_\mu^1}&=\hbar^3\iunit\,  \bar{q}\, \sum\limits_{L=0}^\infty\par[\Big]{\frac{e^{2}}{\hbar}}^{(L+1)}\bar{\mathcal{A}}^{(L)}(p_1,p_2\to p_1+\hbar \bar{q},p_2-\hbar\bar{q})\\
&=\iunit\,  \bar{q}\, \sum\limits_{L=0}^\infty e^{2(L+1)}{\hbar}^{(2-L)}\bar{\mathcal{A}}^{(L)}(p_1,p_2\to p_1+\hbar \bar{q},p_2-\hbar\bar{q})
\end{aligned}$$

as well as the real kernel:[^1]

$$\begin{aligned}

\rKernAA{p_\mu^1}&=\hbar^2\cutint\ddP[\abs {X}]{r_X}\prod\limits_{i=1,2}\dh[4]{w_i}\hat{\delta}(2p_i \cdot w_i+w_i^2)\Theta(p_i^0+w_i^0) \\
&\times w_1^\mu\,\hat{\delta}^{(4)}\left(w_1+w_2+r_{X}\right)
\\
&\times\mathcal{A}\left(p_{1}, p_{2} \rightarrow p_1+w_{1}, p_2+w_{2}, r_{X}\right) 
\mathcal{A}^{*}\left(p_1+\hbar \bar{q},p_2-\hbar \bar{q} \rightarrow p_1+w_{1}, p_2+w_{2}, r_{X}\right)\\
&
\end{aligned}$$
$$\begin{aligned}

=\hbar^2\cutint&\ddP[\abs {X}]{{r}_X}\prod\limits_{i=1,2}\hbar^3\dh[4]{\bar{w}_i}\hat{\delta}(2p_i \cdot \bar{w}_i+\hbar\bar{w}_i^2)\Theta(p_i^0+\hbar \bar{w}_i^0) \\
&\times   \hbar \bar{w}_1^\mu\,\hbar^{-4}\hat{\delta}^{(4)}\par[\big]{\bar{w}_1+\bar{w}_2+\frac{1}{\hbar}r_{X}}
\\
&\times\sum\limits_{L=0}^\infty\par[\Big]{\frac{e^{2}}{\hbar}}^{2L+2+\abs{X})}\bar{\mathcal{A}}^{(L)}\par{p_{1}, p_{2} \rightarrow p_1+\hbar\bar{w}_{1}, p_2+\hbar\bar{w}_2, r_{X}} 
\mathcal\\\\
&\times\bar{\mathcal{A^{*}}}^{(L)}{}\par{p_1+\hbar \bar{q},p_2-\hbar \bar{q} \rightarrow p_1+\hbar\bar{w}_{1}, p_2+\hbar\bar{w}_2, r_{X}}

\end{aligned}$$

$$\begin{aligned}
=\cutint&\ddP[\abs {X}]{{r}_X}\prod\limits_{i=1,2}\dh[4]{\bar{w}_i}\hat{\delta}(2p_i \cdot \bar{w}_i+\hbar\bar{w}_i^2)\Theta(p_i^0+\hbar \bar{w}_i^0) \\
&\times    \bar{w}_1^\mu\,\hat{\delta}^{(4)}\par[\big]{\bar{w}_1+\bar{w}_2+\frac{1}{\hbar}r_{X}}
\\
&\times\sum\limits_{L=0}^\infty e^{2(2L+2+\abs{X})}{\hbar}^{3-2L-\abs{X}}\bar{\mathcal{A}}^{(L)}\par{p_{1}, p_{2} \rightarrow p_1+\hbar\bar{w}_{1}, p_2+\hbar\bar{w}_2, r_{X}} 
\mathcal\\\\
&\times\bar{\mathcal{A^{*}}}^{(L)}{}\par{p_1+\hbar \bar{q},p_2-\hbar \bar{q} \rightarrow p_1+\hbar\bar{w}_{1}, p_2+\hbar\bar{w}_2, r_{X}}\\

\end{aligned}$$

Schematically we have 

$$\begin{aligned}
\vKernAA{p_\mu^1}&=\sum\limits_{L=0}^\infty \mathcal{O}(e^{2(L+1)})\\
\rKernAA{O}&=\sum\limits_{L=0}^\infty \mathcal{O}(e^{4(L+1)+2\abs{X}})
\end{aligned}$$

The contributions from the virtual kernel are lower order for a given loop order. Both kernels contribute together provided that the following equation is verified.

$$L-1=2L'+\abs{X}$$

Where $L$ is the loop count for the virtual kernel and $L'$, $\abs{X}$ are the real kernel loop count and messenger particle count respectively.

Now we see that the leading order contribution [^2]to the impulse $\Delta p_1^{\mu,(0)}$  can only be from the virtual kernel at tree level. Thus we have the following equation.

$$\Delta p_1^{\mu,(0)}=\AAngle{\int \d {\overline{\Psi}(\bar{q})}\exp\par[\big]{-\iunit\bar{q}^\mu b_\mu}\ \vKernAA{p_1^{\mu},L=0}} $$

And the integrand is given by the tree level 4 point amplitude.

$$\vKernAA{p_1^{\mu},L=0}=\iunit\,  \bar{q}^\mu\,  e^{2}{\hbar}^{2}\bar{\mathcal{A}}^{(0)}(p_1,p_2\to p_1+\hbar \bar{q},p_2-\hbar\bar{q})$$

The amplitude is read off from the single tree level diagram and using [[feynman rules for SQED]]. 

$$\iunit\bar{\mathcal{A}}^{(0)}(p_1,p_2\to p_1+\hbar \bar{q},p_2-\hbar\bar{q})=\iunit \frac{Q_1 Q_2 }{\hbar^2\bar{q}^2}\par[\big]{4 p_1 \cdot p_2+\hbar^2\bar{q}^2}$$

We can now safely take the $\hbar \to 0$ limit as the integrand contains no terms singular in $\hbar$ (the $\frac{1}{\hbar^2}$ is cancelled by the $\hbar^2$ pre-factor). Thus the classical limit is carried out and the final integral to compute is obtained. The integration measure is also simplified in the limit $\lim\limits_{\hbar \to0} \d{\overline{\Psi}(\bar{q})}=\dh[4]{\bar{q}} \hat{\delta}(2p_1\cdot\bar{q})\hat{\delta}(2p_1\cdot \bar{q} )$[^3]

$$\Delta p_1^{\mu,(0)}=e^2Q_1Q_2\int\dh[4]{\bar{q}} \hat{\delta}(2p_1\cdot\bar{q})\hat{\delta}(2p_1\cdot \bar{q} )\euler^{-\iunit\bar{q}\cdot b}\bar{q}^\mu \frac{4 p_1 \cdot p_2}{\hbar^2\bar{q}^2}$$

This can be analytically computed (see [[LO impulse SQED]]) to find a closed form for the leading order impulse.

$$\Delta p_1^{\mu,(0)}=-\frac{e^{2} Q_{1} Q_{2}}{2 \pi} \frac{\gamma}{\sqrt{\gamma^{2}-1}} \frac{b^{\mu}}{b^{2}}$$

For [[NLO impulse SQED]], using the order equation above we have a 1-loop contribution from the virtual integrand as well as a tree level cut contribution from the real integrand. See [[NLO impulse SQED]] for details.
 


[^1]: We changed the integration variable from $r_i$ to $w_i=r_i-p_i$ thus the measure changes:$$\ddP[2+\abs{X}]{r_1,r_2,X}=\ddP[\abs {X}]{r_X}\prod\limits_{i=1,2}\dh[4]{w_i}\hat{\delta}(2p_i \cdot w_i+w_i^2)\Theta(p_i^0+w_i^0)$$ where we used the same reasoning as for the $q_i$ variable change.
    
[^2]: Here the expansion is in powers of the coupling constant, so even though we want $\hbar$s to cancel, the loop order will still affect the order of the contribution through the coupling constant $e$  and the leading order corresponds to $e^2$
[^3]: Compare to $$\d{\overline{\Psi}(\bar{q})}=\dh[4]{\bar{q}} \hat{\delta}(2p_1\cdot\bar{q}+\hbar\bar{q}^2)\Theta(p^0_1+q^0) \hat{\delta}(2p_1\cdot \bar{q} +\hbar\bar{q}^2)\Theta(p^0_2+q^0)$$The theta functions cancel as $q^0\to0$ and $p_i$ becomes classical.  And as discussed in [[classical limit of wavefuctions in KMOC]] the integration implicit in the brackets yields new delta functions based on the classical momenta, and with the  $\bar{q}^2$s removed