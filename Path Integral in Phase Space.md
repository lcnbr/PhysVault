# Path Integral in Phase Space
There is one momentum integral more to be done than position integrals, interestingly, the measure factor for a combined position and momentum integral is just $2\pi \hbar$,
$$
\int \frac{\mathrm{d}{q}\mathrm{d}{p}}{2\pi \hbar}.
$$ 
the volume quantum mechanics associates to an elementary cell in phase space.
The exact transition amplitude is obtained by formally taking the limit of infinitely many time slices at infinitesimal intervals

$$A_\text{f,i}= \int \mathcal{D}{q}\mathcal{D}{p}\exp\left(\frac{\iunit}{\hbar}S_\text{f,i}[q,p]\right),$$
where  the phase is now given as a functional of the path ^a2b223
$$S_\text{f,i}[q,p]=\int_{t_\text{i}}^{t_\text{f}} \dd {t}\qty(p(t)\dot q(t)-H(q(t),p(t)))

=\int_\text{i}^\text{f} \left(p\dd{q}-H\dd{t}\right).$$

^46a265

This form is exciting, it is precisely the action in phase space, whose associated [[Euler-Lagrange equations]], are just the [[Hamiltonian#Hamilton's equations|Hamitonian equations of motion]] 

When quantum corrections are taking into account, the allowable paths can wiggle around the classical trajectory slightly, on the order of $\hbar$.

The [[#^a2b223|path integral for the transition amplitude]] $A_\text{f,i}$, keeps the initial and final positions fixed, whereas the momenta $p(t_i)$ and $p(t_f)$ are free. The path integral can also compute other quantities where the boundary conditions are specified differently. We must point out that the path integral may not be well defined in a mathematical sense, especially because the integrand is highly oscillating. Nevertheless, it is reasonably safe to use the path integral in physics by formally manipulating it by the usual rules and inserting suitable regulators such as $\pm \iunit \epsilon$