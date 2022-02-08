---
Alias:
- worldsheet Supersymmetry
- worldsheet supersymmetry
- worldsheet susy
- RNS
- NS
- R-
- R+
---
# Ramond-Neveu-Schwarz Superstring

There is an alternative formulation for the superstring: the so-called Ramond-NeveuSchwarz (RNS) superstring. This formulation has manifest [[Ramond-Neveu-Schwarz Superstring|worldsheet Supersymmetry]] while  [[Green-Schwarz Superstring|spacetime supersymmetry]] is obscured.

# Action. 
The action of the RNS superstring in conformal gauge consists of the real bosonic scalar fields $X^{\mu}$ and a pair of real fermionic spinors of either chirality $\Psi_{\mathrm{L}, \mathrm{R}}^{\mu}$

$$
S \sim \int \mathrm{d} \xi^{2} \eta_{\mu \nu}\left(\frac{1}{2} \partial_{\mathrm{L}} X^{\mu} \partial_{\mathrm{R}} X^{\nu}+i \Psi_{\mathrm{L}}^{\mu} \partial_{\mathrm{R}} \Psi_{\mathrm{L}}^{\nu}+i \Psi_{\mathrm{R}}^{\mu} \partial_{\mathrm{L}} \Psi_{\mathrm{R}}^{\nu}\right) .
$$

This action is manifestly supersymmetric on the worldsheet which implies that bosons and fermions must transform equally under spacetime symmetries. Therefore also the fermionic fields are vectors of $\mathrm{SO}(9,1)$. This appears to violate the spin statistics theorem for the spacetime theory, but this problem can be resolved as we shall see shortly.

The bosonic fields behave as for the bosonic string. For the boundary conditions of the fermionic fields there is an important choice to be made; they can be either periodic or anti-periodic. This leads to two sectors of the theory which are analogous to the various open and closed string sectors. They are represented by two set of vacuum states which are unrelated by acting with string mode excitations. 

# Ramond Sector. 
One sector has periodic boundary conditions for the fermionic field

$$
\Psi(\sigma+2 \pi)=+\Psi(\sigma)
$$

It is called the Ramond $(R)$ sector:

- Alike the bosonic modes $\alpha_{n}^{\mu}$, the fermionic fields are expanded into integer Fourier modes $\beta_{n}^{\mu}$.
- Since there are fermionic zero modes $\beta_{0}^{\mu}$, the vacuum is a supermultiplet. The states transform in a chiral and in an anti-chiral 16-component real spinor of Spin $(9,1)$.
- The intercept is zero
$$
a=-\frac{1}{2} 8 \zeta(-1)+\frac{1}{2} 8 \zeta(-1)=0,
$$
hence there **cannot be tachyons in this sector**.

All above states transform as worldsheet spinors. Therefore they should respect fermionic statistics. However, there are states of either statistics in the Ramond sector.

This problem is resolved by the Glizzi-Scherk-Olive (GSO) projection which essentially restricts to states with fermionic statistics. This is a consistent projection of the string even in the presence of interactions. Note that this leaves a choice: One can assign the chiral vacuum states to be bosonic or fermionic. It leads to two inequivalent Ramond sectors $R+$ and $R-$.

# Neveu-Schwarz Sector. An alternative consistent choice is periodic boundary conditions for the fermionic field

$$
\Psi(\sigma+2 \pi)=-\Psi(\sigma) .
$$

This leads to the so-called Neveu-Schwarz (NS) sector.

- The fermionic fields are expanded into half-integer Fourier modes $\beta_{n+1 / 2}^{\mu}$.

- There are no fermionic zero modes therefore the string vacuum for this sector is a single fermionic scalar.

- The intercept is non-zero
$$
a=-\frac{1}{2} 8 \zeta(-1)+\frac{1}{2} 8 \zeta\left(-1, \frac{1}{2}\right)=\frac{1}{2},
$$
hence the sector contains tachyons.

All the states transform as integer-spin representations of spacetime, but again there are states of either statistics. The GSO projection for the NS sector restricts to bosonic states, i.e. states with an odd number of fermionic generators $\beta$. The GSO projection has the beneficial effect of **removing the tachyonic level 0** . Physical states start at level $1 / 2$ which is massless.

# Type IIA and IIB Superstring models. 
The fermion periodicity conditions in the RNS formulation of the superstring can be selected individually for the left and right moving fields. There are four sectors in a consistent formulation of the closed superstring: NS-NS, NS-R, R-NS, R-R. The NS-NS and R-R sectors provide the bosonic particles, the NS-R and R-NS sectors the fermionic ones.
![[Ramond-Neveu-Schwarz Superstring_2022-01-23 22.32.47.excalidraw]]
For each $\mathrm{R}$ sector there is a choice of Glizzi-Scherk-Olive (GSO) projection $^{6}$. For equal or opposite choices for the left and right moving sectors, one obtains the type IIB and IIA superstrings, respectively.

# Superconformal algebra on the worldsheet. 
Conformal symmetry combines with the manifest [[Supersymmetry]] on the worldsheet to superconformal symmetry. As usual, there are two copies of conformal symmetry for a closed string: one for the left movers and one for the right movers. Let us consider just one copy.

The stress-energy tensor and conformal supercurrent read:

$$
T=\partial X \cdot \partial X+\frac{i}{2} \Psi \cdot \partial \Psi, \quad J=\Psi \cdot \partial X .
$$

The superconformal algebra is generated by bosonic generators $L_{n}$ and fermionic generators $G_{r}$. They obey the following algebra ${ }^{7}$

$$
\begin{aligned}
\left[L_{m}, L_{n}\right] &=(m-n) L_{m+n}+\frac{1}{8} c m\left(m^{2}-1\right) \delta_{m+n}, \\
\left[L_{m}, G_{r}\right] &=\left(\frac{1}{2} m-r\right) G_{m+r}, \\
\left\{G_{r}, G_{s}\right\} &=2 L_{r+s}+\frac{1}{2} c\left(r^{2}-\frac{1}{4}\right) \delta_{r+s} .
\end{aligned}
$$

Here the bosonic generators $L_{n}$ occupy integer modes $n$ while the modes of the fermionic generators depend on the sector. In the $\mathrm{R}$ or NS sectors, $2 r$ is even or odd, respectively. The corresponding superalgebras are called Ramond and Neveu-Schwarz algebras.



|                             |      GS      |     RNS      |
|:---------------------------:|:------------:|:------------:|
|   fermions are spinors in   | target space |  worldsheet  |
|  worldsheet supersymmetry   |    (yes)     |   manifest   |
| superconformal field theory |      no      |     yes      |
| target space supersymmetry  |   manifest   |    (yes)     |
|   supergravity couplings    |     all      | some (NS-NS) |
|     spacetime covariant     |      no      |    (yes)     |

