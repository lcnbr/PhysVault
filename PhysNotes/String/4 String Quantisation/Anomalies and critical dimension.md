# [[../../QFTII/anomaly|Anomalies]] and critical dimension
In [[light cone quantisation]] we have broken manifest $\mathrm{SO}(D-1,1)$ Lorentz symmetry to a $\mathrm{SO}(D-2)$ subgroup.
- Consequently the spectrum of quantum strings organises manifestly into $\mathrm{SO}(D-2)$ multiplets.
- Almost all multiplets fit into $\mathrm{SO}(D-1)$ multiplets.
- Mass assignments fill Poincaré multiplets for $a^{\mathrm{L}}=a^{\mathrm{R}}=1 .$
- [[../Poincare invariance|Poincaré symmetry]] broken unless $a^{\mathrm{L}}=a^{\mathrm{R}}=1$.

[[../../QFTII/anomaly]]: Failure of classical symmetry in quantum theory.
Sometimes [[../../QFTII/anomaly|anomalies]] are permissible, but not here because we want strings to propagate on a Minkowski background with intact [[../Poincare invariance|Poincaré symmetry]].
So far we have only done counting, a more severe problem exists in the algebra. The commutator $\left[M^{-a}, M^{-b}\right]$ is supposed to vanish, but it receives contributions from $\left[\alpha^{-}, \alpha^{a}\right]$ which is non-zero in light cone gauge due to the solution of $\alpha^{-}$in terms of an integral. One finds
$$
\left[M^{-a}, M^{-b}\right]=\sum_{n=1}^{\infty}\left[\left(\frac{D-2}{24}-1\right)\left(n-\frac{1}{n}\right)+\frac{a-1}{n}\right] \times \ldots
$$
This expression vanishes if and only if $D=26$ and $a=1$. String theory predicts twenty-six [[../../QFTII/spacetime]] dimensions.

There is a shortcut derivation: reconsider the nature of the intercept $a$ as a sum of HO ground state energies $\frac{1}{2} \omega_{n}=\frac{1}{2} n$
$$
a=-\sum_{n=1}^{\infty}(D-2) \frac{1}{2} \omega_{n}=-\frac{1}{2}(D-2) \sum_{n=1}^{\infty} n .
$$
This sum is divergent, but black magic helps: $\zeta$-function regularisation
$$
\zeta(z):=\sum_{k=1}^{\infty} \frac{1}{k^{z}}, \quad \text { i.e. } \quad a=-\frac{1}{2}(D-2) \zeta(-1)=\frac{D-2}{24}
$$
Analytical continuation $\zeta(-1)=-\frac{1}{12}$ and use of $a=1$ predicts $D=26 !$ Here a somewhat questionable derivation yields the correct prediction.
