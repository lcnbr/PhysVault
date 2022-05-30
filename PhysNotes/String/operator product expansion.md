---
alias:
- OPE
- OPEs

---

# Operator Product Expansion

In a [[7 CFT/conformal field theory|CFT]] we wish to compute [[correlation functions]]

$$
\left\langle\mathcal{O}_{1}\left(\xi_{1}\right) \mathcal{O}_{2}\left(\xi_{2}\right) \ldots \mathcal{O}_{n}\left(\xi_{n}\right)\right\rangle=F_{12 \ldots n}
$$

Suppose $\xi_{1} \approx \xi_{2}$; then one can Taylor expand

$$
\mathcal{O}_{1}\left(\xi_{1}\right) \mathcal{O}_{2}\left(\xi_{2}\right)=\sum_{n=0}^{\infty} \frac{1}{n !}\left(\xi_{2}-\xi_{1}\right)^{n} \mathcal{O}_{1}\left(\xi_{1}\right) \partial^{n} \mathcal{O}_{2}\left(\xi_{1}\right)
$$

The expansion converts [[Local Operators]] at two points into a sum of [[Local Operators]] at a single point. The classical statement is exact.

# Quantum OPE
Quantum-mechanically there are additional contributions from operator ordering because normal ordering is implicit. However, the product of [[Local Operators]] can still be written as sum of some [[Local Operators]]

$$
\mathcal{O}_{1}\left(\xi_{1}\right) \mathcal{O}_{2}\left(\xi_{2}\right)=\sum_{i} C_{12}^{i}\left(\xi_{2}-\xi_{1}\right) \mathcal{O}_{i}\left(\xi_{1}\right) .
$$

The above statement has to be understood in terms of a [[Conformal Correlators|correlator]]. More precisely, with the insertion of any (non-local combination of) operators "..." it reads

$$
\left\langle\mathcal{O}_{1}\left(\xi_{1}\right) \mathcal{O}_{2}\left(\xi_{2}\right) \ldots\right\rangle=\sum_{i} C_{12}^{i}\left(\xi_{2}-\xi_{1}\right)\left\langle\mathcal{O}_{i}\left(\xi_{1}\right) \ldots\right\rangle
$$

This statement is called *[[.md|operator product expansion]]* (OPE), where $C_{i j}^{k}\left(\xi_{2}-\xi_{1}\right)$ are called *structure constants* and *conformal blocks*. The sum extends over all [[Local Operators]] (including [[../math/descendants]]).

This is a very powerful idea: every (non-local) operator can be written as an expansion in [[Local Operators]]. This statement is analogous to the multipole expansion of electrodynamics. The formalism works exactly in any [[7 CFT/conformal field theory|CFT]] and is a central tool.

# Higher Points. 
Formally, one can compute higher-point correlation functions:

$$
F_{123 \ldots n}=\sum_{i} c_{12}^{i} F_{i 3 \ldots n} .
$$

Recursively, one can reduce to the one-point function, which is trivial except for the unit operator 1

$$
\left\langle\mathcal{O}_{i}\right\rangle=0, \quad\langle 1\rangle=1 .
$$

Higher-point functions can thus be reduced to a sequence of structure constants $C_{i j}^{k}$. This is a vast simplification: one needs only $C_{i j}^{k}$ in order to describe correlators in [[7 CFT/conformal field theory|CFT]]. In practice, the structure constants are hard to compute and moreover the result of a single OPE are infinitely many [[Local Operators]]. Superficially, the result seems to depend on the sequence of reducing correlators using OPE's. This is of course not true because the structure constants are special quantities which obey crossing relations that ensure independence of the way the correlator is decomposed. 

# Lower Points. 
one-point function, is trivial except for the unit operator 1
$$
\left\langle\mathcal{O}_{i}\right\rangle=0, \quad\langle 1\rangle=1 .
$$
The two-point function is equivalent to an OPE onto the unit operator

$$
F_{i j}=\left\langle\mathcal{O}_{i} \mathcal{O}_{j}\right\rangle=\sum_{k} C_{i j}^{k}\left\langle\mathcal{O}_{k}\right\rangle=C_{i j}^{1} .
$$

The OPE constants are determined by the three-point functions

$$
F_{i j k}=\left\langle\mathcal{O}_{i} \mathcal{O}_{j} \mathcal{O}_{k}\right\rangle=\sum_{l} C_{i j}^{l}\left\langle\mathcal{O}_{k} \mathcal{O}_{l}\right\rangle=\sum_{l} F_{k l} C_{i j}^{l} .
$$

Lower-point functions are restricted tightly by [[conformal invariance|conformal symmetry]]:

- Two-point function are non-trivial only for operators related by [[conformal invariance|conformal symmetry]] ([[../math/descendants]]).
- Non-trivial three-point functions exist for three unrelated operators.

[[conformal invariance|Conformal symmetry]] allows to map a triple of points to any other triple of points. Consequently, there are no conformally invariant functions depending on the positions of two or three points only: the correlator will always contain quantities like the scaling weight etc.. This implies the following form for correlation functions:

- The coordinate dependence of a two-point function is fixed (c.f. [[CFT 2-correlator]])
$$
F_{i j} \sim \frac{N_{i j}}{\left|\xi_{i}-\xi_{j}\right|^{2 \Delta_{i}}} .
$$
The form of the exponent $2 \Delta_{i}=\Delta_{i}+\Delta_{j}$ implies that the two-point function is nontrivial only, if the two operators have equal conformal dimension[[[Lorentz invariant]]. 

- The coordinate dependence of a three-point function is fixed
$$
F_{i j k} \sim \frac{N_{i j k}}{\left|\xi_{i}-\xi_{j}\right|^{\Delta_{i j}}\left|\xi_{j}-\xi_{k}\right|^{\Delta_{j k}}\left|\xi_{k}-\xi_{i}\right|^{\Delta_{k i}}}
$$
with scaling weights $\Delta_{i j}=\Delta_{i}+\Delta_{j}-\Delta_{k}$. The numerators $N_{i j}$ and $N_{i j k}$ depend on dimension, spin, level of descendant and operator normalisation.

- Higher-point functions can depend on the available conformally invariant cross ratios in an arbitrary fashion.

Once one has chosen a normalisation for operators, the data in a [[7 CFT/conformal field theory|CFT]] consists of

- [[conformal weight#^scaleingdim|scaling dimension]] along with the [[conformal weight#^confspin|spins]] of the [[Local Operators]]: this gives us the spectrum!,
- coefficients of three-point function: structure constants.