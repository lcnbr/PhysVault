---
sources:
- https://dlmf.nist.gov/10.25
aliases: 
tags: 
date created: Tuesday, May 10th 2022, 5:45:41 pm
date modified: Wednesday, May 11th 2022, 10:54:05 am
---
The [[.md|modified Bessel function of the Second Kind]] is the second standard solution to the [[modified Bessel's equation]]. The defining property of the second standard solution $K_{v}(z)$  is

$$
K_{v}(z) \sim \sqrt{\pi /(2 z)} \mathrm{e}^{-z},
$$
as $z \rightarrow \infty$ in $\abs{\operatorname{ph}z}  \leq \frac{3}{2} \pi-\delta\left(<\frac{3}{2} \pi\right)$. It has a branch point at $z=0$ for all $v \in \mathbb{C}$. The principal branch corresponds to the principal value of the square root, is analytic in $\mathbb{C} \backslash(-\infty, 0]$, and two-valued and discontinuous on the cut $\operatorname{ph}z=\pm \pi$.

# In terms of $I_v$[^1]


$$
K_{v}(z)=\frac{1}{2} \pi \frac{I_{-v}(z)-I_{v}(z)}{\sin (v \pi)}
$$
When $v$ is an integer limiting values are taken:

$$
K_{n}(z)=\frac{(-1)^{n-1}}{2}\left(\left.\frac{\partial I_{v}(z)}{\partial v}\right|_{v=n}+\left.\frac{\partial I_{v}(z)}{\partial v}\right|_{v=-n}\right)
$$

# Integral representations

1. $$\begin{align*}
K_{v}(x)=&\sec \left(\frac{1}{2} v \pi\right) \int_{0}^{\infty} \cos (x \sinh t) \cosh (v t) \dd{t}\\ =&
\csc \left(\frac{1}{2} v \pi\right) \int_{0}^{\infty} \sin (x \sinh t) \sinh (v t) \dd{t}
\end{align*}
$$
For $|\operatorname{Re} v|<1, x>0$
2. $$\begin{align*}
K_{v}(z)&=\frac{\pi^{\frac{1}{2}}\pqty{\frac{1}{2} z}^{v}}{\Gamma\pqty{v+\frac{1}{2}}} \int_{0}^{\infty} \mathrm{e}^{-z \cosh t}(\sinh t)^{2 v} \dd{t}\\
&=\frac{\pi^{\frac{1}{2}}\pqty{\frac{1}{2} z}^{v}}{\Gamma\pqty{v+\frac{1}{2}}} \int_{1}^{\infty} \mathrm{e}^{-z t}\pqty{t^{2}-1}^{v-\frac{1}{2}} \dd{t}
\end{align*}
$$
For $\operatorname{Re} v>-\frac{1}{2},|\operatorname{ph} z|<\frac{1}{2} \pi .$ ^3c41e3
3. 
$$
K_{v}(z)=\int_{0}^{\infty} \mathrm{e}^{-z \cosh t} \cosh (v t) \mathrm{d} t
$$ 
For $|\operatorname{ph} z|<\frac{1}{2} \pi .$
4. $$
K_{v}(z)=\frac{1}{2}\left(\frac{1}{2} z\right)^{v} \int_{0}^{\infty} \exp \left(-t-\frac{z^{2}}{4 t}\right) \frac{\mathrm{d} t}{t^{v+1}}
$$
For $|\operatorname{ph} z|<\frac{1}{4} \pi$




[[modified Bessel Function of the First Kind|^1]]