# Higgs Mechanism. 

The [[continuous symmetry breaking]] model  for $N=2$ is equivalent to a complex scalar field $\phi, \phi^{*}$. We couple it to the electromagnetic field to obtain scalar QED, but we assume that the mass term has the opposite sign
$$
\mathcal{L}_{\mathrm{SQED}}=-\left(D^{\mu} \phi\right)^{*}\left(D_{\mu} \phi\right)+\mu^{2} \phi^{*} \phi-\frac{1}{4} \lambda\left(\phi^{*} \phi\right)^{2}-\frac{1}{4} F^{\mu v} F_{\mu v}
$$
The [[YM covariant derivative|covariant derivative]] is defined as $D_{\mu} \phi=\partial_{\mu} \phi-i q A_{\mu} \phi$.
Here the ground state solution is specified by a point on a circle in the complex plane (c.f. [[continuous symmetry breaking#^e16c3e|O(N)]] or [[discrete symmetry breaking#^b869b7|Z2]])
$$
\phi^{*} \phi=\frac{1}{2} v^{2}, \quad v=\sqrt{4 \mu^{2} / \lambda},
$$
We could go ahead as [[continuous symmetry breaking#^79b5cb|before]] and introduce a shifted quantum field
$$
\phi(x)=\frac{1}{\sqrt{2}}(v+\eta(x)+i \rho(x)) .
$$

^f9e5b8

This would lead to the same form of Lagrangian as [[continuous symmetry breaking#^288446|before]]  with the exception of the kinetic term which yields
$$
\begin{aligned}
-\left(D^{\mu} \phi\right)^{*}\left(D_{\mu} \phi\right)=&-\frac{1}{2}(\partial \eta)^{2}-\frac{1}{2}(\partial \rho)^{2}-\frac{1}{2} q^{2} v^{2} A^{2}+q v A_{\mu} \partial^{\mu} \rho \\
&+\text { interactions. }
\end{aligned}
$$

^891e65

As it stands this is not a very pleasant form due to the quadratic coupling between the gauge field $A_{\mu}$ and the scalar field $\rho$. We must first diagonalise by shifting the gauge field appropriately
$$
A_{\mu}(x)=V_{\mu}(x)+(q v)^{-1} \partial_{\mu} \rho(x) .
$$

^36ff46

This shift changes the kinetic terms in the Lagrangian substantially
$$
-\left(D^{\mu} \phi\right)^{*}\left(D_{\mu} \phi\right)=-\frac{1}{2}(\partial \eta)^{2}-\frac{1}{2} q^{2} v^{2} V^{2}+\text { interactions. }
$$
Note that the kinetic term for the field $\rho$ has cancelled out exactly. What remains is one scalar field $\eta$ and a mass term for the vector field with mass $m=q v$.

This is the Higgs effect: **The coupling of the gauge field to a [[Goldstone's theorem#^a6b82b|conserved current]] of a spontaneously broken symmetry lends the gauge field a mass. Moreover, one of the scalar fields is absorbed completely by this process.**


# Alternative parametrisation
There is an alternative parametrisation of the fields which makes the above statement more obvious. The crucial observation is that the [[#^36ff46|above reparametrisation]] of the gauge field is a [[gauge transformation]]. We thus split the complex scalar field into absolute value and complex phase
$$
\phi(x)=\frac{1}{\sqrt{2}}(v+\eta(x)) \exp (i \alpha(x)) .
$$
By means of a gauge transformation we can remove the phase from the field $\phi$ without changing any of the terms in the Lagrangian
$$(v+\eta(x)) .
$$

It appears as though one degree of freedom is lost. However, it is compensated by the loss of [[gauge symmetry]] since the field $\phi$ is now real and must not be rotated in the complex plane. [[gauge symmetry]] effectively removes one degree of freedom from the gauge field. In that sense, we have merely transferred the complex phase of $\phi$ into the field $A_{\mu}$ which henceforth should be considered a vector field $V_{\mu}$ rather than a gauge field. The resulting Lagrangian reads
$$
\begin{aligned}
\mathcal{L}_{\text {SQED }}=&-\frac{1}{2}(\partial \eta)^{2}-\frac{1}{4} v^{2} \lambda \eta^{2} \\
&-\frac{1}{2}\left(\partial^{\mu} V^{v}\right)\left(\partial_{\mu} V_{v}\right)+\frac{1}{2}(\partial \cdot V)^{2}-\frac{1}{2} q^{2} v^{2} V^{2} \\
&+\frac{1}{16} v^{4} \lambda-\frac{1}{4} \lambda v \eta^{3}-\frac{1}{16} \lambda \eta^{4}-q^{2} v V^{2} \eta-\frac{1}{2} q^{2} V^{2} \eta^{2} 
\end{aligned}
$$

^8dcf8d

We thus obtain a scalar field $\eta$ with mass $\sqrt{v^{2} \lambda / 2}$ and a vector field $V_{\mu}$ with mass $q v$. The scalar field interacts with itself and with the square of the vector field.

The Lagrangian has a very special form: Altogether it has 2 mass terms and 5 interaction terms (the coefficient of $\eta V_{\mu} \partial^{\mu} \eta$ is zero). Using the $\mathbb{Z}_{2}$ symmetry $\eta \rightarrow-2 v-\eta$ these numbers reduce to 4 coefficients. However, there are only three parameters $v, q$ and $\lambda$, so there is one constraint among the set of conceivable parameters. This feature is owed to the [[gauge symmetry]] in the original formulation of the Lagrangian. It will be crucial for a successful renormalisation.


# Comments. 

Above we have presented an example of the Higgs mechanism for an abelian [[gauge symmetry]]. The Higgs mechanism works analogously for a non-abelian [[gauge symmetry]]: **For each broken generator of the gauge group, the associated gauge field acquires a mass. Goldstone bosons never appear for broken gauge symmetries.**
The configuration of massive scalar fields very much depends on the particular model. In principle, spontaneous symmetry breaking can be achieved without additional massive scalar fields. For example, sigma models on group manifolds and coset spaces thereof are particular implementations. However, these models typically have non-polynomial interactions and therefore are non-renormalisable. **Spontaneous symmetry breaking in models with polynomial interactions requires the presence of at least one massive scalar field**. ^[In the above examples, this is the “magnitude” direction of the scalar potential.
] In that sense, **the Higgs mechanism implies a massive scalar field, the so-called Higgs particle.**

Note that the number of independent particle modes is preserved by the Higgs mechanism: We start with some scalar fields and some massless vector fields. **For each broken generator of the gauge algebra one of the scalar fields disappears in favour of a massive vector field**. A massless vector field has two on-shell degrees of freedom whereas a massive one has three. The additional degree of freedom originates from the scalar field; **the gauge field eats a scalar field to become massive**.  ^[In fact, the scalar origin of the additional mode for the massive vector can be observed at very high energies: There the masses of particles are largely irrelevant and the massive vector decomposes into a massless vector and a scalar.
]