# Gauge Sector. 

## Fields in components
First we write the fields in components of the Lie algebra. In the above considerations we have assumed that the fields $A_{\mu}, F_{\mu \nu}, C$ and $\bar{C}$ are $N \times N$ hermitian matrices. In other words we have implicitly used the [[defining representation of su(n)|defining representation]] of $\mathrm{U}(N)$. We furthermore would like to restrict to traceless matrices and the corresponding group $\mathrm{SU}(N)$.

We would like to obtain the Feynman rules for the most general case. Therefore we write the fields $A_{\mu}^{a}$ in a basis $T_{a}$ of the Lie algebra $\mathfrak{g}$. The following relations express the matrix-valued fields in terms of the [[defining representation of su(n)|defining representation]] of $\mathrm{SU}(N)$.
$$
\begin{array}{rlrl}
A_{\mu} & =g T_{a}^{\text {def }} A_{\mu,}^{a} & C & =g T_{a}^{\text {def }} C^{a}, \\
F_{\mu \nu} & =g T_{a}^{\text {def }} F_{\mu \nu \prime}^{a}, & \bar{C} & =g T_{a}^{\text {def }} \bar{C}^{a} .
\end{array}
$$
Here $g$ is a normalisation factor that we will later adjust to be the coupling constant of the gauge field.

## [[Yang-Mills field strength|field strength]]
Let us first express the field strength in terms of components
$$
\begin{aligned}
{F}_{\mu v} &=\left(\partial_{\mu} A_{v}\right)-\left(\partial_{v} A_{\mu}\right)-i\left[A_{\mu}, A_{v}\right] \\
&=g T_{a}^{\operatorname{def}}\left(\partial_{\mu} A_{v}^{a}\right)-g T_{a}^{\operatorname{def}}\left(\partial_{v} A_{\mu}^{a}\right)-i g^{2}\left[T_{b}^{\operatorname{def}}, T_{c}^{\operatorname{def}}\right] A_{\mu}^{b} A_{v}^{c} \\
&=g T_{a}^{\operatorname{def}}\left(\left(\partial_{\mu} A_{v}^{a}\right)-\left(\partial_{v} A_{\mu}^{a}\right)+g f_{b c}{ }^{a} A_{\mu}^{b} A_{v}^{c}\right)
\end{aligned}
$$

Hence we find
$$
F_{\mu \nu}^{a}=\left(\partial_{\mu} A_{v}^{a}\right)-\left(\partial_{\nu} A_{\mu}^{a}\right)+g f_{b c}{ }^{a} A_{\mu}^{b} A_{v}^{c} .
$$

^ef79cc

The Yang-Mills Lagrangian now reads
$$
\begin{aligned}
\mathcal{L}_{\mathrm{YM}} &=-\frac{1}{2 g_{\mathrm{YM}}^{2}} \operatorname{Tr} F^{\mu v} F_{\mu v} \\
&=-\frac{g^{2}}{2 g_{\mathrm{YM}}^{2}} \operatorname{Tr}\left(T_{a}^{\text {def }} T_{b}^{\text {def }}\right) F^{a, \mu v} F_{\mu v}^{b} \\
&=-\frac{g^{2} B^{\text {def }}}{2 g_{\mathrm{YM}}^{2}} k_{a b} F^{a, \mu v} F_{\mu v}^{b}
\end{aligned}
$$
Where in the last line we used the [[structure constants#Killing form and Casimir invariant in basis|killing form in basis]]
In order to obtain a canonical prefactor we shall set ^[For the choice $B^{\text {def }}=1 / 2$ this would simply be $g=g_{\mathrm{YM}}$. However, we shall not fix $B^{\text {def }}$ and continue to work with $g$ instead of $g_{\mathrm{YM}}$.]
$$
g=\frac{g_{\mathrm{YM}}}{\sqrt{2 B^{\mathrm{def}}}} .
$$
Altogether we have
$$
\mathcal{L}_{\mathrm{YM}}=-\frac{1}{4} k_{a b} F^{a, \mu \nu} F_{\mu \nu}^{b} .
$$
This is similar to **one copy of the photon Lagrangian for each of the components of the Lie algebra**. Note, however, that the field strength $F_{\mu \nu}^{a}$ now depends non-linearly on the gauge potential $A_{\mu}^{a}$.([[#^ef79cc]])


## [[Faddeev-Popov ghosts|Ghost]] and gf
Next consider the [[Faddeev-Popov ghosts|ghost]] and [[Faddeev-Popov ghosts|gauge-fixing]] terms. In components they read
$$
\begin{aligned}
\mathcal{L}_{\mathrm{gh}} &=k_{a b} \overline{\mathrm{C}}^{a}\left(\partial^{\mu}\left(D_{\mu}^{\mathrm{ad}} \mathrm{C}\right)^{b}\right) \\
\mathcal{L}_{\mathrm{gf}} &=-\frac{1}{2}{\xi}^{-1} k_{a b}\left(\partial^{\mu} A_{\mu}^{a}\right)\left(\partial^{v} A_{v}^{b}\right)
\end{aligned}
$$


Here the [[YM covariant derivative#For a Gauge field|covariant derivative]] of the [[Faddeev-Popov ghosts|ghost field]] $C$ is defined as
$$
\left(D_{\mu}^{\mathrm{ad}} C\right)^{a}=\left(\partial_{\mu} C^{a}\right)+g f_{b c}^{a} A_{\mu}^{b} C^{c}
$$

## 
Altogether, the pure gauge sector consists of the gauge and [[Faddeev-Popov ghosts|ghost]] fields. In the Feynman graphs the gauge fields are commonly denoted by curly or wiggly lines, and the ghosts by straight dashed lines. Their momentum space Feynman propagators read

![[Pasted image 20220127000118.png|400]]

There are three types of vertices arising from the above Lagrangian: cubic and quartic interactions of the gauge field as well as an interaction of one gauge field with a [[Faddeev-Popov ghosts|ghost]] line ^[Note that the gauge structure of the quartic vertex is equivalent to two cubic vertices connected by a propagator. In fact, one can eliminate the quartic interaction by means of a non-propagating auxiliary field interacting via a cubic term. This would make all vertices cubic and proportional to the structure constants of the gauge group.
]

![[Pasted image 20220127000238.png|500]]




