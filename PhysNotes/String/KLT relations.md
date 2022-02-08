# KLT Relations.
The KLT relations relate scattering amplitudes in closed string theories to the ones in open string theories. This is not a duality: the two physical systems described by open and closed strings have a different spectrum and are distinct.

Any vertex operator corresponding to a massless state in closed string theory can be written as product of two vertex operators in open string theory:

$$
V^{\text {closed }}[q]\left(z_{i}, \bar{z}_{i}\right)=V_{\mathrm{L}}^{\text {open }}[q]\left(z_{i}\right) \bar{V}_{\mathrm{R}}^{\text {open }}[q]\left(\bar{z}_{i}\right) .
$$

While in the closed string the insertion points $z_{i}, \bar{z}_{i}$ are integrated over a two-sphere, in the open-string case the real $z_{i}$ are integrated over the boundary of a disk. In order to express the closed-string integral in terms of open-string integrals, one has to identify and relate the contours of integration in the open-string integrals in a way which yields a consistent closed-string expression. Deforming the contours in the open string integral one will yield various phase factors.

After doing so, one can express the closed-string amplitudes in terms of a sum of products of open-string amplitudes. The total permutation symmetry of the insertion points on the sphere (and thus the total permutation symmetry of the external legs in the closedstring integral) is ensured by a taking particular sums of different products of open-string amplitudes with permuted legs.

![[KLT relations_2022-01-23 17.37.33.excalidraw||center]]

KLT relations are a very convenient way to calculate amplitudes in closed string theory and more so in their low-energy limits, supergravity. In fact: many calculations in supergravity could not have been performed without KLT relations.

The explicit relations depend on the external states of the amplitudes. For the example of pure tachyon amplitudes one finds

$$
M_{4, \text { tach }}^{\text {closed }}(s, t) \sim \frac{1}{\pi} \sin \left(\alpha^{\prime} \pi t / 4\right) A_{4, \text { tach }}^{\text {open }}(s / 4, t / 4) A_{4, \text { tach }}^{\text {open }}(t / 4, u / 4) .
$$

For external gluons, the four-point and five-point KLT relations read

$$
\begin{aligned}
M_{4, \text { grav }}^{\text {closed }}(1,2,3,4)=& \frac{-i}{\alpha^{\prime} \pi} \sin \left(\alpha^{\prime} \pi s\right) \\
& \cdot A_{4, \text { gluon }}^{\text {open }}(1,2,3,4) A_{4, \text { gluon }}^{\text {open }}(1,2,4,3), \\
M_{5, \text { grav }}^{\text {closed }}(1,2,3,4,5)=& \frac{i}{\alpha^{\prime 2} \pi^{2}} \sin \left(\alpha^{\prime} \pi s_{12}\right) \sin \left(\alpha^{\prime} \pi s_{34}\right) \\
& \cdot A_{5, \text { gluon }}^{\text {open }}(1,2,3,4,5) A_{5, \text { gluon }}^{\text {open }}(2,1,4,3,5) \\
&+\frac{i}{\alpha^{\prime 2} \pi^{2}} \sin \left(\alpha^{\prime} \pi s_{13}\right) \sin \left(\alpha^{\prime} \pi s_{24}\right) \\
& \cdot A_{5, \text { gluon }}^{\text {open }}(1,3,2,4,5) A_{5, \text { gluon }}^{\text {open }}(3,1,4,2,5) .
\end{aligned}
$$

Here Mandelstam variables are defined as $s_{i j}=-\left(q_{i}+q_{j}\right)^{2}$, where for the four-point case the usual $s=s_{12}, t=s_{14}$ and $u=s_{13}$ have been used.

The above equalities are exact relations between string theory amplitudes, and so they are valid order by order in $\alpha^{\prime}$. For example, in the limit $\alpha^{\prime} \rightarrow 0$ KLT will relate gluon amplitudes in $\mathcal{N}=4$ SYM to [[graviton]] amplitudes in $\mathcal{N}=8$ supergravity. Being an exact relation between open and closed string amplitudes, the KLT relations are valid for each order in $\alpha^{\prime}$ individually. In particular, one can relate the string corrections to $\mathcal{N}=4$ SYM and $\mathcal{N}=8$ supergravity: using KLT relations one can for example show that the absence of the first-order and second-order corrections to supergravity amplitudes is implied by the particular form of the string corrections to the $\mathcal{N}=4$ SYM theory.

KLT relations do not only relate gluon and [[graviton]] amplitudes in the field theory limits of open and closed string theories, but amplitudes from the full multiplets. In particular, the tensor-decomposition of the Fock space reads

$$
[\mathcal{N}=8] \longleftrightarrow[\mathcal{N}=4]_{\mathrm{L}} \otimes[\mathcal{N}=4]_{\mathrm{R}} .
$$