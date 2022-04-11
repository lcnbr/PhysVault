---
alias:
tag:
---

Metric (+---)
$e=\abs{e}$


Using the [[minimal coupling prescription]]^[[[@colemanQUANTUMFIELDTHEORY2018#27 2 The minimal coupling prescription zotero open-pdf 0_4E7XKTS3 625]] with $Q=\text{diag}(q_1,q_2)$]. We want to couple a set of massive scalar fields to electromagnetism. The minimal coupling prescription works provided that our base mass lagrangian admits a conserved current.
Our base mass lagrangian is: 

$$\mathcal{L}_m=\sum\limits_{i=1}^2 \partial_\mu \phi_i^\dagger\,\partial^\mu \phi_i - m_i^2 \phi^\dagger_i \phi_i$$
Notice that under the following transformation:

$$\begin{aligned}
\phi_i(x) &\rightarrow e^{-\iunit q_i \lambda} \phi_i(x) \\
\phi_i^{\dagger}(x) &\rightarrow e^{\iunit q_i \lambda} \phi_i^\dagger(x) \\
\end{aligned}$$
or infinitesimally:
$$\begin{aligned}
\delta\phi_i &= -\iunit  \phi_i q_i \delta\lambda \\
\delta\phi_i^{\dagger} &= \iunit  \phi_i^\dagger q_i\delta \lambda\\
\end{aligned}$$
the above Lagrangian is unchanged. Note the sign of the transformation is important. If we upgrade the parameter $\lambda$ to a spacetime function $\lambda(x)$, the Lagrangian is not invariant anymore (c.f [[minimal coupling prescription]]) and invariance is restored if we replace all the derivatives $\partial_\mu$ with the [[gauge covariant derivative|covariant derivative]] $D_\mu$, i.e. if along with the transformation above, we perform a gauge transformation of the photon field:

$$A_\mu\rightarrow A_\mu + \frac{1}{e} \partial_\mu \lambda$$

or infinitesimally

$$\delta A_\mu = \frac{1}{e} \partial_\mu \delta \lambda$$
then the whole lagrangian: 

$$\mathcal{L}_{ED}+\mathcal{L}_{m}(\phi_i,\partial_\mu \phi_i)\rightarrow \mathcal{L}_{ED}+\mathcal{L}_{m}(\phi_i,D_\mu \phi_i)$$
is invariant under the above defined gauge transformation, with the [[gauge covariant derivative|covariant derivative]] defined as:

$$D_\mu=\partial_\mu+\iunit \,e\,q_i\,A_\mu$$
And the final lagrangian is:


$$\mathcal{L}=-\frac{1}{4} F_{\mu \nu} F^{\mu \nu}+\sum_{i=1}^{2}\left[\left(D_{\mu} \phi_{i}\right)^{\dagger}\left(D^{\mu} \phi_{i}\right)-m_{i}^{2} \phi_{i}^{\dagger} \phi_{i}\right]$$

with $F_{\mu \nu} \equiv \partial_{\mu} A_{\nu}-\partial_{\nu} A_{\mu}$.

Expanding and then integrating by parts:

$$
\begin{aligned}
\mathcal{L} &=-\frac{1}{4}\left(\partial_{\mu} A_{\nu}-\partial_{\nu} A_{\mu}\right)\left(\partial^{\mu} A^{\nu}-\partial^{\nu} A^{\mu}\right)
+\sum_{i=1}^{2}\left[
    \left(\partial_{\mu}-\iunit\, e\,q_i\, A_{\mu} \right)\phi_{i}^{\dagger}
    \left(\partial_{\mu}+\iunit\, e\,q_i\, A_{\mu}\right)\phi_{i}
    -m_{i}^{2} \phi_{i}^{\dagger} \phi_{i}
    \right]
 \\
&=\underbrace{
    \frac{1}{2} A_{\mu}\left[\eta^{\mu \nu}\partial^{2}-\partial^{\mu} \partial^{\nu}\right] A_{\nu}
    +\sum\limits_{i=1}^2-\phi_i^{\dagger}\left(\partial^{2}+m_i^{2}\right) \phi_i
    }_{\mathcal{L}_{0}}
+\underbrace{
    \sum\limits_{i=1}^2q_i^2\,e^{2} A_{\mu} A^{\mu} \,\phi^{\dagger}_i \phi_i
    -\iunit\, e\,q_i\, A_{\mu}\left(\phi^{\dagger}_i \partial^{\mu} \phi_i-\left(\partial^{\mu} \phi^{\dagger}_i\right) \phi_i\right)
    }_{\mathcal{L}^{\prime}}
\end{aligned}
$$

Since we have a massless photon, and still have gauge freedom we have to implement [[gauge fixing action for EM|gauge fixing]]:

$$\begin{aligned}\mathcal{L}_{\text{eff}}&=\mathcal{L}+\overbracket{\frac{-1}{2 \xi}(\partial_\mu A^\mu)^2}^{\mathcal{L_\text{GF}}}

 \\
&=
    \frac{1}{2} A_{\mu}\underbracket{\bqty{g^{\mu \nu}\partial^{2}-\pqty{1-\frac{1}{\xi}}\partial^{\mu} \partial^{\nu}}}_{\rightarrow \tilde{D}^{\mu \nu}_\xi(k)=\frac{-\iunit}{k^{2}+\iunit \varepsilon}\left[g_{\mu \nu}-(1-\xi) \frac{k_{\mu} k_{\nu}}{k^{2}}\right]} A_{\nu}
    +\sum\limits_{i=1}^2-\phi_i^{\dagger}\underbracket{\pqty{\partial^{2}+m_i^{2}}}_{\tilde{\Delta}_F(q^2)=\frac{\iunit}{p^{2}-m^{2}+\iunit \varepsilon}} \phi_i
    
+
    \sum\limits_{i=1}^2\underbracket{q_i^2\,e^{2}\,\eta^{\mu \nu}}_{\times 2\iunit\rightarrow \mathrm{4-vertex} } A_{\mu} A_{\nu} \,\phi^{\dagger}_i \phi_i
    \underbracket{-\iunit\, e\,q_i\, A_{\mu}\left(\phi^{\dagger}_i \partial^{\mu} \phi_i-\left(\partial^{\mu} \phi^{\dagger}_i\right) \phi_i\right)}_{\times \iunit\rightarrow \mathrm{3-vertex}}
    
\end{aligned}$$
Our fields are given by the usual:
$$
\begin{aligned}
\psi(x) &=\int \frac{d^{3} \mathbf{p}}{(2 \pi)^{3 / 2} \sqrt{2 \omega_{\mathbf{p}}}}\left[b_{\mathbf{p}} e^{-i p \cdot x}+c_{\mathbf{p}}^{\dagger} e^{i p \cdot x}\right] \\
\psi^{*}(x) &=\int \frac{d^{3} \mathbf{p}}{(2 \pi)^{3 / 2} \sqrt{2 \omega_{\mathbf{p}}}}\left[b_{\mathbf{p}}^{\dagger} e^{i p \cdot x}+c_{\mathbf{p}} e^{-i p \cdot x}\right]
\end{aligned}$$
The  feynman rules are thus:

![[feynman rules for SQED]]