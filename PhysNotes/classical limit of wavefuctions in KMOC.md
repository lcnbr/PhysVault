---
aliases: 
tags: 
date created: Tuesday, April 26th 2022, 10:50:56 am
date modified: Tuesday, May 10th 2022, 3:09:12 pm
---
In [[KMOC framework|KMOC]] we are interested in the classical limit of a scattering event. It is then important to understand the precise simplifications this limit yields. 


We have multiple conditions on the wavefunctions. The first are those imposed by [[LSZ reduction|LSZ]]. That is,

- Compact support momentum space [[wavefunction in QFT|wavefunction]]
- Peaked around one value of momenta

Classical limit of the wavefunctions should make sense, thus 

- as $\hbar \to 0$ the wavefunction should approach a delta function
- The spread should not be too large as to interact between the two initial states
- The overlap between the wavefunction and its conjugate should be nearly full, since they represent the same particle classically.

Consider for example a nonrelativistic wavefunction:

$$f(\mathbf{p})=-\exp\pqty\bigg{-\frac{\mathbf{p}}{2 \hbar m \ell_c/\ell_\omega^2}}\stackrel{\hbar=\ell_c m}{=}\exp\qty\bigg(-\frac{\mathbf{p}}{2 m^2 \ell_c^2 /\ell_\omega^2})$$
This wavefunction grows sharper in the $\hbar \to 0$ limit. 

The [[Fourier transform]] of $f(\mathbf{p})$ gives us the position "probability density":
$$\begin{align*}
f(\mathbf{x})&=\int \frac{\dd{p}}{2 \pi} \exp\pqty\Big{-\pqty\Big{\frac{\mathbf{p}}{A}}^2}\exp\pqty\Big{-\frac{\iunit}{\hbar} \mathbf{p}\cdot \mathbf{x}}\\
&=\frac{1}{2\pi}\underbracket{\int \dd{p} \exp\pqty\Big{-\pqty\Big{\frac{\mathbf{p}}{A}-\frac{\iunit\mathbf{x}A}{2 \hbar}}^2}}_{\sqrt{\pi}A}\exp\pqty\Big{- \frac{\mathbf{x}^2A}{4 \hbar^2}}\\
&=\frac{\sqrt{2}A}{2 \pi}\exp\pqty\Big{-\frac{\mathbf{x}^2}{2 \ell_\omega^2}}
\end{align*}$$
[^x0]
This wavefunction grows sharper in the $\ell_\omega^2 \to 0$ limit. We must then still have that $\xi=\pqty{\frac{\ell_c}{\ell_\omega}}^2\to0$ when $\hbar \to 0$ as-well. This works if we just directly take the classical limit to be the $\xi \to 0$ limit.


Going back to the general conditions we want $\phi_i(p_i)$ s.t:

