---
alias:
- electrodynamics
- Maxwell's equations
tag: GR physics
---


# Without gravity
Let us now look at Maxwell's equations.
In the absence of gravity, for an inertial observer, we have


$$
\vec{\nabla} \cdot \vec{E} =\rho, 
$$

^divE

$$
\vec{\nabla} \times \vec{B} =\frac{\partial \vec{E}}{\partial t}+\vec{j}, 
$$

^curlB

$$
\vec{\nabla} \cdot \vec{B} =0, 
$$

^divB

$$
\vec{\nabla} \times \vec{E} =-\frac{\partial \vec{B}}{\partial t} .

$$

^curlE

The $\vec{E}, \vec{B}$ fields make up the components of the field strength tensor
$$
F^{\mu \nu}:\left\{\begin{array}{l}
E_{i}=F^{0 i}, \\
B_{k}=\frac{1}{2} \varepsilon_{i j k} F^{i j}\left(\text { e.g. } B_{2}=F^{31}, B_{3}=F^{12}\right) .
\end{array}\right.
$$
with $F^{\mu \nu}=-F^{\nu \mu}$. Also $J^{\mu} \equiv(\rho, \vec{j})$. Substituting into [[#^divE]] we have
$$
\begin{aligned}
\frac{\partial}{\partial x^{i}} E_{i} &=J^{0} \Rightarrow \frac{\partial}{\partial x^{i}} F^{0 i}=J^{0} \\
\Rightarrow \frac{\partial\cancelto{0}{ F^{00}}}{\partial x^{0}}+\frac{\partial}{\partial x^{i}} F^{0 i}=J^{0} & \Rightarrow \frac{\partial F^{0 \mu}}{\partial x^{\mu}}=J^{0} .
\end{aligned}
$$
Similarly, [[#^curlB]] becomes
$$
\begin{aligned}
\varepsilon_{i j k} \frac{\partial}{\partial x^{j}}\left(\frac{1}{2} \varepsilon_{k l m} F^{l m}\right) &=-\frac{\partial F^{0 i}}{\partial x^{0}}+J^{i} \\
\Rightarrow \quad \begin{array}{ll}
\delta_{i l} & \delta_{i m} \\
\delta_{j l} & \delta_{j m}
\end{array} \frac{\partial}{\partial x^{j}} \frac{F^{l m}}{2} &=+\frac{\partial F^{0 i}}{\partial x^{0}}+J^{i} \\
\Rightarrow \frac{\partial}{\partial x^{j}}\left(\frac{F^{i j}-F^{j i}}{2}\right) &=-\frac{\partial F^{i 0}}{\partial x^{0}}+J^{i} \\
\Rightarrow \frac{\partial F^{i 0}}{\partial x^{0}}+\frac{\partial F^{i j}}{\partial x^{j}} &=J^{i} \Rightarrow \frac{\partial F^{i \mu}}{\partial x^{\mu}}=J^{i} .
\end{aligned}
$$
Putting the last two results together, we have

$$
\frac{\partial F^{\mu \nu}}{\partial x^{\mu}}=-J^{\nu}
$$

^Fup

[[#^divB]] becomes
$$
\begin{aligned}
0 &=\vec{\nabla} \cdot \vec{B}=\frac{\partial}{\partial x^{i}} B_{i}=\frac{1}{2} \frac{\partial}{\partial x^{i}} \varepsilon_{i j k} F^{j k} \\
0 &=\varepsilon_{i j k} \frac{\partial}{\partial x^{i}} F^{j k} \\
\Rightarrow 0 &=\frac{\partial}{\partial x^{1}} F^{23}+\frac{\partial}{\partial x^{2}} F^{31}+\frac{\partial}{\partial x^{3}} F^{12} .
\end{aligned}
$$
[[#^curlE]] gives an analogous result. Collectively, [[#^divB]] and [[#^curlE]] become

$$
\varepsilon^{\alpha \beta \gamma \delta} \frac{\partial}{\partial x^{\beta}} F_{\gamma \delta}=0$$

^LeviCivitaForm

$$\implies\frac{\partial}{\partial x^{\alpha}} F_{\beta \gamma}+\frac{\partial}{\partial x^{\beta}} F_{\gamma \alpha}+\frac{\partial}{\partial x^{\gamma}} F_{\alpha \beta}=0
$$

^Fdown

## Gauge potentials

Note that for $\alpha . \beta . \gamma$ all different, Eq. [[#^Fdown]] is the same as [[#^LeviCivitaForm]] for instance, setting $\alpha=0$ in [[#^LeviCivitaForm]] gives the same result as setting $\alpha \beta \gamma=123$ in [[#^Fdown]]. On the other hand, for two indices equal, Eq. [[#^Fdown]] is an identity; for instance, if $\beta=\gamma$ then [[#^Fdown]] reads
$$
\frac{\partial}{\partial x^{\beta}} F_{\beta \alpha}+\frac{\partial}{\partial x^{\beta}} F_{\alpha \beta}=0 \quad \text { (not summed) }
$$
and this is identically true because $F_{\alpha \beta}=-F_{\beta \alpha}$
Equation [[#^LeviCivitaForm]] allows us to represent $F_{\gamma \delta}$ as a "curl"' of a four-vector $A_{\gamma}$ :


$$
F_{\gamma \delta}=\frac{\partial}{\partial x^{\gamma}} A_{\delta}-\frac{\partial}{\partial x^{\delta}} A_{\gamma}
$$

^gaugeFormfieldStrength

With this form, [[#^Fup|rest of Maxwell's equations]]  reduce to

$$
\square^{2} A_{\alpha}- \pdv{}{x^\alpha}{x^\beta}A^\beta=-J_{\alpha}
$$

^PotMax

Where $\square^2$ or $\partial^2$ is the [[D'Alambert operator in GR|d'Alembertian]]:

$$
\partial^2=\square^{2}=\eta^{\alpha \beta} \frac{\partial}{\partial x^{\beta}} \frac{\partial}{\partial x^{\alpha}}=\nabla^{2}-\frac{\partial^{2}}{\partial t^{2}}
$$

^dAlembertian

is also invariant.


# With gravity
We will now attempt to generalize [[#^Fup]] and [[#^Fdown]] in the presence of gravity. Our method will be to replace derivatives with covariant derivatives as well as the Minkowskian metric with the gravitational metric, as described in [[covariant derivative#Importance]]. So the Maxwell equations should be substituted by
$$
\begin{aligned}
F^{\mu \nu}{}_{; \mu} &=J^{\nu}, \\
F_{\mu \nu ; \rho}+F_{\nu \rho ; \mu}+F_{\rho \mu ; \nu} &=0 .
\end{aligned}
$$

There is a simplification that we can make due to the fact that the field strength tensor is antisymmetric. Writing the covariant derivatives out we have
$$
\begin{aligned}
&\frac{\partial}{\partial x^{\rho}} F_{\mu \nu}
+\frac{\partial}{\partial x^{\mu}} F_{\nu \rho}
+\frac{\partial}{\partial x^{\nu}} F_{\rho \mu} \\
&\quad
\cancel{-\Gamma^{\alpha}{ }_{\nu \rho} F_{\mu \alpha}}
\bcancel{-\Gamma^{\alpha}{ }_{\mu \rho} F_{\alpha \nu}}
\bcancel{-\Gamma^{\alpha}{ }_{\mu \rho} F_{\nu \alpha}}
\cancel{\bcancel{-\Gamma^{\alpha}{ }_{\nu \mu} F_{\alpha \rho}}}
\cancel{-\Gamma^{\alpha}{ }_{\rho \nu} F_{\alpha \mu}}
\cancel{\bcancel{-\Gamma^{\alpha}{ }_{\mu \nu} F_{\rho \alpha}}}=0 \\
\end{aligned}
$$
$$
\implies \frac{\partial}{\partial x^{\rho}} F_{\mu \nu}+\frac{\partial}{\partial x^{\mu}} F_{\nu \rho}+\frac{\partial}{\partial x^{\nu}} F_{\rho \mu}=0

$$
The divergence of the field strength tensor is
$$
\begin{aligned}
F^{\mu \nu}{ }_{; \mu} &=\frac{\partial F^{\mu \nu}}{\partial x^{\mu}}
+\Gamma^\mu{}_{\mu \rho} F^{\rho \nu}
+\cancelto{ 0}{\underbracket{\Gamma^\nu{}_{\mu \rho} F^{\mu  \rho} }_{\text {sym. } \times \text { antisym. }}} \\
&=\frac{\partial F^{\mu \nu}}{\partial x^{\mu}}
+\Gamma^{\mu}{ }_{\mu \rho} F^{\rho \nu} .
\end{aligned}
$$
Then, analogously to what we did for the [[covariant divergence|divergence]] of a contravariant vector, we have
$$
F^{\mu \nu}{ }_{; \mu}=\frac{1}{\sqrt{g}} \frac{\partial}{\partial x^{\mu}}\left(\sqrt{g} F^{\mu \nu}\right),
$$
and the remaining Maxwell equations become
$$
\begin{align}
 \frac{1}{\sqrt{g}} \frac{\partial}{\partial x^{\mu}}\left(\sqrt{g} F^{\mu \nu}\right)=-J^{\nu} \\
\implies \frac{\partial}{\partial x^{\mu}}\left(\sqrt{g} F^{\mu \nu}\right)=-\sqrt{g} J^{\nu}
\end{align}
$$
Acting with normal derivative on the above, we find
$$
\begin{aligned}
\underbracket{\frac{\partial^{2}}{\partial x^{\nu} \partial x^{\mu}}}_{\text {symm. }} & \underbracket{\left(\sqrt{g} F^{\mu \nu}\right)}_{\text {antisymm. }}=-\frac{\partial}{\partial x^{\nu}}\left(\sqrt{g} J^{\nu}\right) \\
\implies & 0=\frac{\partial}{\partial x^{\nu}}\left(\sqrt{g} J^{\nu}\right) \\
\implies & 0=\frac{1}{\sqrt{g}} \frac{\partial}{\partial x^{\nu}}\left(\sqrt{g} J^{\nu}\right) \\
\implies & J^\nu{}_{; \nu}=0
\end{aligned}
$$
which is the charge conservation equation in General Relativity. ([[covariant divergence|divergence]] theorem)
Exercise: Show that the above equation leads to the conservation of the electric charge.


