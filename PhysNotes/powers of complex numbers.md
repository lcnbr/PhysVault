---
aliases: 
tags: 
sources: 
- https://dlmf.nist.gov/4.2#iv
date created: Wednesday, May 11th 2022, 10:07:41 am
date modified: Wednesday, May 11th 2022, 10:13:52 am
---


The general $a^{\text {th }}$ power of $z\in \mathbb{C}$ is defined by
$$
z^{a}=\exp (a \operatorname{Ln} z)
$$
In particular, $z^{0}=1$, and if $a=n=1,2,3, \ldots$, then
$$
z^{a}=\underbrace{z \cdot z \cdots z}_{n \text { times }}=1 / z^{-a}
$$

In all other cases, $z^{a}$ is a multivalued function with branch point at $z=0$. The principal value is

$$
z^{a}=\exp (a \ln z)
$$
This is an analytic function of $z$ on $\mathbb{C} \setminus]-\infty, 0]$, and is two-valued and discontinuous on the cut $]-\infty, 0]$ , unless $a \in \mathbb{Z}$.

$$
\begin{gathered}
\left|z^{a}\right|=|z|^{\Re a} \exp (-(\mathfrak{I} a) \operatorname{ph} z), \\
\operatorname{ph}\left(z^{a}\right)=(\Re a) \operatorname{ph} z+(\mathfrak{J} a) \ln |z|,
\end{gathered}
$$

where $\operatorname{ph} z \in[-\pi, \pi]$ for the principal value of $z^{a}$, and is unrestricted in the general case. When $a$ is real

$$
\begin{aligned}
\left|z^{a}\right| &=|z|^{a} \\
\operatorname{ph}\left(z^{a}\right) &=a \operatorname{ph} z
\end{aligned}
$$
Unless indicated otherwise, it is assumed throughout the DLMF that a power assumes its principal value. With this convention,

$$
\mathrm{e}^{z}=\exp z
$$
but the general value of $\mathrm{e}^{z}$ is

$$
\mathrm{e}^{z}=(\exp z) \exp (2 k z \pi iu)
$$