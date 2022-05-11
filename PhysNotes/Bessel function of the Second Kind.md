---
aliases: 
- Weber's function
tags: 
sources:
- https://dlmf.nist.gov/10.2#E4
date created: Wednesday, May 11th 2022, 10:18:05 am
date modified: Wednesday, May 11th 2022, 10:21:02 am
---

$$
Y_{v}(z)=\frac{J_{v}(z) \cos (v \pi)-J_{-v}(z)}{\sin (v \pi)}
$$
Where $J_v(z)$ is a [[Bessel Function of the First Kind]]. When $v$ is an integer the right-hand side is replaced by its limiting value:
$$
Y_{n}(z)=\left.\frac{1}{\pi} \frac{\partial J_{v}(z)}{\partial v}\right|_{v=n}+\left.\frac{(-1)^{n}}{\pi} \frac{\partial J_{v}(z)}{\partial v}\right|_{v=-n}
$$
Whether or not $v$ is an integer $Y_{v}(z)$ has a branch point at $z=0$. The principal branch corresponds to the principal branches of $J_{\pm v}(z)$ with a cut in the $z$-plane along the interval $(-\infty, 0]$.

Except in the case of $J_{\pm n}(z)$, the principal branches of $J_{v}(z)$ and $Y_{\nu}(z)$ are two-valued and discontinuous on the cut ph $z=\pm \pi$.
Both $J_{v}(z)$ and $Y_{v}(z)$ are real when $v$ is real and ph $z=0$.
For fixed $z(\neq 0)$ each branch of $Y_{v}(z)$ is entire in $v$.