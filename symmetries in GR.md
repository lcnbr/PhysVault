---
alias:
tag: GR physics
---

The [[Action principle for gravity|gravitational action]]
$$
    S = \int\dd[4]{k}\sqrt{g}\left(-\frac{R}{16\pi G} + matter\right),
$$
is invariant under general coordinate transformations $x\to x^\prime=x^\prime(x)$. Often we find coordinate transformations which not only preserve the action, but they also preserve the form of the metric. Such symmetries are called [[isometry|isometries]]. They are defined as the coordinate transformations
$$
    x\to x^\prime=x^\prime(x)\ \mathrm{with}\ g^{\mu\nu}(x^\prime)=g_{\mu\nu}(x).
$$
From 
$$
\begin{split}
    g\ind{}{\mu\nu}(x^\prime) &= \frac{\partial x^\rho}{\partial x^{\prime\mu}}\frac{\partial x^\sigma}{\partial x^{\prime\nu}}g_{\rho\sigma}(x) \\
    \Leftrightarrow\ g_{\mu\nu}(x)& = \frac{\partial x^{\prime\rho}}{\partial x^\mu}\frac{\partial x^{\prime\sigma}}{\partial x^\nu}g\ind{}{\rho\sigma}(x^\prime),
\end{split}
$$
we get for an isometry
$$
    g_{\mu\nu}(x) = \frac{\partial x^{\prime\rho}}{\partial x^\mu}\frac{\partial x^{\prime\sigma}}{\partial x^\nu}g_{\rho\sigma}(x^\prime).
\label{eq:metric for isometry}
$$
Let us now focus on small isometry transformations
$$
    x^\mu\to x^{\prime\mu}=x^\mu+\varepsilon\xi^\mu\quad \varepsilon\ \mathrm{small}.
$$
This is always sufficient for continuous symmetry transformations, as large symmetry transformation can be built by performing many successive small transformation. Substituting the above into \eqref{eq:metric for isometry} and expanding in $\varepsilon$ through the linear $\mathcal{O}(\varepsilon)$ term we have
$$
\begin{split}
    g_{\mu\nu}(x) &= \left(\delta\ind{\rho}{\mu}+\varepsilon\frac{\partial\xi^\rho}{\partial x^\mu}\right)\left(\delta\ind{\sigma}{\nu}+\varepsilon\frac{\partial\xi^\sigma}{\partial x^\nu}\right)g_{\rho\sigma}(x+\varepsilon\xi) \\
    &= \left(\delta\ind{\rho}{\mu}+\varepsilon\frac{\partial\xi^\rho}{\partial x^\mu}\right)\left(\delta\ind{\sigma}{\nu}+\varepsilon\frac{\partial\xi^\sigma}{\partial x^\nu}\right)\left(g_{\rho\sigma}(x)+\varepsilon\xi^\alpha\frac{\partial g_{\rho\sigma}(x)}{\partial x^\alpha}+\cdots\right) \\
    &= g_{\mu\nu}(x) + \varepsilon\left( g_{\rho\sigma}(x)\frac{\partial\xi^\sigma}{\partial x^\nu}+g_{\rho\nu}(x)\frac{\partial\xi^\rho}{\partial x^\mu}+\xi^\alpha\frac{\partial g_{\mu\nu}}{\partial x^\alpha} \right) + \mathcal{O}(\varepsilon^2).
