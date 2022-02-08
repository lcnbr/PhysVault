---
alias:
tag: GR physics
---


Given the uniqueness of a maximally symmetric space of a certain curvature $\kappa$, we can construct its metric in any way we can (guess it). One possibility is to start from a flat $(D+1)$ space with a metric
$$
    \dd{\tau}^2 = g_{AB}\dd{x}^A\dd{x}^B = c_{\mu\nu}\dd{x}^\mu\dd{x}^\nu + \frac{\dd{z}^2}{\kappa},
$$
where $\kappa,\,c_{\mu\nu}$ are constants and constrain a $D$ dimensional space on a "sphere",
$$
    z^2+\kappa c_{\alpha\beta}x^\alpha x^\beta = 1.
$$
Notice that both of the above equations are invariant under rigid rotations

$$
\begin{split}
    x^\mu&\to x^{\prime\mu} = R\ind{\mu}{\nu}x^\nu + R\ind{\mu}{z}z \\
    z&\to z^\prime = R\ind{z}{\mu}x^\mu + R\ind{z}{z}z,
\end{split}
$$

^symmetries

with
$$
\begin{split}
    c_{\mu\nu}R\ind{\mu}{\rho}R\ind{\nu}{\sigma} + \kappa^{-1}R\ind{z}{\rho}R\ind{z}{\rho} &= c_{\rho\sigma} \\
    c_{\mu\nu}R\ind{\mu}{\rho}R\ind{\nu}{z}+\kappa^{-1}R\ind{z}{\rho}R\ind{z}{z}&=0 \\
    c_{\mu\nu}R\ind{\mu}{z}R\ind{\nu}{z}+\kappa^{-1}\left(R\ind{z}{z}\right)^2 &= \kappa^{-1},
\end{split}
$$

^symCond


which have $\frac{D(D+1)}{2}$ generators. The resulting space inherits the same rotation symmetries and will thus have the maximum number of [[symmetries in GR|Killing vectors]] in $D$ dimensions. The metric in the $D$-dimensional space is easily computed. We find
$$
    \dd{z}^2 = \frac{\kappa^2\left(c_{\mu\nu}x^\mu\dd{x}^\nu\right)^2}{\left(1-\kappa c_{\alpha\beta}x^\alpha x^\beta\right)},
$$
and thus
$$
    \dd{\tau}^2 = c_{\mu\nu}\dd{x}^\mu\dd{x}^\nu + \frac{\kappa^2}{\kappa}\frac{\left(c_{\mu\alpha}c_{\nu\beta}x^\alpha x^\beta\right)\dd{x}^\mu\dd{x}^\nu}{\left(1-\kappa c_{\alpha\beta}x^\alpha x^\beta\right)},
$$
which yields $\dd{\tau}^2=g_{\mu\nu}\dd{x}^\mu\dd{x}^\nu$ with

$$
    g_{\mu\nu}(x) = c_{\mu\nu} + \kappa\frac{c_{\mu\alpha}c_{\nu\beta}x^\alpha x^\beta}{1-\kappa c_{\alpha\beta}x^\alpha x^\beta}.

$$

^maxSymMetric

**Exercise** Calculate the affine connection.
$$
    \Gamma\ind{\mu}{\nu\rho} = -\kappa x^\mu g_{\nu\rho}.
$$
Then, we can easily compute the Riemann tensor
$$
\begin{split}
    R\ind{\mu}{\nu\rho\sigma} &= \frac{\partial\Gamma\ind{\mu}{\nu\rho}}{\partial x^\sigma} + \Gamma\ind{\alpha}{\nu\rho}\Gamma\ind{\mu}{\alpha\sigma} - \frac{\partial\Gamma\ind{\mu}{\nu\sigma}}{\partial x^\rho} - \Gamma\ind{\alpha}{\nu\sigma}\Gamma\ind{\mu}{\alpha\rho} \\
    \Rightarrow\ R_{\mu\nu\rho\sigma} &= \kappa\left(g_{\mu\sigma}g_{\rho\nu} - g_{\mu\rho}g_{\nu\sigma}\right).
\end{split}
$$
Thus $\kappa$ is the curvature constant.

