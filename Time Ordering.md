---
alias:
tags:
- qftII
---
# Time Ordering

Suppose we have $n$ operators $\hat O_k$ at times $t_k$, respectively, with $t_\text{f}>t_n>\ldots>t_2>t_1>t_\text{i}$. We [[single operator insertion|insert]] them into the transition amplitude and obtain a path integral with $n$ operator insertions
$$
\begin{align}
&
\bra{q_\text{f},t_\text{f}}\hat O_n\ldots\hat O_2\hat O_1\ket{q_\text{i},t_\text{i}}.
\\
&=\int \mathcal{D}{q} \mathcal{D}{p}
O_1(t_1)
O_2(t_2)
\ldots
O_n(t_n)
\exp\pqty{\frac{\iunit}{ \hbar}S_\text{f,i}[q,p]}.
\end{align}
$$
It is crucial that all the operators are in proper time order. Only then all the time evolution operators $U(t_k,t_{k-1})$ will shift time forward as in the above derivation of the path integral.

Conversely, a set of operators insertions in the path integral corresponds to a time-ordered product of quantum operators inserted into the transition amplitude
$$
\begin{align}
&\int \mathcal{D}{q} \mathcal{D}{p}
\prod_{k=1}^n
O_k(t_k)
\exp\pqty{\frac{\iunit}{ \hbar}S_\text{f,i}[q,p]}.
\\
&=
\bra{q_\text{f},t_\text{f}}\mathrm{T}\bqty{\hat O_1\hat O_2\ldots \hat O_n}\ket{q_\text{i},t_\text{i}}.
\end{align}
$$
Hence the path integral performs time-ordering automatically.^[To compute expectation values of quantum operators
which are not in proper time order with the path integral
is more laborious, but could be handled
by integrating over the fields
in the intermediate regions of time more than once
in order to go back and forth in time.]

In some sense, the time ordering enters by the very definition
of the path integral:
- There is precisely one position for each time,
- the trajectory strictly moves forward in time,
- there cannot be loops in time.
This ordering of times is forced upon the operator insertions.