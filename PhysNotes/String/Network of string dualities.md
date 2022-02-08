# Network of string dualities

In the early 90 's five different string theories were defined at the perturbative level only, while there was little understanding of the dynamical principles of the theory. Considering the degenerate ground states after compactification (which are parametrised by scalars/moduli), it was not clear which of the reductions could possibly correspond to the Standard Model. Most annoyingly, there were five different versions of string theory available while the theory had set off to be a candidate for a unique unifying theory. The resolution to those problems appeared with the advent of string dualities. Two theories are called dual, if they describe the same physics using different "languages", that is, different fields, coupling constants and interactions. Hereby dualities can relate fields of completely different nature. Dualities lead to the identification of different vacua and finally allow - in combination with weak-coupling or strong-coupling limits - to identify M-theory as the link between the five different string theories, thus being closer to the unified description aimed at.

While T-duality will be the main working example here, there are other forms of dualities, in particular S-duality. In contrast to T-duality, which is a weak-weak duality relating the weak-coupling regimes of two theories to each other, S-duality is more interesting from the point of understanding the complete dynamics of a theory: It maps the non-perturbative strong-coupling sector of one theory to the perturbative weak-coupling sector of another theory.

In the following the arrows in the following figure shall be explained:

![](https://cdn.mathpix.com/cropped/2022_01_21_4a32c94eb29a468254abg-15.jpg?height=221&width=658&top_left_y=567&top_left_x=293)

Here, dashed arrows denote S-duality, dotted arrows mark T-duality and solid arrows are compactifications on a suitable interval.

# T-Duality

Within the context of the string theories explored so far there are two famous examples of T-duality: type IIA and IIB string theory can be shown to describe the same physics if one dimension is compactified on a circle. This is the example to be explored below. Furthermore, the two heterotic string theories HET-O and HET-E with gauge groups $\mathrm{SO}(32)$ and $\mathrm{E}_{8} \times \mathrm{E}_{8}$, respectively, are related by T-duality.

# T-Duality between IIA and IIB String Theory. 
Consider T-duality between the background fields in the [[Ramond-Neveu-Schwarz Superstring|NS]]-[[Ramond-Neveu-Schwarz Superstring|NS]] and the [[Ramond-Neveu-Schwarz Superstring|R-]]R sector: $G, B, \Phi, F$. The relations between the fields $G$ and $B$ from the [[Ramond-Neveu-Schwarz Superstring|NS]]-[[Ramond-Neveu-Schwarz Superstring|NS]] sector and their duals $\tilde{G}$ and $\tilde{B}$ can be obtained by starting from the non-linear sigma-model in conformal gauge

$$
S=-\frac{1}{4 \pi \kappa^{2}} \int \mathrm{d} \xi^{2}\left(\eta^{\alpha \beta} G_{\mu \nu}-\varepsilon^{\alpha \beta} B_{\mu \nu}\right) \partial_{\alpha} X^{\mu} \partial_{\beta} X^{\nu} .
$$

In order to derive the so-called **Buscher rules** for the fields $G$ and $B$, the ten-dimensional metric and antisymmetric tensor need to be split in Kaluza-Klein form for a compact direction $X^{9}$. After doing so and requiring the background fields $G$ and $B$ to be independent of the compact dimension, one finds that the fields are related by:

$$
\begin{array}{ll}
\tilde{G}_{i j}=G_{i j}-\frac{G_{i 9} G_{j 9}-B_{i 9} B_{j 9}}{G_{99}}, & \tilde{G}_{9 i}=-\frac{B_{9 i}}{G_{99}}, \quad \tilde{G}_{99}=\frac{1}{G_{99}}, \\
\tilde{B}_{i j}=B_{i j}+\frac{G_{i 9} B_{j 9}-G_{j 9} B_{i 9}}{G_{99}}, & \tilde{B}_{9 i}=-\frac{G_{9 i}}{G_{99}} .
\end{array}
$$

The dilaton transformation cannot be derived that easily: it can be inferred from demanding conformal invariance of the full (non-gauged) non-linear sigma-model action

$$
\begin{aligned}
S=&-\frac{1}{4 \pi \kappa^{2}} \int \mathrm{d} \xi^{2}\left[\left(\sqrt{-\operatorname{det} g} g^{\alpha \beta} G_{\mu \nu}-\varepsilon^{\alpha \beta} B_{\mu \nu}\right) \partial_{\alpha} X^{\mu} \partial_{\beta} X^{\nu}\right.\\
&+\kappa^{2} \sqrt{-\operatorname{det} g} \Phi(X) R[g]
\end{aligned}
$$

T-duality for the fields from the [[Ramond-Neveu-Schwarz Superstring|R-]]R sector can be derived in a similar manner. It is easy to check that the number of components for the [[Ramond-Neveu-Schwarz Superstring|R-]]R fields $F_{i}$ in type IIA string theory equals the number of free components in the type IIB theory. Indeed one finds

$$
\begin{gathered}
\underbrace{\left(\begin{array}{c}
10 \\
0
\end{array}\right)}_{F_{0}}+\underbrace{\left(\begin{array}{c}
10 \\
2
\end{array}\right)}_{F_{2}}+\underbrace{\left(\begin{array}{c}
10 \\
4
\end{array}\right)}_{F_{4}}=1+45+210=256, \\
\underbrace{\left(\begin{array}{c}
10 \\
1
\end{array}\right)}_{F_{1}}+\underbrace{\left(\begin{array}{c}
10 \\
3
\end{array}\right)}_{F_{3}}+\frac{1}{2} \underbrace{\left(\begin{array}{c}
10 \\
5
\end{array}\right)}_{F_{5}}=10+120+126=256 .
\end{gathered}
$$





# Strong/Weak Coupling Duality: S-Duality

S-duality is the analogue of electric-magnetic duality. Its name originates from the fact that it relates the strong-coupling and weak-coupling limits of theories.

S-duality provides a way to access theories beyond perturbation theory. Consider a theory at small values of the coupling $g_{\mathrm{s}}$ : There are electrically charged elementary states which can be handled by perturbation theory. Likewise there are magnetically charged solitonic states, which are very massive and strongly coupled. For these heavy states, perturbation theory is not a good description. Montonen and Olive proposed that for $g_{\mathrm{s}} \rightarrow \infty$ their roles might be reversed: they conjectured that one can reformulate a theory in terms of dual fields in such a way that the weakly coupled electrically charged states would turn into strongly coupled magnetic ones and vice versa.

