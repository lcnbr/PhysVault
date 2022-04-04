---
title: Scalar QED as a toy model for higher-order effects in classical gravitational scattering
authors: Zvi Bern, Juan Pablo Gatica, Enrico Herrmann, Andres Luna, Mao Zeng
year: 2021
---
[Item](zotero://select/items/@bernScalarQEDToy2021)

## Highlights:
[[@bernScalarQEDToy2021annotations]]

# Mentions:
- [[effective one body formalism]]^[![[@bernScalarQEDToy2021annotations#^7e27bb]]]
- [[numerical relativity]]^[![[@bernScalarQEDToy2021annotations#^ae2631]]]
- [[self-force formalism]]
- [[effective field theory]]
- [[nonrelativistic general relativity]]
- [[post-Minkowskian expansion]]^[![[@bernScalarQEDToy2021annotations#^09545f]]]
- [[Newton]]

# Summary

**Contents**

##  [1 Introduction](zotero://open-pdf/0_VLMHF4E2/2)

The landmark detection of gravitational waves \[1, 2\] has opened a remarkable new window into the Universe that promises major new advances into black holes, neutron stars, and perhaps even provides new insights into fundamental physics. ^[![[@bernScalarQEDToy2021annotations#^56f6bf]]]. The aim of the game is to predict gravitational wave signals. The tools used are varied but the most prominent is the [[post-Minkowskian expansion]]. On top of being useful in the [[post-Minkowskian expansion|PM expansion]] amplitudes enable the description of the hyperbolic motion of classical objects from the asymptotic past to the asymptotic future ^[![[@bernScalarQEDToy2021annotations#^aa210e]]] as implemented in the [[KMOC framework]]. The usefulness of the scattering amplitude framework has been demonstrated through the first construction of the conservative two-body Hamiltonian at $\mathcal{O}(G^3)$, as well as new results at $\mathcal{O}(G^4)$^[![[@bernScalarQEDToy2021annotations#^087cd9]]] .

### PLAN:
1. Use Kosower-Maybee-O’Connell formalism to obtain the impulse on two massive charged scalar particles scattering at large impact parameter b from which we extract the scattering angle^[![[@bernScalarQEDToy2021annotations#^b0394b]]]
2. extract the eikonal phase from the scattering amplitude which allows us to determine the scattering angle^[![[@bernScalarQEDToy2021annotations#^6c0ca1]]]
3. extracting from the scattering amplitude a radial action that determines the scattering angle, including radiative effects. ^[![[@bernScalarQEDToy2021annotations#^376f6d]]]

All three of these approaches for extracting the classical scattering angle match, and agree with the result from the classical approach of Ref. \[90\].^[![[@bernScalarQEDToy2021annotations#^038ace]]]


In electromagnetism we encounter a mass singularity in the scattering angle, which does not cancel between potential and radiative contributions, as it does in the corresponding O(G3) calculation in gravity [127, 128]^[![[@bernScalarQEDToy2021annotations#^260d9e]]] we interpret this singularity as a breakdown of the classical expansion which requires $m^2 \abs{b}^2\gg 1$ 


##  [2 Review of Methods](zotero://open-pdf/0_VLMHF4E2/5)

#defintion Two loop order: $\mathcal{O}(\alpha^3)$ where $\alpha = \frac{e^2 }{4 \pi}$ is the [[fine structure constant]]

# PLAN:

- review the kinematic parametrization tailored towards the classical expansion of quantum scattering amplitudes in Subsection 2.1 ^[![[@bernScalarQEDToy2021annotations#^f4a4b5]]]
- Outline the generalized unitarity framework to determine the amplitude integrands in Subsection 2.2 ^[![[@bernScalarQEDToy2021annotations#^d615bb]]]
- Subsection 2.3, we telegraphically sketch the applicability of modern collider-physics based integration tools to compute precision-level classical observables with the help of integration-by-parts reduction to a minimal set of master integrals and their evaluation by differential equation methods ^[![[@bernScalarQEDToy2021annotations#^52f488]]]
- Subsection 2.4 introduces a new concept that allows us to define a radial action in the presence of soft-region radiation effects ^[![[@bernScalarQEDToy2021annotations#^3dabc1]]]
- Subsection 2.5, we briefly summarize the ([[KMOC framework|KMOC]]) formalism which allows us to extract the classical electromagnetic impulse, the radiated momentum, and the classical scattering angle up to $\mathcal{O}(\alpha^3)$.

###  [2.1 Classical limit of quantum scattering amplitudes–soft and potential region](zotero://open-pdf/0_VLMHF4E2/5)

Relativistic scattering of two point-charges in a [[post-Lorentzian expansion|PL expansion]]^[![[@bernScalarQEDToy2021annotations#^06ee81]]]. Suppose that the particles are spinless and structureless (massive [[scalar fields in GR|scalar field]]). 
We convert scales to momentum space by: assuming that the masses are very large and the momentum transfer $\abs{q} \sim \frac{1}{\abs{b}}$ is small: $(-q^2)\ll m_i^2$

We redefine the incoming and outgoing momenta to facilitate the [[soft expansion]] (small $\abs{q}$)

$p_1 = - \pqty{\bar{p}_1-\frac{q}{2}},p_2 = - \pqty{\bar{p}_2+\frac{q}{2}},p_3 =  \pqty{\bar{p}_2-\frac{q}{2}},p_4 =  \pqty{\bar{p}_1+\frac{q}{2}}$

The barred variables are such that, for [[on-shell]] momenta ($p_i^2=m_{I_i}^2$) for $I_i=\left\{\begin{aligned}&1 \text{ for } i\in\Bqty{1,4}\\&2 \text{ for } i \in\Bqty{2,3}\end{aligned}\right.$ , $\overline{p}_I \cdot q=0$, i.e. are orthogonal to the momentum transfer $q$. 
![[Pasted image 20220330221749.png]]

Also introduce soft-masses $\overline{m}_I$:
$$
m_{I_i}^2=p_i^2=\overline{p}_{I_i} ^2 \pm \underbracket{\overline{p}_{I_i}\cdot q}_{0} + q^2=\overline{p}_{I_i}^2+\frac{q^2}{4}$$ 


$$ \overline{m}_I^2\overset{\text{def}}{=}\overline{p}_I^2=m_I^2-\frac{q^2}{4} \implies \overline{m}_I=m_I + {\frac{(-q^{2})}{8 \, m_{I}}}  + \mathcal{O}\left(q^{4}\right)$$
^massExp
  
And normalised momenta called *soft velocities* of the two black holes: $u_i^{\mu}=\overline{p}_i^\mu/\abs{\overline{p}_i}$. Such that the dimensionless parameter $y$, or its rationalized version $x$ can be written:

$$
y =\frac{1+x^{2}}{2 x}\equiv u_{1} \cdot u_{2}={\left.\sigma-(-q^{2}\right)} \frac{\left(m_{1}^{2}+m_{2}^{2}\right) \sigma+2 m_{1} m_{2}}{8 m_{1}^{2} m_{2}^{2}}+\mathcal{O}\left(q^{4}\right)
$$
^yEq

Where $\sigma=\cosh\eta=\frac{s-m_{1}^{2}-m_{2}^{2}}{2m_{1}m_{2}}=\frac{p_{1}\cdot p_{2}}{m_{1}m_{2}}\,$ is simply the relativistic factor of particle 1 in the rest-frame of particle 2.  The last equality is obtained by expanding out $p_1 \cdot p_2$ in terms of the barred momenta:

$$p_1 \cdot p_2= -\frac{1}{4} \, q^{2} + \frac{1}{2} \,\cancelto{0}{q \cdot{\overline{p}_1}} - \frac{1}{2} \, \cancelto{0}{q \cdot{\overline{p}_2}} + {\overline{p}_1} \cdot{\overline{p}_2}$$

$$u_1 \cdot u_2=\frac{{\overline{p}_1} {\overline{p}_2}}{{\overline{m}_1} {\overline{m}_2}} = \frac{4 \, p_{1} p_{2} + q^{2}}{4 \, {\overline{m}_1} {\overline{m}_2}}$$
Then expanding $\overline{m}_I$ out in terms of $q$ ([[#^massExp]]) yields: [[#^yEq]]. 

Importantly the barred variables don't change the regions:  the physical scattering region $s>(m_1 + m_2)^2$, $q^2<0$ remains the same ^[![[@bernScalarQEDToy2021annotations#^35020d]]], for $s=(\overline{p}_1+\overline{p}_2)^2=(p_1+p_2)^2$ the [[Mandelstam invariants|s-channel]].  The *soft velocities* $u_i$ coincide with the classical four velocities of the massive scalars only up to corrections of $\mathcal{O}(q)$^[![[@bernScalarQEDToy2021annotations#^1f325c]]]

In the classical limit we want to compute in the [[method of regions|region]] associated to the following scale hierarchy: $\abs{l}\sim\abs{q}\ll\abs{\overline{p}_i},m,\sqrt{s}$ where $l$ schematically represents arbitrary combinations of photon momenta of the form ^[![[@bernScalarQEDToy2021annotations#^d2fd0c]]] $l_1,l_2,l_1\pm l_2,\dots$

The massless propagators do not need expansion in q: $\frac{1}{l^2}$,$\frac{1}{(l-q)^2}$, as they already exhibit homogenous $\abs{q}$ scaling.

But the matter propagators have non-trivial $\abs{q}$ expansion:

$$
\frac{1}{\left(\ell-p_{i}\right)^{2}-m_{i}^{2}}=\frac{1}{\ell^{2}-2 \ell \cdot p_{i}}=\frac{1}{2 u_{i} \cdot \ell} \frac{1}{m_{i}}-\frac{\ell^{2} \mp \ell \cdot q}{\left(2 u_{i} \cdot \ell\right)^{2}} \frac{1}{m_{i}^{2}}+\cdots
$$


###   [2.2 Generalized Unitarity and scalar QED scattering amplitudes up to $\mathcal{O}(\alpha^3)$](zotero://open-pdf/0_VLMHF4E2/7)
        
###   [2.3 Soft and potential region expansion, IBP, and differential equations](zotero://open-pdf/0_VLMHF4E2/11)
        
###   [2.4 Soft radial action and master integral subtraction of classically divergent terms](zotero://open-pdf/0_VLMHF4E2/12)
        
###  [2.5 KMOC framework for classical conservative and radiative observables](zotero://open-pdf/0_VLMHF4E2/15)

Follows mainly [[@herrmannRadiativeClassicalGravitational2021]] and [[@kosowerAmplitudesObservablesClassical2019]]




        
## [3 Conservative dynamics at $\mathcal{O}(\alpha^3)$](zotero://open-pdf/0_VLMHF4E2/20)
    
### [3.1 Conservative scattering amplitudes](zotero://open-pdf/0_VLMHF4E2/20)
        
### [3.2 Eikonal approach to classical conservative scattering](zotero://open-pdf/0_VLMHF4E2/21)
        
### [3.3 Conservative eikonal phase, scattering angle, and two-body Hamiltonian](zotero://open-pdf/0_VLMHF4E2/22)
        
###  [3.4 Conservative impulse and scattering angle via KMOC](zotero://open-pdf/0_VLMHF4E2/25)
        
## [4 Radiative dynamics at $\mathcal{O}(\alpha^3)$](zotero://open-pdf/0_VLMHF4E2/26)
    
### [4.1 Radiative scattering amplitudes](zotero://open-pdf/0_VLMHF4E2/26)
        
### [4.2 Eikonal approach to classical scattering including radiation effects](zotero://open-pdf/0_VLMHF4E2/27)
        
### [4.3 Radiative impulse, energy loss, and scattering angle via KMOC](zotero://open-pdf/0_VLMHF4E2/33)
        
### [4.4 Radiative radial action](zotero://open-pdf/0_VLMHF4E2/34)
        
##  [5 Conclusions](zotero://open-pdf/0_VLMHF4E2/35)
    



 

