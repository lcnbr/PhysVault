# Matter Couplings. 

In our [[YM eoms#Matter eom|previous]] [[N QED fields#spinor matter coupling| discussion]] of matter fields we assumed that the gauge group is $\operatorname{SU}(N)$ and that there are $N$ matter fields. In other words, they transform in the [[defining representation of su(n)|defining representation]] of $\mathrm{SU}(N)$.

Let us now consider spinor matter fields transforming in some unitary representation $R$ of the gauge group. The kinetic term for spinor matter in Yang-Mills theory reads
$$
\mathcal{L}_{\text {spinor }}=\bar{\psi}\left(\gamma^{\mu} D_{\mu}^{R}-m\right) \psi .
$$
We now expand the matter field $\psi=v_{k} \psi^{k}$ in a basis $v_{k}$ of $\mathbb{V}$. The conjugate field $\bar{\psi}=\bar{\psi}_{k} v^{k}$ is expanded in the dual basis $v^{k}$ of the dual space $\mathbb{V}^{*}$. The component Lagrangian now reads
$$
\mathcal{L}_{\text {spinor }}=\bar{\psi}_{k}\left(\gamma^{\mu}\left(D_{\mu}^{R} \psi\right)^{k}-m \psi^{k}\right)
$$
with the matter [[YM covariant derivative#For a Gauge field|covariant derivative]], where we used [[YM gauge sector Feynman rules#Fields in components]]
$$
\left(D_{\mu}^{R} X\right)^{k}=\left(\partial_{\mu} X^{k}\right)-i g\left(T_{a}^{R}\right)^{k}{ }_{j} A_{\mu}^{a} X^{j} .
$$

# Spinor fields
This results in the following Feynman rules involving the spinor field
![[Pasted image 20220127064202.png|400]]

# Scalar fields 
The Feynman rules for interactions with[[N QED fields#Scalar matter|scalar fields]] are slightly different, so let us display this case briefly ^[Here we assume a real representation $R$ as opposed to the complex representation for spinors. We suppose an orthonormal basis $v_{j} \cdot v_{k}=\delta_{j k}$.]
$$
\begin{aligned}
\mathcal{L}_{\text {scalar }} &=-\frac{1}{2}\left(D^{R, \mu} \phi\right) \cdot\left(D_{\mu}^{R} \phi\right)-\frac{1}{2} m^{2} \phi \cdot \phi \\
&=-\frac{1}{2}\left(D^{R, \mu} \phi\right)^{k}\left(D_{\mu}^{R} \phi\right)^{k}-\frac{1}{2} m^{2} \phi^{k} \phi^{k} .
\end{aligned}
$$
The resulting Feynman rules now include an extra quartic interaction $\phi^{2} A^{2}$
![[Pasted image 20220127064234.png|400]]
Finally, we can discuss interaction between the fields. In renormalisable field theories, there are three types of interactions: cubic and quartic interactions of the scalars as well as Yukawa interactions between two spinors and a scalar
$$
\begin{aligned}
\mathcal{L}_{\text {cubic }} &=\frac{1}{6} c_{j k l} \phi^{j} \phi^{k} \phi^{l} \\
\mathcal{L}_{\text {quartic }} &=\frac{1}{24} c_{j k l m} \phi^{j} \phi^{k} \phi^{l} \phi^{m} \\
\mathcal{L}_{\text {Yukawa }} &=c^{k}{ }_{l j} \bar{\psi}_{k} \psi^{l} \phi^{j}
\end{aligned}
$$
Gauge symmetry requires the terms to be invariant under gauge transformations. This implies that the constants $c_{j k l}, c_{j k l m}$ and $c_{l j}^{k}$ are invariant tensors of the gauge group. The existence of such tensors crucially depends on the specific group and representations of the fields. ^[The tensor product of the corresponding representations must contain a trivial representation so that $c$ does not transform under gauge transformations.] For example, a symmetric cubic tensor $c_{j k l}$ is rather rare whereas a symmetric quartic tensor $c_{j k l m}$ exists much more frequently.

