---
alias:
- conserved current
- charge density
- current density
tags: SR GR
---

Assume a set $\{n\}$ of particles with 4 -velocities $\dv{ x_n^{\mu}}{ \tau}$. Suppose that each particle is endowed with some intrinsic conserved quantity such as an electric charge $q_n$. We can identify a relativistic charge and current density

$$
J^{\mu}=\sum_n q_n \dv{ x_n^{\mu}}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) .
$$

^currentDensity

Notice that the $\delta$-function defines the coordinates of the particles $\vec{x}_n(t)$ in spacetime. For $\mu=0$ ^d7784b
$$
\begin{aligned}
J^{0} &=\sum_n q_n \dv{ x_n^{0}}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=\sum_n q_n \dv{ t}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=\sum_n^{q} q_n \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right)=\rho \quad \text { (charge density). }
\end{aligned}
$$
For $\mu=i=1,2,3$ we have 
$$ 
\begin{aligned} J^i &=\sum_n q_n \dv{ x_n^i}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\ &=\sum_n^n q_n v_n^i \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \quad(\text { current density }) . \\\end{aligned} $$


We have that
$$
\begin{aligned}

\pdv{}{x^i} J^i &=\sum_n q_n \dv{x_n^i}{ t} \pdv{}{x^i}\left[\delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right)\right] \\
&=\sum_n q_n \dv{ x_n^i}{ t}\left[-\pdv{}{x_n^i} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right)\right] \\
&=-\sum_n q_n \underbracket{\left[\dv{ x_n^i}{ t} \pdv{}{ x_n^i}\right]}_{\dv{}{ t}} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=-\dv{}{ t}\left(\sum_n q_n \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right)\right)=-\dv{ J^{0}}{ t} \\
& \Rightarrow \dv{ J^{0}}{ t}+\vec{\nabla} \cdot \vec{J}=0
\end{aligned}
$$
which is the continuity equation. It can be rewritten as

$$
\partial_{\mu} J^{\mu}=0
$$

^contEq

The continuity equation implies the conservation of charge. Indeed just as in [[Noether's theorem]]
$$
\dv{ Q}{ t}=\dv{}{ t} \int  \dd[3]{x} J^{0}(\vec{x})=\int  \dd[3]{x} \dv{}{ t} J^{0}(\vec{x})=-\int  \dd[3]{x} \vec{\nabla} \cdot \vec{J}(\vec{x}) \underset{\text { Gauss }}{=} 0 .
$$

The current density is indeed a [[contravariant vectors in SR|contravariant vector]]. We can write it as a 4-vector: 

$$
\begin{aligned}
J^{\mu} &=\sum_n q_n \dv{ x_n^{\mu}}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=\sum_n q_n \dv{ x_n^{\mu}}{ \tau} \dv{ \tau}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=\sum_n q_n \int  \dd{t} \dv{ \tau}{ t} \dv{ x_n^{\mu}}{ \tau} \delta^{(3)}\left(\vec{x}-\vec{x}_n(\tau)\right) \delta(t-t(\tau)) \\
&=\sum_n q_n \int \dd{\tau}  \dv{ x_n^{\mu}}{ \tau} \delta^{(4)}\left(x^{\mu}-x_n^{\mu}(\tau)\right) .
\end{aligned}
$$

^current4vec

Under a [[Lorentz transformation]]
$$
\begin{aligned}
(J^\mu)' &=\sum_n q_n \int  \dd{\tau} \dv{ (x_n^{ \mu})'}{ \tau} \delta^{(4)}\left(x^{\prime \mu}-x_n^{\prime \mu}(\tau)\right) \\
&=\sum_n q_n \int  \dd{\tau} \Lambda_{\nu}^{\mu} \dv{ x_n^{\nu}}{ \tau} \delta^{(4)}\left(\Lambda_{\rho}^{\mu}\left(x^{\rho}-x_n^{\rho}(\tau)\right)\right) \\
&=\Lambda^{\mu}{}_{\nu} \sum_n q_n \int  \dd{\tau} \dv{ x_n^{\nu}}{ \tau} \frac{\delta^{(4)}\left(x^{\mu}-x_n^{\mu}(\tau)\right)}{\underbrace{|\operatorname{det} \Lambda|}_{=1}} \\
&=\Lambda^{\mu}{}_{\nu} J^{\nu}
\end{aligned}
$$
Where we used [[delta function#Composition with a function]]. Note that for [[general coordinate transformation|general coordinate transformations]] the determinant of the Jacobian is not one and current densities transform differently than vectors.