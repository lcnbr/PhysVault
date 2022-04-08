---
---

We want a manifestly [[Lorentz group|Lorentz invariant]] momentum state. Starting from the completeness relations:

$1=\int \dd[3]{\mathbf{p}}\dyad{\mathbf{p}}$

Since $\dd[3]{\mathbf{p}}$ is not [[Lorentz group|Lorentz invariant]] we use the [[Lorentz invariant measure]]:

$1=\int \frac{\dd[3]{\mathbf{p}}}{2 \omega_\mathbf{p}} \dyad{p'} \iff \ket{p'}=\sqrt{2 \omega_\mathbf{p}}\ket{\mathbf{p}}$

But since we want all the fourrier normalisation in momentum space we additionally normalise by $2 \pi$ :

$1=\int \frac{\dd[3]{\mathbf{p}}}{(2 \pi)^3 2 \omega_\mathbf{p}}=\int \dd[4]{p} \delta(p^{2}-\mu^{2}) \theta(p^{0}) \dyad{p} \iff \ket{p}=\sqrt{(2 \pi)^3}\sqrt{2 \omega_\mathbf{p}}\ket{\mathbf{p}}$