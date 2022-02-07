# T-Duality
In the previous subsection, we have seen a similar behaviour for the small-radius and large-radius limit of a compactified dimension: the only difference was that the role of [[Kaluza-Klein Modes|KK modes]] and [[winding modes]] was switched. $\rightarrow$ [[T-duality]].
Our starting point is the [[Polyakov action#Action in conformal gauge]] of the 25direction $X:=X^{25}$
$$
-\frac{1}{2 \pi \kappa^{2}} \int \mathrm{d} \xi^{2} \frac{1}{2} \eta^{a b} \partial_{a} X \partial_{b} X
$$
The action has a global shift symmetry $X \rightarrow X+\epsilon$. The [[winding modes]] could be viewed as a shift by $\epsilon=2 \pi m R$ which is localised to the boundary.

We make the symmetry local by introducing a new [[gauge field]] $A_{a}$
$$
\frac{1}{2 \pi \kappa^{2}} \int \mathrm{d} \xi^{2}\left(-\frac{1}{2} \eta^{a b}\left(\partial_{a} X+A_{a}\right)\left(\partial_{b} X+A_{b}\right)-\varepsilon^{a b} \tilde{X} \partial_{a} A_{b}\right)
$$

This action is now invariant under a local shift symmetry $X \rightarrow X+\epsilon$ together with $A_{a} \rightarrow A_{a}-\partial_{a} \epsilon$. We have added two d.of. in the field $A_{a}$ and one local redundancy in the shift by $\epsilon$. We remove the remaining additional d.o.f. by demanding $F_{a b}=\partial_{a} A_{b}-\partial_{b} A_{a}=0$ through a [[Lagrange multiplier]] $\tilde{X}$. This implies that locally the gauge field $A_{a}$ is trivial, i.e. it is gauge equivalent to $A_{a}=0$. The new action is therefore equivalent to the old one
The field $A_{a}$ has no derivatives in the action, it is algebraic, and we can integrate it out exactly. The e.o.m. read
$$
A_{a}=-\partial_{a} X-\eta_{a c} \varepsilon^{c b} \partial_{b} \tilde{X} .
$$
We substitute them into the action and obtain a new action (up to a boundary term)
$$
-\frac{1}{2 \pi \kappa^{2}} \int \mathrm{d} \xi^{2} \frac{1}{2}^{a b} \partial_{a} \tilde{X} \partial_{b} \tilde{X} .
$$
This action has the same form as before, but it is expressed in terms of $\tilde{X}$ instead of $X$.
Now we can set $A_{a}=0$ to go back to the original formulation, and obtain the duality relation
$$
\partial_{a} X=-\eta_{a c} \varepsilon^{b b} \partial_{b} \tilde{X}, \quad \text { i.e. } \quad \dot{X}=\tilde{X}^{\prime}, \quad X^{\prime}=\dot{X} \text {. }
$$
This transformation is called [[T-duality]] Since the action in the dual coordinates is the same as before, solutions are mapped to solutions (potentially modulo boundary conditions). For the standard solution $X$ we find the dual solution $\tilde{X}$
$$
\begin{aligned}
&X=x+\kappa^{2} \frac{n}{R} \tau+m R \sigma+\text { modes, } \\
&\tilde{X}=\tilde{x}+m R \tau+\kappa^{2} \frac{n}{R} \sigma+\text { modes. }
\end{aligned}
$$
The duality interchanges the radii $R \leftrightarrow \tilde{R}=\kappa^{2} / R$ as well as the winding and KK numbers $m \leftrightarrow n .$

Therefore T-duality relates string theory on two backgrounds with different compactification radii.
![[Pasted image 20220120234251.png|300]]

This implies that $R=\kappa$ is effectively the minimum compactification radius. It is indeed a special "self-dual" point. For this special point, the duality between two models turns into an enhanced symmetry of a single model.
$R=\kappa$ is the minimum length scale in string theory. This may hint at a quantisation of spacetime in quantum gravity.

