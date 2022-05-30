---
alias: 
- parallel transported
- parallely transported
tag: GR physics
---
![[Pasted image 20220205191415.png#leftwrap|300]]We discussed parallel transport in the context of [[spin in GR|spin]], and concluded that it would necessarily be [[.md|parallel transported]] because its eom was:

![[spin in GR#^eaf4ec|spin]]
It is often the case that a vector $A^{\mu}(\tau)$ carried along a curve by a particle does not change at $\tau$ if viewed from a reference frame $\xi_{x(\tau)}$ that is locally inertial at $x(\tau)$. In this frame the [[affine connection]] as well as $d A^{\mu} / d \tau$ vanishes, so
$$
\frac{D A^{\mu}}{D \tau}=0
$$
This being a covariant statement, and true at $x(\tau)$ in the locally inertial system $\xi_{x(\tau)}$, it is therefore true in all coordinate systems. The vector $A^{\mu}$ is then subject to the first-order differential equations

$$
\frac{d A^{\mu}}{d \tau}=-\Gamma^\mu{}_{v \lambda} \frac{d x^{\lambda}}{d \tau} A^{v}
$$

^diffEq

that define $A^{\mu}$ for all $\tau$, given $A^{\mu}$ at some initial $\tau$. A vector $A^{\mu}(\tau)$ defined in this way along a curve $x^{\mu}(\tau)$ is said to be defined by parallel transport. Any tensor can be defined along a curve by parallel transport by requiring its [[covariant derivative#Along a curve]] to vanish.

Now an interesting  question is what happens when we complete a [[round trips by parallel transport|round trip]].