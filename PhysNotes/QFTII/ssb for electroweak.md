---
alias:
- electroweak lagrangian
tags:
- qftII
---
The electroweak theory is based on the [[gauge group]] $\mathrm{SU}(2) \times \mathrm{U}(1)$ (c.f [[unitary group]] and [[special unitary group]]). We denote the associated gauge potentials by the $2 \times 2$ traceless matrix $W_{\mu}$ and the field $B_{\mu}$ acting as a $2 \times 2$ matrix proportional to unity. The coupling constants for these groups are denoted by $g$ and $g^{\prime}$, respectively. We define the corresponding field strengths as
$$
\begin{aligned}
W_{\mu v} &=\partial_{\mu} W_{v}-\partial_{\nu} W_{\mu}-i g\left[W_{\mu}, W_{\nu}\right] \\
B_{\mu \nu} &=\partial_{\mu} B_{v}-\partial_{\nu} B_{\mu} .
\end{aligned}
$$
The contribution to the Lagrangian reads
$$
\mathcal{L}_{\text {gauge }}=-\frac{1}{2} \operatorname{Tr} W^{\mu \nu} W_{\mu \nu}-\frac{1}{4} B^{\mu \nu} B_{\mu \nu} .
$$
[[spontaneous symmetry breaking]] is achieved by a doublet of complex scalar fields denoted by $H$. It transforms in the (iso)spin- $1 / 2$ representation of $\mathrm{SU}(2)$ and has a (hyper)charge of $1 / 2$ of $\mathrm{U}(1)$. Hence, the [[YM covariant derivative|covariant derivative]] of $H$ is defined as
$$
D_{\mu} H=\partial_{\mu} H-i g W_{\mu} H-\frac{i}{2} g^{\prime} B_{\mu} H .
$$
We design the scalar potential to have a global minimum at $|H|^{2}=$ $v^{2} / 2$. The scalar contribution to the Lagrangian therefore reads (c.f. [[Higgs Mechanism]])
$$
\mathcal{L}_{\text {scalar }}=-\left(D^{\mu} H\right)^{\dagger}\left(D_{\mu} H\right)-\frac{1}{2} \lambda\left(H^{\dagger} H-\frac{1}{2} v^{2}\right)^{2} .
$$
We use the $\mathrm{SU}(2)$ gauge symmetry to rotate the scalar field to the configuration (c.f.[[Higgs Mechanism#Alternative parametrisation]])
$$
H(x)=\frac{1}{\sqrt{2}}\left(\begin{array}{c}
0 \\
v+\eta(x)
\end{array}\right)
$$
where $\eta(x)$ is a real field called the Higgs field. Let us furthermore parametrise the $\mathrm{SU}(2)$ gauge field as
$$
W=\frac{1}{2}\left(\begin{array}{cc}
+W^{0} & \sqrt{2} W^{+} \\
\sqrt{2} W^{-} & -W^{0}
\end{array}\right) \text {. }
$$
We can now extract the masses for the various fields by extracting the quadratic contributions to the Lagrangian
$$
\begin{aligned}
\mathcal{L}=&-\frac{1}{2} W^{-, \mu v} W_{\mu \nu}^{+}-\frac{1}{4} W^{0, \mu v} W_{\mu \nu}^{0}-\frac{1}{4} B^{\mu v} B_{\mu v} \\
&-\frac{1}{4} g^{2} v^{2} W^{-} \cdot W^{+}-\frac{1}{8} v^{2}\left(g W^{0}-g^{\prime} B\right)^{2} \\
&-\frac{1}{2}(\partial \eta)^{2}-\frac{1}{2} \lambda v^{2} \eta^{2}+\text { interactions. }
\end{aligned}
$$
Now we observe mixing between the fields $W^{0}$ and $B$. This can be resolved by a rotation of the basis of gauge fields 
$$
\left(\begin{array}{c}
A \\
Z^{0}
\end{array}\right)=\frac{1}{\sqrt{g^{2}+g^{\prime 2}}}\left(\begin{array}{cc}
g & g^{\prime} \\
-g^{\prime} & g
\end{array}\right)\left(\begin{array}{c}
B \\
W^{0}
\end{array}\right) .
$$

The coupling constants are commonly parametrised using the Weinberg angle $\theta_{\mathrm{W}}$
$$
g=g_{\mathrm{EW}} \cos \theta_{\mathrm{W}}, \quad g^{\prime}=g_{\mathrm{EW}} \sin \theta_{\mathrm{W}}
$$
After the rotation we find
$$
\begin{aligned}
\mathcal{L}=&-\frac{1}{2} W^{-, \mu v} W_{\mu \nu}^{+}-\frac{1}{4} Z^{0, \mu v} Z_{\mu v}^{0}-\frac{1}{4} F^{\mu v} F_{\mu v} \\
&-\frac{1}{4} g^{2} v^{2} W^{-} \cdot W^{+}-\frac{1}{8} v^{2} g_{\mathrm{EW}}^{2}\left(Z^{0}\right)^{2} \\
&-\frac{1}{2}(\partial \eta)^{2}-\frac{1}{2} \lambda v^{2} \eta^{2}+\text { interactions. }
\end{aligned}
$$
Now the mass terms are easily read off
$$
m_{W}=\frac{1}{2} g_{\mathrm{EW}} \cos \left(\theta_{\mathrm{W}}\right) v, \quad m_{\mathrm{Z}}=\frac{1}{2} g_{\mathrm{EW}} v, \quad m_{\eta}=\sqrt{\lambda} v
$$
The field $A$ remains massless.
**The masslessness of $A$ is due to the fact that a $U(1)$ subgroup of the gauge symmetry is unbroken.** This subgroup is a mixture of the original $\mathrm{U}(1)$ and one component of the $\mathrm{SU}(2)$. It represents the electromagnetic field. It makes sense to inspect the [[YM covariant derivative|covariant derivative]] of the Higgs field
$$
\begin{aligned}
g W+\frac{1}{2} g^{\prime} B=& \frac{g_{\mathrm{EW}}}{2}\left(\begin{array}{cc}
\cos \left(2 \theta_{\mathrm{W}}\right) Z^{0} & \sqrt{2} \cos \left(\theta_{\mathrm{W}}\right) W^{+} \\
\sqrt{2} \cos \left(\theta_{\mathrm{W}}\right) W^{-} & Z^{0}
\end{array}\right) \\
&+\frac{g_{\mathrm{EW}}}{2} \sin \left(2 \theta_{\mathrm{W}}\right)\left(\begin{array}{ll}
1 & 0 \\
0 & 0
\end{array}\right) A
\end{aligned}
$$
This tells us two things:
- The (lower) component of the scalar field representing the Higgs particle is uncharged. The (upper) component which has been gauged away has charge $+1$
$$
H=\left(\begin{array}{c}
H^{+} \\
H^{0}
\end{array}\right) .
$$
- In general, the electromagnetic charge is the sum of one component of the $\mathrm{SU}(2)$ isospin (in our choice of vacuum it is measured by $\frac{1}{2} \sigma_{3}$ for a isospin $1 / 2$ representation) and of the hypercharge.
- The coupling strength of the electromagnetic field is given by
$$
q=\frac{1}{2} g_{\mathrm{EW}} \sin \left(2 \theta_{\mathrm{W}}\right) .
$$