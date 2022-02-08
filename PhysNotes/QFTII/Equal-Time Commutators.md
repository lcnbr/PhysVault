---
alias:
tags:
- qftII
---
# Equal-Time Commutators
The strict built-in [[Time Ordering|ordering of times]] makes
commutation relations between the operators irrelevant. The only operator algebra we can possibly consider is at equal times.
Let us therefore understand how to realise the fundamental commutation relation
$$
\comm{\hat q}{\hat p}=\iunit\hbar.
$$
We would like to [[single operator insertion|insert]] the operator $\hat O=\comm{\hat q}{\hat p}$ into
the path integral.
Unfortunately, there is no classical equivalent $O(q,p)$ to $\hat O$
except for the number $\iunit\hbar$, but that would amount to postulation
rather than derivation.

The trick is to separate the times slightly:
^[In fact, the product $q(t)p(t)$ at equal
times is ill-defined in the continuous path integral
since the insertion $q(t)p(t+\delta t)$ is discontinuous at $\delta t=0$
(by precisely $\iunit\hbar$).]
$$
O(t)=q(t) p(t-\epsilon) - p(t+\epsilon) q(t).
$$

The position variables $q_k$ were defined at times $t_k$.
The associated momenta $p_k$, however, are not located at $t_k$,
but rather between $t_k$ and $t_{k-1}$.
This fact is most evident in
the expression for the [[Path Integral for Transition Amplitude#^discAction|discretised action]]

The above operator is therefore discretised as follows
$$
O=q_k p_k - p_{k+1} q_k.
 $$

We [[single operator insertion|insert]] the operator into the [[free particle path integral#^cd1a51|discretised path integral for the transition amplitude of free non-relativistic particle]]: $\bra{q_\text{f},t_\text{f}}\hat O\ket{q_\text{i},t_\text{i}}$

We can perform most integrations trivially as before
$$
\require{color}
\definecolor{light-yellow}{rgb}{1,0.98,0.77}
\newcommand{\highlight}[1]{%
  \colorbox{light-yellow}{$\displaystyle#1$}}
 

\begin{align}
&
\int \frac{\dd{p_k}}{2\pi \hbar} \highlight{\dd{q_k}} \frac{\dd{p_{k+1}}}{2\pi \hbar}
\highlight{q_k}(p_k-p_{k+1})
\\
&\quad\cdot
\exp\pqty{-\frac{\iunit}{2 \hbar m}\pqty{(t_n-t_k)p_{k+1}^2+(t_k-t_0)p_k^2}}
\\
&\quad\cdot
\exp\pqty{\iunit \hbar^{-1}(p_{k+1}q_n-p_kq_0)}
\exp\pqty{\iunit \hbar^{-1}(p_k-p_{k+1})\highlight{q_k}}.
\end{align}
$$
We then convert the factor $q_k$ to a differential operator
acting on the latter exponent, and perform the integral
over $q_k$ as the derivative of a delta-function
$$
\begin{align}
& \int \frac{\dd{p_k}}{2\pi \hbar} \dd{p_{k+1}} \highlight{\phantom{\dd{}}}
(p_k-p_{k+1})
\\
&\quad\cdot
\exp\pqty{-\frac{\iunit}{2 \hbar m}\pqty{(t_n-t_k)p_{k+1}^2+(t_k-t_0)p_k^2}}
\\
&\quad\cdot
\exp\pqty{\frac{\iunit}{ \hbar}(p_{k+1}q_n-p_kq_0)}
%\exp\pqty{\iunit \hbar^{-1}p_{k}(q_n-q_0)}
%\\
%&\cdot
\pqty{-\iunit\hbar \highlight{\frac{\partial}{\partial p_k} \delta(p_{k+1}-p_k)}}.
\end{align}
$$
Now the only thing that protects the factor
$(p_k-p_{k-1})$ from vanishing by means of the [[delta function]]
$\delta(p_k-p_{k-1})$ is the derivative $\partial/\partial p_k$.
We therefore integrate by parts and let the
derivative act on the remainder of the integrand.
Unless it hits the factor $(p_k-p_{k-1})$, the integral must vanish, hence
$$
\begin{align}
&
\int \frac{\dd{p_k}}{2\pi \hbar} \dd{p_{k+1}}\delta(p_{k+1}-p_k)
\pqty{\iunit \hbar\frac{\partial}{\partial p_k}(p_k-p_{k+1})}
\\
&\quad\cdot
\exp\pqty{\frac{\iunit }{\hbar}\pqty{-(t_n-t_0) \frac{p_{k}^2}{2m}+p_{k}(q_n-q_0)}}
\\
&=
\iunit\hbar
\int \frac{\dd{p}}{2\pi \hbar}
\exp\pqty{\frac{\iunit}{ \hbar}\pqty{-(t_n-t_0)\frac{p^2}{2m}+p(q_n-q_0)}}.
\end{align}
$$
This is precisely $\iunit\hbar$ times the transition amplitude $A_{n,0}$.
Hence we learn from the path integral that
$$
\bra{q_\text{f},t_\text{f}}\comm{\hat q}{\hat p}\ket{q_\text{i},t_\text{i}}
=\iunit\hbar \braket{q_\text{f},t_\text{f}}{q_\text{i},t_\text{i}},
$$
which is fully consistent with canonical quantisation.