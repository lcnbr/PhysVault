---
alias: 
- energy-momentum tensor
- stress-energy tensor
tags: SR GR
---

We can now extend the formalism of current density in order to describe the density and flow of energy and momentum. Recall the definition of the [[currents and densities in SR|current density]]
![[currents and densities in SR#^currentDensity|current density]] and now substitute the charge $q_n$ with the momentum components of the particle:  the [[relativistic energy and momentum|momentum 4-vector]]. This defines a tensor which is called the energy-momentum tensor

$$
T^{\mu \nu}=\sum_n p_n^{\mu} \dv{ x_n^{\nu}}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) .
$$

^tensor

Despite its appearance this is a symmetric tensor. Indeed
$$
\begin{aligned}
T^{\mu \nu} &=\sum_n p_n^{\mu} \dv{ x_n^{\nu}}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=\sum_n p_n^{\mu} \frac{m_n \dv{ x_n^{\nu}}{ \tau_n}}{m_n \dv{ t}{ \tau_n}} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=\sum_n \frac{p_n^{\mu} p_n^{\nu}}{E_n} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right),
\end{aligned}
$$
where we used [[relativistic energy and momentum|momentum four-vector]]:
$$
p_n^{\mu}=\left(E_n, \vec{p}_n\right)=\left(m_n \gamma_n, m_n \gamma_n \vec{v}_n\right), \quad  \dd{\tau_n}=\gamma_n  \dd{t} .
$$
We can also write the energy-momentum tensor as an integral using the [[currents and densities in SR#^current4vec|current density 4 vector]] of the form 

$$
T^{\mu \nu}=\int  \dd{\tau} \sum_n p_n^{\mu} \dv{ x_n^{\nu}}{ \tau} \delta^{(4)}\left(x-x_n(\tau)\right) .
$$

^integralForm

In this form we see explicitly that this is a $2^{\text {nd }}$ rank tensor. Let us now calculate the divergence of the energy-momentum tensor

$$
\begin{aligned}
\pdv{}{ x^i} T^{\mu i} 
&=\sum_n p_n^{\mu} \dv{ x_n^i}{ t} \pdv{}{ x_n^i} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=\sum_n p_n^{\mu} \dv{ x_n^i}{ t}\left(-\pdv{}{ x_n^i}\right) \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=-\sum_n p_n^{\mu} \dv{}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=-\dv{}{ t}\left(\sum_n p_n^{\mu} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right)\right)+\sum_n \dv{ p_n^{\mu}}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=-\dv{}{ t} T^{\mu 0}+\sum_n \dv{ p_n^{\mu}}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
\implies & \dv{}{ t} T^{\mu 0}+\pdv{}{ x^i} T^{\mu i}=\sum_n \dv{ p_n^{\mu}}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
 
\end{aligned}
$$

$$\implies \boxed{\partial_{\nu} T^{\mu \nu}=G^{\mu}}$$

^contEq

where
$$
\begin{aligned}
G^{\mu} &=\sum_n \dv{ p_n^{\mu}}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=\sum_n \dv{ p_n^{\mu}}{ \tau} \dv{ \tau}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=\sum_n f_n^{\mu} \dv{ \tau}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right)
\end{aligned}
$$
is the density of [[particle dynamics in SR|relativistic force]]. For a system of particles which interact collisionally with [[relativistic energy and momentum|momentum 4-vector]] being conserved at each collision.
![[Pasted image 20220202224142.png#center|400]]
Then
$$
\begin{aligned}
G^{\mu} &=\sum_n \dv{ p_n}{ t} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
        &=\sum_{c \in\text {collisions}} \delta^{(3)}\left(\vec{x}-\vec{x}_{c}(t)\right)  \sum_{n \in c}\dv{p_n^\mu}{ t} =\sum_{c \in\text {collisions}} \delta^{(3)}\left(\vec{x}-\vec{x}_{c}(t)\right)  \dv{}{ t}\underbracket{\sum_{n \in c}p_n^{\mu} }_{\text {=0}}=0
\end{aligned}
$$
In such case, we have that

$$
\begin{aligned}
\partial_{\nu} T^{\mu \nu} &=0 \\
\implies P^{\mu} & \equiv \int  \dd[3]{x} T^{\mu 0}=\int \dd[3]{x}  \sum_n p_n^{\mu} \delta^{(3)}\left(\vec{x}-\vec{x}_n(t)\right) \\
&=\sum_n p_n^{\mu}=\text { conserved. }
\end{aligned}
$$

^conservedT