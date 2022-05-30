At next to leading order (NLO) we have from [[KMOC in SQED]] that 

$$L-1=2L'+\abs{X}$$

Where $L$ is the loop count for the virtual kernel and $L'$, $\abs{X}$ are the real kernel loop count and messenger particle count respectively. Plugging in $L=1$ imposes $L'=\abs{X}=0$. Putting things together we have:

$$\Delta p_1^{\mu,(0)}=\AAngle{\int \d {\overline{\Psi}(\bar{q})}\euler^{-\iunit\bar{q}\cdot b}\par[\big]{\ \vKernAA{p_1^{\mu},L=1}+\rKernAA{p_1^{\mu},L=0,\abs{X}=0}}} $$

Let us first look at the virtual kernel. It is given by a 1-loop amplitude. 

$$\vKernAA{p_1^{\mu},L=1}=\iunit\,  \bar{q}^\mu\,  e^{4}{\hbar}^{1}\bar{\mathcal{A}}^{(1)}(p_1,p_2\to p_1+\hbar \bar{q},p_2-\hbar\bar{q})$$

The amplitude is read off from the one loop level diagrams and using [[feynman rules for SQED]]. 

![[NLOVirtualDiags.excalidraw.svg]]



$$\iunit\bar{\mathcal{A}}^{(1)}(p_1,p_2\to p_1+\hbar \bar{q},p_2-\hbar\bar{q})=\iunit \frac{Q_1 Q_2 }{\hbar^2\bar{q}^2}\par[\big]{4 p_1 \cdot p_2+\hbar^2\bar{q}^2}$$