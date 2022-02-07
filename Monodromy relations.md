# Monodromy Relations.

![[Pasted image 20220123175355.png]]
$\quad$ Monodromy relations arise from deforming the contour of integration and thus relating open-string amplitudes with different ordering of legs (or different successions of inserting the corresponding vertex operators on the boundary of the disk. The simplest example is again the four-point amplitude. Here we will not specify the particle content, but rather focus on the kinematical dependence of the amplitude. Fixing the Möbius symmetry on the [[worldsheet]] by choosing $z_{1}=0, z_{3}=1$ and $z_{4}=\infty$, one can write the three configurations of amplitudes which are not related by cyclicity and reflection as

$$
\begin{aligned}
&A_{4}^{\text {open }}(2,1,3,4) \sim \int_{-\infty}^{0} \mathrm{~d} z_{2}\left(-z_{2}\right)^{\alpha^{\prime} q_{1} \cdot q_{2}}\left(1-z_{2}\right)^{\alpha^{\prime} q_{2} \cdot q_{3}}, \\
&A_{4}^{\text {open }}(1,2,3,4) \sim \int_{0}^{1} \mathrm{~d} z_{2}\left(z_{2}\right)^{\alpha^{\prime} q_{1} \cdot q_{2}}\left(1-z_{2}\right)^{\alpha^{\prime} q_{2} \cdot q_{3}}, \\
&A_{4}^{\text {open }}(1,3,2,4) \sim \int_{1}^{\infty} \mathrm{d} z_{2}\left(z_{2}\right)^{\alpha^{\prime} q_{1} \cdot q_{2}}\left(z_{2}-1\right)^{\alpha^{\prime} q_{2} \cdot q_{3}} .
\end{aligned}
$$

Analytically continuing the variable $z_{2}$ to the complex plane one can consider integrating the integrand of the first amplitude, $A_{4}^{\text {open }}(2,1,3,4)$ over a contour closed at infinity. Assuming the poles at $z_{2}=0$ and $z_{2}=1$ to be outside the integration regime, one finds immediately

$$
\begin{aligned}
0=& \int_{-\infty}^{0} \mathrm{~d} z_{2}\left(-z_{2}\right)^{\alpha^{\prime} q_{1} \cdot q_{2}}\left(1-z_{2}\right)^{\alpha^{\prime} q_{2} \cdot q_{3}} \\
&+\int_{0}^{1} \mathrm{~d} z_{2}\left(-z_{2}\right)^{\alpha^{\prime} q_{1} \cdot q_{2}}\left(1-z_{2}\right)^{\alpha^{\prime} q_{2} \cdot q_{3}} \\
&+\int_{1}^{\infty} \mathrm{d} z_{2}\left(-z_{2}\right)^{\alpha^{\prime} q_{1} \cdot q_{2}}\left(1-z_{2}\right)^{\alpha^{\prime} q_{2} \cdot q_{3}},
\end{aligned}
$$

which can be easily rewritten as

$$
\begin{aligned}
& A_{4}^{\text {open }}(2,1,3,4) \\
=&-\int_{0}^{1} \mathrm{~d} z_{2}\left(-z_{2}\right)^{\alpha^{\prime} q_{1} \cdot q_{2}}\left(1-z_{2}\right)^{\alpha^{\prime} q_{2} \cdot q_{3}}
\end{aligned}
$$



$$
\begin{aligned}
&-\int_{1}^{\infty} \mathrm{d} z_{2}\left(-z_{2}\right)^{\alpha^{\prime} q_{1} \cdot q_{2}}\left(1-z_{2}\right)^{\alpha^{\prime} q_{2} \cdot q_{3}} \\
=&-\mathrm{e}^{i \pi \alpha^{\prime} q_{1} \cdot q_{2}} \int_{0}^{1} \mathrm{~d} z_{2}\left(z_{2}\right)^{\alpha^{\prime} q_{1} \cdot q_{2}}\left(1-z_{2}\right)^{\alpha^{\prime} q_{2} \cdot q_{3}} \\
&-\mathrm{e}^{i \pi \alpha^{\prime}\left(q_{1} \cdot q_{2}+q_{2} \cdot q_{3}\right)} \int_{1}^{\infty} \mathrm{d} z_{2}\left(z_{2}\right)^{\alpha^{\prime} q_{1} \cdot q_{2}}\left(z_{2}-1\right)^{\alpha^{\prime} q_{2} \cdot q_{3}} \\
=&-\mathrm{e}^{i \pi \alpha^{\prime} q_{1} \cdot q_{2}} A_{4}^{\text {open }}(1,2,3,4)-\mathrm{e}^{i \pi \alpha^{\prime}\left(q_{1} \cdot q_{2}+q_{2} \cdot q_{3}\right)} A_{4}^{\text {open }}(1,3,2,4)
\end{aligned}
$$

The above equality is the monodromy relation for the four point string amplitudes. In the low-energy limit $\left(\alpha^{\prime} \rightarrow 0\right)$, its real part corresponds to the photon-decoupling identity for gauge theory amplitudes, while the imaginary part yields the Bern-Carrasco-Johansson relations. The analysis can be performed in the same way for amplitudes with more external legs, which leads to the general form of the monodromy relations:

$$
\begin{aligned}
&A_{n}^{\text {open }}(1,2,3,4, \ldots, n)+\mathrm{e}^{i \alpha^{\prime} \pi s_{12}} A_{n}^{\text {open }}(2,1,3,4, \ldots, n) \\
&+\mathrm{e}^{i \alpha^{\prime} \pi\left(s_{12}+s_{13}\right)} A_{n}^{\text {open }}(2,3,1,4, \ldots, n) \\
&+\ldots \\
&+\mathrm{e}^{i \alpha^{\prime} \pi\left(s_{12}+s_{13}+\ldots+s_{1, n-1}\right)} A_{n}^{\text {open }}(2,3,4, \ldots, n-1,1, n)=0,
\end{aligned}
$$

where again $s_{i j}=-\left(q_{i}+q_{j}\right)^{2}$. Employing cyclicity, reflection symmetry as well as the monodromy relations collectively reduces the number of independent amplitudes with $n$ legs to $(n-3) !$.