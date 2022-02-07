---
alias:
tags:
- qftII
---
Above we have discussed equations that hold due to symmetries in the QFT. An important aspect of symmetries in QFT is that they may break due to quantum effects. Such symmetries are called [[anomaly|anomalous]].

- [[scaling anomaly]]
- [[axial anomaly in massless QED]]

# Comments. 
Anomalies are an exciting topic of quantum field theory which we cannot treat in detail in this course. Let us nevertheless make a few more remarks:

Anomalies are often related to **topological issues of spacetime and of the gauge groups**. The corresponding anomalous Slavnov-Taylor identity is typically one-loop exact.

Gauge fields can also be coupled to the axial current. In fact, the electroweak sector of the standard model relies on such couplings. **The presence of an axial anomaly would be disastrous since it would violate gauge invariance. Gladly, all such anomalies cancel in the standard model due to a particular arrangement of spinor fields**. This is called anomaly cancellation and it represents one of the consistency requirements of QFT on the particle spectrum.

Note that the coupling of a chiral spinor to a gauge field effectively is a combination of vector and axial vector currents. Hence, chiral spinor fields are the origin of the so-called chiral anomaly. The chiral anomaly for quarks can be observed in meson decay.

Anomalies are universal statements of QFT. They state that certain symmetries are incompatible with the quantisation procedure. An anomaly can only occur for non-manifest symmetries which are not respected by the regulator. When the regulator is removed after renormalisation, some of these non-manifest symmetries may turn out intact if the renormalisation parameters are chosen appropriately. **If there is no way to recover the symmetry using local counterterms, the symmetry is anomalous.**

The amount by which the symmetry is broken is a universal statement independent of the regularisation scheme. The anomaly is typically attributed to non-invariance of the integration measure D $\Psi$ of the path integral.

Note that even though anomalies are universal, some details may depend on the implementation. Some anomalies refer to pairs of symmetries which cannot be realised simultaneously. The renormalisation process can be adjusted to preserve one symmetry at the cost of the other. Alternatively the other symmetry can be preserved with suitable counterterms. A third option is to break both symmetries. For example, the axial current can be redefined to be exactly conserved, but only at the cost of an anomaly for the vector current. The latter is highly undesirable since it would definitely break gauge invariance. Therefore, one usually makes sure that the vector current is non-anomalous.