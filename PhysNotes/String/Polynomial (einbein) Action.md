# Polynomial (einbein) Action

Let us introduce an auxiliary variable (or 1D [[../AnalyticalMech/Field|field]]) $e(\tau)$ into the [[worldline]] and write ^[[[broedela-2 Point Particle actions#^225814]]]

$$S[X,e]=\frac{1}{2} \int d \tau\left(e^{-1} \dot{X}^{2}-e m^{2}\right)$$ ^835a8d

Where we've used the notation $\dot{X}^{2}$ for $\dot{X}^{\mu} \dot{X}^{\nu} \eta_{\mu \nu}$ The [[../AnalyticalMech/equations of motion|e.o.m.]]^[[[broedela-2 Point Particle actions#^9f611d]]] (obtained by varying the [[../AnalyticalMech/Action|action]]) is:

$$m^{2} e^{2}+\dot{X}^{2}=0, \quad e \ddot{X}^{\mu}-\dot{e} \dot{X}^{\mu}=0$$ ^8793e7

Which when combined, yields the same [[Worldline action for a relativistic point particle#^49738e|equation]] as for the [[Worldline action for a relativistic point particle#^d3e42f|worldline action]]. The [[../AnalyticalMech/Conjugate momenta]] to $X^\mu$ is $P_\mu=\frac{\dot{X}^\mu}{e}$, which reduces the [[#^8793e7|eom]] to: $P^2=-m^2$. And the [[../AnalyticalMech/Conjugate momenta|momentum conjugate]] to $e$ vanishes. 

Crucially, here the massless case is valid^[[[broedela-2 Point Particle actions#^045308]]]! Setting $m=0$ leads to constant $\dot{X}^\mu$ and thus constant momentum $P_\mu$ with $P^2=0$^[[[broedela-2 Point Particle actions#^79455c]]]. Additionally $e$ is not fixed by the [[#^8793e7|eom]], there is a remaining gauge freedom^[[[broedela-2 Point Particle actions#^5e1b66]]]

## Geometric picture

The [[#^835a8d|action]] makes it look as if we have coupled the [[worldline]] theory to 1d gravity, with the field $e(\tau)$ acting as an [[einbein]] (in the sense of [[vierbeins]] that are introduced in [[general relativity]]). Changing notation slightly, makes this more obvious:

$$
S=-\frac{1}{2} \int \mathrm{d} \tau ~ \sqrt{-g_{\tau \tau}}\left(g^{\tau \tau} \dot{X}^{2}+m^{2}\right)
$$

Where $g_{\tau \tau}=(g^{\tau \tau})^{-1}$ is the (inverse) [[metric]] on the [[worldline]] and $g_{\tau \tau}=e^2$^[[[broedela-2 Point Particle actions#^017c29]]]

## Gauge freedom
We now have two [[../AnalyticalMech/degrees of freedom|d.o.f.]]s too many and thus can choose various reparametrizations of $\tau$ to fix their values:

- [[Temporal Gauge]]^[[[broedela-2 Point Particle actions#^65d9df]]]
- [[Spacial Gauge]]^[[[broedela-2 Point Particle actions#^9c74e9]]]
- [[Light Cone Gauge]]^[[[broedela-2 Point Particle actions#^eaa622]]]
- [[Proper Time Gauge]]^[[[broedela-2 Point Particle actions#^232f84]]]
- [[2 Point particle actions/Constant Einbein Guage]]^[[[broedela-2 Point Particle actions#^42aa1e]]]