---
alias:
- Mandelstam variables
- s-channel
- s-variable
- t-channel
- t-variable
- u-channel
- u-variable
tag:
- qft
- feynmanDiag
---
In -+++
 $s, t, u$

$$
s=-\left(q_{1}+q_{2}\right)^{2}, \quad t=-\left(q_{1}+q_{4}\right)^{2}, \quad u=-\left(q_{1}+q_{3}\right)^{2},
$$

with the relation $s+t+u=-q_{1}^{2}-q_{2}^{2}-q_{3}^{2}-q_{4}^{2}$

In +---

From landau lifshitz 4


Let us consider some kinematic relations for scattering processes in which there are only two particles, both in the initial state and in the final state. The relations in question are deduced from the general conservation laws alone, and are therefore valid for all particles and all laws of interaction.

![[../../Attachements/s-channel 2022-04-29 14.44.24.excalidraw|100|left-wrap]]
The law of conservation of 4-momentum, in a general form that does not specify which are the initial and which the final particles, is$$
q_{1}+q_{2}+q_{3}+q_{4}=0 .
$$Here $\pm q_{a}$ are the momentum 4-vectors; two of them pertain to the incident particles and two to the scattered particles, the momenta for the latter being $-q_{a}$. Thus for two of the $q_{a}$ the time component $q_{a}^{0}>0$, and for two $q_{a}^{0}<0$. ^ca96c7

The law of charge conservation must be satisfied as well as that of 4-momentum conservation. Here the charge may be interpreted not only as the electric charge but as any other conserved quantity whose sign is opposite for particles and antiparticles.

For given types of particles concerned in the process, the squares of the 4-vectors $q_{a}$ are the squares of the particle masses, which are fixed $\left(q_{a}^{2}=m_{a}^{2}\right)$. Three different reactions occur, according to the values taken by the time components $q_{a}^{0}$ and the values of the charges. These reactions may be written
(I) $1+2 \rightarrow 3+4$,
(II) $1+\overline{3} \rightarrow \overline{2}+4$,
(III) $1+\overline{4} \rightarrow \overline{2}+3$.
Here the numbers refer to the particles, and the bar over a number denotes the corresponding antiparticle. The change from one reaction to another, i.e. the transfer of a particle to the opposite side of the formula, corresponds to a change in sign of the corresponding time component $q_{a}^{0}$ and in the sign of the charge (i.e. a replacement of the particle by its antiparticle). The reactions inverse to (66.2) are also possible, of course.

The three processes (66.2) are referred to as three cross-channels of a single general reaction.

The following are some examples. If particles 1 and 3 are electrons, and 2 and 4 are photons, then channel I represents the scattering of a photon by an electron; channel III is the same as channel I, since the photon is strictly neutral. Channel II is the conversion of an electron-positron pair into two photons. If all four particles are electrons, then channel I is the scattering of an electron by an electron, and channels II and III the scattering of a positron by an electron. If particles 1 and 3 are electrons, and 2 and 4 are muons, then channel $I$ is the scattering of $e$ by $\mu$, channel III the scattering of $e$ by $\bar{\mu}$, and channel II the conversion of a pair $e \bar{e}$ into a pair $\mu \bar{\mu}$.

In the discussion of scattering processes, the invariant quantities which can be constructed from the 4-momenta are particularly important. The invariant scattering amplitudes are functions of these quantities ( $\S 70)$.

Two independent invariants can be constructed from four 4-momenta, since, according to (66.1), only three of the 4-vectors $q_{a}$ are independent. Let these be $q_{1}$, $q_{2}, q_{3}$. From them, six invariants can be constructed: the three squares $q_{1}^{2}, q_{2}^{2}, q_{3}^{2}$ and the three products $q_{1} q_{2}, q_{1} q_{3}, q_{2} q_{3}$. But the first three are the given squares of the masses, and the second three satisfy one relation which follows from the equation $\dagger$
$$
\left(q_{1}+q_{2}+q_{3}\right)^{2}=q_{4}^{2}=m_{4}^{2} .
$$
In order to increase the symmetry it is, however, convenient to consider not two but three invariants, which may be taken 

$$
s =\left(q_{1}+q_{2}\right)^{2}=\left(q_{3}+q_{4}\right)^{2}, $$
^sInvariant

$$t  =\left(q_{1}+q_{3}\right)^{2}=\left(q_{2}+q_{4}\right)^{2}$$

^tInvariant
$$
u =\left(q_{1}+q_{4}\right)^{2}=\left(q_{2}+q_{3}\right)^{2} 
$$

^uInvariant

