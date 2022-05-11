---
aliases: 
tags: 
alias:
- KMOC
- Kosower, Maybee, and O’Connell
tag:
- QM
date created: Friday, March 25th 2022, 6:07:25 pm
date modified: Wednesday, April 27th 2022, 2:37:37 pm
---
Kosower, Maybee, and O’Connell framework


Original paper:
[[@kosowerAmplitudesObservablesClassical2019]]

allows us to extract classical observables directly from scattering amplitudes and what are essentially unitarity cuts.[^1]

Throughout we use [[relativistically natural units]], i.e. we do *not* set $\hbar=1$.

We want to scatter a two particle [[LSZ reduction|in state]] into an at least 2 particle [[LSZ reduction|out state]]. 

Thus the [[LSZ reduction|in state]] is given by 
![[@kosowerAmplitudesObservablesClassical2019#^inState]]



The $e^{\iunit b_\mu p^\mu_1 /\hbar}$ factor encodes the fact that we have translated the wavepacket of particle $1$ relative to particle $2$ by the impact parameter $b$ .[^2] We take it to be perpendicular to the initial momenta $p_1,p_2$.

The [[KMOC framework]] concerns itself with the change of an observable during a scattering event. For such an observable ${O}$, its change can be simply obtained by evaluating the difference of the expectation value of the corresponding Hermitian operator, $\mathbb{O}$, between in and out states
$$
\Delta O=\expval{\hat{O}}{\text{out}}-\expval{\hat{O}}{\text{in}}
$$
In quantum mechanics, the out states are related to the in states by the time evolution operator, i.e. the S-matrix: $\ket{\text{out}}=S \ket{\text{in}}$ and we can write
$$\begin{align*}
\Delta O&=\expval{S^\dagger\hat{O}S}{\text{in}}-\ev{\hat{O}}{\text{in}}\\
&\stackrel{S^\dagger S=1}{=} \ev{S^\dagger [\hat{O},S]}{\text{in}}\\
&\stackrel{S=1+\iunit T}{=} \ev{[\hat{O},1+\iunit T ]}{\text{in}}-\ev{\iunit T^\dagger [\hat{O},1+\iunit T]}{\text{in}}\\
&=\ev{\iunit[\hat{O}, T ]}{\text{in}}+\ev{ T^\dagger [\hat{O}, T]}{\text{in}}\\
&=\Delta O_\text{v}+\Delta O_\text{r}
\end{align*}$$

^98a88f

If we put in the definition of our [[@kosowerAmplitudesObservablesClassical2019#^inState|in state]] we have:


$$\Delta O = \int \dd{\Phi_4(p_1,p_2,p_1',p_2')} \phi_1(p_1)\phi_2(p_2)\phi_1^\dagger(p_1')\phi_2^\dagger(p_2')\,e^{\iunit b_\mu\frac{p_1^\mu-p_1'^\mu}{\hbar}}\bqty{\mathcal{I_\text{v}}(O)-\mathcal{I}_\text{r}(O)}$$
Where 
$$\begin{align*}
\mathcal{I}_\text{v}(O)&=\mel{p_1'p_2'}{\iunit[\hat{O}, T ]}{p_1p_2}\\
\mathcal{I}_\text{r}(O)&=\mel{p_1'p_2'}{T^\dagger[\hat{O}, T ]}{p_1p_2}
\end{align*}$$
>NB: the notation is slightly different in the [[@bernScalarQEDToy2021]] paper

Let us first look at the virtual integrand $\mathcal{I}_\text{v}$:

$$\begin{align*}
\mathcal{I}_\text{v}(O)&=\mel{p_1'p_2'}{\iunit[\hat{O}, T ]}{p_1p_2}\\
&=\mel{p_1'p_2'}{\iunit\hat{O}T }{p_1p_2}- \mel{p_1'p_2'}{\iunit T\hat{O} }{p_1p_2}\\
&=\iunit O_{\text{in}'} \mel{p_1'p_2'}{T}{p_1p_2}- \iunit O_{\text{in}}\mel{p_1'p_2'}{T}{p_1p_2}\\
&=\iunit \underset{p-p'}{\Delta} O \mel{p_1'p_2'}{T}{p_1p_2}\\
&=\iunit \underset{p-p'}{\Delta}O \hat{\delta}^{(4)}(p_1+p_2-p_1'-p_2') \mathcal{A}(p_1,p_2 \to p_1',p_2')
\end{align*}$$

Note that the amplitude is from in states to in states!
Now for the real integrand $\mathcal{I}_\text{r}$ we insert a complete set of states :[^3]
$$\begin{align*}
\mathcal{I}_\text{r}(O)&=\mel{p_1'p_2'}{T^\dagger[\hat{O}, T ]}{p_1p_2}\\
&=\sum\limits_X \int \dd{\Phi_{2+\abs{X}}}(r_1,r_2,X)\mel{p_1'p_2'}{T^\dagger}{r_1 r_2 X}\mel{r_1 r_2 X}{[\hat{O}, T ]}{p_1p_2}\\
&=\sum\limits_X \int \dd{\Phi_{2+\abs{X}}}(r_1,r_2,X)  \hat{\delta}^{(4)}\left(p_{1}+p_{2}-r_{1}-r_{2}-r_{X}\right)\mathcal{A}\left(p_{1}, p_{2} \rightarrow r_{1}, r_{2}, r_{X}\right) \\
&\qquad \underset{rX-p}{\Delta}\!\! O \,\hat{\delta}^{(4)}\left(p_{1}^{\prime}+p_{2}^{\prime}-r_{1}-r_{2}-r_{X}\right)   \mathcal{A}^{*}\left(p_{1}^{\prime}, p_{2}^{\prime} \rightarrow r_{1}, r_{2}, r_{X}\right)

\end{align*}
$$

For both integrands we can preform some variable changes and eliminate certain delta functions. We introduce momentum shifts $q_i=p'_i-p_i$ and then integrate over $q_2$ finally relabelling $q_1 \to q$.[^4] Thus we have

$$\begin{align*}
\Delta O_\text{v}=\int \dd{\Phi_2(p_1,p_2)} \hat{\dd[4]}q\, &\hat{\delta}(2 p_1 \cdot q+q^2) \Theta(p^0_1+q^0)\, \hat{\delta}(2 p_2 \cdot q-q^2) \Theta(p^0_2-q^0)\\
&\times\phi_1(p_1)\phi_2(p_2)\phi_1^\dagger(p_1+q)\phi_2^\dagger(p_2-q)\,e^{-\frac{\iunit}{\hbar} b_\mu q^\mu}\\
&\times \iunit \underset{q}{\Delta} O\, \mathcal{A}(p_1,p_2 \to p_1+q,p_2-q)

\end{align*}
$$

^deltaOv


$$
\begin{align*}
\Delta O_\text{r}=\sum\limits_X \int \dd{\Phi_{2+\abs{X}}}(r_1,&r_2,X)\,\dd{\Phi_2(p_1,p_2)} \hat{\dd[4]}q\,\hat{\delta}(2 p_1 \cdot q+q^2) \Theta(p^0_1+q^0)\\
&\times \hat{\delta}(2 p_2 \cdot q-q^2) \Theta(p^0_2-q^0)\\
&\times\phi_1(p_1)\phi_2(p_2)\phi_1^\dagger(p_1+q)\phi_2^\dagger(p_2-q)\,e^{-\frac{\iunit}{\hbar} b_\mu q^\mu}\\
&\times\underset{rX-p}{\Delta}\!\! O \,\hat{\delta}^{(4)}\left(p_{1}+p_{2}-r_{1}-r_{2}-r_{X}\right) \\
&\times   \mathcal{A}\left(p_{1}, p_{2} \rightarrow r_{1}, r_{2}, r_{X}\right) \mathcal{A}^{*}\left(p_{1}+q, p_{2}-q \rightarrow r_{1}, r_{2}, r_{X}\right)
\end{align*}$$

^deltaOr


# Classical limit of wavefunctions

[[classical limit of wavefuctions in KMOC]]



[^1]: ![[@bernScalarQEDToy2021annotations#^cccd89]]
[^2]: consider a one particle in state with coordinate-space [[wavefunction in QFT|wavefunction]] $f(x)=\int \dd{\Phi(p)} \tilde{f}(\boldsymbol{p})e^{-\frac{\iunit}{\hbar} p^\mu x_\mu}$. Then a shifted, i.e. translated version of $f(x)$ can be written:$$\begin{align*}
f(x-x_0)&=\int \dd{\Phi(p)} \tilde{f}(\boldsymbol{p})\,e^{-\frac{\iunit}{\hbar} p_\mu (x^\mu-x_0^\mu)}\\
&=\int \dd{\Phi(p)} \tilde{f}(\boldsymbol{p})\,e^{\frac{\iunit}{\hbar}p_\mu x^\mu_0}\,e^{-\frac{\iunit}{\hbar} p_\mu x^\mu}
\end{align*}$$
Thus the associated, translated state is:
$$\ket{f}=\int \dd{\Phi(p)} \tilde{f}(\boldsymbol{p})\,e^{\frac{\iunit}{\hbar}p_\mu x^\mu_0}\,\ket{p }$$
[^3]: $1=\sum\limits_X \int \dd{\Phi_{2+\abs{X}}}(r_1,r_2,X)\dyad{r_1 r_2 X}$ Where we could consider the states ${r_1,r_2,X}$ to be the final states after the scattering
[^4]: Introducing the momentum shifts modifies the measure in the following way:
    $$\dd{\Phi(p_i')=\dd{\Phi(p_i+q_i)}}=\hat{\dd[4]}q_i\,\hat{\delta}((p_i+q_i)^2-m_i^2) \Theta(p^0_i+q_i^0)$$
            Now since we also have the on shell enforcing delta function from $\dd{\Phi(p_i)}$ we can rewrite the delta functions:     $$\dd{\Phi(p_i)}\hat{\delta}((p_i+q_i)^2-m_i^2)=\dd{\Phi(p_i)}\hat{\delta}(\underbracket{(p_i^2-m_i^2)}_{\text{redundant}}+2 p_i \cdot q_i+q_i^2)=\dd{\Phi(p_i)}\hat{\delta}(2 p_i \cdot q_i+q_i^2)$$
            Finally when integrating over $q_2$ we choose to hit $\hat{\delta}^{(4)}(p_1+p_2-p_1'-p_2')=\hat{\delta}^{(4)}(q_1+q_2)$ and thus we just set $q_2=-q_1$