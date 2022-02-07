Gauge Theory. Let us finally discuss the renormalisation of YangMills theory coupled to matter, in particular its consistency.

In non-abelian gauge theory we have various couplings between the gauge, [[Faddeev-Popov ghosts|ghost]] and matter fields

![[Pasted image 20220127083325.png|400]]

Furthermore, there are some pure matter couplings such as mass terms, cubic and quartic couplings of the scalars as well as Yukawa couplings which we will not consider here.

For gauge invariance it is crucial that the various interactions have a very specific form: **For instance, every cubic vertex should contain a factor of $g$ and some gauge invariant tensor relative to the kinetic term with one gauge leg removed. Likewise the quartic vertices have these factors squared.**

All the above couplings have dimension 4 and therefore are expected to require renormalisation. On general grounds we should expect that all couplings renormalise independently. It is conceivable that each graph may have a counterterm with an individual coefficient. This would be troublesome for two reasons:
- At leading order all the gauge couplings were determined by a universal constant $g$ and the discrete choice of representation. Renormalisation would introduce an individually tunable constant for each type of field, and thus reduce the predictive power of the model.
- Gauge invariance would break down which in turn would break renormalisability of the vector field.

Does gauge invariance survive renormalisation?
Gladly, it turns out that the above vertices renormalise coherently. The reason is symmetry. Although we had to break gauge symmetry to quantise the theory, there are two parts left:

- Manifest global symmetry under the gauge group: This symmetry ensures that all vertices are governed by invariant tensors of the gauge group. Moreover, the relative coefficients are fixed by the Ward-Takahashi identity which is the quantum analog of the conservation of Noether currents. Therefore the coupling $g$ acts as a universal renormalised gauge coupling constant.
- BRST symmetry: This symmetry ensures that the ghosts and the unphysical polarisations of the vector field are equivalent up to signs which make their overall contribution cancel exactly.

The above 5 classes of terms therefore lead to 6 independent renormalisation coefficients:
- One renormalisation coefficient for each line.
- In total one relative renormalisation coefficient for the elements in each line.

They are interpreted as follows:
- One coefficient to renormalise the kinetic term of each type of field, namely the gauge, [[Faddeev-Popov ghosts|ghost]], spinor and scalar fields. These are all independent and they have no physical relevance on their own. Nevertheless, they are important coefficients which contribute to each graph via the external legs.
- One coefficient to (potentially) renormalise the constant $\xi$.
- One coefficient to renormalise the gauge coupling $g$.