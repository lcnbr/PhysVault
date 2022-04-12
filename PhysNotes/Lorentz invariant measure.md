---
---

$\dd[4]p$ is [[Lorentz group|Lorentz invariant]] but we usually only want positive energy and thus restrict to the hyperboloid $p^{2}=\left(p^{0}\right)^{2}-|\mathbf{p}|^{2}=\mu^{2}, p^{0}>0$. To restrict it to the hyperboloid, multiply it by the Lorentz invariant factor $\delta\left(p^{2}-\mu^{2}\right) \theta\left(p^{0}\right)$. That yields our relativistic measure on the hyperboloid
$$
\int_{p^{0}=-\infty}^{\infty} d p^{0}\left\{d^{3} \mathbf{p} \delta\left(p^{2}-\mu^{2}\right) \theta\left(p^{0}\right)\right\}=\frac{d^{3} \mathbf{p}}{2 \omega_{\mathbf{p}}}
$$
where
$$
\omega_{\mathbf{p}}=\sqrt{|\mathbf{p}|^{2}+\mu^{2}}, \quad p^{\mu}=\left(\omega_{\mathbf{p}}, \mathbf{p}\right)
$$
The equality follows from the identity $\delta(f(x))=\sum_{i} \frac{\delta\left(x-a_{i}\right)}{\left|f^{\prime}\left(a_{i}\right)\right|}$ where $\left\{a_{i}\right\}$ are the zeroes of $f(x)$. Then
$$
\delta\left(p^{2}-\mu^{2}\right)=\delta\left(\left(p^{0}\right)^{2}-\omega_{\mathbf{p}}^{2}\right)=\frac{\delta\left(p^{0}-\omega_{\mathbf{p}}\right)}{2 \omega_{\mathbf{p}}}+\frac{\delta\left(p^{0}+\omega_{\mathbf{p}}\right)}{2 \omega_{\mathbf{p}}}
$$
The $\theta\left(p^{0}\right)$ factor kills the second delta function, and integrating over $p^{0}$ gives just the factor $\left(2 \omega_{\mathbf{p}}\right)^{-1}$, times the remaining $d^{3} \mathbf{p}$. Similarly, one can show $d^{3} \mathbf{x} \delta\left(|\mathbf{x}|^{2}-R^{2}\right)=\frac{1}{2} R \sin \theta d \theta d \phi$.