These are easily seen to be related by
$$
s+t+u=h
$$
where
$$
h=m_{1}^{2}+m_{2}^{2}+m_{3}^{2}+m_{4}^{2} .
$$
$+$ In the general case of a reaction involving $n(\geqslant 4)$ particles, the number of functionally independent invariant quantities is $3 n-10$. There are altogether $4 n$ quantities, the components of the $n$ 4-momenta $q_{a}$, between which there are $n$ functional relations $q_{a}^{2}=m_{a}^{2}$ and four given by the conservation law $\Sigma q_{a}=0$. Arbitrary values can be assigned to six quantities, in accordance with the number of parameters which define the general Lorentz transformation (a general

In the [[I)](../s-channel.md|principal channel (I)]], the invariant $s$ has a simple physical significance. It is the square of the total energy of the colliding particles $(1$ and 2$)$ in their [[../center of momentum frame|centre-of-mass system]] (for $\mathbf{p}_{1}+\mathbf{p}_{2}=0, s=\left(\varepsilon_{1}+\varepsilon_{2}\right)^{2}$ ). In channel II, the invariant $t$ has a similar significance, and in channel III the invariant $u$. The three channels are therefore of called $s, t$ and $u$ channels. 

It is easy to express each of the invariants $s, t$ and $u$ in terms of the energies and momenta of the colliding particles in each channel. Let us consider the $s$ channel. In the centre-of-mass system of particles 1 and 2 , the time and space components of the 4-vectors $q_{a}$ are
$$
\begin{array}{ll}
q_{1}=p_{1}=\left(\varepsilon_{1}, \mathbf{p}_{s}\right), & q_{2}=p_{2}=\left(\varepsilon_{2},-p_{s}\right), \\
q_{3}=-p_{3}=\left(-\varepsilon_{3},-\mathbf{p}_{s}^{\prime}\right), & q_{4}=-p_{4}=\left(-\varepsilon_{4}, \mathbf{p}_{s}^{\prime}\right) ;
\end{array}
$$
the suffix $s$ in $\mathbf{p}_{s}$ and $\mathbf{p}_{s}^{\prime}$ indicates that these momenta refer to the reaction in the $s$ channel. Then
$$
\begin{array}{c}
s=\varepsilon_{s}^{2}, \quad \varepsilon_{s}=\varepsilon_{1}+\varepsilon_{2}=\varepsilon_{3}+\varepsilon_{4} \\
4 s \mathbf{p}_{s}^{2}=\left[s-\left(m_{1}+m_{2}\right)^{2}\right]\left[s-\left(m_{1}-m_{2}\right)^{2}\right] \\
4 s \mathbf{p}_{s}^{\prime 2}=\left[s-\left(m_{3}+m_{4}\right)^{2}\right]\left[s-\left(m_{3}-m_{4}\right)^{2}\right] \\
2 t=h-s+4 \mathbf{p}_{s} \cdot \mathbf{p}_{s}^{\prime}-\frac{1}{s}\left(m_{1}^{2}-m_{2}^{2}\right)\left(m_{3}^{2}-m_{4}^{2}\right) \\
2 u=h-s-4 \mathbf{p}_{s} \cdot \mathbf{p}_{s}^{\prime}+\frac{1}{s}\left(m_{1}^{2}-m_{2}^{2}\right)\left(m_{3}^{2}-m_{4}^{2}\right)
\end{array}
$$
For elastic scattering $\left(m_{1}=m_{3}, m_{2}=m_{4}\right)$, we have $\left|\mathbf{p}_{s}\right|=\left|\mathbf{p}_{s}^{\prime}\right|$, and hence $\varepsilon_{1}=\varepsilon_{3}$, $\varepsilon_{2}=\varepsilon_{4}$. Instead of (66.9), the simpler formulae
$$
\left.\begin{array}{l}
t=-\left(\mathbf{p}_{s}-\mathbf{p}_{s}^{\prime}\right)^{2}=-2 \mathbf{p}_{s}^{2}\left(1-\cos \theta_{s}\right) \\
u=-2 \mathbf{p}_{s}^{2}\left(1+\cos \theta_{s}\right)+\left(\varepsilon_{1}-\varepsilon_{2}\right)^{2}
\end{array}\right\}
$$
are then obtained, where $\theta_{s}$ is the angle between $\mathbf{p}_{s}$ and $\mathbf{p}_{s}^{\prime}$. The invariant $-t$ is here the square of the (three-dimensional) momentum transfer in the collision.

