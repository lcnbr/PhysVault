---
alias:
- spin
- angular momentum tensor
- total angular momentum
tag: SR GR
---
# Angular momentum tensor
Let us assume a system with [[energy-momentum tensor in SR#^conservedT|conserved]] [[energy-momentum tensor in SR|energy-momentum tensor]] $_{\nu} T^{\mu \nu}=0$. We can construct an **"angular momentum" tensor** which is also conserved

$$
M^{\alpha \mu \nu} \equiv x^{\mu} T^{\nu \alpha}-x^{\nu} T^{\mu \alpha}
$$

^angularMomentumTensor

Then

$$
\begin{aligned}
\pdv{}{ x^{\alpha}} M^{\alpha \mu \nu} = & \pdv{}{ x^{\alpha}}\left(x^{\mu} T^{\nu \alpha}-x^{\nu} T^{\mu \alpha}\right) \\
&=\delta^{\mu}_{\alpha} T^{\nu \alpha}-\delta^{\nu}_{\alpha} T^{\mu \alpha}+\cancel{x^{\mu} \pdv{}{ x^{\alpha}} T^{\nu \alpha}}-\cancel{x^{\nu} \pdv{}{ x^{\alpha}} T^{\mu \alpha}} \\
&=T^{\nu \mu}-T^{\mu \nu} \underset{\text { symmetry }}{=} 0
\end{aligned}
$$

# Total angular momentum
The **"total angular momentum"**

$$
J^{\mu \nu}=\int \dd[3]{x}\left(x^{\mu} T^{\nu 0}-x^{\nu} T^{\mu 0}\right)
$$

^totalAngularMomentum

is then conserved. 

# Spin
Notice that under translations $x^{\mu} \rightarrow (x^\mu)'=x^{\mu}+a^{\mu}$
$$
J^{\mu \nu} \rightarrow J^{\mu \nu}+\left(a^{\mu} P^{\nu}-a^{\nu} P^{\mu}\right) .
$$

(see [[energy-momentum tensor in SR#^conservedT|energy-momentum tensor]])
But there is a part of angular momentum which is intrinsic (always the same irrespective of shifts of the origin of the coordinate system). This part is called **spin**. It can be obtained via

$$
S_{\alpha} \equiv \frac{1}{2} \varepsilon_{\alpha \beta \gamma \delta} J^{\beta \gamma} V^{\delta}
$$

the with $V^{\delta} \equiv \frac{P^{\delta}}{\sqrt{P^{2}}}$ the total 4-velocity of the system defined by [[energy-momentum tensor in SR#^conservedT|total 4-momentum]]. We then get that under translations $x^{\mu} \rightarrow x^{\mu}+a^{\mu}$
$$
\begin{aligned}
S_{\mu} \rightarrow (S_{\mu})^{\prime} &=S_{\mu}+\frac{1}{2} \varepsilon_{\mu \nu \rho \sigma}\left(a^{\nu} P^{\rho}-a^{\rho} P^{\nu}\right) V^{\sigma} \\
&=S_{\mu}+\underbracket{\varepsilon_{\mu \nu \rho \sigma}}_{\text {antisymm. }} a^{\nu} \underbracket{\frac{P^{\rho} P^{\sigma}}{\sqrt{P^2}}}_{\text {symm. }} \\
&=S_{\mu}+0 .
\end{aligned}
$$
So the spin vector is invariant under translations (unlike orbital angular momentum).
In the center of mass frame of the system we have that
$$
\sum_{n} P_{n}=0 \implies P^{\mu}=\sqrt{P^{2}}(1, \vec{0}) \quad \text { and } \quad V^{\mu}=\frac{P^{\mu}}{\sqrt{P^{2}}}=(1, \vec{0}) \text {. }
$$
Then
$$
\begin{aligned}
S_{\mu} &=\frac{1}{2} \varepsilon_{\mu \alpha \beta \gamma} J^{\alpha \beta} V^{\gamma}=\frac{1}{2} \varepsilon_{\mu \alpha \beta 0} J^{\alpha \beta} 1 \\
\Rightarrow S_{0} &=\frac{1}{2} \varepsilon_{0 \alpha \beta 0} J^{\alpha \beta}=0 \\
S_{1} &=\frac{1}{2} \varepsilon_{1 \alpha \beta 0} J^{\alpha \beta}=\frac{1}{2} \varepsilon_{1230} J^{23}+\frac{1}{2} \varepsilon_{1320} J^{32} \\
&=\varepsilon_{1230} \frac{J^{23}-J^{32}}{2}=-\varepsilon_{0123} \frac{J^{23}-J^{32}}{2}
\end{aligned}
$$
Recall that
$$
\begin{aligned}
J^{23} &=\int \mathrm{d}^{3} x\left(x^{2} T^{30}-x^{3} T^{20}\right)=-J^{32} \\
\Rightarrow S_{1} &=\left(-\varepsilon_{0123}\right) J^{23}
\end{aligned}
$$
Also
$$
\begin{aligned}
\varepsilon_{0123} &=\eta_{0 \mu} \eta_{1 \nu} \eta_{2 \rho} \eta_{3 \sigma} \varepsilon^{\mu \nu \rho \sigma} \\
&=\eta_{00} \eta_{11} \eta_{22} \eta_{33} \varepsilon^{0123} \\
&=(+1)(-1)(-1)(-1)(+1)=-1,
\end{aligned}
$$
so that
$$
S_{1}=J^{23}
$$
Similarly, we find that $S_{2}=J^{31}$ and $S_{3}=J^{12}$. The spin vector has three components (rather than four) in every inertial frame. Indeed, we find that
$$
S_{\mu} V^{\mu}=\frac{1}{2} \varepsilon_{\mu \nu \rho \sigma} J^{\nu \rho} V^{\sigma} V^{\mu}=\frac{1}{2} \underbracket{\varepsilon_{\mu \nu \rho \sigma}}_{\text {antisymm. }} J^{\nu \rho} \underbracket{V^{\sigma} V^{\mu}}_{\text {symm. }}=0 .
$$
Therefore, the spin 4-vector always satisfies the constraint $S_{\mu} V^{\mu}=0$ reducing its independent components from four to three.

Note: In the above derivations we often used that a contraction of a symmetric $(S)$ and an antisymmetric $(A)$ tensor vanishes. Indeed
$$
\begin{aligned}
S_{\mu \nu} A^{\mu \nu} &=S_{\mu \nu} \frac{A^{\mu \nu}-A^{\nu \mu}}{2} \\
&=\frac{1}{2} S_{\mu \nu} A^{\mu \nu}-\frac{1}{2} S_{\mu \nu} A^{\nu \mu} \\
&=\frac{1}{2} S_{\mu \nu} A^{\mu \nu}-\frac{1}{2} S_{\nu \mu} A^{\mu \nu} \\
&=\frac{1}{2} \underbrace{\left(S_{\mu \nu}-S_{\nu \mu}\right)}_{=0} A^{\mu \nu}=0 .
\end{aligned}
$$