---
alias:
tag: GR physics
---

Einstein's equations
![[Einstein's field equations#^EinsteinfieldEq|Einstein's equations]]
or, equivalently,
![[Einstein's field equations#^EinsteinEqWithoutR|Einstein's equation]]

are non linear partial differential equations, which are hard to solve analytically. They can be tackled in a more general framework numerically (with expensive computations) and when appropriate with approximate methods, expanding typically around the limit of weak gravitational fields.

We will now focus to a particular case where an analytic solution, the so called Schwarzschild solution can be found. It corresponds to the physical situation of a spherical or point-like object with a mass $M$ which produces an isotropic gravitational field.
![[Pasted image 20220206164744.png#leftwrap|200]]$T_{\mu \nu}=0$ except at center,
static and isotropic metric.


We will solve Einsteins equations away from the massive object, where the energy momentum tensor vanishes. The equations then reduce to
$$
R_{\mu \nu}=0 .
$$
Proper time intervals will be given in terms of the metric as

![[principle of equivalence#^prorTimeGeneric|PoE]]

Due to the static configuration we expect that
$$
\frac{\partial}{\partial t} g_{\mu \nu}=0 \text {, }
$$
and thus
$$
g_{\mu \nu}(x)=g_{\mu \nu}(\vec{x}) .
$$
Due to isotropy, the proper time interval should be rotationally invariant. Its space-like part can then be made of three-dimensional scalar products
$$
\mathrm{d} \vec{x}^{2}, \vec{x}^{2} \equiv r^{2}, \vec{x} \cdot \mathrm{d} \vec{x} .
$$
A generic Ansatz is the following

$$
\dd{\tau}^{2}=\alpha(r) \dd{t}^{2}-\beta(r) \dd{t}(\vec{x} \cdot \mathrm{d} \vec{x})-\gamma(r)(\vec{x} \cdot \mathrm{d} \vec{x})^{2}-\delta(r) \mathrm{d} \vec{x}^{2} .
$$

^genericAnstaz

We can now change to spherical coordinates
$$
x^{3}=r \cos \theta, x^{2}=r \sin \theta \sin \varphi, x^{1}=r \sin \theta \cos \varphi \text {. }
$$
This yields using [[contravariance and covariance]]
$$
\begin{aligned}
\vec{x}^{2} &=r^{2}, \\
\vec{x} \cdot \mathrm{d} \vec{x} &=r \dd{r}, \\
\mathrm{~d} \vec{x}^{2} &=\dd{r}^{2}+r^{2}\left(\dd{\theta}^{2}+\sin ^{2} \theta \dd{\varphi}^{2}\right) .
\end{aligned}
$$
The metric becomes
$$
\dd{\tau}^{2}=\alpha(r) \dd{t}^{2}-\beta(r) r \dd{r} \dd{t}-\gamma(r) \dd{r}^{2}-\delta(r)\left(\dd{r}^{2}+r^{2} \dd{\theta}^{2}+r^{2} \sin ^{2} \theta \dd{\varphi}^{2}\right) .
$$
Let us now make a change of time coordinates of the form
$$
t \rightarrow t^{\prime}=t+f(r) .
$$
Then
$$
\dd{t} \rightarrow \dd{t}^{\prime}=\frac{\partial(t+f(r))}{\partial t} \dd{t}+\frac{\partial(t+f(r))}{\partial r} \dd{r}=\dd{t}+f^{\prime}(r) \dd{r} .
$$
Then the [[#^genericAnstaz]] becomes
$$
\begin{aligned}
\dd{\tau}^{2} &=
\alpha(r)\left(\dd{t}^{\prime}-f(r)\right) \dd{r}^{2}
-\beta(r) r\left(\dd{t}^{\prime}-f(r)\right) \dd{r}
-\gamma(r) \dd{r}^{2}-\delta(r) r^{2}\left(\dd{\theta}^{2}+\sin ^{2} \theta \dd{\varphi}^{2}\right) \\

&=\alpha(r) \dd{t}^{\prime 2}
-r \dd{t}^{\prime} \dd{r}\left(2 f(r)+\beta(r)\right)
-\omega(r) \dd{r}^{2}
-\delta(r) r^{2}\left(\dd{\theta}^{2}+\sin ^{2} \theta \dd{\varphi}^{2}\right) .
\end{aligned}
$$
We can now pick a $f(r)$ such that
$$
2 f(r)+\beta(r)=0 .
$$
With this choice of coordinate system, the metric simplifies to
$$
\dd{\tau}^{2}=\alpha(r) \dd{t}^{\prime 2}-\omega(r) \dd{r}^{2}-\delta(r) r^{2}\left(\dd{\theta}^{2}+\sin ^{2} \theta \dd{\varphi}^{2}\right) .
$$
We can now perform one more change of variables
$$
r \rightarrow r^{\prime}=\frac{r}{\sqrt{\delta(r)}},
$$
anrename all primed coordinates to the unprimed versions for clarity. Then the metric will simplify further, to its "standard form"

$$
\dd{\tau}^{2}=B(r) \dd{t}^{2}-A(r) \dd{r}^{2}-r^{2}\left(\dd{\theta}^{2}+\sin ^{2} \theta \dd{\varphi}^{2}\right) .
$$

^standardInt

We can now read off the components of the metric from the above equation. We have the following non-zero terms

$$
g_{t t}=B(r), g_{r r}=-A(r), g_{\theta \theta}=-r^{2}, g_{\varphi \varphi}=-r^{2} \sin ^{2} \theta .
$$

^metricTerms

All other terms vanish. The metric should satisfy Einstein's field equations which take the form
$$
R_{\mu \nu}=0 .
$$

# Computing the [[Ricci tensor]] of the Schwarzschild metric
In what follows, we will construct the Ricci tensor which corresponds to the metric of [[#^metricTerms]] to do this we need to compute the [[affine connection]]. The [[affine connection]] requires the inverse of the metric. It is also diagonal with elements

$$
g^{t t}=1 / B(r), g^{r r}=-1 / A(r), g^{\theta \theta}=-1 / r^{2}, g^{\varphi \varphi}=-\frac{1}{r^{2} \sin ^{2} \theta} .
$$
This constrains the $A(r)$ and $B(r)$ functions up to a constant. The non-vanishing elements of the affine connection,
$$
\Gamma_{\alpha \beta}^{\mu}=\frac{1}{2} g^{\mu \rho}\left[\frac{\partial g_{\alpha \rho}}{\partial x^{\beta}}+\frac{\partial g_{\rho \beta}}{\partial x^{\alpha}}-\frac{\partial g_{\alpha \beta}}{\partial x^{\rho}}\right]
$$
are

$$
\begin{aligned}
\Gamma_{t r}^{t}=\Gamma_{r t}^{t} &=\frac{\dv{}{r} B(r)}{2 B(r)} \\

\Gamma_{t t}^{r} &=\frac{\dv{}{ r} B(r)}{2 A(r)} \\

\Gamma_{r r}^{r} &=\frac{\dv{}{ r} A(r)}{2 A(r)} \\

\Gamma_{\theta \theta}^{r} &=-\frac{r}{A(r)} \\

\Gamma_{\varphi \varphi}^{r} &=-\frac{r\left(\sin ^{2}(\theta)\right)}{A(r)} \\

\Gamma_{r \theta}^{\theta}=\Gamma_{\theta r}^{\theta} &=\frac{1}{r} \\

\Gamma_{r \varphi}^{\varphi}=\Gamma_{\varphi r}^{\varphi} &=\frac{1}{r} \\

\Gamma_{\varphi \varphi}^{\theta} &=-\sin (\theta) \cos (\theta) \\

\Gamma_{\varphi \theta}^{\varphi}=\Gamma_{\theta \varphi}^{\varphi} &=\frac{\cos (\theta)}{\sin (\theta)}
\end{aligned}
$$

^AffineconnectionComp

With the [[affine connection]] at hand, we find that the [[Ricci tensor]] has the following non-vanishing matrix elements
$$
\begin{aligned}
R_{\varphi \varphi} &=\sin ^{2} \theta R_{\theta \theta} \\
R_{\theta \theta} &=\frac{r\left(\dv{}{r} B(r)\right)}{2 A(r) B(r)}-\frac{r\left(\dv{}{r} A(r)\right)}{2 A(r)^{2}}-1+\frac{1}{A(r)} \\
R_{r r} &=-\frac{\left(\dv{}{r} B(r)\right)^{2}}{4 B(r)^{2}}+\frac{\dv{^{2}}{r^{2}} B(r)}{2 B(r)}-\frac{\left(\dv{}{r} A(r)\right)\left(\dv{}{r} B(r)\right)}{4 A(r) B(r)}-\frac{\dv{}{r} A(r)}{A(r) r} \\
R_{t t} &=\frac{\left(\dv{}{r} B(r)\right)\left(\dv{}{r} A(r)\right)}{4 A(r)^{2}}-\frac{\dv{^{2}}{r^{2}} B(r)}{2 A(r)}+\frac{\left(\dv{}{r} B(r)\right)^{2}}{4 A(r) B(r)}-\frac{\dv{}{r} B(r)}{A(r) r}
\end{aligned}
$$
 We now notice that
$$
-r A(r)\left(R_{t t} A(r)+R_{r r} B(r)\right)=\dv{(A(r) B(r))}{r}
$$
Since the left-hand side of the above vanishes due to Einstein's equations $\left(R_{r r}=R_{t t}=0\right)$, we obtain that
$$
A(r)=\frac{\kappa}{B(r)}, \quad \kappa=\text { constant. }
$$
Substituting into $R_{\theta \theta}$, we find that
$$
R_{\theta \theta}=\frac{\dv{}{r}(B(r) r)}{\kappa}-1=0
$$
which has the solution
$$
B(r)=\frac{c_{1}}{r}+\kappa .
$$
The constants can be fixed by the expected behaviour at large distances, given by the [[Newtonian limit]]
$$
B(r)=g_{t t} \stackrel{r \rightarrow \infty}{\approx} 1+2 \phi(r)=1-\frac{2 G M}{r} .
$$
We then have that $c_{1}=-2 G M$ and $\kappa=1$. This specifies completely the solution for the metric. The final result is the so called Schwarzschild solution,

$$
\dd{\tau^{2}}=\left[
    1-\frac{r_{S}}{r}
    \right]\dd{t^{2}}
-\frac{\dd{r^2}}{1-\frac{r_{S}}{r}}-r^{2}\left(\dd{ \theta^2}+\sin ^{2} \theta \dd{ \varphi^2}\right)
$$

^ScwarzschildSol

and the length

$$
r_{S} \equiv 2 G M
$$

^SchwarzschildRad

is the Schwarzschild radius, characterizing the strength of the gravitational field due to the mass $M$ laying at the center of our isotropic space.

We can now concern ourselves with the [[equations of motion in a Schwarzschild space]]