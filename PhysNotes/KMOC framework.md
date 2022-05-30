---
sources:
aliases: 
tags: 
alias:
- KMOC
- Kosower, Maybee, and O’Connell
tag:
- QM
date created: Friday, March 25th 2022, 6:07:25 pm
date modified: Wednesday, May 18th 2022, 3:20:04 pm
---
Kosower, Maybee, and O’Connell framework
$\newcommand{\d}[1]{\,\mathrm{d}#1\,}$
$\newcommand{\dd}[2][]{\,\mathrm{d}^{#1}#2\,}$
$\newcommand{\dh}[2][]{\,\mathrm{ \hat{d}}^{#1}#2\,}$
$\newcommand{\ddP}[2][]{\,\mathrm{d}\Phi_{#1}(#2)\,}$
$\newcommand{\AAngle}[1]{\Bigg\langle\hspace{-0.6em}\Bigg\langle #1\Bigg\rangle\hspace{-0.6em}\Bigg\rangle}$
$\newcommand{\def}{\coloneqq}$
Original paper:
[[../Zotero/@kosowerAmplitudesObservablesClassical2019]]
$\newcommand{\par}[2][]{#1(#2 #1)}$
allows us to extract classical observables directly from scattering amplitudes and what are essentially unitarity cuts.[^1]

Throughout we use [[relativistically natural units]], i.e. we do *not* set $\hbar=1$.

We want to scatter a two particle [[LSZ reduction|in state]] into an at least 2 particle [[LSZ reduction|out state]]. 

Thus the [[LSZ reduction|in state]] is given by 
![[../Zotero/@kosowerAmplitudesObservablesClassical2019#^inState]]



The $e^{\iunit b_\mu p^\mu_1 /\hbar}$ factor encodes the fact that we have translated the wavepacket of particle $1$ relative to particle $2$ by the impact parameter $b$ .[^2] We take it to be perpendicular to the initial momenta $p_1,p_2$.

The [[.md|KMOC framework]] concerns itself with the change of an observable during a scattering event. For such an observable ${O}$, its change can be simply obtained by evaluating the difference of the expectation value of the corresponding Hermitian operator, $\mathbb{O}$, between in and out states
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

^DeltaO

If we put in the definition of our [[../Zotero/@kosowerAmplitudesObservablesClassical2019#^inState|in state]] we have:


$$\Delta O = \int \dd{\Phi_4(p_1,p_2,p_1',p_2')} \phi_1(p_1)\phi_2(p_2)\phi_1^\dagger(p_1')\phi_2^\dagger(p_2')\,e^{\iunit b_\mu\frac{p_1^\mu-p_1'^\mu}{\hbar}}\bqty{\mathcal{I_\text{v}}(O)-\mathcal{I}_\text{r}(O)}$$
Where 
$$\begin{align*}
\mathcal{I}_\text{v}(O)&=\mel{p_1'p_2'}{\iunit[\hat{O}, T ]}{p_1p_2}\\
\mathcal{I}_\text{r}(O)&=\mel{p_1'p_2'}{T^\dagger[\hat{O}, T ]}{p_1p_2}
\end{align*}$$
>NB: the notation is slightly different in the [[../Zotero/@bernScalarQEDToy2021]] paper

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
\Delta O_\text{v}=\int \ddP[2]{p_1,p_2} \dh[4]q\, &\hat{\delta}(2 p_1 \cdot q+q^2) \Theta(p^0_1+q^0)\, \hat{\delta}(2 p_2 \cdot q-q^2) \Theta(p^0_2-q^0)\\
&\times\phi_1(p_1)\phi_2(p_2)\phi_1^\dagger(p_1+q)\phi_2^\dagger(p_2-q)\,e^{-\frac{\iunit}{\hbar} b_\mu q^\mu}\\
&\times \iunit \underset{q}{\Delta} O\, \mathcal{A}(p_1,p_2 \to p_1+q,p_2-q)

\end{align*}
$$

^deltaOv


$$
\begin{align*}
\Delta O_\text{r}=\sum\limits_X \int \ddP[2+\abs{X}]{r_1,&r_2,X}\,\ddP[2]{p_1,p_2} \dh[4]q\,\hat{\delta}(2 p_1 \cdot q+q^2) \Theta(p^0_1+q^0)\\
&\times \hat{\delta}(2 p_2 \cdot q-q^2) \Theta(p^0_2-q^0)\\
&\times\phi_1(p_1)\phi_2(p_2)\phi_1^\dagger(p_1+q)\phi_2^\dagger(p_2-q)\,e^{-\frac{\iunit}{\hbar} b_\mu q^\mu}\\
&\times\underset{rX-p}{\Delta}\!\! O \,\hat{\delta}^{(4)}\left(p_{1}+p_{2}-r_{1}-r_{2}-r_{X}\right) \\
&\times   \mathcal{A}\left(p_{1}, p_{2} \rightarrow r_{1}, r_{2}, r_{X}\right) \mathcal{A}^{*}\left(p_{1}+q, p_{2}-q \rightarrow r_{1}, r_{2}, r_{X}\right)
\end{align*}$$

^deltaOr

# Classical limit

Since we are concerned with classial observables we need to explore the classical limit of [[#^DeltaO]], i.e. the limit of $\hbar \to 0$. The first target is the wavefunctions. 

## Classical limit of wavefunctions

[[classical limit of wavefuctions in KMOC]]

## Notation

As we have now seen the phase space integrals over initial momenta, and over the wavefunctions can be readily eliminated in the classical limit, in which case the momenta   $p_1$ and $p_2$ can be replaced by their classical values. To make explicit that idea we introduce the following notation:



$$\AAngle{f(p_1,p_2,\dots)}\def \int\limits \ddP{p_1}\ddP{p_2} \abs{\phi_1(p_1)}^2\abs{\phi_2(p_2)}^2\,f(p_1,p_2,\dots)$$

We can now rewrite [[#^deltaO]]:

$$\Delta O= \AAngle{\int \overbracket{\dh[4]{q} \hat{\delta}(2p_1\cdot q +q^2)\Theta(p^0_1+q^0)  \hat{\delta}(2p_1\cdot q +q^2)\Theta(p^0_2+q^0)}^{\dd{\Psi(q)}}\exp({-\frac{\iunit}{\hbar}}q^\mu b_\mu)\par[\Big]{\mathcal{I}_\text{v}'(O)+\mathcal{I}_\text{r}'(O)} }$$

Where 
$$\begin{aligned}
\mathcal{I}_\text{v}'(O)&=\iunit\,  \underset{q}{\Delta} O\, \mathcal{A}(p_1,p_2 \to p_1+q,p_2-q)\\
\mathcal{I}_\text{r}'(O)&=\sum\limits_X \int \ddP[2+\abs{X}]{r_1,r_2,X}\underset{rX-p}{\Delta}\!\! O \,\hat{\delta}^{(4)}\left(p_{1}+p_{2}-r_{1}-r_{2}-r_{X}\right) \\
&\times   \mathcal{A}\left(p_{1}, p_{2} \rightarrow r_{1}, r_{2}, r_{X}\right) \mathcal{A}^{*}\left(p_{1}+q, p_{2}-q \rightarrow r_{1}, r_{2}, r_{X}\right)


\end{aligned}$$

Additionally we want to make clear the dependence on $\hbar$ since we want to eventually take the $\hbar \to0$ limit. We can change integration variables to $\bar{q}=\frac{q}{\hbar}$ and absorb that $\hbar$ dependence into the redefinition of the integrands:

$$\begin{aligned}
\d{\Psi(q)}
&=\hbar^2\d{\overline{\Psi}(\bar{q})}
=\hbar^{\cancelto{2}{4}}\dh[4]{\bar{q}} 
\cancel{\frac{1}{\hbar}}\hat{\delta}(2p_1\cdot\bar{q}+\hbar\bar{q}^2)
\Theta(p^0_1+q^0) 
\cancel{\frac{1}{\hbar}}\hat{\delta}(2p_1\cdot \bar{q} +\hbar\bar{q}^2)
\Theta(p^0_2+q^0)
\end{aligned}$$
$$
\begin{aligned}


\overline{\mathcal{I}_\text{v}'}(O)&=\hbar^2\mathcal{I}_\text{v}'(O)\\
\overline{\mathcal{I}_\text{r}'}(O)&=\hbar^2\mathcal{I}_\text{r}'(O)
\end{aligned}$$

We can finally neatly write:

$$\Delta O=\AAngle{\int \d {\overline{\Psi}(\bar{q})}\exp\par[\big]{-\iunit\bar{q}^\mu b_\mu}\par[\Big]{\overline{\mathcal{I}_\text{v}'}(O)+\overline{\mathcal{I}_\text{r}'}(O)}}  $$

Now the $\hbar$ dependence is all in the integrands  (ignoring the $\hbar \bar{q}^2$ factors in the delta function). 

We can now explore the integrands in different theories: 

[[KMOC in SQED]]






[^2]: $f(x)=\int \ddP{p} \tilde{f}(\boldsymbol{p})e^{-\frac{\iunit}{\hbar} p^\mu x_\mu}$. Then a shifted, i.e. translated version of $f(x)$ can be written:$$\begin{align*}
f(x-x_0)&=\int \ddP{p} \tilde{f}(\boldsymbol{p})\,e^{-\frac{\iunit}{\hbar} p_\mu (x^\mu-x_0^\mu)}\\
&=\int \ddP{p} \tilde{f}(\boldsymbol{p})\,e^{\frac{\iunit}{\hbar}p_\mu x^\mu_0}\,e^{-\frac{\iunit}{\hbar} p_\mu x^\mu}
\end{align*}$$
Thus the associated, translated state is:
$$\ket{f}=\int \ddP{p} \tilde{f}(\boldsymbol{p})\,e^{\frac{\iunit}{\hbar}p_\mu x^\mu_0}\,\ket{p }$$
[^3]: $1=\sum\limits_X \int \dd{\Phi_{2+\abs{X}}}(r_1,r_2,X)\dyad{r_1 r_2 X}$ Where we could consider the states ${r_1,r_2,X}$ to be the final states after the scattering
[^4]: Introducing the momentum shifts modifies the measure in the following way:
    $$\ddP{p_i'}=\ddP{p_i+q_i}=\dh[4]q_i\,\hat{\delta}((p_i+q_i)^2-m_i^2) \Theta(p^0_i+q_i^0)$$
            Now since we also have the on shell enforcing delta function from $\ddP{p_i}$ we can rewrite the delta functions:     $$\ddP{p_i}\,\hat{\delta}((p_i+q_i)^2-m_i^2)=\ddP{p_i}\hat{\delta}(\underbracket{(p_i^2-m_i^2)}_{\text{redundant}}+2 p_i \cdot q_i+q_i^2)=\ddP{p_i}\hat{\delta}(2 p_i \cdot q_i+q_i^2)$$
            Finally when integrating over $q_2$ we choose to hit $\hat{\delta}^{(4)}(p_1+p_2-p_1'-p_2')=\hat{\delta}^{(4)}(q_1+q_2)$ and thus we just set $q_2=-q_1$