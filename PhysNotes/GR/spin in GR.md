---
alias: spin
tag: GR physics
---

In [[special relativity]] the spin of a free particle for an inertial observer is preserved (c.f. [[spin and angular momentum in SR|spin]])

$$
\frac{\mathrm{d} S_{\mu}}{\mathrm{d} \tau}=0 .
$$

^SRspin

In the rest-frame of the particle the spin four-vector takes the form $S_{\mu}=(0, \vec{S})$. Thus $S_{0}=0$. The above equation can be boosted to any inertial frame as
$$
S_{\mu} V^{\mu}=0 \text {, }
$$
which in the rest frame $(\mathrm{d} \tau=\mathrm{d} t)$ gives
$$
S_{0} \frac{\mathrm{d} t}{\mathrm{~d} \tau}+S_{i} \cancelto{0}{\frac{\mathrm{d} x ^{j} }{\mathrm{~d} \tau}}=0 \quad \Rightarrow \quad S_{0}=0
$$
In the absence of gravity we can explicitly write for the magnitude of spin
$$
\begin{aligned}
\frac{\mathrm{d} S_{\mu}}{\mathrm{d} \tau} =0 \implies& S^{\mu} \frac{\mathrm{d} S_{\mu}}{\mathrm{d} \tau}=0 \\
\implies& \frac{\mathrm{d}}{\mathrm{d} \tau}\left(S_{\mu} S^{\mu}\right) =0 .
\end{aligned}
$$
In the presence of gravity, we can generalize [[#^SRspin]] as
$$
\begin{gather}
\frac{\mathrm{D} S_{\mu}}{\mathrm{D} \tau} =0 \\
\iff \frac{\mathrm{d} S_{\mu}}{\mathrm{d} \tau}-\Gamma^\rho{}_{\mu \nu} S_{\rho} V^{\nu} =0 \\
\iff \frac{\mathrm{d} S_{\mu}}{\mathrm{d} \tau}=\underbracket{\Gamma^\rho{}_{\mu \nu}}_{\text {effects of gravity }} S_{\rho} V^{\nu} \neq0 .
\end{gather}
$$

^eaf4ec

For the magnitude of the spin we have
$$
\frac{\mathrm{D}}{\mathrm{D} \tau}\left(S_{\alpha} S^{\alpha}\right)=0
$$
As $S_{\alpha} S^{\alpha}$ is a scalar, the [[covariant derivative]] turns into a normal derivative. So, the above simplifies to $\frac{\mathrm{d}}{\mathrm{d} \tau}\left(S_{\alpha} S^{\alpha}\right)=0$. **Thus, we conclude that gravity changes the spin-direction of a falling particle but not its magnitude (precession of spin)**.