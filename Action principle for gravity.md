---
alias:
- Einstein-Hilbert action
- gravitational action
tag: GR physics
---

The [[Einstein's field equations|Einstein's equation]] have the form
$$
    R_{\mu\nu}-\frac{1}{2}g_{\mu\nu}R+8\pi GT_{\mu\nu} =0,
$$
where $R_{\mu\nu}$ is the [[Ricci tensor]], $R=g^{\alpha\beta}R_{\alpha\beta}$ the [[Ricci scalar|curvature scalar]] and $T_{\mu\nu}$ is the [[energy-momentum tensor in GR|energy-momentum tensor]]. We will show that the above can be derived as the [[Euler-Lagrange equations]] of an [[action]] integral
$$
    S = \int\dd[4]{x}\sqrt{g}\mathcal{L},
$$
where the [[Lagrangian density]] will be decomposed into a gravitation and a "matter", part
$$
    \L = \L_G+\L_M.
$$
In the above, $\L_M$ will be responsible for generating the energy-momentum tensor term in Einstein`s equations.

The action of gravitation should be built of the principle of being [[Tensors and tensor densities in General Relativity|general invariance|invariant]] under [[general coordinate transformation|general coordinate transformations]]
$$
\begin{split}
    x &\to x^\prime \\
    S^\prime &= \int\dd[4]{x}^\prime\sqrt{g^\prime}\L^\prime = \int\dd[4]{x}\sqrt{g}\L.
\end{split}
$$
We have already taken care that the measure $\dd[4]{x}\sqrt{g}$ is invariant under such transformations
$$
    \dd[4]{x}^\prime\sqrt{g^\prime} = \dd[4]{x}\sqrt{g}.
$$

We first focus on the [[gravitational Lagrangian density]], and we see that for $\mathcal{L}_G=const\cdot R-2\Lambda$ we obtain exactly [[Einstein's field equations|Einstein's equations]]! Now we can add a mass field: [[matter field Lagrangian with gravity]] and the normalisation yields the **Einstein Hilbert action**:

![[matter field Lagrangian with gravity#^EHaction]]

^EHaction