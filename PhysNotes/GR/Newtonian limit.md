---
alias: 
tag: GR physics
---

We shall now apply the equations of motion derived above to the limit of
- a slow moving particle
- inside a static and weak gravitational field.

# Slow moving
As the particle is slow moving, we have that
$$
\frac{\mathrm{d} x^{i}}{\mathrm{~d} \tau}=\frac{\mathrm{d} x^{i}}{\mathrm{~d} t} \frac{\mathrm{d} t}{\mathrm{~d} \tau}=\underbrace{v_{i}}_{\text {velocity }} \frac{\mathrm{d} t}{\mathrm{~d} \tau} \ll \frac{\mathrm{d} t}{\mathrm{~d} \tau} .
$$

Then the [[principle of equivalence#^eomGeneric|equations of motion]] simplify to

$$

\begin{align}

\implies \frac{\mathrm{d}^{2} x^{\alpha}}{\mathrm{d} t^{2}}\left(\frac{\mathrm{d} t}{\mathrm{~d} \tau}\right)^{2}+\Gamma^{\alpha}{ }_{00}\left(\frac{\mathrm{d} t}{\mathrm{~d} \tau}\right)^{2} \approx & 0 \\
\implies \frac{\mathrm{d}^{2} x^{\alpha}}{\mathrm{d} t^{2}} \approx &-\Gamma^{\alpha}{ }_{00}
\end{align}
$$

^eom

The [[affine connection]] is
$$
\Gamma^{\alpha}{ }_{00}=\frac{1}{2} g^{\alpha \rho}\left\{\frac{\partial g_{0 \rho}}{\partial x^{0}}+\frac{\partial g_{0 \rho}}{\partial x^{0}}-\frac{\partial g_{00}}{\partial x^{\rho}}\right\} .
$$

# Weak and Static field
As we approximate the field to be static, we neglect the time derivatives of the metric and thus,
$$
\Gamma^{\alpha}{ }_{00} \approx-\frac{1}{2} g^{\alpha i} \frac{\partial g_{00}}{\partial x^{i}} .
$$

^static

At last, we will use the approximation that the gravitational field is weak (e.g. far away from very massive bodies). We can write the metric as the [[Minkowski metric]] plus a small perturbation
$$
g_{\mu \nu}=\eta_{\mu \nu}+h_{\mu \nu}, \quad\left|h_{\mu \nu}\right| \text { small. }
$$

^weak

Then
$$
\begin{aligned}
\Gamma^{\alpha}{ }_{00} & \approx-\frac{1}{2} \eta^{\alpha i}+h^{\alpha i} \frac{\partial}{\partial x^{i}}\left(\eta_{00}+h_{00}\right) \\
& \approx-\frac{1}{2} \eta^{\alpha i} \frac{\partial h_{00}}{\partial x^{i}}
\end{aligned}
$$
The components are
$$
\begin{aligned}
&\Gamma^{0}{ }_{00} \approx-\frac{1}{2} \eta^{0 i} \frac{\partial h_{00}}{\partial x^{i}}=-\frac{1}{2} \frac{\partial h_{00}}{\partial t}=0 \\
&\Gamma^{j}{ }_{00} \approx-\frac{1}{2} \eta^{j i} \frac{\partial h_{00}}{\partial x^{i}}=\frac{1}{2} \frac{\partial h_{00}}{\partial x^{j}}
\end{aligned}
$$
Then, the [[#^eom|equations of motion]] become
$$
 \frac{\mathrm{d}^{2} t}{\mathrm{~d} \tau^{2}}=\Gamma^{0}{ }_{00}=0

$$
and
$$
\frac{\mathrm{d}^{2} x^{j}}{\mathrm{~d} t^{2}}=-\Gamma^{j}{ }_{00}=-\frac{1}{2} \frac{\partial h_{00}}{\partial x^{j}},
$$
or, in a vectorial form,
$$
\frac{\mathrm{d}^{2} \vec{x}}{\mathrm{~d} t^{2}}=-\vec{\nabla}\left(\frac{1}{2} h_{00}\right)
$$

We can compare this result with the Newtonian theory, which gives
$$
\frac{\mathrm{d}^{2} \vec{x}}{\mathrm{~d} t^{2}}=-\vec{\nabla} \phi
$$
with $\phi(\vec{x})$ being the gravitational potential. We naturally identify
$$
h_{00}=2 \phi+\text { constant }
$$
At infinity
$$
\overbracket{\lim _{|\vec{x}| \rightarrow \infty} h_{00}\left(\vec{x}\right)}^{0}=2 \overbracket{\lim _{|\vec{x}| \rightarrow \infty} \phi(\vec{x})}^{0}+\text { constant },
$$
we expect the gravitational potential to vanish and the metric to be [[Minkowski metric|Minkowskian]]. Therefore, we obtain a zero constant and we thus have

$$
h_{00}=2 \phi(\vec{x}) .
$$

^newtonianVariation

The metric element is

$$
g_{00}=1+2 \phi(\vec{x}) .
$$

^newtonMetric

As we know the metric defines the geometrical properties of spacetime. These properties have been altered due to gravity. 

Let us get an estimate of how much the metric changes with respect to the [[Minkowski metric]] on the surface of the earth. The potential at the surface is given by
$$
\begin{aligned}
\phi=-\frac{G M}{R} &=-\left(\frac{G M}{R^{2}}\right) R \\
&=-\underbrace{g}_{9,81 \mathrm{~m} / \mathrm{s}^{2}} \overbrace{R}^{6371 \mathrm{~km}} \\
\stackrel{\text { natural units }}{=} &-\frac{g R}{c^{2}} \approx-\frac{10 \cdot 6 \cdot 10^{6}}{\left(3 \cdot 10^{8}\right)^{2}} \\
& \approx-0.7 \cdot 10^{-9} .
\end{aligned}
$$
So the deviation from [[Minkowski metric|Minkowskian]] geometry of spacetime due to the gravitational field of the earth is tiny on its surface. This renders direct experimental confirmations of General Relativity difficult. But they are not impossible and by now the theory has been tested in various ways.