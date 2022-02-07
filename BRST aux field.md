# Auxiliary Field.
To see the symmetry more clearly, we first rewrite the Lagrangian. Consider the following Lagrangian of the gauge potential $A_{\mu}$, the scalar fermionic [[Faddeev-Popov ghosts|ghost]] fields $C, \bar{C}$ and an auxiliary scalar bosonic field $B$
$$
\mathcal{L}_{\mathrm{BRST}}=\frac{2}{g_{\mathrm{YM}}^{2}} \operatorname{Tr}\left(\bar{C}\left(\partial^{\mu}\left[D_{\mu}, C\right]\right)+B\left(\partial^{\mu} A_{\mu}\right)+\frac{1}{2} \xi B^{2}\right) .
$$
The field $B$ is free and non-propagating, and it can be integrated out exactly by replacing it by its saddle point solution $B=-\xi^{-1} \partial^{\mu} A_{\mu}$. This yields precisely the conventional [[Faddeev-Popov ghosts|gauge-fixing]] and [[Faddeev-Popov ghosts|ghost]] terms ^[One may choose to work without the auxiliary field $B$, but then some properties (closure of the BRST algebra, existence of $K_{\mathrm{BRST}}$ ) are obscured.]
$$
\mathcal{L}_{\mathrm{BRST}} \simeq \frac{2}{g_{\mathrm{YM}}^{2}} \operatorname{Tr}\left(\bar{C}\left(\partial^{\mu}\left[D_{\mu}, C\right]\right)-\frac{1}{2} \xi^{-1}\left(\partial^{\mu} A_{\mu}\right)^{2}\right) .
$$