\end{split}
$$
The above is satisfied trivially at $\mathcal{O}(\varepsilon^0)$. Requiring that it is also satisfied at $\mathcal{O}(\varepsilon)$ we obtain the following condition for small isometry transformations
$$
\begin{split}
    g_{\mu\rho}\frac{\partial\xi^\sigma}{\partial x^\nu} + g_{\rho\nu}\frac{\partial\xi^\rho}{\partial x^\mu} + \xi^\alpha\frac{\partial g_{\mu\nu}}{\partial x^\alpha} &= 0 \\
    \Rightarrow\ \frac{\partial}{\partial x^\nu}\left(g_{\mu\sigma}\xi^\sigma\right) + \frac{\partial}{\partial x^\mu}\left(g_{\rho\nu}\xi^\rho\right) - \xi^\sigma\frac{\partial g_{\mu\sigma}}{\partial x^\nu} - \xi^\rho\frac{\partial g_{\nu\rho}}{\partial x^\mu} + \xi^\alpha\frac{\partial g_{\mu\nu}}{\partial x^\alpha} &= 0 \\
    \frac{\partial\xi_\mu}{\partial x^\nu} + \frac{\partial\xi_\nu}{\partial x^\mu} -\xi^\alpha\left(\frac{\partial g_{\mu\alpha}}{\partial x^\nu}+\frac{\partial g_{\nu\alpha}}{\partial x^\mu}-\frac{\partial g_{\mu\nu}}{\partial x^\alpha}\right) &= 0 \\
    \Rightarrow\ \frac{\partial\xi_\mu}{\partial x^\nu}+\frac{\partial\xi_\nu}{\partial x^\mu}-2\xi_\beta\Gamma\ind{\beta}{\mu\nu} &= 0 \\
    \left(\frac{\partial\xi_\mu}{\partial x^\nu}-\xi_\beta\Gamma\ind{\beta}{\mu\nu}\right)+\left(\frac{\partial\xi_\nu}{\partial x^\mu}-\xi_\beta\Gamma\ind{\beta}{\mu\nu}\right) &= 0.
\end{split}
$$
This leads to the condition
$$
    \boxed{\xi_{\mu;\nu}+\xi_{\nu;\mu}=0}
\label{eq:killing vector}
$$
for the vector $\xi_\mu$ to generate an isometry. Vectors which satisfy this equation are called  Killing vectors.

Let us now look at the second derivative of the Killing vector. We start with the commutator
$$
    \xi_{\mu;\alpha;\beta}-\xi_{\mu;\beta;\alpha} = -R\ind{\rho}{\mu\alpha\beta}\xi_\rho.
\label{eq:comm of kill vec 2 der}
$$
Relabeling indices, we also write
$$
\begin{split}
    \xi_{\alpha;\beta;\mu} - \xi_{\alpha;\mu;\beta} &= -R\ind{\rho}{\alpha\beta\mu}\xi_\rho \\
    \xi_{\beta;\mu;\alpha} - \xi_{\beta;\alpha;\mu} &= -R\ind{\rho}{\beta\mu\alpha}\xi_\rho.
\end{split}
$$
Adding the above three equations, we have
$$
    \xi_{\mu;\alpha;\beta}-\xi_{\mu;\beta;\alpha} + \xi_{\alpha;\beta;\mu} - \xi_{\alpha;\mu;\beta} + \xi_{\beta;\mu;\alpha} - \xi_{\beta;\alpha;\mu} = -\xi_\rho\underbrace{\left(R\ind{\rho}{\mu\alpha\beta}+R\ind{\rho}{\alpha\beta\mu}+R\ind{\rho}{\beta\mu\alpha}\right)}_{=0,\ \mathrm{cyclicity}}=0.
$$
This equation is valid for any vector. For a killing vector satisfying \eqref{eq:killing vector} it simplifies to
$$
    2\xi_{\mu;\alpha;\beta}-2\xi_{\mu;\beta;\alpha}-2\xi_{\beta;\alpha;\mu} =0,
$$
and thus
$$
    \xi_{\beta;\alpha;\mu} = \xi_{\mu;\alpha;\beta}-\xi_{\mu;\beta;\alpha}.
$$
Substituting the right-hand side of the above into \eqref{eq:comm of kill vec 2 der} we have
$$
    \xi_{\beta;\alpha;\mu} = -R\ind{\rho}{\mu\alpha\beta}\xi_\rho.
