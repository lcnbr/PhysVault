---
alias:
- ghost field
- anti-ghost field
- ghost
- Faddeev-Popov
tags:
- qftII
---

The crucial difference to the abelian case is that the determinant still depends on the gauge potential and cannot be pulled in front of the integral. (c.f. [[YM gauge fixing#^7ceeb2]]). The final trick used by Faddeev and Popov is to reconstruct the determinant as a fermionic path integral. Consider a pair of [[Grassmann variables|fermionic fields]] $C, \bar{C}$ ^[Even though the notation is suggestive, the fields $C$ and $\bar{C}$ are not exactly (hermitian) conjugates] belonging to the same space as each component $A_{\mu}$ of the gauge potential. **The field $C$ is called the ghost field, $\bar{C}$ is called the anti-ghost.** Define its action as a quadratic functional of the new fields^[${ }^{12}$ Even though the notation is suggestive, the fields $C$ and $\bar{C}$ are not exactly (hermitian) conjugates.
${ }^{13}$ The normalisation of a quadratic term is inessential because it only affects a constant prefactor.]
$$
\begin{aligned}
S_{\mathrm{gh}}[C, \bar{C}, A] &=\frac{2}{g_{\mathrm{YM}}^{2}} \int \mathrm{d} x^{4} \operatorname{Tr} \bar{C}\left(\partial^{\mu} D_{\mu}^{\mathrm{ad}} C\right) \\
&=\frac{2}{g_{\mathrm{YM}}^{2}} \int \mathrm{d} x^{4} \operatorname{Tr} \bar{C}\left(\partial^{\mu}\left[D_{\mu}, C\right]\right)
\end{aligned}
$$
A quadratic action leads to a Gaußian path integral which can be evaluated in closed form as a determinant
$$
\int \mathrm{DC\,D} \overline{\mathrm{C}} \exp \left(i S_{\mathrm{gh}}[C, \bar{C}, A]\right)=\operatorname{Det}\left(\partial^{\mu} D_{\mu}^{\mathrm{ad}}\right) .
$$
The argument of the determinant is precisely the operator acting on C. We use this identity to convert the determinant to some extra path integrals in [[YM gauge fixing#^1e83f9]]
$$
\begin{aligned}
Z[J]&=\int \operatorname{DC\,D\overline{C}\,DA}  \Delta[G[A, \Omega]]   \\
\cdot & \exp \left(i S_{Y M}[A, J]+i S_{g h}[C, \bar{C}, A]\right)
\end{aligned}
$$
Finally, we can treat the delta-functional as [[gauge fixing action for EM|before]] in the abelian case  by [[gauge fixing action for EM|averaging]] over the field $\Omega$. We then obtain the gauge-fixed Yang-Mills path integral
$$
\begin{aligned}
Z[J]=& \int \operatorname{DC\,D\overline{C}\,DA} \\
& \cdot \exp \left({i S}_{\mathrm{YM}}[A, J]+i S_{\mathrm{gh}}[C, \bar{C}, A]+i S_{\mathrm{gf}}[A]\right)
\end{aligned}
$$
with gauge-fixing term
$$
S_{\mathrm{gf}}[A]=-\frac{1}{\xi g_{\mathrm{YM}}^{2}} \int \mathrm{d} x^{4} \operatorname{Tr}(\partial \cdot A)^{2}
$$