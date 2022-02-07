One-Loop Renormalisation in Yang-Mills Theory. Let us discuss the renormalisation of the Yang-Mills coupling $g$. In order to extract it, we need to consider the kinetic term and the cubic coupling of gauge fields. For simplicity, we shall discard the contributions of scalar fields.
![[Pasted image 20220127083708.png]]
It takes some patience to evaluate these graphs since there are many contributions, and since the coupling of gauge fields has many terms. To simplify the calculation one can instead consider the kinetic term of some other field, e.g. the spinor or even better the [[Faddeev-Popov ghosts|ghost]], along with its coupling to the gauge field. Note that the kinetic term for the gauge field is still relevant since it fixes the normalisation of the gauge field in the interaction vertex. The graphs with two external spinors (or equivalently ghosts) take the form:
![[Pasted image 20220127083726.png]]
We shall not evaluate the graphs in full detail, let us merely investigate their structure in terms of the gauge algebra.

When some matter fields in representation $R$ form a loop with coupling to two external gluons, the resulting gauge algebra structure reads
$$
\operatorname{Tr} T_{a}^{R} T_{b}^{R}=B^{R} k_{a b} .
$$
For three external gluons the structure is ${ }^{14}$
$$
\operatorname{Tr}\left[T_{a}^{R}, T_{b}^{R}\right] T_{c}^{R}=i f_{a b}{ }^{d} \operatorname{Tr} T_{d}^{R} T_{c}^{R}=i B^{R} f_{a b c} .
$$
We observe that both gauge algebra structures match the structures of the quadratic and cubic terms in the Yang-Mills action. Moreover, both coefficients are proportional to the constant $B^{R}$ related to the representation of the matter fields.

An analogous result holds for loops made from gluons and ghosts. For two external gluons we find
$$
f_{a c}^{d} f_{b d}^{c}=-B^{\mathrm{ad}} k_{a b} .
$$
For three gluons the result reduces to an analogous combination ${ }^{15}$
$$
\begin{aligned}
f_{a d}{ }^{e} f_{b e}{ }^{f} f_{c f}{ }^{d} &=\frac{1}{2} f_{a d}{ }^{e} f_{b e}{ }^{f} f_{c f}{ }^{d}-\frac{1}{2} f_{d b}{ }^{e} f_{a e}{ }^{f} f_{c f}{ }^{d}-\frac{1}{2} f_{b a}{ }^{e} f_{d e}{ }^{f} f_{c f}{ }^{d} \\
&=-\frac{1}{2} f_{a b}{ }^{e} f_{e d}{ }^{f} f_{c f}{ }^{d}=\frac{1}{2} B^{\mathrm{ad}} f_{a b c} .
\end{aligned}
$$
We learn that the renormalisation of the gluon normalisation and of the gauge coupling can both be expressed as some linear combination of $B^{\text {ad }}$ and $B^{R}$.

For completeness, let us discuss the corresponding processes for two external spinors in representation $R$ of the gauge algebra (and equivalently for two ghosts in representation $R=\mathrm{ad}$ ). The correction to the kinetic term directly yields the quadratic Casimir eigenvalue in representation $R$
$$
k^{a b} T_{a}^{R} T_{b}^{R}=C_{2}^{R}
$$
We can now add an external gluon in two inequivalent places. When it is attached to the matter line we obtain
$$
\begin{aligned}
k^{b c} T_{b}^{R} T_{a}^{R} T_{c}^{R} &=k^{b c}\left[T_{b}^{R}, T_{a}^{R}\right] T_{c}^{R}+k^{b c} T_{a}^{R} T_{b}^{R} T_{c}^{R} \\
&=-\frac{1}{2} f_{a}^{d c} f_{d c}{ }^{e} T_{e}^{R}+C_{2}^{R} T_{a}^{R} \\
&=-\frac{1}{2} B^{\mathrm{ad}} T_{a}^{R}+C_{2}^{R} T_{a}^{R} \\
&=\left(C_{2}^{R}-\frac{1}{2} B^{\mathrm{ad}}\right) T_{a}^{R}
\end{aligned}
$$
When it is attached to the gluon line instead we obtain the structure
$$
f_{a}^{b c} T_{b}^{R} T_{c}^{R}=\frac{1}{2} f_{a}^{b c}\left[T_{b}^{R}, T_{c}^{R}\right]=\frac{i}{2} f_{a}^{b c} f_{b c}^{d} T_{d}^{R}=\frac{i}{2} B^{\mathrm{ad}} T_{a}^{R} .
$$
Again the gauge theory structures come out as expected, but we obtain a different set of constants, namely $C_{2}^{R}$ and $B^{\text {ad }}$.

How can the latter possibly yield the same renormalisation of the gauge coupling which we determined to be a linear combination of $B^{R}$ and $B^{\text {ad }}$ ? ${ }^{16}$ It turns out that $C_{2}^{R}$ merely contributes to the spinor field normalisation. The dependence on $B^{R}$ enters through the gluon normalisation.

Altogether both approaches to compute the gauge coupling renormalisation yield the same final result after the respective loop integrals are evaluated. It is usually expressed in terms of the so-called beta-function ${ }^{17}$
$$\beta(g)=\frac{g^{3}}{16 \pi^{2}}\pqty{\frac{11}{3} B^{\text {ad }}-\frac{4}{3} \sum_{\text {Dirac spinors }} B^{R}-\frac{1}{6} \sum_{\text {real }} B^{R}}+\mathcal{O}\left(g^{5}\right)
$$
Here the first sum is over the representations $R$ of Dirac spinor fields and the second sum over the representations $R$ of real scalar fields. 18 Note that the different prefactors of the $B^{\prime}$ s are characteristic numbers for type of particles. ${ }^{19}$ In the special case of $N_{\mathrm{f}}$ flavours of Dirac fermions in a $\mathrm{SU}\left(N_{\mathrm{c}}\right)$ gauge theory we recover the famous combination $\frac{11}{3} N_{\mathrm{C}}-\frac{4}{3} N_{\mathrm{f}}$.
