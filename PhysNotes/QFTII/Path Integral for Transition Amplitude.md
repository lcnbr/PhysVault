---
alias:
tags:
- qftII
---
$\newcommand{\iunit}{{\mathring{\imath}}}$
# 1.2 Path Integral for Transition Amplitude

![[rev.pdf]]

We follow [[QFTIIconventions#Operators]], and make $\hbar$ explicit.

We [[canonical quantisation|canonically quantise]] the  classical [[../AnalyticalMech/Hamiltonian]], and promote it to an operator: $\hat{H}=H(\hat{q},\hat{p})$


# Transition Amplitude
 Want the [[transition amplitude]] $A_{f,i}$ between position $q_i$ at time $t_i$ and position $q_f$ at time $t_f$, which merely uses the classical [[../AnalyticalMech/Hamiltonian]] $H(p,q)$ instead of the [[Hamiltonian operator]] $\hat{H}$.

 
# Time Slices
First we interrupt the [[time evolution operator|time evolution]] at some intermediate time $t_f> t_k> t_i$ by using the [[time evolution operator#Group property|group property of time evolution]], and  we insert a complete set of [[position eigenstate#Complete set|complete set of position states]] at time $t_k$. Altogether we obtain an identity for [[transition amplitude]]:
$$A_{f,i}=\int \mathrm{d}q_k~ A_{f,k}A_{k,i}$$
We iterate the subdivision $n$ times to obtain a very fine resolution for the [[time evolution operator|time evolution]]:
$$
A_{\mathrm{f}, \mathrm{i}}=\int \mathrm{d} q_{n-1} \ldots \mathrm{d} q_{1} A_{\mathrm{f}, n-1} \ldots A_{1, \mathrm{i}}=\int \prod_{k=1}^{n-1} \mathrm{~d} q_{k} \prod_{k=1}^{n} A_{k, k-1}
$$
![[file:///C:/Users/Lucien/Documents/UNI/images/image25.png||300]]
For a sufficiently small time interval we can approximate the [[time evolution operator|time evolution]] by an exponential

$$
\hat{U}\left(t_{k}, t_{k-1}\right)=\exp \left(-\iunit \hbar^{-1}\left(t_{k}-t_{k-1}\right) \hat{H}\right) \simeq 1-\iunit  \hbar^{-1}\left(t_{k}-t_{k-1}\right) \hat{H} .
$$
 In other words we should be able to evaluate:
 $$\bra{q_k}\hat{H}\ket{q_{k-1}}=\bra{q_k}H(\hat{q},\hat{p})\ket{q_{k-1}}$$
This expression certainly depends on the ordering of factors $\hat{q}$ and $\hat{p}$ in $H( \hat{q},\hat{p})$ which is not determined by the classical [[../AnalyticalMech/Hamiltonian]] function [[q, p)](H(q, p|H(q, p)]]): 
- If we order all $\hat{q}$ to be to the left of all $\hat{p}$ we will get $$\bra{q_k}H(q_k,\hat{p})\ket{q_{k-1}}$$
- If we all $\hat{q}$ to be to the right of all $\hat{p}$ we will get $$\bra{q_k}H(q_{k-1},\hat{p})\ket{q_{k-1}}$$
- Weyl order: we could order the operators such that $\hat{q}$ evaluates to $\bar{q_k}=\frac{1}{2}(q_k+q_{k-1})$:$$\bra{q_k}H(\bar{q_k},\hat{p})\ket{q_{k-1}}$$
 
-  In fact, all orderings are equivalent up to simpler terms of order $\hbar$, and the precise definition of $\bar{q}_{k}$ does not matter be it $q_{k}, q_{k-1}$, their average or any other combination that limits to $\bar{q}_{k} \rightarrow q\left(t_{k}\right)$ at $t_{k-1} \rightarrow t_{k}$.

Note that it is crucial that only a single factor of $\hat{H}$ appears. In higher powers of $\hat{H}$ the non-trivial operator ordering would prevent us from replacing $\hat{q}$ by some average value $\bar{q}_{k}$. Hence we need a sufficiently large number of intermediate time slices for a good approximation.

In order to evaluate the momentum operator, we insert a [[momentum eigenstate#Complete set|complete set of momentum eigenstates]]. 
This yields
$$\begin{align}
\ip{q_k}{q_{k-1}}
&=\int \frac{\mathrm{d}{p_k}}{2\pi\hbar}\ip{q_k}{p_k}\ip{p_k}{q_{k-1}},\\
\bra{q_k}\hat H\ket{q_{k-1}}
&=\int \frac{\mathrm{d}{p_k}}{2\pi\hbar}\bra{q_k}H(\bar q_k, \hat p)\ket{p_k}\ip{p_k}{q_{k-1}}.
\end{align}$$
We substitute the [[momentum and position eigenstates#Fourrier exponent|Fourier exponent]] and the [[eigenvalue]] $H(\bar q_k, \hat p)\ket{p_k}=H(\bar q_k, p_k)\ket{p_k}$ to obtain an approximation for $A_{k,k-1}$
$$\int \frac{\mathrm{d}{p_k}}{2\pi\hbar}\exp\left[-\frac{\iunit}{\hbar}(t_k-t_{k-1})H(\bar q_k, p_k)
+\frac{\iunit}{\hbar}p_k(q_{k}-q_{k-1} \right].
$$
Putting everything together we now have an integral expression for the transition amplitude $A_{n,0}$ in terms of the classical [[../AnalyticalMech/Hamiltonian]]
$$
A_\text{f,i}
\approx A_{n,0}\coloneq
\int \prod_{k=1}^{n-1} \mathrm{d}{q_k}\prod_{k=1}^{n} \frac{\mathrm{d}{p_k}}{2\pi \hbar}
\exp\left(\frac{\iunit}{\hbar}S_{n,0}[q,p]\right),
$$

^transAmp

with the phase of the exponential determined by the function
$$
S_{n,0}[q,p]:=\sum_{k=1}^n \left(
-(t_k-t_{k-1})H(\bar q_k,p_k)
+p_k(q_k-q_{k-1}) \right).
$$
^discAction

![[file:///C:/Users/Lucien/Documents/UNI/images/image54.png||300]]
  
![[Path Integral in Phase Space]]

![[Path Integral in Position Space]]