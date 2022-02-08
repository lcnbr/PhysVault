---
alias:
tag: GR physics
---


A generic tensor $T_{\mu\nu\cdots}$ is called form-invariant if
$$
    \eval{T_{\mu\nu\cdots}(x) }_{x=x'}= T\ind{}{\mu\nu\cdots}(x^\prime),
$$
under a coordinate transformation $x\to x^\prime = x^\prime(x)$. Due to the tensor properties of $T_{\mu\nu\cdots}$ we have that
$$
    T_{\mu\nu\cdots}(x) = \frac{\partial x^{\prime\rho}}{\partial x^\mu}\frac{\partial x^{\prime\sigma}}{\partial x^\nu}\cdots T\ind{}{\rho\sigma\cdots}(x^\prime),
$$
and from form invariance we have
$$
    T_{\mu\nu}(x) = \frac{\partial x^{\prime\rho}}{\partial x^\mu}\frac{\partial x^{\prime\sigma}}{\partial x^\nu}\eval{T_{\rho\sigma}(x)}_{x=x'},
$$
limiting the rank to two, for illustration purposes. For infinitesimal transformations
$$
    x^{\prime\mu} = x^\mu + \varepsilon\xi^\mu(x),
$$
we obtain (taylor expanding)
$$
    \xi^\alpha\frac{\partial}{\partial x^\alpha}T_{\mu\nu}(x) + \frac{\partial\xi^\alpha}{\partial x^\mu}T_{\alpha\nu}(x) + \frac{\partial x^\alpha}{\partial x^\nu}T_{\mu\alpha}(x) = 0.
$$
Specializing to a scalar $S(x)$, the above gives
$$
    \xi^\alpha(x)\frac{\partial}{\partial x^\alpha}S(x) =0.
$$
In a maximally symmetric space there are [[symmetries in GR|Killing vectors]] which are arbitrary at any point $x$. Then we get
$$
    \frac{\partial}{\partial x^\alpha}S(x) =0\ \Rightarrow\ S(x) = constant.
$$
In a maximally symmetric space , we can also choose [[symmetries in GR|Killing vectors]] which vanish at any given point $X$, $\xi^\alpha(X)=0$, but their covariant derivatives do not and form an antisymmetric tensor
$$
    \xi_{\mu;\rho}(X)=-\xi_{\rho;\mu}(X).
$$
We have
$$
\begin{split}
    \xi_{\sigma;\mu}(X) &= g_{\sigma\rho}(X)\left[\frac{\partial\xi^\rho}{\partial x^\mu} + \Gamma\ind{\rho}{\alpha\mu}\underbrace{\xi^\alpha(x)}_{=0}\right]_{x=X} \\
    \Rightarrow\ \xi_{\sigma;\mu}(X) &= g_{\sigma\rho}(X)\left(\frac{\partial\xi^\rho(x)}{\partial x^\mu}\right)_{x=X}.
\end{split}
$$
Then
$$
\begin{split}
    \xi^\alpha(x)\frac{\partial T_{\mu\nu}}{\partial x^\alpha} + \frac{\partial\xi^\alpha}{\partial x^\alpha}T_{\alpha\nu} + \frac{\partial\xi^\alpha}{\partial x^\nu}T_{\mu\alpha} &= 0 \\
    \overset{x=X}{\Rightarrow}\ \frac{\partial\xi^\alpha}{\partial x^\mu}g_{\alpha\rho}T\ind{\rho}{\nu} + \frac{\partial\xi^\alpha}{\partial x^\nu}g_{\alpha\rho}T\invind{\mu}{\rho} &=0 \\
    \Rightarrow\ \xi_{\rho;\mu}T\ind{\rho}{\nu}+\xi_{\rho;\nu}T\invind{\mu}{\rho} &= 0 \\
    \Rightarrow\ \underbrace{\xi_{\rho;\sigma}}_{\mathclap{\mathrm{antisymm.}}}\left(\delta\ind{\sigma}{\mu}T\ind{\rho}{\nu}+\delta\ind{\sigma}{\nu}T\invind{\mu}{\rho}\right) &= 0.
\end{split}
$$
Because of the $\xi_{\rho;\sigma}$ antisymmetry we must have that its coefficient at $X$ is symmmetric. This then gives

$$
    \delta\ind{\sigma}{\mu}T\ind{\rho}{\nu} + \delta\ind{\sigma}{\nu}T\invind{\mu}{\rho} = \delta\ind{\rho}{\mu}T\ind{\sigma}{\nu} + \delta\ind{\rho}{\nu}T\invind{\mu}{\rho}.

$$

^maxSymVector

Similarly, for a vector we have
$$
    \delta\ind{\sigma}{\mu}A^\rho = \delta\ind{\rho}{\mu}A^\sigma.
$$
Let us contract the above equation in $\rho=\mu$
$$
\begin{split}
    \delta\ind{\sigma}{\mu}A^\mu &= \delta\ind{\mu}{\mu}A^\sigma \\
    \Rightarrow\ A^\sigma &= DA^\sigma\ \Rightarrow\ (D-1)A^\sigma =0 \\
    \Rightarrow\ A^\sigma &= 0\quad\mathrm{for}\ D>1.
\end{split}
$$
Similarly, for [[#^maxSymVector]] setting $\rho=\mu$ gives
$$
\begin{split}
    T\ind{\sigma}{\nu}+\delta\ind{\sigma}{\nu}T\invind{\mu}{\mu} &= DT\ind{\sigma}{\nu} + T\invind{\nu}{\sigma} \\
    \overset{\times g_{\mu\sigma}}{\Rightarrow} T_{\mu\nu} + g_{\mu\nu}T\invind{\alpha}{\alpha} &= DT_{\mu\nu} + T_{\nu\mu} \\
    \Rightarrow\ (D-1)T_{\mu\nu} + T_{\nu\mu} &= g_{\mu\nu}T\invind{\alpha}{\alpha}.
\end{split}
$$
Also 
$$
    (D-1)T_{\nu\mu}+T_{\mu\nu} = g_{\nu\mu}T\invind{\alpha}{\alpha}\quad (\nu\leftrightarrow\mu).
$$
Substituting the two equations gives
$$
\begin{split}
    (D-2)\left(T_{\mu\nu}-T_{\nu\mu}\right) &=0 \\
    \Rightarrow\ T_{\mu\nu} &= T_{\nu\mu}\quad \mathrm{for}\ D\geq3.
\end{split}
$$
Then 
$$
\begin{split}
    DT_{\mu\nu} &= g_{\mu\nu}T\ind{\alpha}{\alpha} \\
    \Rightarrow\ T_{\mu\nu} &= \frac{g_{\mu\nu}}{D}T\ind{\alpha}{\alpha}.
\end{split}
$$
As $T\ind{\alpha}{\alpha}$ is a scalar, it is a constant. T**herefore the only tensor of rank-2 in a maximally symmetric space is the metric**. We generally have
$$
    T_{\mu\nu}=\frac{g_{\mu\nu}}{D}\times constant.
$$
**Exercise:** Repeat this type of analysis for a rank-3 or rank-4 tensor.