- $\ev{p^\mu_i}=\int \dd{\Phi(p_i)} p^\mu_i \abs{\phi_i(p_i)}^2\stackrel{!}{=}m_i \breve{u}_i^\mu f_{p,i}(\xi)$[^1] with $f_{p,i}(\xi)=1+\mathcal{O}(\xi^{\beta'})$
- $\sigma^2(p_i)/m_i^2=\ev{(p_i-\ev{p_i})^2}/m_i^2=(\ev{p^2_i}-\ev{p_i}^2)/m_i^2=c_\Delta\xi^\beta$[^2]
- $\breve{u}_i \cdot u_i = 1+ \mathcal{O}(\xi^{\beta''})$[^3]

Additionally the wavefunction should be Lorentz invariant, thus naively we would have that $\phi(p_i^\mu)=\tilde{\phi}(p_i^2)$ however the integration measure enforces an on shell condition: $m_i^2=p_i^2$. Thus the wavefunction cannot usefully depend on $p_i^2$, we need to introduce at least one additional four vector parameter $u$. The simplest dimensionless combination of parameters it then $\frac{p \cdot u }{m}$. Of course the wavefunction must also depend on $\xi$ and the simplest form of argument will thus be $\frac{p \cdot u }{m \xi}$ so that any $p$ not aligned with $u$ will be strongly suppressed in the $\xi \to0$ limit.

We now have control over most of the conditions:

- The classical limit is well defined
- The wavefunction spread is controlled
- The arguments of the wavefunction is clear

The last requirement concerns the overlap of $\phi$ and $\phi^\dagger$ must be $\mathcal{O}(1)$, equivalently and more precisely:

$$\phi^\dagger(p+q)\sim \phi^\dagger(p) \implies \phi^\dagger(p+q)- \phi^\dagger(p)\ll 1 \implies q^\mu\partial_\mu{\phi^\dagger}(p)\ll1$$
Making explicit the $\frac{p \cdot u }{m \xi}$ dependence: $\phi(p)=\varphi(\frac{p \cdot u }{m \xi})$   for $\varphi(x)$ a scalar function.
$$\implies \frac{q^\mu u_\mu}{m \xi}\pdv{\varphi^\dagger}{x}(\frac{p \cdot u }{m \xi})\ll1$$
Thus we require that for a characteristic value of $q=q_0$ we have:

$$\frac{q_0\cdot u}{m \xi}=\bar{q}_0 \cdot u\frac{\ell_\omega^2}{\ell_c}\ll1\iff \bar{q}_0 \cdot u\,\ell_\omega\ll \sqrt{ \xi}$$[^4]
We now want to examine the classical limit of something like  [[KMOC framework#^deltaOv]]. If we consider just the integration over the initial momenta $p_i$ and the initial wavefunctions with $\hat{\delta}(2 p_i \cdot q+q^2)$, the delta function will smear out to a sharply peaked function whose scale is the same order as the original wavefunctions. As $\xi$ gets smaller, this function will turn back into a delta function  
imposed on the $q$ integration.[^5] Let us examine this statement more closely:


$$d(m,\xi,u,q)=\int \dd{\Phi(p)} \hat{\delta}(2 p \cdot q+q^2) \Theta(p^0+q^2)\varphi(\frac{p \cdot u }{m \xi})\varphi^\dagger(\frac{(p+q) \cdot u }{m \xi})$$
^dfunct

This integral must be Lorentz invariant and depends on $m,\xi, u,q$ thus it must manifestly only depend on the following [[math/Lorentz group|Lorentz invariants]]: $u^2,q^2,u \cdot q, \xi$. One of these is not actually a variable as we will normalise $u^2=1$. The rest aren't fully dimensionless, and we can render them dimensionless:[^6]

$$\begin{align*}
[q^2]&=[\hbar \bar{q}]^2=[M]^2\implies[\ell_c \sqrt{-\bar{q}^2}]=[\frac{\hbar}{m}\sqrt{-\bar{q}^2}]=\frac{[M]}{[M]}=1\\
[u \cdot q]&=[M]\implies [\frac{u \cdot\bar{q}}{\sqrt{-\bar{q}^2}}]= [\frac{u \cdot{q}}{\sqrt{-{q}^2}}]=\frac{[M]}{[M]}=1\\
[\xi]&=1
\end{align*}$$
If we call $\frac{1}{\sqrt{-\bar{q}^2}}=\ell_s$ a scattering length[^7] then our dimensionless ratios are :

$$\frac{\ell_c}{\ell_s} \qqtext{and} \ell_s\,\bar{q} \cdot u $$
The delta function can be rewritten as:
$$\hat{\delta}(2 p \cdot q+q^2)=\hat{\delta}(2\hbar m\, u\cdot \bar{q}+\hbar^2 \bar{q}^2)=\frac{1}{\hbar m}\hat{\delta}(2 \bar{q} \cdot u-\frac{\ell_c}{\ell_s^2})=\frac{\ell_s}{\hbar m}\hat{\delta}(2\ell_s\, \bar{q} \cdot u-\frac{\ell_c}{\ell_s})$$




[^1]: $A$ absorbs the various constants, with $A=\sqrt{2}m\frac{\ell_c}{\ell_\omega}$ and $\mathbf{x}_0$ 
[^2]: This means that the classical value of momentum $m_i \breve{u}_i^\mu$ is reached in the $\xi \to 0$ limit
[^3]: This encodes the limit of the spread as $\xi \to0$. $\ev{p_i^2}=m_i^2$ is enforced by the measure $\dd{\Phi(p)}$
[^4]: This enforces the normalisation condition $\breve{u}_i^2=1$ in the $\xi \to0$ limit 
[^5]: Here $\bar{q}=\frac{q}{\hbar}$ is the wavenumber
[[relativistically natural units|^6]]
[[relativistically natural units|^7]] $[\frac{1}{\sqrt{-\bar{q}^2}}]=[T]=[L]=[\ell_s]$
[[example wavefunction in KMOC|^8]]