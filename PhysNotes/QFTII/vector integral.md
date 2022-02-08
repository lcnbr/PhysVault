---
alias:
tags:
- qftII
---
For models with spin, we will have to deal with vectors in the numerator of the [[basic integral]], for example 
$$
\begin{aligned}
I_{n}^{\mu}(X) &=\int \frac{-i \mathrm{~d} \ell^{D}}{(2 \pi)^{D}} \frac{\ell^{\mu}}{\left(\ell^{2}+X-i \epsilon\right)^{n}}=0 \\
I_{n}^{\mu v}(X) &=\int \frac{-i \mathrm{~d} \ell^{D}}{(2 \pi)^{D}} \frac{\ell^{\mu} \ell^{v}}{\left(\ell^{2}+X-i \epsilon\right)^{n}}
\end{aligned}
$$
Evidently, the first integral vanishes because the integrand is an antisymmetric function. An alternative derivation uses Lorentz symmetry: The result must transform as a vector. However, there is no vector at our disposal after the integral is done. Hence the result must vanish. The second integral can be performed by a similar trick: The only Lorentz-invariant bi-vector is the metric tensor $\eta_{\mu \nu}$, so the integral must be proportional to it. To find the factor of proportionality, take the trace with $\eta_{\mu \nu}$. This yields using [[basic integral#^5ee300]]
$$
\begin{aligned}
I_{n}^{\mu v}(X) &=\frac{\eta^{\mu v}}{D} \eta_{\rho \sigma} I_{n}^{\rho \sigma}(X)=\frac{\eta^{\mu v}}{D}\left(I_{n-1}(X)-X I_{n}(X)\right) \\
&=\frac{\Gamma(n-1-D / 2)}{2(4 \pi)^{D / 2} \Gamma(n)} \frac{\eta^{\mu v}}{(X-i \epsilon)^{n-1-D / 2}} .
\end{aligned}
$$
Note that one has to pay attention to the dimensionality of vectors and matrices. For consistency all vectors should be defined in $D=$ $4-2 \epsilon$ dimensions. Likewise the [[Minkowski metric]] must be defined in $D=4-2 \epsilon$ dimensions, which implies that its trace equals $D,$
$$
\delta_{\mu}^{\mu}=\eta_{\mu \nu} \eta^{\mu \nu}=D=4-2 \epsilon
$$
Although, the difference between $D$ and 4 is small, it can be important in the case of divergences which contribute factors of $1 /(D-4)$.