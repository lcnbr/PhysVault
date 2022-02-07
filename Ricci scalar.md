---
alias: curvature scalar
tag: GR physics
---

We have already proven that the [[Riemann curvature tensor|Riemann tensor]] and its linear combinations are the only possible tensors where second derivatives of the [[metric tensor|metric]] enter linearly. One such possible linear combination is the [[Ricci scalar]] or curvature scalar
$$
R \equiv g^{\mu \nu} R_{\mu \nu}=R_{\alpha \beta \gamma \delta} g^{\alpha \gamma} g^{\beta \delta} .
$$

^09f107

No other scalar possibilities exist due to the antisymmetry and cyclicity of the Riemann tensor. Notice also that
$$
\begin{aligned}
0 &=\varepsilon^{\mu \nu \rho \sigma} \overbrace{\left(R_{\mu \nu \rho \sigma}+R_{\mu \rho \sigma \nu}+R_{\mu \sigma \nu \rho}\right)}^{=0} \\
&=R_{\mu \nu \rho \sigma}\left(\varepsilon^{\mu \nu \rho \sigma}+\varepsilon^{\mu \rho \sigma \nu}+\varepsilon^{\mu \nu \nu \rho}\right) \\
&=R_{\mu \nu \rho \sigma}\left(\varepsilon^{\mu \nu \rho \sigma}+(-1)(-1) \varepsilon^{\mu \nu \rho \sigma}+(-1)(-1) \varepsilon^{\mu \nu \rho \sigma}\right) \\
\rightarrow 0 &=\varepsilon^{\mu \nu \rho \sigma} R_{\mu \nu \rho \sigma} .
\end{aligned}
$$
So, while we could potentially contract the Riemann tensor with a Levi-Civita symbol to form a scalar, this contraction yields zero.


# Weak field approximation

Using [[Ricci tensor#weak field approximation]] we obtain the  linear [[Ricci scalar]] $R^{(1)}=\eta^{\mu \nu}R^{(1)}{}_{\mu \nu}$:

$$
\implies R^{(1)}  = \eta^{\mu \nu}\eta^{\alpha\rho}\left[ \frac{\partial^2 h_{\rho\alpha}}{\partial x^\mu\partial x^\nu}   - \frac{\partial^2 h_{\nu\rho}}{\partial x^\mu\partial x^\alpha} \right] 
$$

^LinScal

Or graphically:

![[Pasted image 20220206160225.png#center|400]]