# Relativistic particle^[[[broedela-2 Point Particle actions#^b56027]]]

## Naive Worldline [[Action]]
Physics, should (and does) not depend on the formulation chosen^[[[broedela-2 Point Particle actions#^721288]]], thus one should always use a [[covariant]] framework. The simplest Lorentz-invariant quantity is the so-called line-element of the [[ worldline]]^[[[broedela-2 Point Particle actions#^229921]]]:

$$S = -mc \int \! ~\mathrm{d}s$$ ^2d6e55

Where $\mathrm{d}s$ is the [[spacetime interval]] and we have^[[[broedela-2 Point Particle actions#^1cbe3b]]]:

$$
-\mathrm{d} s^{2}=-c^{2} \mathrm{~d} t^{2}+\left(\mathrm{d} x^{1}\right)^{2}+\left(\mathrm{d} x^{2}\right)^{2}+\left(\mathrm{d} x^{3}\right)^{2}
$$

Thus ^[[[broedela-2 Point Particle actions#^419390]]]

$$
\mathrm{d} s=c \mathrm{~d} t \sqrt{1-\frac{\dot{\vec{x}}^{2}}{c^{2}}}
$$


Taylor expanding around $1$ yields^[[[broedela-2 Point Particle actions#^cc1768]]]:

$$
L=-m c \sqrt{c^{2}-\dot{\vec{x}}^{2}}=-m c^{2}+\frac{1}{2} m \dot{\vec{x}}^{2}+\frac{1}{8} m c^{-2} \dot{\vec{x}}^{4}+\ldots
$$

The $-m c^{2}$ term is useless in the eom and can be readily forgotten^[[[broedela-2 Point Particle actions#^a832b1]]]. The second order term is the [[Lagrangian]] for the [[Non relativitstic particle]]. Using the [[Euler-Lagrange equations]] on the non expanded [[Lagrangian]], we obtain the following [[equations of motion]]^[[[broedela-2 Point Particle actions#^5a993a]]]^[[[broedela-2 Point Particle actions#^a3674a]]]:
$$
\left(c^{2}-\dot{\vec{x}}^{2}\right) \ddot{\vec{x}}+(\dot{\vec{x}} \cdot \ddot{\vec{x}}) \dot{\vec{x}}=0
$$

^b50546

These imply collinearity of the first and second derivative: $\ddot{\vec{x}}= \alpha \dot{\vec{x}}$^[[[broedela-2 Point Particle actions#^4729f3]]], which when plugging back in simplifies the [[equations of motion|eom]] to: ^fbc68b

$$\alpha c^2 \dot{\vec{x}}  =   0$$

One solution is to set $\alpha$ to $0$ which then implies that $\ddot{\vec{x}}=0$ like for the [[Non relativitstic particle]]. 

The [[Conjugate momenta]]^[[[broedela-2 Point Particle actions#^ab2473]]] is: 

$$
\vec{p}=\frac{m c \dot{\vec{x}}}{\sqrt{c^{2}-\dot{\vec{x}}^{2}}}
$$

^d0d9e6

And [[Hamiltonian]] is:

$$
H=c \sqrt{m^{2} c^{2}+\vec{p}^{2}}=E
$$

While the [[Lagrangian]] is now properly relativistic, the spacetime coordinates are still expressed in terms of the time $t$, which is defined in a particular [[Lorentz frame]]^[[[broedela-2 Point Particle actions#^612462]]], i.e. the position $x$ is a dynamical degree of freedom. In contrast, time $t$ is merely a parameter providing a label for the position. When we apply a [[Lorentz transformation]], we would like to have the transformation manifest. Thus we require that both time and space be on equal footing.

![[Worldline action for a relativistic point particle]]

![[Polynomial (einbein) Action]]