---
alias: 
- relativistic energy
- momentum four-vector
- momentum 4-vector
tags: SR GR
---

From [[particle dynamics in SR]] and the [[relativistic particle]] we define
$$
p^{\mu}=m \frac{\mathrm{d} x^{\mu}}{\mathrm{d} \tau}
$$
which seems like an intuitive generalization of $\vec{p}=\frac{\mathrm{d} \vec{x}}{\mathrm{~d} E}$ from classical mechanics. Under a [[Lorentz transformation]]
$$
p^{\prime \mu}=\Lambda^{\mu}{}_{\nu} p^{\nu} .
$$
In the [[instantaneous rest frame|rest frame]]
$$
p_{\text{rest}}^{\mu}=m \dv{x^{\mu}}{t} \Rightarrow\left\{\begin{array}{l}
p^{0}=m, \\
p^{i}=0 .
\end{array}\right.
$$
In the [[Lorentz transformation#^boost|boosted]] frame where the particle has a velocity $\vec{v}$, we have
$$
\begin{aligned}
& p^{\mu}=\Lambda(\vec{v})^{\mu}{}_{\nu} p_{\text {rest }}^{\nu} \\
\implies & p^{0}=m \gamma \\
\implies & p^{i}=m \gamma v_{i}
\end{aligned}
$$
Let us analyze the time component
$$
p^{0}=m \gamma=\frac{m}{\sqrt{1-\vec{v}^{2}}}=m+\overbracket{\frac{1}{2} m \vec{v}^{2}}^{\text {kin. en.}}+\mathcal{O}\left(\vec{v}^{4} .\right)
$$
We will identify $p^{0}$ with the energy of the particle. We have
$$

E =p^{0}=m \gamma, 
\quad \vec{p} =m \gamma \vec{v} .
$$
We also have
$$
E^{2}-\vec{p}^{2}=m^{2} \gamma^{2}\left(1-\vec{v}^{2}\right)=m^{2},
$$
or
$$
E=\sqrt{m^{2}+\vec{p}^{2}}
$$
Finally, let us recall that
$$
f^{\mu}=m \frac{\mathrm{d}^{2} x^{\mu}}{\mathrm{d} \tau^{2}}=\frac{\mathrm{d} p^{\mu}}{\mathrm{d} \tau} .
$$
Remark: For us the mass $m$  is always a constant physical parameter. We will not combine $m \gamma=\frac{m}{\sqrt{1-\vec{v}^{2}}}$ into a "relativistic mass" $\bcancel{\cancel{\vec{m}(\vec{v})=\frac{m}{\sqrt{1-\vec{v}^{2}}}}}$. While this can give us a nice qualitative picture to describe various phenomena with words, it can also cause confusion.