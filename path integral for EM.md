Consider the action for the electromagnetic field with sources ^[The current $J$ can be an external field or it may represent couplings to matter fields such as $J^{\mu}=-i \bar{\psi} \gamma^{\mu} \psi$. The latter is conserved provided that the field $\psi$ obeys the equation of motion. Strictly speaking, coupling to charged scalar fields is not of this form due to the terms quadratic in gauge fields. Nevertheless, scalar fields can be added to the action without complications as long as the latter remains gauge invariant.]
$$
S_{\mathrm{EM}}[A, J]=\int \mathrm{d} x^{4}\left(-\frac{1}{4} F^{\mu v} F_{\mu v}-J^{\mu} A_{\mu}\right) .
$$
The action is invariant under gauge transformations 
$$
S_{\mathrm{EM}}\left[A^{\prime}, J\right]=S_{\mathrm{EM}}[A, J]=S_{\mathrm{EM}}[[A], J]
$$
with
$$
A_{\mu}^{\prime}=A_{\mu}+\left(\partial_{\mu} \alpha\right),
$$
Where $[A]$ is a gauge equivalence class, provided that the source field is conserved,
$$
\partial_{\mu} J^{\mu}=0
$$
Naively, the [[graph generating functional|path integral]] reads
$$
Z[J]=\int \mathrm{D} A \exp \left(i S_{\mathrm{EM}}[A, J]\right) .
$$
Gauge invariance of the action implies that the integrand of the path integral is constant along all gauge-equivalent field configurations $A$
$$
\begin{aligned}
Z[J] &=\int \mathrm{D} A \exp \left(i S_{\mathrm{EM}}[A, J]\right) \\
&=\left(\int \mathrm{D} \alpha\right) \cdot \int \mathrm{D}[A] \exp \left(i S_{\mathrm{EM}}[[A], J]\right)=\infty
\end{aligned}
$$
This shows that the path integral over the gauge potential $A$ overcounts the admissible field configurations. ^[On the one hand, the gauge orbits are infinite-dimensional spaces and therefore the path integral will formally not converge. On the other hand, the path integral diverges anyway.
] We would like to divide out the divergent integral $\int \mathrm{D} \alpha$ over gauge orbits, and keep just the integral $\int \mathrm{D}[A]$ over **gauge equivalence classes**, but it is not evident how to do the latter in practice.