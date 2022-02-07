---
alias:
tags:
- qftII
---
The BRST transformation is defined as the following variation of the fields
$$
\begin{aligned}
\delta A_{\mu} &=\delta \epsilon\left[D_{\mu}, C\right]= \delta \varepsilon Q A_{\mu} \Rightarrow & Q A_{\mu} &\left.=C D_{\mu}, C\right] \\
\delta C &=i \delta \epsilon C C=\frac{i}{2} \delta \epsilon\{C, C\}, & Q C &=\frac{i}{2}\{C, C\} \\
\delta \bar{C} &=-\delta \epsilon B, & Q \bar{C} &=-B \\
\delta B &=0 . & Q B &=0
\end{aligned}
$$
Note that the transformation parameter $\delta \epsilon$ must be a [[Grassmann variables|Grassmann odd number]]  in order to match the statistics on both sides of the equation. It is straight-forward to confirm that the Lagrangian is invariant under the BRST transformation
$$
\delta \mathcal{L}_{\mathrm{BRST}}=0
$$
Likewise, the Yang-Mills Lagrangian $\mathcal{L}_{Y M}$ is invariant since the BRST transformation on the ordinary fields is a plain [[infinitesimal YM gauge transformations|gauge transformation]]  with transformation parameter $\delta \epsilon C$. ^f64663

Let us write the BRST transformation as a fermionic operator $Q$ such that
$$
\delta=\delta \epsilon Q
$$
This BRST operator has the important property that it is nilpotent
$$
Q^{2}=0
$$
as can be verified easily by acting with $Q^{2}$ on all fields. In fact we can write the BRST Lagrangian as a BRST variation of some other function $K_{\mathrm{BRST}}$
$$
\mathcal{L}_{\mathrm{BRST}}=Q K_{\mathrm{BRST}}, \quad K_{\mathrm{BRST}}=\frac{2}{g_{\mathrm{YM}}^{2}} \operatorname{Tr}\left(-\bar{C}\left(\partial^{\mu} A_{\mu}\right)-\frac{1}{2} \xi \bar{C} B\right) .
$$

^e15f52

It is then evident that $Q \mathcal{L}_{\mathrm{BRST}}=Q^{2} K_{\mathrm{BRST}}=0$. The Yang-Mills Lagrangian, on the other hand, cannot be written as a BRST variation of something, since the gauge field strength $F_{\mu \nu}$ is never produced by the action of $Q$ ^f33149
$$
\mathcal{L}_{\mathrm{YM}} \neq Q K_{\mathrm{YM}}
$$
Another new symmetry is the [[Faddeev-Popov ghosts|ghost]] number $N_{\mathrm{gh}}$. It counts the number of ghosts $C$ minus the number of anti-ghosts $\bar{C}$. The gauge and auxiliary fields carry no [[Faddeev-Popov ghosts|ghost]] number.