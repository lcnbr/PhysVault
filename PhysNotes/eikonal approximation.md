---
---

6.5 EIKONAL APPROXIMATION
This approximation covers a situation in which $V(\mathbf{x})$ varies very little over a distance of order of wavelength $\bar{\lambda}$ (which can be regarded as "small"). Note that $V$ itself need not be weak as long as $E \gg|V|$; hence the domain of validity here is different from the Born approximation. Under these conditions, the semiclassical^[[../Zotero/@sakuraiModernQuantumMechanics2011|![@sakuraiModernQuantumMechanics2011]]]

As is standard in the discussion of the eikonal approximation, we introduce an auxiliary $(D-2)$-dimensional vector $q$ such that $\mathbf{q}^{2}=-t$ and then take the Fourier transform to rewrite the result in terms of the conjugate variable $b$ (the impact parameter). We can now define the corresponding amplitudes in impact parameter space which are defined via,
$$
\tilde{\mathcal{A}}_{n}\left(s, m_{i}, \mathbf{b}\right)=\frac{1}{4 E p} \int \frac{\mathrm{d}^{D-2} \mathbf{q}}{(2 \pi)^{D-2}} e^{i \mathbf{q b}} \mathcal{A}_{n}\left(s, m_{i}, q\right)
$$
where $E=E_{1}+E_{2}$ is the total energy, $p=|\mathbf{p}|$ is the absolute value of the space-like momentum in the center of mass frame of the two scattering particles and we have written $q=|\mathbf{q}|$. The normalisation is a non-relativistic normalisation factor that we have introduced to make the definition of the eikonal phase below more straightforward. We recall that the $E p$ factor can be written in terms of the Mandelstam variables or incoming momenta as per (2.6).

We can generally write the gravitational S-matrix in impact parameter space as 139,140 ,
$$
S\left(s, m_{i}, \mathbf{b}\right)=1+i \sum_{n=1}^{\infty} \tilde{\mathcal{A}}_{n}\left(s, m_{i}, \mathbf{b}\right)
$$
where $\tilde{\mathcal{A}}_{n}\left(s, m_{i}, \mathbf{b}\right)$ is the full amplitude with $n$ graviton exchanges in impact parameter space including the appropriate normalisation as defined in (2.74).^[[../Zotero/@colladoEikonalApproximationGravitational2020|![@colladoEikonalApproximationGravitational2020]]]