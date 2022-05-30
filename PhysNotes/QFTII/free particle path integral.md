---
alias:
tags:
- qftII
---
# 1.3 Free Particle

Consider now the [[../AnalyticalMech/Hamiltonian#Free Particle]].

## Phase space
The   [[Path Integral for Transition Amplitude#^discAction|discretised action]] is:

$$S_{n,0}[q,p]:=\sum_{k=1}^n \pqty{
-(t_k-t_{k-1}) \frac{p_k^2}{2m}
+p_k(q_k-q_{k-1})}.$$

^cd1a51

We observe that each variable $q_k$ appears only in a product with either $p_k$ or $p_{k+1}$. The [[Path Integral for Transition Amplitude#^transAmp|transition amplitude]] integral  over $q_k$ therefore yields a [[../delta-function]]:
$$\int \dd{q_k}\exp\pqty{\iunit \hbar^{-1}q_k(p_k-p_{k+1})}=2\pi \hbar\, \delta(p_k-p_{k+1})$$
We can therefore perform the rest of the $p_k$ integrals and obtain:
$$\begin{align}
A_{n,0}
&= \int \prod_{k=1}^{n-1} \dd{q_k}\prod_{k=1}^{n} \frac{\dd{p_k}}{2\pi \hbar} \exp(\frac{\iunit}{ \hbar} S_{n,0}[q,p]),
\\
&= \int \frac{\dd{p}}{2\pi \hbar} \exp\bqty{\frac{\iunit}{\hbar}
\pqty{
-(t_n-t_0) \frac{p^2}{2m}
+p(q_n-q_0)
}}
\\
&=
\sqrt{\frac{m}{2\pi\hbar \iunit (t_n-t_0) }}
\exp\pqty{\frac{\iunit m(q_n-q_0)^2}{2\hbar(t_n-t_0)}}.
\end{align}
$$
^phase

## Position Space
Alternatively, we can start with the classical discretised action

$$S_{n,0}[q]= \frac{1}{2} m\sum_{k=1}^n
 \frac{(q_k-q_{k-1})^2}{t_k-t_{k-1}}
.$$
It turns out that every integral over a $q_k$ in the [[Path Integral in Position Space#^8ff1e5|transition amplitude]] simply eliminates the set of variables $(q_k, t_k)$ from their sequences without leaving a gap. In the end we find:
$$A_{n,0}
=
\sqrt{\frac{m}{2\pi \hbar \iunit(t_n-t_0)}}
\exp\pqty{ \frac{\iunit m(q_n-q_0)^2}{2\hbar(t_n-t_0)}}$$
^pos

Gladly the two results agree [[#^phase]] vs [[#^pos]]