Similar formulae for the other channels are found by a straightforward change of notation. For the $t$ channel we must interchange $s$ and $t$, and 2 and 3 , in (66.6)-(66.10); for the $u$ channel, we interchange $s$ and $u$, and 2 and 4 .
§67. Physical regions
When considering the scattering amplitudes as functions of the independent variables $s, t, u$ (which are related only by $s+t+u=h$ ), we encounter the need to distinguish regions in which their values are physically permissible from those in which they are not. Values which can correspond to a physical process of scattering must satisfy certain conditions which follow from the law of conservation of 4-momentum and the fact that the square of each of the 4-vectors $q_{a}$ is a given quantity $m_{a}^{2}$.
The product of two 4 -momenta
$$
p_{a} p_{b} \geqslant m_{a} m_{b}
$$
Hence
$$
\left(q_{a}+q_{b}\right)^{2}=\left(p_{a}+p_{b}\right)^{2} \geqslant\left(m_{a}+m_{b}\right)^{2}
$$
if $q_{a}=p_{a}, q_{b}=p_{b}\left(\right.$ or $\left.q_{a}=-p_{a}, q_{b}=-p_{b}\right)$; or
$$
\left(q_{a}+q_{b}\right)^{2}=\left(p_{a}-p_{b}\right)^{2} \leqslant\left(m_{a}-m_{b}\right)^{2},
$$
if $q_{a}=p_{a}, q_{b}=-p_{b}$. Hence, for a reaction in the $s$ channel,
$$
\left.\begin{array}{c}
\left(m_{1}+m_{2}\right)^{2} \leqslant s \geqslant\left(m_{3}+m_{4}\right)^{2} \\
\left(m_{1}-m_{3}\right) \geqslant t \leqslant\left(m_{2}-m_{4}\right)^{2}, \\
\left(m_{1}-m_{4}\right)^{2} \geqslant u \leqslant\left(m_{2}-m_{3}\right)^{2}
\end{array}\right\}
$$
and similarly in the $t$ and $u$ channels.
To determine the remaining conditions, we form a 4-vector $L$ which is dual to the product of any three of the 4-vectors $q_{a}$, say
$$
L_{\lambda}=e_{\lambda \mu \nu \rho} q_{1}^{\mu} q_{2}^{\nu} q \xi .
$$
In the rest frame of particle 1 , say, we have $q_{1}=\left(q_{1}^{0}, 0\right)$. Then $L$ has only the spatial components $L_{i}=e_{i 0 k 1} q_{1}^{0} q_{2}^{k} q_{3}^{1}$. Thus $L$ is a space-like vector, and $L^{2} \leqslant 0$ in every frame of reference. Expanding $L^{2}$, we obtain the condition
$$
\left|\begin{array}{ccc}
q_{1}^{2} & q_{1} q_{2} & q_{1} q_{3} \\
q_{2} q_{1} & q_{2}^{2} & q_{2} q_{3} \\
q_{3} q_{1} & q_{3} q_{2} & q_{3}^{2}
\end{array}\right| \geqslant 0 .
$$
This can be expressed in terms of the invariants $s, t, u$ in a form which is the same for all channels:
$$
s t u \geqslant a s+b t+c u,
$$
where
$$
\left.\begin{array}{l}
a h=\left(m_{1}^{2} m_{2}^{2}-m_{3}^{2} m_{4}^{2}\right)\left(m_{1}^{2}+m_{2}^{2}-m_{3}^{2}-m_{4}^{2}\right) \\
b h=\left(m_{1}^{2} m_{3}^{2}-m_{2}^{2} m_{4}^{2}\right)\left(m_{1}^{2}+m_{3}^{2}-m_{2}^{2}-m_{4}^{2}\right) \\
c h=\left(m_{1}^{2} m_{4}^{2}-m_{2}^{2} m_{3}^{2}\right)\left(m_{1}^{2}+m_{4}^{2}-m_{2}^{2}-m_{3}^{2}\right)
\end{array}\right\}
$$

For a graphical representation of the regions of variation of $s, t$ and $u$, it is convenient to use triangular coordinates in a plane, called the Mandelstam plane (S. Mandelstam, 1958). The coordinate axes are three straight lines which intersect to form an equilateral triangle. The coordinates $s, t, u$ are measured along directions perpendicular to these three lines; the directions towards the interior of the triangle are reckoned positive, as shown by the arrows in Fig. 5. Thus each point in the plane has corresponding values of $s, t$ and $u$ which are represented (with the appropriate signs) by the lengths of the perpendiculars to the three axes. The condition $s+t+u=h$ is satisfied on account of a known theorem of geometry, $h$ being equal to the altitude of the triangle. $\dagger$

Let us consider the important case where the principal channel ( $s$ ) corresponds to elastic scattering. Then the masses of the particles are equal in pairs:
$$
m_{1}=m_{3} \equiv m, \quad m_{2}=m_{4} \equiv \mu
$$
Let $m>\mu$. The condition (67.5) has
$$
h=2\left(m^{2}+\mu^{2}\right), \quad a=c=0, \quad b=\left(m^{2}-\mu^{2}\right)^{2}
$$
so that
$$
s u t \geqslant\left(m^{2}-\mu^{2}\right)^{2} t
$$
The boundary of the region defined by this inequality comprises the straight line $t=0$ and the hyperbola
$$
s u=\left(m^{2}-\mu^{2}\right)^{2},
$$
whose two branches lie in the sectors $u<0, s<0$ and $s>0, u>0$; the axes $s=0$