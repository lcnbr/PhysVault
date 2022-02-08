---
alias:
tag: GR physics
---
Consider a scalar field $\phi(x)$ with a mass $m$. This will contribute to the action with the term
$$
\begin{split}
    S_{matter}=S_M &= \frac{1}{2}\int\dd[4]{x}\sqrt{g}\left[\left(\partial_\mu\phi\right)\left(\partial^\mu\phi\right)-m^2\phi\right] \\
    &= \frac{1}{2}\int\dd[4]{x}\sqrt{g}\left[\left(\partial^\mu\phi\right)\left(\partial^\nu\phi\right)g_{\mu\nu}-m^2\phi\right].
\end{split}
$$
Notice the appearances of the metric, showing the [[principle of equivalence|equivalence principle]]. Under $g_{\mu\nu}\to g_{\mu\nu}+\delta g_{\mu\nu}$ the variation of the action is
$$
\begin{split}
    \delta S_M &= \int\dd[4]{x}\,\left[(\delta\sqrt{g})\L_M + \frac{1}{2}(\partial^\mu\phi)(\partial^\nu\phi)\sqrt{g}\delta g_{\mu\nu}\right] \\
    &= \int\dd[4]{x}\,\left[-\frac{1}{2}\sqrt{g}g^{\mu\nu}\L_M\delta g_{\mu\nu}+\frac{1}{2}(\partial^\mu\phi)(\partial^\nu\phi)\sqrt{g}\delta g_{\mu\nu}\right] \\
    \rightarrow\ \delta S_M &= \int\dd[4]{x}\frac{1}{2}\sqrt{g}\delta g_{\mu\nu}\left[(\partial^\mu\phi)(\partial^\nu\phi)-\L_Mg^{\mu\nu}\right].
\end{split}
$$
We define the energy-momentum tensor of the scalar field as being
$$
    T^{\mu\nu}_M = (\partial^\mu\phi)(\partial^\nu\phi)-g^{\mu\nu}\L_M.
$$
Notice that by replacing $g^{\mu\nu}\to\eta^{\mu\nu}$ we do recover the correct definition of the energy-momentum tensor for a scalar field in flat spacetime.
Putting together the $S_G$ and $S_M$ terms, we have
$$
    S = S_G + S_M = \int\dd[4]{x}\sqrt{g}\left(const.(R-2\Lambda)+\L_M\right).
$$
The variation under $g_{\mu\nu}\to g_{\mu\nu}+\delta g_{\mu\nu}$ is
$$
    \delta S = \frac{1}{2}\int\dd[4]{x}\sqrt{g}\delta g_{\mu\nu}\left[-2const.\left(R^{\mu\nu}-\frac{g^{\mu\nu}}{2}R+\Lambda g^{\mu\nu}\right)+T^{\mu\nu}\right] =0.
$$
This gives indeed [[Einstein's field equations|Einstein's equations]], if we normalize $const. = -\frac{1}{16\pi G}$. Then the action takes the form

$$
    S = \int\dd[4]{x}\sqrt{g}\left(-\frac{1}{16\pi G}(R-2\Lambda)+\L_M\right),

$$

^EHaction

and the equations of motion by varying the gravitational field are 
$$
    R^{\mu\nu}-g^{\mu\nu}R+\Lambda g^{\mu\nu}+8\pi GT^{\mu\nu} =0.
$$
[[#^EHaction]] is the so-called [[Action principle for gravity|Einstein-Hilbert action]]. Before we conclude, let us check the Euler-Lagrange equations we get by varying the scalar field
$$
    \phi\to\phi+\delta\phi.
$$
This yields
$$
\begin{split}
    \delta S &= \int\dd[4]{x}\sqrt{g}\left[ g^{\mu\nu}(\partial_\mu\phi)(\partial_\nu\delta\phi)-m^2\phi\delta\phi\right] \\
    &= \int\dd[4]{x}\,\left[\partial_\nu\left(\sqrt{g}g^{\mu\nu}(\partial_\mu\phi)\delta\phi\right)-\partial_\nu\left(\sqrt{g}g^{\mu\nu}\partial_\mu\phi\right)\delta\phi-m^2\phi\sqrt{g}\delta\phi\right] \\
    &= -\int\dd[4]{x}\sqrt{g}\delta\phi\left[m^2\phi+\frac{1}{\sqrt{g}}\partial_\nu\left(\sqrt{g}g^{\mu\nu}\partial_\mu\phi\right)\right],
\end{split}
$$
which yields the equations of motion
$$
\begin{split}
    \frac{1}{\sqrt{g}}\partial_\nu\left(\sqrt{g}g^{\mu\nu}\partial_\mu\phi\right)+m^2\phi &=0 \\
    \Leftrightarrow\ \frac{1}{\sqrt{g}}\partial_\nu\left(\sqrt{g}g^{\mu\nu}\phi_{;\mu}\right)+m^2\phi &=0 \\
    \Leftrightarrow\ \left(g^{\mu\nu}\phi_{;\mu}\right)_{;\nu}+m^2\phi &=0 \\
    \Leftrightarrow\ g^{\mu\nu}\phi_{;\mu;\nu}+m^2\phi &=0.
\end{split}
$$
For $g_{\mu\nu} = \eta_{\mu\nu}$ and $\Gamma\ind{\mu}{\nu\rho}=0$ we do obtain the correct equations of motion for a scalar field in [[special relativity]]
$$
    \eta^{\mu\nu}\partial_\mu\partial_\nu\phi+m^2\phi = 0\ \Leftrightarrow\ (\Box+m^2)\phi =0.
$$
Analogously, we can couple gravity to the electromagnetic field (or any other field - but spinor fields do require some extra care and the vierbein (tetrad) formalism). To include the electromagnetic field we have
$$
    S = \int\dd[4]{x}\,\bigg[-\frac{1}{16\pi G}(R-2\Lambda)-\frac{1}{4}F_{\mu\nu}F^{\mu\nu}+\frac{1}{2}(\partial_\mu\phi)(\partial^\mu\phi)-\frac{m^2}{2}\phi^2+\underbrace{\cdots}_{\text{other fields}}\bigg].
$$
