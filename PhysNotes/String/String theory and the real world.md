# String theory and the real world

In this chapter, some of the attempts of connecting string theory to the standard model will be discussed. In particular we will discuss, what can be learnt from string theory and what the current hopes and expectations are. In what sense does string theory answer the questions of quantum gravity?
![[Pasted image 20220123230942.png]]
# Standard Model and Gravity

Making connection to the real world first and foremost refers to reproducing the gauge group of the standard model along with the [[Higgs Mechanism]]. The standard model, comprising three generations of quarks and leptons as well as the gauge bosons for the electromagnetic, the weak and the strong interactions and the Higgs particle is a nonabelian gauge theory with gauge group $\mathrm{SU}(3) \times \mathrm{SU}(2) \times \mathrm{U}(1)$. So far, the standard model has passed all experimental tests performed. The standard model, however, appears to be rather arbitrary: there are around twenty constants which have to be adjusted to very high precision in order to reproduce the experimental findings. The origin of those constants remains unclear: it would be desirable, to have a theory not only predicting the general mechanisms underlying the standard model but as well the coupling strengths and masses of and between the constituents.

In terms of a gravitational theory, the state of the art is described very quickly: starting from Einstein gravity, the most successful model based on a Friedman-Robertson-Walker solution is the $\Lambda$-cold-dark-matter model. It is capable of describing the expansion of the universe in the way we observe it with the price of introducing dark matter and dark energy. So far the search for the dark matter has not been successful: no particle from the standard model does satisfy the bounds on mass (and thus coupling to gravity) as well as the other constraints originating in the observed interactions with visible matter. In addition, it is clear that the perturbative expansion of Einstein gravity is not sufficient to describe the physics in highly curved spaces such as they appear shortly after the big bang. In order to predict the processes in those regimes, a renormalisable theory for quantum gravity is unavoidable. Up to date, no renormalisable quantum field theory for gravity is known.

Supersymmetry. So far, supersymmetry has not been observed and is not part of the standard model. From the string theory perspective, however, supersymmetry is desirable in order to obtain a theory free of tachyons with stable D-branes, which in addition allows to maintain the ratio between the electroweak scale and the Planck mass. On the other hand, one can show that supersymmetric theories with $\mathcal{N}>1$ do not allow for the chiral spectrum we observe. Balancing the two requirements leads to the goal of a four-dimensional theory with $\mathcal{N}=1$ supersymmetry.

This theory should obviously contain the standard model. The minimal solution one can have is the so called minimal supersymmetric standard model. It contains all the particles of the standard model with the addition of a Higgs doublet. Each of the particles will be assigned a superpartner. All gauge interactions are fixed by the non-supersymmetric part of the standard model. All other (non-gauge) interactions are however not constrained, which leads in the smallest version to a model exhibiting even up to about a hundred constants to fix. Another problem is that the supersymmetric partners of the standard model particles will have the same masses as the original particles. If this was the case, one would have seen the superpartners already in collider experiments. So one will have to find a mechanism spreading the masses between superpartners.

Aiming at a theory which contains gravity as well as gauge interactions, the obvious strategy is to start from $\mathcal{N}=(1,0)$ heterotic string theories in ten dimensions because these theories readily contain gauge groups which appear to be large enough to accommodate the standard model gauge group. The second ingredient allowing to shape the effective fourdimensional theory is a suitable compactification manifold: the structure of this manifold will - among many other things - determine the amount of supersymmetry present.

In practice, there are two ways to proceed: one can either construct a conformal field theory with suitable boundary conditions giving rise to a $\mathcal{N}=1$ theory in four dimensions. This leads to the orbifold compactifications. The other way is to start with the effective supergravity action derived from the heterotic theory in ten dimension and then compactify on a suitable manifold: this will lead to Calabi-Yau compactifications.

\subsection{Geometry of Toroidal Manifolds and Orbifolds}

Compactifying a theory on a torus does not break supersymmetry. In order to produce the desired $\mathcal{N}=1$ theory in four dimensions, one needs to think about a more sophisticated compactification manifold. One of the simplest generalisation of toric manifolds are orbifolds.

