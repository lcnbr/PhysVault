---
alias:
tags:
- qftII
---
# Path Integral in Position Space
For common physical systems we can transform the path integral back to the original [[Lagrangian]] framework, assume a  [[Hamiltonian#Quadratic momentum|quadratic momentum Hamiltonian]], this  allows to integrate all momenta out in the [[Path Integral for Transition Amplitude#^transAmp|transition amplitude]] using the [[Gaussian integral]]:

$$A_{n,0}=\int \prod_{k=1}^{n-1} \dd{q_k}\prod_{k=1}^{n}\sqrt{\frac{M(\bar q_k)}{2\pi \hbar \iunit(t_k-t_{k-1})}}\exp\qty(\frac{\iunit}{\hbar} S_{n,0}[q]),$$
^8ff1e5

Where the [[Path Integral for Transition Amplitude#^discAction|discrete action]] becomes: 
$$\begin{align}
S_{n,0}[q]\MoveEqLeft=\sum_{k=1}^n(t_k-t_{k-1})\bigg[-V(\bar q_k)\\
&+\frac{1}{2} M (\bar q_k)\qty(\frac{q_k-q_{k-1}}{t_k-t_{k-1}}-K\qty(\bar q_k))^2
\bigg].
\end{align}$$
Going to the [[continuum limit]], the [[Path Integral for Transition Amplitude#^transAmp|transition amplitude]] becomes the following [[Path Integral in Phase Space#^a2b223|path integral]]:
$$A_\text{f,i}=\int \mathcal{D}{q}\exp(\frac{\iunit}{\hbar}S_\text{f,i}[q]),$$
where the phase is given by the conventional [[Action]] for a particle (c.f. [[Path Integral in Phase Space#^46a265|this]]):

$$S_\text{f,i}[q]=\int_{t_\text{i}}^{t_\text{f}} \dd{t}\pqty{\frac{1}{2}M(q)(\dot q-K(q))^2 -V(q)}=\int \dd{t} L(q,\dot q)$$
Evidently, this action is classically equivalent to the above action in [[Hamiltonian]] form, however the  quantum equivalence is not to be expected in general for two equivalent classical actions
Note measure factor hidden in $\mathcal{D}{q}$ is substantially more complicated compared to the combination $\mathcal{D}{q}\mathcal{D}{p}$