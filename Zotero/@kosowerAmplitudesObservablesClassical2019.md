
---
title: Amplitudes, observables, and classical scattering
authors: David A. Kosower, Ben Maybee, Donal O'Connell
year: 2019
contained in: Journal of High Energy Physics

DOI: 10.1007/JHEP02(2019)137
url: 

---
# [Amplitudes, observables, and classical scattering](zotero://select/items/@kosowerAmplitudesObservablesClassical2019)

**Contents**

# [Introduction](zotero://open-pdf/0_XIBRM7N7/3)

we must understand  systematically how to extract the classical result using on-shell quantum-mechanical scattering amplitudes.  Our formalism applies to both electrodynamics and gravity. And for simplicity we restrict to spinless scattering.
    
# [Restoring $\hbar$](zotero://open-pdf/0_XIBRM7N7/5)

#convention Use [[relativistically natural units]] i.e. $c=1 \implies [L][T]^{-1}=1 \implies [L]=[T]$ 


A straightforward and pragmatic approach to restoring all factors of $\hbar$ in an expression is  dimensional analysis.

#definition : Denote dimensions of mass and length by $[M]$ and $[L]$, respectively ^[![[@kosowerAmplitudesObservablesClassical2019annotations#^dimension]]]
#definition : Denote spatial three vectors in bold i.e. $p^i=\boldsymbol{p}$

