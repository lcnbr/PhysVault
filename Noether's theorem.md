---
alias:
- Noether charge
- Noether current
---
Suppose the action $S[\Psi]$ is invariant under a global symmetry
$$
0=\frac{\delta S}{\delta \alpha}=\int \mathrm{d} x^{D} \frac{\delta \Psi(x)}{\delta \alpha} \frac{\delta S}{\delta \Psi(x)}
$$
Vanishing of the integral on the r.h.s. implies that the integrand is a total derivative. ${ }^{3}$ We define the Noether current $N^{\mu}(x)$ implicitly by generating the total derivative
$$
\frac{\delta \Psi(x)}{\delta \alpha} \frac{\delta S}{\delta \Psi(x)}=: \partial_{\mu} N^{\mu}(x)
$$
This current is conserved on solutions of the [[Euler-Lagrange equations]] because the l.h.s. of this equation vanishes
$$
\partial_{\mu} N^{\mu}=\frac{\delta \Psi}{\delta \alpha} \frac{\delta S}{\delta \Psi}=0
$$

# Noether charge
From a constant current $\partial_{\mu} N^{\mu}=0$ we  can expand to
$$
\partial_{0} N^{0}+\nabla \cdot \boldsymbol{N}=0
$$
where $N$ is the 3-vector spatial part of $N^{\mu}$. Integrating this over some fixed volume $V$ we get from Gauss's theorem the condition
$$
\begin{aligned}
\partial_{0} \int_{V} \dd[3] {x} N^{0} &=-\int_{V} \dd[3] {x} \nabla \cdot \boldsymbol{N} \\
&=-\int_{S} \dd[2]{S}  \hat{\boldsymbol{n}} \cdot \boldsymbol{N}
\end{aligned}
$$
where $S$ is the surface bounding $V$. In other words, the flow of $\boldsymbol{N}$ across the boundary (note the negative sign) is balanced by the rate of change of $N^{0}$ inside $V$. We can therefore think of $N^{0}$ as some conserved 'charge'-like quantity and $N$ as the current of this quantity. If we assume that the current falls to zero at infinity, then the current across the surface at infinity is zero, so
$$
\partial_{0} \int \dd[3] {x} N^{0}=0
$$
That is, the total quantity $\int_{V} \dd[3]{x} N^{0}=Q$ is conserved. This is what we call **Noether charge**