\label{eq:2nd der of killing vec}
$$
This expresses the second derivative of the killing vector in terms of its first derivative and the vector itself. To assess the consequence of it, consider a function $f(x)$ with
$$
    f^{\prime\prime}(x) = \alpha(x)f^\prime(x)+\beta(x)f(x),
\label{eq:diffeq for 1D show}
$$
which is the structure (stripped of the indices etc.) of \eqref{eq:2nd der of killing vec}. $f(x)$ is a smooth, well-behaved function and we can expand it around $x=X$ as an infinite Taylor series. We have
$$
\begin{split}
    f(x) &= f(X) + f^\prime(X)(x-X) + f^{\prime\prime}(X)\frac{(x-X)^2}{2!} + \left(f^{\prime\prime}(X)\right)^\prime\frac{(x-X)^3}{3!} + \cdots \\
    &= f(X) + f^\prime(X)(x-X) + \left(\alpha(X)f^\prime(X)+\beta(X)f(X)\right)\frac{(x-X)^2}{2!} \\
    &\hspace{3cm} + \frac{\diff}{\diff x}\left.\left(\alpha(x)f^\prime(x)+\beta(x)f(x)\right)\right|_{x=X}\frac{(x-X)^3}{3!} + \cdots.
\end{split}
$$
From the above we see that the only input needed to determine the function $f(x)$ at any point $x$ is the value of the function and its first derivative at one point $X$. The complete function should be of the form
$$
    f(x) = \underbrace{f(X)}_{const.}w(x) + \underbrace{f^\prime(X)}_{const.}y(x).
\label{eq:func in terms of f fprime}
$$
We can now ask how many linearly independent functions $f^{(n)}(x)$ can satisfy the differential equation \eqref{eq:diffeq for 1D show}. This number is equal to at most $2$, which is the number of function coefficients $w(x),\,y(x)$. Let us assume that there is a third function satisfying \eqref{eq:diffeq for 1D show} and \eqref{eq:func in terms of f fprime}. For the first two functions we can write
$$
\begin{split}
    \begin{pmatrix} f^{(1)}(x) \\ f^{(2)}(x) \end{pmatrix} &= \underbrace{\begin{pmatrix}
    f^{(1)}(X) & {f^{(1)}}^\prime(X) \\ f^{(2)}(X) & {f^{(2)}}^\prime(X)
    \end{pmatrix}}_{= C,\ constants}\begin{pmatrix} w(x) \\ y(x) \end{pmatrix} \\
    \Rightarrow\ \begin{pmatrix} w(x) \\ y(x) \end{pmatrix} &= C^{-1} \begin{pmatrix} f^{(1)}(x) \\ f^{(2)}(x) \end{pmatrix}
\end{split}
$$
Substituting, \eqref{eq:func in terms of f fprime} can be written as
$$
    f(x) = c_1f^{(1)}(x) + c_2 f^{(2)}(x).
$$
Then any other function $f^{(3)}(x)$ will be a linear composition of the other two. Let us now aply the same arguments to Killing vectors, satisfying \eqref{eq:2nd der of killing vec}. A Killing vector will be expressed as a linear superposition of 
$$
    \xi_\mu(x) = \alpha\ind{\rho}{\mu}(x)\xi_\rho(X) + \beta\ind{\nu\rho}{\mu}(x)\xi_{\nu;\rho}(X).
$$
Due to the  antisymmetry $\xi_{\nu;\rho}=-\xi_{\rho;\nu}$ the number of independent $\beta\ind{\nu\rho}{\mu}(x)$ functions in $D$ dimensions is $\frac{D(D-1)}{2}$. In addition we require $D$ independent functions for $\alpha\ind{\rho}{\mu}$. In total the functional form of $\xi_\mu(x)$ depends on $\frac{D(D-1)}{2}+D = \frac{D(D+1)}{2}$ function coefficients. Therefore, in $D=4$ dimensions one can have at most $\frac{D(D+1)}{2}=10$ linearly independent Killing vectors.
