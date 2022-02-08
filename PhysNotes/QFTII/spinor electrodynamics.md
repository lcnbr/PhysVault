
Let us briefly review electrodynamics coupled to spinor matter. Its fundamental fields are the electromagnetic potential $A_{\mu}$, the Dirac spinor field $\psi$ and its conjugate $\bar{\psi}$. The Lagrangian reads
$$
\mathcal{L}_{\mathrm{QED}}=\bar{\psi}\left(\gamma^{\mu} D_{\mu}-m\right) \psi-\frac{1}{4} F^{\mu \nu} F_{\mu \nu}
$$
The electromagnetic field strength $F_{\mu \nu}$ and the [[YM covariant derivative|covariant derivative]] $D_{\mu}$ associated to the gauge potential $A_{\mu}$ acting on a field of charge $q$ are defined as ^ddae11

$$
F_{\mu \nu}=\left(\partial_{\mu} A_{\nu}\right)-\left(\partial_{\nu} A_{\mu}\right), \quad D_{\mu}=\partial_{\mu}-i q A_{\mu}
$$

^fieldandgauge

The above Lagrangian turns out to have a large amount of symmery or redundancy. Define  [[gauge transformations]] as the following transformation with a transformation parameter field $\alpha(x)$

$$
\begin{aligned}
\psi^{\prime}(x) &=\exp (+i q \alpha(x)) \psi(x) \\
\bar{\psi}^{\prime}(x) &=\exp (-i q \alpha(x)) \bar{\psi}(x) \\
A_{\mu}^{\prime}(x) &=A_{\mu}(x)+\left(\partial_{\mu} \alpha(x)\right)
\end{aligned}
$$

^gaugetransformations

It is not immediately evident that the local symmetry transformation is compatible with the various derivatives appearing in the Lagrangian. However, the consistent use of the [[YM covariant derivative|gauge covariant]] derivaive $D_{\mu}$ guarantees gauge invariance by means of the transformation aw
$$
D_{\mu}^{\prime}=\exp (+i q \alpha(x)) D_{\mu} \exp (-i q \alpha(x)) .
$$

^931f34

The [[YM covariant derivative|covariant derivative]] simply pushes the transformation factor from the right to the left across the derivative. Moreover the field strength $F_{\mu v}$ can be defined as a commutator of two covariant derivatives which immediately shows that it is [[gauge symmetry|gauge invariant]] ^[In this chapter we assume (partial and covariant) derivatives to be operators which act on everything on their right unless restricted by brackets. E.g., in this notation a derivative can be written in two equivalent ways as $\left[\partial_{\mu}, X\right]=$ $\left(\partial_{\mu} X\right) .$ Note that this relationship remains true when supplemented by any terms on the right.]
$$
F_{\mu v}=i q^{-1}\left[D_{\mu}, D_{\nu}\right], \quad F_{\mu \nu}^{\prime}=F_{\mu \nu} .
$$

^e4faa1

The local symmetries in quantum electrodynamics are described by the abelian [[Lie group]] $U(1)$. This is the group of complex phase rotations $\psi \mapsto \exp (i q \alpha) \psi$.