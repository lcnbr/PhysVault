---
Alias:
- worldline action
---
# Worldline action for a relativistic point particle^[[[broedela-2 Point Particle actions#^7575db]]]

We set c=1.

One possibility is to treat both time and space as labels. This leads to [[Classical Field Theory]]. The other possibility is to promote time to a dynamical degree of freedom, this leads then to [[String theory framework]]. To properly do this, we need a way to promote time to a degree of freedom without it really being a true dynamical degree of freedom. This will be accomplished using [[gauge symmetry]]. Starting from the same  [[relativistic particle#^2d6e55|action]], this time we parametrise the worldline using an auxilary curve parameter $\tau$

$$
S=-m\int \mathrm{d} \tau ~  \sqrt{-\left(\frac{\mathrm{d} X(\tau)}{\mathrm{d} \tau}\right)^{2}}= -m \int \mathrm{d} \tau ~\sqrt{-\dot{X}^{\mu} \dot{X}^{\nu} \eta_{\mu \nu}}
$$

^d3e42f

Where we denote $\frac{d}{d \tau}$ by a dot: $\dot{\square}$ and $\mu=0,\dots,D-1$ and we use [[Einstein summation]]. This is now manifestly [[Lorentz transformation]] invariant. The [[equations of motion]] (obtained by variying the [[Action|action]]) now read:


$$
\dot{X}^{2} \ddot{X}^{\mu}=(\dot{X} \cdot \ddot{X}) \dot{X}^{\mu}
$$

^49738e

They look awfully similar to [[relativistic particle#^b50546|before]] and again implying colinearity $\ddot{X^\mu}=\beta(\tau) \dot{X}^\mu, ~\forall \tau$, also as [[relativistic particle#^fbc68b|before]]. Additionally the [[Conjugate momenta]] are:

$$
P_{\mu}=\frac{m \dot{X}_{\mu}}{\sqrt{-\dot{X}^{2}}}\implies~ P^2=-m^2 ~ \text{(Mass on shell)}
$$

Also similar to [[relativistic particle#^d0d9e6|before]]. The [[mass on shell]] condition is a testament to the fact that the momenta are not all independent!

However, the naive [[Hamiltonian]] is $=0$. And we have one too many [[degrees of freedom]], as $X^0:=t(\tau)$ is among our dynamical variables, it is redundant^[[[broedela-2 Point Particle actions#^764d85]]] (a fake [[degrees of freedom|d.o.f.]]). But crucially the [[#^d3e42f|action]] is [[reparametrisation invariance|reparametrisation invariant]], i.e if we pick a different parameter $\tilde{\tau}=\tilde{\tau}(\tau)$ on the worldline, related to $\tau$ by any monotonic function, then we still have:

$$
S=-m \int \mathrm{d}  \tilde{\tau}~ \sqrt{-\frac{d X^{\mu}}{d \tilde{\tau}} \frac{d X^{\nu}}{d \tilde{\tau}} \eta_{\mu \nu}}
$$

Because the measure changes as: $\mathrm{d} \tau= \mathrm{d}\tilde{\tau} ~ |\frac{d \tau}{d \tilde{\tau}}|$ and the velocities as: $\frac{d X^{\mu} }{ d \tau}=\left(\frac{d X^{\mu} }{ d \tilde{\tau}}\right)(\frac{d \tilde{\tau}}{d \tau})$. This is so called [[gauge freedom]], and we can use it to set various gauges, i.e. various specific reparametrizations which removes the redundancy^[[[broedela-2 Point Particle actions#^52d94c]]]

To summarise this action is a fully relativistic formulation featuring [[gauge invariance]]: this complicates the formulation. It is, however, an advantage as well, as it allows to access the [[quantum symmetries]] of the theory easier.^[[[broedela-2 Point Particle actions#^e7718d]]]. It is not [[Polynomial (einbein) Action|polynomial]]^[[[broedela-2 Point Particle actions#^c8085d]]], which complicates quantisation^[[[broedela-2 Point Particle actions^]]], and since it is proportional to the mass it obviously does not work for massless particles^[[[broedela-2 Point Particle actions#^79cb2b]]]. To solve some of these issues we turn to the [[Polynomial (einbein) Action]].