Orbifolds. An orbifold is a generalisation of a manifold: it is a quotient space of a Euclidean space by a finite group. Orbifolds will have orbifold fixed points, which are the points invariant under the identification. In the vicinity of those singular points, a quantum field (or string) theory defined on the orbifold will become singular itself, which will effectively reduce the number of states in the theory. In other words, respecting the symmetry group of the orbifold puts constraints on the theory defined on it. Simultaneously, at the singular points one can add new states to the theory: those go under the name of twisted sectors and they render a string theory completely smooth when combined with the regular parts.

In order to get used to the concept of an orbifold, let us start with an easy example. Take the real line $\mathbb{R}$, define a lattice

$$
\Lambda=a \mathbb{Z}
$$

and identify points via

$$
x \simeq x+l \quad \text { for all } x \in \mathbb{R}, l \in \Lambda .
$$

The interval $0 \leq x<a$ is called the fundamental domain, while $\mathbb{R}$ is the covering space of the torus $T$. Now one defines a parity operation

$$
P x=-x \quad \text { for all } x \in \mathbb{R}
$$

and identifies

$$
x \simeq P x \quad \text { for all } x \in \mathbb{R} .
$$

Noticing that $P^{2}=1, P$ is a realisation of the cyclic group $\mathbb{Z}_{2}$. The fixed points under the combined lattice and parity identifications are $x=0$ and $x=1 / 2$. The resulting space is the orbifold $T / \mathbb{Z}_{2}$.

In order to get from ten dimensions to four, one needs to choose a manifold of the form

$$
O^{6}=T^{6} / \mathrm{G},
$$

where, for simplicity, $\mathrm{G}$ is assumed to be a finite abelian point group. In the following we will work with the example $\mathrm{G}=\mathbb{Z}_{3}$. Conveniently, a point on this orbifold can be labelled by complex coordinates $z_{i}$ with $i=1,2,3$, which corresponds to splitting the torus into $T^{6}=T_{1}^{2} \times T_{2}^{2} \times T_{3}^{2}$. An orbifold with this property is called factorisable.

In complete analogy to the physicality conditions for the periodicity conditions for the compactification of one dimension in the context of T-duality, the periodicity conditions on the orbifold read

$$
z_{i} \sim z_{i}+2 \pi R_{i} \text { and } z_{i} \sim z_{i}+2 \pi R_{i} \rho_{i} \text {, }
$$

where $R_{i}$ are the radii of the tori and $\rho_{i}$ are the corresponding complex structure moduli (which are the equivalent of the quantity $\tau$ in the discussion of the fundamental domain of the worldsheet).

In terms of the coordinates $z_{i}$ one can define the orbifold action $\Theta$, which reads

$$
\Theta\left(z_{i}\right)=\exp \left(2 \pi i \phi_{i}\right) z_{i},
$$

where the phases $\phi_{i}$ have to be integral multiples of $1 / 3$ in order to yield $\Theta^{3}=1$. The orbifold action needs to be compatible with the torus lattice, which in turn is defined by the complex structure moduli $\rho_{i}$. These conditions are pretty restrictive and allow to fix the phases $\phi$ uniquely to

$$
\phi=\frac{1}{3}(1,1,-2) .
$$

Breaking of Supersymmetry. Let us now see, how the manifold $T^{6} / \mathbb{Z}_{3}$ described above actually will break the supersymmetry in the original theory in a way that the fourdimensional effective theory will have $\mathcal{N}=1$ supersymmetry. In ten dimensions, the supercharge $Q$ is a 16-component spinor, which can be represented by a state $\left|s_{-1}, s_{0}, s_{1}, s_{2}, s_{3}\right\rangle$ with $s=\pm 1 / 2$ and $\prod_{i=-1}^{3} s_{i}=1 / 2$. The orbifold action $\Theta$ acts as

