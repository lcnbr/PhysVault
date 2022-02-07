---
alias:
tags:
- qftII
- YM
---
When handling long expressions, the full gauge transformation rules are sometimes hard to handle. In physics one often considers only the infinitesimal transformations. When they apply everywhere, they are as good as finite transformation for practical purposes.

Finite transformations can be written using the exponential map of a matrix of transformation parameters $\alpha$
$$
U=\exp (i \alpha)
$$
Unitarity of $U$ translates to hermiticity of $\alpha$
$$
\alpha^{\dagger}=\alpha
$$
The transformation rules can be summarised as follows
$$
\begin{aligned}
\psi^{\prime} &=U \psi \\
\bar{\psi}^{\prime} &=\bar{\psi} U^{-1} \\
A_{\mu}^{\prime} &=U A_{\mu} U^{-1}+i U\left(\partial_{\mu} U^{-1}\right) \\
D_{\mu}^{\prime} &=U D_{\mu} U^{-1} \\
F_{\mu \nu}^{\prime} &=U F_{\mu \nu} U^{-1}
\end{aligned}
$$
Consider now the infinitesimal transformation where only the linear orders in $\delta \alpha$ are relevant
$$
U=1+i \delta \alpha+\ldots
$$
The infinitesimal transformation parameter $\delta \alpha$ must be hermitian, $\delta \alpha^{\dagger}=\delta \alpha .$ The infinitesimal transformation rules then read
$$
\begin{aligned}
\delta \psi^{\prime} &=i \delta \alpha \psi, \\
\delta \bar{\psi}^{\prime} &=-i \bar{\psi} \delta \alpha, \\
\delta A_{\mu} &=\left(\partial_{\mu} \delta \alpha\right)+i\left[\delta \alpha, A_{\mu}\right]=\left[D_{\mu}, \delta \alpha\right], \\
\delta D_{\mu} &=i\left[\delta \alpha, D_{\mu}\right], \\
\delta F_{\mu \nu} &=i\left[\delta \alpha, F_{\mu \nu}\right] .
\end{aligned}
$$
Importantly, a finite transformation by matrix conjugation with $U$ translates to commutators with $\delta \alpha$.