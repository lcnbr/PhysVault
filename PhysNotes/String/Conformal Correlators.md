# Conformal Correlators

In a quantum theory, one is usually interested in the spectrum of [[operators]], which in our situation is just the [[string spectrum]]. Furthermore, one would like to calculate probabilities, which in turn can be derived from expectation values of operators acting on states. 

In a [[quantum field theory]], there are two formulations available for calculating the [[vacuum expectation values]]. 
- Starting from [[../QFTII/momentum eigenstate]], the [[S-matrix]] describing the scattering of particles is defined via
$$
\left\langle\vec{q}_{1}, \vec{q}_{2}, \ldots|S| \vec{p}_{1}, \vec{p}_{2}, \ldots\right\rangle=\left\langle 0\left|a\left(\vec{q}_{1}\right) a\left(\vec{q}_{2}\right) \ldots S \ldots a^{\dagger}\left(\vec{p}_{2}\right) a^{\dagger}\left(\vec{p}_{1}\right)\right| 0\right\rangle
$$
- In terms of [[position eigenstates]], one calculates [[time-ordered]] [[correlation functions]]
$$
\left\langle\Phi\left(x_{1}\right) \Phi\left(x_{2}\right) \ldots\right\rangle=\left\langle 0\left|\mathrm{~T}\left[\Phi\left(x_{1}\right) \Phi\left(x_{2}\right) \ldots\right]\right| 0\right\rangle
$$ ^9cdb6f

# Correlator of String Coordinates. 
As an example of the [[#^9cdb6f|latter]] quantity, one can compute a [[worldsheet correlator]] using the underlying oscillator relations

$$
\begin{aligned}
\left\langle 0\left|X^{\nu}\left(\xi_{2}\right) X^{\mu}\left(\xi_{1}\right)\right| 0\right\rangle=&-\frac{\kappa^{2}}{2} \eta^{\mu \nu} \log \left(\exp \left(i \xi_{2}^{\mathrm{L}}\right)-\exp \left(i \xi_{1}^{\mathrm{L}}\right)\right) \\
&-\frac{\kappa^{2}}{2} \eta^{\mu \nu} \log \left(\exp \left(i \xi_{2}^{\mathrm{R}}\right)-\exp \left(i \xi_{1}^{\mathrm{R}}\right)\right) \\
&+\ldots
\end{aligned}
$$

Is it possible, to produce the same answer from the [[worldsheet]] [[7 CFT/conformal field theory|CFT]]? In order to answer this question, let us first consider which properties the corresponding [[CFT 2-correlator]] should have: ![[CFT 2-correlator#^191134]]

# Wick Rotation. 
![[Wick rotation#In conformal field theory CFT]]