$$
\begin{aligned}
\Theta\left|s_{-1}, s_{0}, s_{1}, s_{2}, s_{3}\right\rangle &=\exp \left(2 \pi i \sum_{i=1}^{3} \phi_{i} s_{i}\right)\left|s_{-1}, s_{0}, s_{1}, s_{2}, s_{3}\right\rangle \\
& \stackrel{!}{=}\left|s_{-1}, s_{0}, s_{1}, s_{2}, s_{3}\right\rangle,
\end{aligned}
$$

and needs to leave the spinor invariant. For the values of $\phi_{i}$ fixed by the periodicity conditions on the orbifold, there is exactly one solution to the above equation $(\alpha=\pm 1)$ :

$$
\left|s_{-1}, s_{0}, \frac{1}{2} \alpha, \frac{1}{2} \alpha, \frac{1}{2} \alpha\right\rangle .
$$

Counting the number of independent spinor components of the above form reveals that the orbifold geometry indeed singles out four of the sixteen spinors in ten dimensions, which effectively leads to $\mathcal{N}=1$ supersymmetry in four dimensions.

One can construct a worldsheet conformal field theory with appropriate non-trivial boundary conditions, which will lead to this orbifold compactification in target space. From the worldsheet perspective this is still a free conformal field theory which can be solved exactly. This means in particular that one can derive the complete partition function and demand modular invariance, which will lead to additional constraints on the target space theory. The calculation is rather involved, but easy enough to allow for a complete classification of all possible orbifold conformal field theories originating from the orbifold $T^{6} / \mathbb{Z}_{3}$ starting from the heterotic string with gauge group $\mathrm{SO}(32)$.

The gauge groups of the resulting effective four-dimensional theories are very large and appear to be rather arbitrary. This unsatisfactory situation can be improved by introducing Wilson lines, which can be thought of as constant gauge fields in the string background. The introduction of these Wilson lines allows to equip the twisted sectors of different orbifold fixed points with different gauge groups. Correspondingly, the boundary conditions for the conformal field theory change. For the $T^{6} / \mathbb{Z}_{3}$-orbifold, one can add up to three Wilson lines.

There exists a $T^{6} / \mathbb{Z}_{3}$-model obtained from a heterotic string theory with gauge group $\mathrm{E}_{8} \times \mathrm{E}_{8}$ with the field content of the minimal supersymmetric standard model. However, in addition to the desired particles, there are many vector-like exotic particles, which do not decouple completely and thus yield additional unwanted states.

\subsection{Calabi-Yau Compactification of $D=10$ Super- gravity}

Let us just briefly comment on the second option pointed out above: one could as well start with the effective action of ten-dimensional supergravity coupled to ten-dimensional SYM theory and compactify this on a suitable manifold. As opposed to the orbifolds in the previous subsection, which are singular spaces, here one will use non-singular (or smooth) spaces.

Compactifying on a non-singular space, one still wants to obtain a $\mathcal{N}=1$ supersymmetric model in four dimensions with three generations of leptons and quarks. The translation of those properties into constraints on the compactification manifold leads to a very special type of manifolds: the Calabi-Yau manifolds.

While numerous Calabi-Yau compactifications have been studied, the best known is the so-called standard embedding: it starts from the ten-dimensional effective action of the heterotic $\mathrm{E}_{8} \times \mathrm{E}_{8}$ string. After compactifying on a suitable Calabi-Yau manifold one will obtain a four-dimensional model with gauge group $\mathrm{E}_{6} \times \mathrm{E}_{8}$. For some ranges of parameters, this model will yield the minimal supersymmetric standard model.

\subsection{String Theory as a Phenomenological Model}

The investigation of string compactifications is still an active field of research. However, finding a compactification yielding an effective model which is just the standard model has not been successful so far. If one allows for the minimal supersymmetric extension of the standard model, string theory can produce something similar, however, usually there are additional states which can not be consistently decoupled.

In terms of quantum gravity, string theory provides a structurally sound model for a theory of quantum gravity. Practically, however, experiments which would be capable of confirming the validity of the string theory predictions beyond the classical limit are insurmountable.

Overall, string theory appears to be a promising concept. However, the amount of engineering needed to relate string theories to realistic quantum field theories seems rather unnatural.