Using 
$$
\bqty\big{\hat{a}_{p}, \hat{a}_{p^{\prime}}^{\dagger}}=(2 \pi)^{3} \delta^{(3)}\pqty{\boldsymbol{p}-\boldsymbol{p}^{\prime}},
$$
to define the dimensions of $\hat{a}_p$, using that $\delta^{(n)}([x])=[x]$^[[[delta function#In dimensional analysis]]] we have:

$$\bqty{\bqty\big{\hat{a}_{p}, \hat{a}_{p^{\prime}}^{\dagger}}}=\bqty{\hat{a}_{p}}^2=\bqty{ \delta^{(3)}\pqty{\boldsymbol{p}-\boldsymbol{p}^{\prime}}}=\bqty{\boldsymbol{p}}^{-3}=[M]^{-3}$$
Thus $[\hat{a}_p]=[M]^{-\frac{3}{2}}$

#definition Single particle state: $\ket{p}=\sqrt{2E_p} \hat{a}^\dagger_p \ket{0}$ with dimension ^[in [[relativistically natural units]]] $[M]^{\frac{1}{2}}[M]^{-\frac{3}{2}}=[M]^{-1}$ ^[![[@kosowerAmplitudesObservablesClassical2019annotations#^singlePart]]]

#definition $\hat{\delta}^{(n)}(p) \equiv(2 \pi)^{n} \delta^{(n)}(p)$ ^[![[@kosowerAmplitudesObservablesClassical2019annotations#^delta]]]

#definition We define the amplitudes in four dimensions as usual by$\mel{p'_1 \cdots p'_m}{T}{p_1 \cdots p_n}=\mathcal{A}(p_1 \cdots p_n\rightarrow p'_1 \cdots p'_m)\hat{\delta}(p_1 +\cdots+ p_n- p'_1- \cdots-p'_m)$with an in out momentum convention. ^[![[@kosowerAmplitudesObservablesClassical2019annotations#^amplitude]]]

#definition  wavenumber $\bar{p}$ associated with a  momentum $p$: $\bar{p}\equiv \frac{p}{\hbar}$ ^[![[@kosowerAmplitudesObservablesClassical2019annotations#^wavenumber]]]

We consider the scattering  of two point-like objects, with momenta $p_{1,2}$, initially separated by a transverse impact  parameter $b_\mu$^[![[@kosowerAmplitudesObservablesClassical2019annotations#^transverseImpact]]]

#definition (reduced) Compton wavelengths $\ell_c^{(i)}\equiv  \frac{\hbar}{m_i}$  


The point-particle description will be  accurate provided that
$$\sqrt{-b^2}\gg \ell^{(1,2)}_c$$

There is another important length scale:
#definition: the spread of the wavepackets, $\ell_w$

The quantum-mechanical expectation values of observables, as we  will discuss, are well-approximated by the corresponding classical ones, when the packet spreads are in the ‘Goldilocks’ zone:

$$\ell_c\ll\ell_w\ll\sqrt{-b^2}$$


### Restoring $\hbar$
When $\hbar \neq 1$, the dimensions of the momenta and masses in the amplitude are unchanged.

> I would think that the momenta go from [M] to [M][L][T]^-1, but that is only for c also not equal to 1!!

But the dimensionless couplings in scalar QED and gravity have a factor of $\frac{1}{\sqrt{\hbar}}$ thus the restoring algorithm is: each factor of a coupling is multiplied by   an additional factor of $\frac{1}{\sqrt{\hbar}}$. And importantly as we take $\hbar$ to $0$ we consider that point particles have momenta which are fixed whereas massless particles and momentum transfers between massive particles it is the wavenumber which we should  treat as fixed in the limit.



# [Impulse and radiated momentum in quantum field theory](zotero://open-pdf/0_XIBRM7N7/7)

We examine scattering events in which two widely separated particles are prepared at $t \rightarrow - \infty$, and then shot at each other with impact parameter $b_\mu$. We will also restrict  our attention to scattering processes in which quanta of fields 1 and 2 are both present in  the final state.


    
## [The incoming state](zotero://open-pdf/0_XIBRM7N7/7)

$$\ket{\psi}_{\text{in}}=\int \dd{\Phi_2(p_1,p_2)} \phi_1(p_1) \phi_2(p_2) e^{\iunit b_\mu p^\mu_1 /\hbar}\ket{p_1,p_2}_\text{in}$$

Where we use the multiple [[Lorentz invariant measure]]. Note the explicit phase extracted from the two wavepackets functions such that the wavepacket of particle 1 is translated by the impact parameter $b$ relative to particle 2.


        
## [The impulse on a particle](zotero://open-pdf/0_XIBRM7N7/9)

#definition : the *impulse* on a particle during  a scattering event: at the classical level, this is simply the total change in the momentum  of one of the particles — say particle 1 — during the collision.

We place detectors at asymptotically large distances pointing  at the collision region.

#definition : $\mathbb{P}_i^\mu$ be the momentum operator for particle $i$ 

We then have the expectation value of particle 1's outgoing momentum is:

$$
\begin{align}
\ev{p^\mu_{\text{out},1}}&=\prescript{}{\text{out}}{\ev{\mathbb{P}_1^\mu}{\psi}}_\text{out}\\
&=\prescript{}{\text{out}}{\ev{\mathbb{P}_1^\mu\, U(\infty,-\infty)}{\psi}}_\text{in}\\
&=\prescript{}{\text{in}}{\ev{U(\infty,-\infty)^\dagger\,\mathbb{P}_1^\mu \,U(\infty,-\infty)}{\psi}}_\text{in}\\
\end{align}$$

#definition : $U(\infty,-\infty)$ is the time evolution operator from the far past to the far future also called the S matrix


        
## [Impulse in terms of amplitudes](zotero://open-pdf/0_XIBRM7N7/10)
        
## [The momentum radiated during a collision](zotero://open-pdf/0_XIBRM7N7/13)
        
## [Conservation of momentum](zotero://open-pdf/0_XIBRM7N7/15)
        
# [Classical point particles](zotero://open-pdf/0_XIBRM7N7/17)
    
## [Wavefunctions](zotero://open-pdf/0_XIBRM7N7/17)
        
## [An example wavefunction](zotero://open-pdf/0_XIBRM7N7/22)
        
## [Classical impulse](zotero://open-pdf/0_XIBRM7N7/24)
        
## [Classical radiation](zotero://open-pdf/0_XIBRM7N7/26)
        
## [Conservation of momentum](zotero://open-pdf/0_XIBRM7N7/28)
        
# [Examples](zotero://open-pdf/0_XIBRM7N7/29)
    
## [Leading-order electromagnetic impulse](zotero://open-pdf/0_XIBRM7N7/29)
        
## [Next-to-leading order impulse](zotero://open-pdf/0_XIBRM7N7/31)
        
### [Purely quantum contributions](zotero://open-pdf/0_XIBRM7N7/32)
            
### [Triangles](zotero://open-pdf/0_XIBRM7N7/33)
            
### [Boxes](zotero://open-pdf/0_XIBRM7N7/34)
          
### [Cut box](zotero://open-pdf/0_XIBRM7N7/36)
            
### [Combining contributions](zotero://open-pdf/0_XIBRM7N7/37)
            
### [On-shell cross check](zotero://open-pdf/0_XIBRM7N7/39)
            
### [Radiation](zotero://open-pdf/0_XIBRM7N7/40)
        
## [Momentum conservation and radiation reaction](zotero://open-pdf/0_XIBRM7N7/42)
        
# [Classical calculations](zotero://open-pdf/0_XIBRM7N7/44)
    
## [The classical electromagnetic impulse](zotero://open-pdf/0_XIBRM7N7/44)
        
### [Leading order](zotero://open-pdf/0_XIBRM7N7/45)
            
 
### [Classical radiated momentum](zotero://open-pdf/0_XIBRM7N7/48)
        
### [General expressions](zotero://open-pdf/0_XIBRM7N7/48)
            
### [Application at leading order](zotero://open-pdf/0_XIBRM7N7/50)
            
## [Momentum conservation and the radiation reaction force](zotero://open-pdf/0_XIBRM7N7/51)
        
# [Discussion and conclusions](zotero://open-pdf/0_XIBRM7N7/53)
    
# [Conventions](zotero://open-pdf/0_XIBRM7N7/55)
    
# [Linear wavefunction integrals](zotero://open-pdf/0_XIBRM7N7/55)
    
# [Angular integrals](zotero://open-pdf/0_XIBRM7N7/58)
    
# [An alternative classical point of view on momentum radiation](zotero://open-pdf/0_XIBRM7N7/59)