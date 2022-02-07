---
alias:
tag: GR physics
---

We want to solve: 

![[gravitational waves#^linearizedEq]]

^linEq

Whe first equation we have already encountered in  [[electrodynamics in GR#Gauge potentials|electrodynamics]] in the lorenz gauge. We find a retarded Green's function
$$
    G_{\mathrm{ret}}(x-x^\prime) = -2\pi\,\delta\left((x-x^\prime)^2\right)\Theta(x^0>x^{\prime0}),
$$
which satisfies

$$
    \Box_xG_{\mathrm{ret}}(x-x^\prime) = \delta(x-x^\prime).
$$

Then, the solution is

$$
    h_{\mu\nu}(x) = 8G\int\dd[4]{x^\prime}\,G_{\mathrm{ret}}(x-x^\prime)S_{\mu\nu}(x^\prime),

$$

^hsolInhom

as
$$
    \Box_xh_{\mu\nu} = 8G\int\dd[4]{x^\prime}\,\big(\underbrace{\Box_xG_{\mathrm{ret}}(x-x^\prime)}_{=-2\pi\,\delta(x-x^\prime)}\big) S_{\mu\nu}(x^\prime) = -16\pi GS_{\mu\nu}(x).
$$
Performing the $x^{\prime0}$ integration in [[#^hsolInhom]], we have
$$
\begin{split}
    h_{\mu\nu}(x) &= 8G\int\dd[3]{x^\prime}\,S_{\mu\nu}(\x^{\,\prime},t)\dd{t^\prime}\frac{\delta(t\prime-(t-|x-\x^{\,\prime}|))}{2|x-\x^{\,\prime}|} \\
    h_{\mu\nu}(\x,t) &= 4G\int\dd[3]{x}\,\frac{S_{\mu\nu}(\x^{\,\prime},t-|\x-\x^{\,\prime}|)}{|\x-\x^{\,\prime}|}.
\end{split}

$$
The retarded solution above satisfies the [[coordinate conditions|harmonic coordinate condition]] of [[#^linEq]]. Indeed, we have
$$
    T\ind{\mu\nu}{;\mu}=0\ \Rightarrow\ \frac{\partial T^{\mu\nu}}{\partial x^\mu}+\underbracket{\Gamma\,\Gamma\,}_{\mathclap{\mathrm{non-linear}}}=0\ \Rightarrow\ \frac{\partial T^{\mu\nu}}{\partial x^\mu}=0,
$$
ignoring non-linearities. Then, 
$$
    \frac{\partial}{\partial x^\mu}S^{\mu\nu} = \partial_\mu\left(T^{\mu\nu}-\frac{\eta^{\mu\nu}}{2}T\ind{\alpha}{\alpha}\right) = -\frac{\eta^{\mu\nu}}{2}\frac{\partial}{\partial x^\mu}T\ind{\alpha}{\alpha}.
$$
Also
$$
    S\ind{\mu}{\mu} = T\ind{\mu}{\mu} -\frac{\delta\ind{\mu}{\mu}}{2}T\ind{\alpha}{\alpha} = -T\ind{\alpha}{\alpha}.
$$
Thus
$$
\begin{split}
    \frac{\partial S^{\mu\nu}}{\partial x^\mu} &= \frac{1}{2}\frac{\partial S\ind{\alpha}{\alpha}}{\partial x^\mu}\eta^{\mu\nu} \\
    \frac{\partial S\ind{\mu}{\nu}}{\partial x^\mu} &= \frac{1}{2}\frac{\partial S\ind{\alpha}{\alpha}}{\partial x^\nu}.
\end{split}
$$
Then
$$
\begin{split}
    \frac{\partial h\ind{\mu}{\nu}}{\partial x^\mu} &= 8G\frac{\partial}{\partial x^\mu}\int\dd[4]{x^\prime}\,G_{\mathrm{ret}}(x-x^\prime)S\ind{\mu}{\nu}(x^\prime) \\
    
    &= 8G\int\dd[4]{x^\prime}\,\frac{\partial G_{\mathrm{ret}}(x-x^\prime)}{\partial x^\mu}S\ind{\mu}{\nu}(x^\prime) \\
    
    &= -8G\int\dd[4]{x^\prime}\left(\frac{\partial}{\partial x^{\prime\mu}}G_{\mathrm{ret}}(x-x^\prime)\right)S\ind{\mu}{\nu}(x^\prime) \\
    &= \underbrace{8GG_{\mathrm{ret}}(x-x^\prime)\delta\ind{\mu}{\nu}(x^\prime)}_{=0\ \mathrm{for}\ x=x^\prime} + 8G\int\dd[4]{x^\prime}\,G_{\mathrm{ret}}\frac{\partial S\ind{\mu}{\nu}(x^\prime)}{\partial x^{\prime\mu}} \\
    &= 8G\int\dd[4]{x^\prime}\,G_{\mathrm{ret}}(x-x^\prime)\frac{1}{2}\frac{\partial S\ind{\mu}{\mu}(x^\prime)}{\partial x^{\prime\nu}} \\
    &= \cdots \\
    &= \frac{\partial}{\partial x^\nu}\left[ 8G\int\dd[4]{x^\prime}\,G_{\mathrm{ret}}(x-x^\prime)\frac{S\ind{\mu}{\mu}(x^\prime)}{2} \right] \\
    &= \frac{1}{2}\frac{\partial h\ind{\mu}{\mu}(x)}{\partial x^\nu}.\ \checkmark
\end{split}
$$

# Homogenous solution
The general solution consists of the solution of [[#^hsolInhom]] and the solution of the homogeneous equation (compare to [[#^linEq]])

$$
\begin{split}
    \Box h_{\mu\nu} &= 0 \\
    \partial_\mu h\ind{\mu}{\nu} &= \frac{1}{2}\partial_\nu h\ind{\mu}{\mu}.
\end{split}
$$

^hSolHom

The above can be solved as plane waves. The metric $h_{\mu\nu}$ ought to be real-valued, thus we seek real solutions of the form

$$
    h_{\mu\nu} = \varepsilon_{\mu\nu}e^{\im k\cdot x} + \varepsilon^\ast_{\mu\nu}e^{-\im k\cdot x},
$$

^ansatz

where 
$$
    k\cdot x\equiv\eta_{\mu\nu}k^\mu k^\nu = k_\mu x^\mu.
$$
Substituting into $\Box h_{\mu\nu}=0$ gives $k_\mu k^\mu\equiv k^2=0$. From
$$
    \frac{\partial h\ind{\mu}{\nu}}{\partial x^\mu} = \frac{1}{2}\frac{\partial h\ind{\mu}{\mu}}{\partial x^\nu},
$$
we have

$$
    \varepsilon\ind{\mu}{\nu}k_\mu = \frac{1}{2}\varepsilon\ind{\mu}{\mu}k_\nu.

$$

^polteq

## Polarisation tensor
Let us now count the independent components of the tensor $\varepsilon_{\mu\nu}$, which is known as the **polarization tensor**.

-  Due to the symmetry of $h_{\mu\nu}$, the polarization tensor $\varepsilon_{\mu\nu}$ is also symmetric
- The ten components of $\varepsilon_{\mu\nu}$ are related vie the four-equations of [[#^polteq]]. Thus $\varepsilon_{\mu\nu}$ has at most six independent components.

Let us now investigate further the freedom that we have to perform coordinate transformations. Under transformations 
$$
    x^\mu\to x^{\prime\mu}=x^\mu +\omega^\mu(x),
$$
the metric transforms as
$$
    g_{\mu\nu}\to g\ind{}{\mu\nu}(x^\prime) = \frac{\partial x_\mu}{\partial x^{\prime\rho}}\frac{\partial x_\nu}{\partial x^{\prime\sigma}}g_{\rho\sigma}(x).
$$
In the primed coordinate system, we want that the metric is still a small deviation from the Minkowskian values. Thus, we will only consider coordinate transformations with $\omega^\mu\sim h^{\mu\nu}$ small. From
$$
\begin{split}
    \frac{\partial x^{\prime\mu}}{\partial x^\rho}\frac{\partial x^\rho}{\partial x^{\prime\nu}} &= \delta\ind{\mu}{\nu} \\
    
    \implies\ \left(\delta\ind{\mu}{\rho}+\frac{\partial\omega^\mu}{\partial x^\rho}\right)\frac{\partial x^\rho}{\partial x^{\prime\nu}} &= \delta\ind{\mu}{\nu} \\
    \implies\ \left(\delta\ind{\alpha}{\mu}-\frac{\partial\omega^\alpha}{\partial x^\mu}\right)\left(\delta\ind{\mu}{\rho}+\frac{\partial\omega^\mu}{\partial x^\rho}\right)\frac{\partial x^\rho}{\partial x^{\prime\nu}} &= \delta\ind{\mu}{\nu}\left(\delta\ind{\alpha}{\mu}-\frac{\partial\omega^\alpha}{\partial x^\mu}\right) \\
    \left(\delta\ind{\alpha}{\rho}-\frac{\partial\omega^\alpha}{\partial x^\rho}+\frac{\partial\omega^\alpha}{\partial x^\rho}+\mathcal{O}(\omega^2)\right)\frac{\partial x^\rho}{\partial x^{\prime\nu}} &= \delta\ind{\alpha}{\nu}-\frac{\partial\omega^\alpha}{\partial x^\nu} \\
    \Rightarrow\ \frac{\partial x^\alpha}{\partial x^{\prime\nu}} &\approx \delta\ind{\alpha}{\nu}-\frac{\partial\omega^\alpha}{\partial x^\nu}.
\end{split}
$$
Then
$$
\begin{split}
    g\ind{\prime}{\mu\nu}(x^\prime) &= \left(\delta\ind{\alpha}{\nu}-\frac{\partial\omega^\alpha}{\partial x^\nu}\right)\left(\delta\ind{\beta}{\mu}-\frac{\partial\omega^\beta}{\partial x^\mu}\right)\left(\eta_{\alpha\beta}+h_{\alpha\beta}\right) \\
    &\approx \eta_{\mu\nu} + h_{\mu\nu} -\frac{\partial\omega_\mu}{\partial x^\nu}-\frac{\partial\omega_\nu}{\partial x^\mu}.
\end{split}
$$
We have already required the harmonic coordinate condition, $g_{\alpha\beta}\Gamma\ind{\mu}{\alpha\beta}=0$, on $h_{\mu\nu}$. A generic coordinate transformation could spoil that. However, if we restrict ourselves to the linear approximation it is still possible to find $x\to x + \varepsilon$ with $\varepsilon^\mu(x)$ such that the harmonic coordinate condition is satisfied in the new frame too. Indeed, we can have
$$
\begin{split}
    g\ind{\prime}{\alpha\beta}\Gamma\ind{\prime\mu}{\alpha\beta} &= 0 \\
    \Rightarrow\ \frac{\partial h\ind{\prime\mu}{\nu}}{\partial x^\mu} &= \frac{1}{2}\frac{\partial h\ind{\prime\mu}{\mu}}{\partial x^\nu} \\
    \Rightarrow\ \frac{\partial}{\partial x^\mu}\left(h\ind{\mu}{\nu}-\frac{\partial\omega^\mu}{\partial x^\nu}-\frac{\partial\omega_\nu}{\partial x_\mu}\right) &\equiv \frac{1}{2}\frac{\partial}{\partial x^\nu}\left(h\ind{\mu}{\mu}-\frac{\partial\omega^\mu}{\partial x^\mu}-\frac{\partial\omega_\mu}{\partial x_\mu}\right) \\
    -\Box\omega_\nu(x)-\frac{\partial^2\omega^\mu(x)}{\partial x^\mu\partial x^\nu} &= -\frac{1}{2}\frac{\partial^2\omega^\mu(x)}{\partial x^\mu\partial x^\nu}-\frac{1}{2}\frac{\partial^2\omega^\mu(x)}{\partial x^\mu\partial x^\nu} \\
    \Rightarrow\ \Box\omega_\nu(x)&=0.
\end{split}
$$
Thus, the harmonic coordinate condition does not fix the coordinate system completely in the linearized theory. For example, we can choose
$$
    \omega_\mu(x) = -\im \varepsilon_\mu e^{-\im k\cdot x}+\im\varepsilon_\mu^\ast e^{+\im k\cdot x}.
$$
Then $h_{\mu\nu}=\varepsilon_{\mu\nu}e^{\im k\cdot x}+\varepsilon\ind{\ast}{\mu\nu} e^{-\im k\cdot x}$ becomes
$$
    h\ind{\prime}{\mu\nu} = \varepsilon\ind{\prime}{\mu\nu}e^{\im k\cdot x}+\varepsilon\ind{\prime\ast}{\mu\nu} e^{-\im k\cdot x}
$$
with
$$
    \varepsilon\ind{\prime}{\mu\nu} = \varepsilon_{\mu\nu} + k_\mu\varepsilon_\nu + k_\nu\varepsilon_\mu.
$$
Both $h_{\mu\nu}$ and $h\ind{\prime}{\mu\nu}$ are physically equivalent. However, the corresponding coordinate transformation induces four arbitrary parameters via the vectors $\varepsilon_\mu$. It should then happen that these four arbitrary parameters \underline{affect only} combinations of the polarization tensor components which do not affect physical quantities. As a conclusion, \underline{only two out of six} components of $\varepsilon_{\mu\nu}$ are physical.

To illustrate this, let us choose the direction of the wave to be in the positive $\hat{z}$-axis, $k^\mu = k(1,0,0,1)$. Then
$$
    k_\mu\varepsilon\ind{\mu}{\nu} = \frac{1}{2}k_\nu\varepsilon\ind{\mu}{\mu},
$$
or, equivalently, 
$$
    k^\mu\varepsilon_{\mu\nu} = \frac{1}{2}\varepsilon_{\mu\rho}\eta^{\rho\mu}\eta_{\nu\alpha} k^\alpha.
$$
This yields
$$
\begin{split}
    \varepsilon_{01} &= -\varepsilon_{13} \\
    \varepsilon_{02} &= -\varepsilon_{23} \\
    \varepsilon_{03} &= -\frac{1}{2}\left(\varepsilon_{00}+\varepsilon_{33}\right) \\
    \varepsilon_{22} &= -\varepsilon_{11},
\end{split}
$$
which indeed reduces the number of independent components of $\varepsilon_{\mu\nu}$ to six. Let us now perform the change of coordinates describes above giving $h_{\mu\nu}\to h\ind{\prime}{\mu\nu}$, where both satisfy the harmonic coordinate condition. We observe the changes, explicitly, to the polarization tensor $\varepsilon_{\mu\nu}\to\varepsilon\ind{\prime}{\mu\nu}=\varepsilon_{\mu\nu}+k_\mu\varepsilon_\nu+k_\nu\varepsilon_\mu$. The components
$$
\begin{split}
    \varepsilon_{11}\to\varepsilon\ind{\prime}{11}&=\varepsilon_{11} \\
    \varepsilon_{12}\to\varepsilon\ind{\prime}{12}&=\varepsilon_{12},
\end{split}
$$
remain unchanged, while
$$
\begin{split}
    \varepsilon_{13}\to\varepsilon\ind{\prime}{13}&=\varepsilon_{13} - k\varepsilon_1 \\
    \varepsilon_{23}\to\varepsilon\ind{\prime}{23}&=\varepsilon_{23} - k\varepsilon_2 \\
    \varepsilon_{00}\to\varepsilon\ind{\prime}{00}&=\varepsilon_{00} + 2k\varepsilon_0 \\
    \varepsilon_{33}\to\varepsilon\ind{\prime}{33}&=\varepsilon_{33} - 2k\varepsilon_3.
\end{split}
$$
We can tune 
$$
    \varepsilon_1=\frac{\varepsilon_{13}}{k},\ \varepsilon_2=\frac{\varepsilon_{23}}{k},\ \varepsilon_3=\frac{\varepsilon_{33}}{2k},\ \varepsilon_0=-\frac{\varepsilon_{00}}{2k}.
$$
In these coordinates the wave has only two degrees of freedom
$$
    \varepsilon\ind{\prime}{11}=\varepsilon_{11},\ \&\ \varepsilon\ind{\prime}{12}=\varepsilon_{12},
$$
while all other independent components of the polarization tensor are in this way made to vanish.

Let us now perform a rotation by an angle $\theta$ about the $z$-axis ($\vec{k}=k\hat{z}$ wave direction). Then, the polarization tensor will change as
$$
    \varepsilon_{\mu\nu}\to\varepsilon\ind{\prime}{\mu\nu}=R\invind{\mu}{\rho}R\invind{\nu}{\sigma}\varepsilon_{\rho\sigma}.
$$
with
$$
\begin{split}
    R\invind{1}{1}&=\cos\theta\qquad R\invind{1}{2}=\sin\theta \\
    R\invind{2}{1}&=-\sin\theta\quad\, R\invind{2}{2}=\cos\theta \\
    R\invind{3}{3}&=R\invind{0}{0}=1\quad\text{and all other }R\invind{\mu}{\nu}=0.
\end{split}
$$
Defining
$$
\begin{split}
    e_\pm &= \varepsilon_{11}\mp\im\varepsilon_{12} \\
    f_\pm &= \varepsilon_{31}\mp\im\varepsilon_{32},
\end{split}
$$
we have that
$$
\begin{split}
    e\ind{\prime}{\pm} &= e^{\pm2\im\theta}e_\pm \quad\ \, \rightarrow\text{"helicity $\pm2$\grqq} \\
    f\ind{\prime}{\pm} &= e^{\pm\im\theta}f_\pm \qquad\rightarrow\text{"helicity $\pm1$\grqq} \\
    \varepsilon\ind{\prime}{33} &= \varepsilon_{33},\ \varepsilon\ind{\prime}{00}=\varepsilon_{00}\quad\rightarrow\text{"scalar\grqq}.
\end{split}
$$
 