# [[symmetries in GR|Killing vectors]]

We will now identify independent [[symmetries in GR|Killing vectors]] generating the isometries of our maximally symmetric space. We have two subsets of the [[#^symmetries|symmetry transformation]] is

## Rotations
 $$
\begin{split}
    x^\mu&\to x^{\prime\mu} = R\ind{\mu}{\nu}x^\nu \\
    z&\to z^\prime = z,
\end{split}
$$
$R\ind{\mu}{\nu}$ arbitrary, $R\ind{z}{\mu}=R\ind{\mu}{z}=0$, $R\ind{z}{z}=1$. Then using [[#^symCond]]
$$
    R\ind{\mu}{\alpha}R\ind{\nu}{\beta}c_{\mu\nu} = c_{\alpha\beta}.
$$
For infinitesimal transformations, we have
$$
\begin{split}
    \left(\delta\ind{\mu}{\alpha}+\Omega\ind{\mu}{\alpha}\right)\left(\delta\ind{\nu}{\beta}+\Omega\ind{\nu}{\beta}\right)c_{\mu\nu} &= c_{\alpha\beta} \\
    \Rightarrow \Omega\ind{\mu}{\alpha}c_{\mu\beta} + \Omega\ind{\nu}{\beta}c_{\alpha\nu} &= 0.
\end{split}
$$

^infTrans

We also have
$$
    x^{\prime\mu} = x^\mu + \Omega\ind{\mu}{\alpha} x^\alpha = x^\mu + \xi^\mu_{\Omega}(x).
$$
We can indeed check that [[#^infTrans]] is equivalent to the condition
![[symmetries in GR#^killingVec]]
of [[symmetries in GR|Killing vectors]].

## Translations

We have infinitesimal translations with [[symmetries in GR|Killing vectors]]
$$
    \xi^\mu_{(a)} = a^\mu(1-\kappa c_{\mu\nu}x^\mu x^\nu)^{1/2}.
$$
**Exercise:** Check that 
$$
    \xi_{(a)\mu;\rho}+\xi_{(a)\rho;\mu}=0.
$$
We can transform further the metric of [[#^maxSymMetric]] by performing a linear transformation
$$
    x^\mu\to x^{\prime\mu}=A\ind{\mu}{\nu}x^\nu.
$$
Then 
$$
    c_{\mu\nu}x^\mu x^\nu \to c_{\mu\nu} A\ind{\mu}{\rho}A\ind{\nu}{\sigma}x^\rho x^\sigma \to c\ind{\prime}{\rho\sigma}x^\rho x^\sigma,
$$
with $c\ind{\prime}{\rho\sigma}=c_{\mu\nu}A\ind{\mu}{\rho}A\ind{\nu}{\sigma}$. We can choose the transformation matrix $A\ind{\mu}{\rho}$ such that $c\ind{\prime}{\rho\sigma}$ is brought to a diagonal form. For a Euclidian space we have all eigenvalues of the metric of the same sign and we can write
$$
    c_{\mu\nu}=\lambda\delta\ind{\mu}{\nu}.
$$
Then
$$
    \dd{s}^2 = g_{\mu\nu}\dd{x}^\mu\dd{x}^\nu = \lambda\dd{\x}^2 + \frac{\kappa\lambda^2\left(\x\cdot\dd{\x}\right)^2}{1-\kappa\lambda^2\left(\x\cdot\dd{\x}\right)^2}.
$$
If $\kappa=0$, we can pick $\lambda=1$ and then
$$
    \dd{s}^2 = \frac{1}{|\kappa|}\left[\dd{\x}^2 + \mathrm{sgn}(\kappa)\frac{\left(\x\cdot\dd{\x}\right)^2}{1-\mathrm{sgn}(\kappa)\x^2}\right].
$$
For a space with a metric of $(+,-,-,-)$ eigenvalues we can diagonalize of $c_{\mu\nu}=-\eta_{\mu\nu}$ yields
$$
    \dd{\tau}^2 = \dd{t}^2-\dd{\x}^2 + \frac{\kappa\left(t\dd{t}-\x\cdot\dd{\x}\right)^2}{1+\kappa\left(t^2-\x^2\right)}.
$$
