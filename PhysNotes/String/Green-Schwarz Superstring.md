---
alias:
- spacetime Supersymmetry
- target space supersymmetry
---
# Green-Schwarz Superstring

There are two approaches to formulate a supersymmetric string theory in $D=10$ dimensions. One can either make the worldsheet or the [[embedding space|target space]] supersymmetric. Both approaches turn out to be equivalent. Here we shall begin with [[embedding space|target space]] [[Supersymmetry]]: the corresponding approach is called the Green-Schwarz superstring.

# Action. 
We shall discuss the type II superstring where we add two fermionic fields $\Theta_{I}^{m}$, $I=1,2$, to the worldsheet theory. The fields transform as worldsheet scalars and [[embedding space|target space]] spinors. They have equal or opposite chirality for so-called IIB and IIA string theory, respectively.

[[embedding space|Target space]] is now a superspace with coordinates $X^{\mu}$ and $\Theta_{I}^{m}$. The worldsheet theory of string theory is formulated in terms of line elements. The supersymmetric line elements $\Pi$ receive some extra contributions from the fermionic directions

$$
\Pi_{\alpha}^{\mu}=\partial_{\alpha} X^{\mu}+\delta^{I J} \gamma_{m n}^{\mu} \Theta_{I}^{m} \partial_{\alpha} \Theta_{J}^{n}
$$

The action then takes the convenient form

$$
\begin{aligned}
S \sim & \int \mathrm{d} \xi^{2} \sqrt{-\operatorname{det} g} g^{\alpha \beta} \eta_{\mu \nu} \Pi_{\alpha}^{\mu} \Pi_{\beta}^{\nu} \\
&+\int\left(\left(\Theta^{1} \gamma_{\mu} \mathrm{d} \Theta^{1}-\Theta^{2} \gamma_{\mu} \mathrm{d} \Theta^{2}\right) \mathrm{d} X^{\mu}+\Theta^{1} \gamma_{\mu} \mathrm{d} \Theta^{1} \Theta^{2} \gamma^{\mu} \mathrm{d} \Theta^{2}\right) .
\end{aligned}
$$

In addition to diffeomorphisms, this action has so-called kappa symmetry which is a local worldsheet [[Supersymmetry]] and which effectively removes half of the fermionic fields. Importantly, this symmetry applies only in $D=10$ dimensions of [[embedding space|target space]]!

Note: the fermions $\Theta$ have first and second class constraints. Non-linear equations of motion. In general difficult to quantise canonically. Conformal gauge does not resolve these difficulties.


# Spectrum. 
Next let us consider the vacuum energy, CFT central charge and anomaly cancellations:

- For the left and right movers, there are 8 bosonic and 8 fermionic d.o.f. each where the latter contribute with negative sign to the intercept $a$

$$
a_{\mathrm{L} / \mathrm{R}}=\frac{1}{2} 8 \zeta(-1)-\frac{1}{2} 8 \zeta(-1)=0 .
$$
There is no shift $a$ for the $L_{0}$ constraint. Therefore the level zero is massless. **There is no tachyon**!

Importantly, the number of bosonic and fermionic d.o.f. is precisely the same. This can only happen in particular low number of spacetime dimensions such as $D=10$.

- Before light cone gauge, there are 10 bosonic fields $X^{\mu}$ and 32 fermionic fields $\Theta_{I}^{m}$. Due to kappa symmetry, only half of the latter to the CFT central charge

$$
c=10+32 \frac{1}{2}=26 \text {. }
$$

This number is the same as for bosonic string theory and cancels precisely against the contribution of [[Faddeev-Popov ghosts|ghost]] fields.

- The super-Poincaré anomaly cancels in light cone gauge.

As for the bosonic string, we can expand the closed superstring fields into Fourier modes. This leads to the bosonic modes $\alpha_{n}$ and fermionic modes $\beta_{n}$, where the modes $n<0$, $n=0, n>0$ take the roles of creation operators, zero modes and annihilation operators, respectively.

