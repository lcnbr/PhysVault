# Open strings

Considering open strings in addition to the closed-string states discussed above, leads to additional states, fields and couplings. They complete the geometric picture of [[Dp-branes|D-branes]] in string theory in an exciting way. Introducing open string leads to

- additional string states; e.g. the [[open string spectrum#Quantisation|massless vectors (photon]]):

$$
|\zeta ; q\rangle=\zeta_{\mu} \alpha_{-1}^{\mu}|0 ; q\rangle .
$$

- corresponding to additional vertex operators defined on the ends of the string; e.g. for the photon

$$
V[\zeta, q] \sim \int \mathrm{d} \tau \zeta_{\mu} \partial_{\tau} X^{\mu} \exp (i q \cdot X) .
$$

- The additional fields of the background geometry couple to (are located at / live) the ends of the string. Upon closer inspection, they follow the same logic and mechanism as for closed strings: adding the vertex operator to the action has the same effect as switching on a background field.

The precise nature of the coupling to the ends of the open string depends on the choice of string boundary conditions. Here is, where the connection to $\mathrm{D} p$-[[Dp-branes|branes]] comes in.

Let us therefore discuss [[Neumann boundary conditions|Neumann conditions]] and [[6 Open strings and D/Dirichlet boundary conditions]]  .

 # [[Neumann boundary conditions|Neumann boundaries]]. 
 Consider the coordinates $X^{a}, a=0, \ldots, p$, with [[Neumann boundary conditions|Neumann conditions]]: We couple an abelian one-form gauge field $A$ to the end of a string

$$
\int_{\text {end }} \mathrm{d} \tau \dot{X}^{a} A_{a}(X)=\int_{\text {end }} A .
$$

- This is the natural coupling of a charged point-particle to a gauge field $A$. - The string end is a charged point-like object with a worldline.

Interestingly, the gauge field $A_{a}$ needs to exist only on the $\mathrm{D} p$-[[Dp-branes|brane]] to which the string ends are constrained. That is, one can have lower-dimensional gauge fields confined to (,,living on") a $\mathrm{D} p$-[[Dp-branes|brane]].

The classical coupling of $A$ respects [[Weyl invariance|Weyl symmetry]], while the quantum anomaly is described by a beta function

$$
\beta_{a}^{A} \sim \kappa^{4} \partial^{b} F_{a b} .
$$

Demanding absence of the conformal anomaly translates into the Maxwell equation $\partial^{b} F_{a b}=$ 0 to hold. Consequently, the associated low-energy effective action reads

$$
S \sim-\kappa^{4} \int \mathrm{d} x^{p+1} \frac{1}{4} F_{a b} F^{a b} .
$$

It is an action in the $(p+1)$-dimensional worldvolume of the $\mathrm{D} p$-[[Dp-branes|brane]].

For planar $\mathrm{D} p$-[[Dp-branes|branes]] in a flat background we can also include higher corrections in $\kappa$. This leads to the exact Born-Infeld action

$$
S \sim \int \mathrm{d} x^{p+1} \sqrt{-\operatorname{det}\left(\eta_{a b}+2 \pi \kappa^{2} F_{a b}\right)} .
$$

The leading order is the Maxwell kinetic term, but there are corrections at higher orders in $\kappa$.

# [[6 Open strings and D/Dirichlet boundary conditions|Dirichlet Boundaries]]. 
The coupling of the [[6 Open strings and D/Dirichlet boundary conditions|Dirichlet]] directions $X^{m}, m=p+1, \ldots, D-$ 1 , is rather different:

- The field $X^{m}$ is fixed, but we can use $X^{\prime m}$ for the coupling to background fields.

- The corresponding background field $Y_{m}$ describes displacement of the D $p$-[[Dp-branes|brane]] in transverse directions. This renders $\mathrm{D} p$-[[Dp-branes|branes]] in fact dynamical objects!

The beta function at leading order describes a collection of massless scalars

$$
\beta_{m}^{Y} \sim \partial^{a} \partial_{a} Y_{m} .
$$

The leading order action for these degrees of freedom is evident. The effective action for planar $\mathrm{D} p$-[[Dp-branes|branes]] at higher orders is the Dirac action

$$
S \sim \int \mathrm{d} x^{p+1} \sqrt{-\operatorname{det}\left(g_{a b}\right)},
$$

which measures the volume of the $\mathrm{D} p$-[[Dp-branes|brane]] via the induced worldvolume metric $g_{a b}=$ $\partial_{a} Y^{m} \partial_{b} Y_{m}$. This form of action clearly identifies the field $Y_{m}$ as a displacement of the $\mathrm{D} p$-[[Dp-branes|brane]] away from its classical planar configuration.

![](https://cdn.mathpix.com/cropped/2022_01_21_6a05ef3b6320b8a7606bg-07.jpg?height=163&width=176&top_left_y=1473&top_left_x=528)

# Dirac-Born-Infeld (DBI) action. 
The actions for all open string effective degrees of freedom can be combined into the so-called Dirac-Born-Infeld action

$$
S \sim \int \mathrm{d} x^{p+1} \sqrt{-\operatorname{det}\left(g_{a b}+2 \pi \kappa^{2} F_{a b}\right)} .
$$

The action is a combination of

- the Dirac action for the dynamics of $p$-[[Dp-branes|branes]] and

- the Born-Infeld action for gauge fields on the $p$-[[Dp-branes|brane]].

One can even add the effect of all the closed string fields to the $p$-[[Dp-branes|brane]] action

$$
S \sim \int \mathrm{d} x^{p+1} \mathrm{e}^{-\Phi} \sqrt{-\operatorname{det}\left(g_{a b}+2 \pi \kappa^{2} F_{a b}+B_{a b}\right)} .
$$

- $g_{a b}$ is the induced metric from the curved background.

- $B_{a b}$ is the pull back of the 2 -form field $B_{\mu \nu}$ to the $\mathrm{D} p$-[[Dp-branes|brane]].

- The combination $2 \pi \kappa^{2} F_{a b}+B_{a b}$ is gauge invariant.

- The dilaton couples as a prefactor as for the closed string.

# Coincident [[Dp-branes|branes]]. 
Similar to the considerations done above, one can now think about putting several [[Dp-branes|D-branes]] to one position. For a single [[Dp-branes|D-brane]], the vector field $A_{a}$ has an associated $\mathrm{U}(1)$ symmetry. For $N$ coincident [[Dp-branes|D-branes]] the gauge group enlarges from $\mathrm{U}(1)^{N}$ to $\mathrm{U}(N)$

The non-abelian gauge field should couple to the end of a string via a Wilson line

$$
\mathrm{T} \exp \int_{\text {end }} A .
$$

The resulting effective action is (at leading order)

$$
S \sim \int \mathrm{d} x^{p+1} \operatorname{tr}\left(-\frac{1}{4}\left(F_{a b}\right)^{2}+\frac{1}{2}\left(D_{a} Y_{m}\right)^{2}+\frac{1}{4}\left[Y_{m}, Y_{n}\right]^{2}\right) .
$$

This is a Yang-Mills action coupled to massless adjoint scalars with quartic interactions.