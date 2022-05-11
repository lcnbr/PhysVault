---
sources:
aliases: 
tags: 
date created: Tuesday, May 10th 2022, 2:45:26 pm
date modified: Wednesday, May 11th 2022, 11:43:36 am
---
Let us take a look at the $d$ [[classical limit of wavefuctions in KMOC#^dfunct|function]] for a specific wavefunction: 

$$\phi(p)=\varphi\pqty\Big{\frac{p \cdot u }{m \xi}}=\mathcal{N}\exp\pqty\Big{-\frac{p \cdot u }{m \xi}}$$
We can use the normalisation condition
$$1= \int \dd{\Phi(p)} \abs{\phi(p)}^2 $$ to get that[^1]
$$\mathcal{N}=\frac{1}{m}\sqrt{\frac{2\xi\pi^2}{K_1(2/\xi)}}$$
where $K_1$ is a [[modified Bessel function of the Second Kind]].[^2]

Now we want to evaluate: 

$$T(q)=\mathcal{N}^2\int \dd{\Phi(p)} \hat{\delta}(2 p \cdot q+q^2) \exp\pqty\Big{-\frac{p \cdot u }{m \xi}}\exp\pqty\Big{-\frac{(p+q) \cdot u }{m \xi}}$$

We use the [[hyperbolic parametrisation]] and boost to the rest frame of  $u$ s.t. $u=(1,0,0,0)$ and align the $z$-axis along $q$, meaning that $p \cdot q=p_0q_0-p_zq_z$. We thus have: 

$$T(q)=\underbracket{\frac{\xi\pi^2}{K_1(2/\xi)}\exp\pqty\Big{-\frac{q_0}{m \xi}}}_{\alpha}\int\limits_0^\infty\hat{\dd}\zeta\,\sinh^{2}(\zeta)\int\limits_0^\pi \hat{\dd}\theta\,\sin(\theta)\int \limits_0^{2 \pi}\hat{\dd}\phi\,\hat{\delta}(2m(q_0\cosh \zeta-q_z \sinh \zeta\cos \theta)+q^2)\exp\pqty\Big{-\frac{2\cosh \zeta}{\xi}}$$

We can easily integrate over $\phi$ (the integral evaluates to 1) and change variables to $w=\cosh(\zeta)$:

$$T(q)=\alpha\int\limits_1^\infty\hat{\dd}w\,\sqrt{w^{2}-1}\exp\pqty\Big{-\frac{2w}{\xi}}\int\limits_0^\pi \hat{\dd}\theta\,\sin(\theta)\,\hat{\delta}(2m(q_0w-q_z \sqrt{w^{2}-1}\cos \theta)+q^2)$$

The integral over $\theta$ is of the following form:

$$\int \limits_0^\pi \hat{\dd}\theta\,\sin(\theta)\,\hat{\delta}(B-A\cos \theta)$$

changing variables we have: 

$$\frac{1}{A}\int \limits_{B-A}^{B+A} \dd{u}\delta(u)=\frac{1}{A}\int \dd{u} \Theta(u+A-B)\Theta(A+B-u)\delta(u)=\frac{1}{A}\Theta(A-B)\Theta(A+B)$$

Thus we now have:

$$T(q)=\alpha\int\limits_1^\infty\hat{\dd}w\,\frac{1}{2mq_z}\exp\pqty\Big{-\frac{2w}{\xi}}\Theta(A-B)\Theta(A+B)$$

where $A=2mq_z\sqrt{w^{2}-1}$ and $B=2mq_0w+q^2$. The second theta function $\Theta(A+B)$ has no effect in the $\hbar \to 0$ limit and the first one changes the integration bound to:

$$w\geq-\frac{q_0}{2m}+\frac{q_z}{\sqrt{-q^2}}\sqrt{1-\frac{q^2}{4m^2}}=D$$

Finally 
$$T(q)=\alpha\int\limits_D^\infty\hat{\dd}w\,\frac{1}{2mq_z}\exp\pqty\Big{-\frac{2w}{\xi}}=\frac{\alpha}{4\pi mq_z}\frac{\xi}{2} \exp\pqty\Big{-\frac{2D}{\xi}} $$

Plugging in the definition for $\alpha$ we get:

$$T(q)=\frac{\xi\pi^\cancel{2}}{K_1(2/\xi)}\exp\pqty\Big{-\frac{q_0}{m \xi}}\frac{1}{4\cancel{\pi} mq_z}\frac{\xi}{2} \exp\pqty\Big{-\frac{2D}{\xi}}$$

[^1]: to do this we use the [[hyperbolic parametrisation]], and since $1$ is [[Lorentz invariant]] we can boost to any frame we want. Thus we boost to [[center of momentum frame|CM frame]] of $u$ s.t. $u=(1,0,0,0)$:
$$1=\frac{m^2\mathcal{N}^2}{2}\int\limits_0^\infty\hat{\dd}\zeta\,\sinh^{2}(\zeta)\int\limits_0^\pi \hat{\dd}\theta\,\sin(\theta)\int \limits_0^{2 \pi}\hat{\dd}\phi\, \exp\pqty\Big{-2\frac{\cosh \zeta }{ \xi}}  \,$$Integration over $\theta$  yields $\frac{1}{\pi}$ from the hat and integration over $\phi$ yields $1$ we are thus left with this equation:$$\frac{1}{\mathcal{N}}=\sqrt{\frac{m^2}{2\pi}\int\limits_0^\infty\hat{\dd}\zeta\,\sinh^{2}(\zeta)\exp\pqty\Big{-2\frac{\cosh \zeta }{ \xi}}}$$
The integral over $\zeta$ can be identified with a [[modified Bessel function of the Second Kind#^3c41e3]]: $$\frac{1}{\mathcal{N}}=\sqrt{\frac{m^2}{4 \pi^2}\frac{\sqrt{\pi}}{\xi\Gamma\pqty{1+\frac{1}{2}}}K_1(\frac{2}{\xi})}$$Using the properties of the [[gamma function]]: $\Gamma(z+1)=z \Gamma (z)$ and $\Gamma(\frac{1}{2})=\sqrt{\pi}$ we get:$$\mathcal{N}=\frac{1}{m}\sqrt{\frac{2\xi\pi^2}{K_1(2/\xi)}}$$