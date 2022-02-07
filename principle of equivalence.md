---
alias:
- Einstein's PoE
- PoE
- inertial mass
- equivalence principle
- EP
- EEP
- gravitational mass
- locally inertial frame
tag: GR SR physics
---
# The principle of equivalence
Let us return to Newtonian mechanics and write the equations of motion for a particle in a homogeneous gravitational field. The particle is additionally subject to other forces $\vec{F}$. We have, for an inertial observer,
$$
m_{I} \ddot{\vec{x}}=m_{G} \vec{g}+\vec{F}
$$
In the above, we have distinguished between the mass coefficient of the acceleration, the so called **"inertial mass"** $m_{I}$, and the **"gravitational mass"** $m_{G}$ which enters the computation of the gravitational force in the right-hand side. We now perform a coordinate transformation
$$
\vec{x}=\vec{x}^{\prime}+\frac{1}{2} \vec{g} t^{2} \quad\left(t=t^{\prime}\right) .
$$
In this new accelerated frame we have
$$
m_{I} \ddot{\vec{x}^{\prime}}=\left(m_{G}-m_{I}\right) \vec{g}+\vec{F}^{\prime}
$$
In classical mechanics we claim that the gravitational and inertial masses are equal (or equivalent)
$$
m_{I}=m_{G}=m .
$$
Then the equations of motion in the accelerated frame take the form
$$
m \ddot{\vec{x}}^{\prime}=\vec{F}^{\prime}
$$
**In the above, the force of gravity has been eliminated. We have thus found that the gravitational force manifest in a coordinate system can be traded with acceleration.**

A condition for the above to hold was the the gravitational field needed to be uniform. This is of course unrealistic at large scales. However, if we **restrict ourselves to very small regions of space and small times we can consider the gravitational field to be sufficiently uniform**. This sounds like an unwanted approximation, but it is not. We can make our space-time intervals infinitesimally small. This can be compensated by erecting infinitely many local accelerated inertial frames corresponding to each of the infinitesimal space-time segments.

# Principle

Einstein took this observation and used it as a physical principle upon which he constructed the theory of general relativity. Concretely, the principle states:

*Locally (i.e. small spacetime regions) we can erect coordinate systems in which the laws of physics take the form which holds in [[inertial frames of reference]]. This form is the one we expect in [[special relativity]].*

Let us apply this principle to a single particle which is inside an arbitrary gravitational field. The particle is subjected only to the gravitational force and no other forces act on it. Einstein's principle of equivalence tells us that in small spacetime regions we can find coordinate transformations 
$$
\underbracket{x^\alpha}_{\text {lab-frame }} \rightarrow \underbracket{\xi^\alpha}_{\begin{array}{c}
\text { locally } \\
\text { inertial } \\
\text { frame }
\end{array}}
$$
that cancel the effect of gravity. One needs a different transformation of this kind in different patches of spacetime. However, such transformations must exist, according to the equivalence principle, for all patches.

# Locally inertial frame and the laws of nature

Let us focus on one such local patch. In the new reference frame $\left(\xi^\alpha\right.$ coordinates $)$ the laws of physics take their [[special relativity]] form. Namely, [[infinitesimal proper time interval in SR|proper time intervals]] will be given by

$$
 \dd{\tau^2}=\eta_{\mu \nu}  \dd{\xi^\mu}\dd{\xi^\nu}
$$

^propTimeIntInertial

where the metric $\eta_{\mu \nu}$  is the [[Minkowski metric]]. The [[particle dynamics in SR|equations of motion]] for the particle will be the ones of a free particle. Namely,

$$
\dv[2]{\xi^\mu}{ \tau}=0
$$

^eomInertial

What is the form of the [[#^propTimeIntInertial|proper time]] and the [[#^eomInertial|eoms]] in the "lab-frame", where gravity is not eliminated? We have
$$
 \dd{\tau^2}
 = \eta_{\mu \nu}  \dd{\xi^\mu}\dd{\xi^\nu}
 =\eta_{\mu \nu} \frac{\partial \xi^\mu}{\partial x^\alpha} \frac{\partial \xi^\nu}{\partial x^{\beta}}  \dd{x^\alpha}  \dd{x^{\beta}}
$$

$$
\implies \boxed{ \dd{\tau^2}=g_{\alpha \beta}(x)  \dd{x^\alpha}  \dd{x^{\beta}}}

$$

^prorTimeGeneric


where we define a new (non [[Minkowski metric|Minkowskian]]) [[metric tensor|metric]]:

$$
\boxed{g_{\alpha \beta}(x) \equiv \eta_{\mu \nu} \frac{\partial \xi^\mu}{\partial x^\alpha} \frac{\partial \xi^\nu}{\partial x^{\beta}}}
$$

^metric

We will see soon that the metric encodes the gravitational potential. The equations of motion of the particle in terms of the lab-frame variables are:
$$
\begin{aligned}
0 &=\dv[2]{\xi^\alpha}{\tau}
= \dv{}{\tau} \dv{\xi^\alpha}{\tau}
= \dv{}{ \tau} \left(\frac{\partial \xi^\alpha}{\partial x^\mu} \dv{ x^\mu}{ \tau}\right) \\

&=\frac{\partial \xi^\alpha}{\partial x^\mu} \dv[2]{ x^\mu}{ \tau}
+\dv{ x^\mu}{ \tau} \dv{}{ \tau} \frac{\partial \xi^\alpha}{\partial x^\mu} \\

&=\frac{\partial \xi^\alpha}{\partial x^\mu} \dv[2]{ x^\mu}{ \tau}
+\dv{ x^\mu}{ \tau} \dv{ x^\nu}{ \tau} \frac{\partial^{2} \xi^\alpha}{\partial x^\mu \partial x^\nu} \\

\pdv{x^\gamma}{\xi^\alpha}\cdot\implies 0 &
=\frac{\partial x^{\gamma}}{\partial \xi^\alpha} \frac{\partial \xi^\alpha}{\partial x^\mu} \dv[2]{ x^\mu}{ \tau}
+\dv{ x^\mu}{ \tau} \dv{ x^\nu}{ \tau} \frac{\partial x^{\gamma}}{\partial \xi^\alpha} \frac{\partial^{2} \xi^\alpha}{\partial x^\mu \partial x^\nu} \\

 &=\delta_\mu^{\gamma} \dv[2]{ x^\mu}{ \tau}
 +\dv{ x^\mu}{ \tau} \dv{ x^\nu}{ \tau} \frac{\partial x^{\gamma}}{\partial \xi^\alpha} \frac{\partial^{2} \xi^\alpha}{\partial x^\mu \partial x^\nu}
\end{aligned}$$
we write

$$
\dv[2]{\xi^\mu}{ \tau}=0\implies\boxed{ \dv[2]{ x^{\gamma}}{ \tau}+\Gamma^\gamma{}_{\mu \nu} \dv{ x^\mu}{ \tau} \dv{ x^\nu}{ \tau}=0}
$$

^eomGeneric

where

$$
\boxed{\Gamma^\gamma{}_{\mu \nu} \equiv 
\frac{\partial x^{\gamma}}{\partial \xi^\alpha} \frac{\partial^{2} \xi^\alpha}{\partial x^\mu \partial x^\nu}}
$$

^affineConnection

is called the "**[[affine connection]]**".  The [[#^eomGeneric|eoms]] can be approximated in the [[Newtonian limit]].