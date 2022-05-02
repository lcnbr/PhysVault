A general state in QFT is defined from a superposition of n-particle states:

$$\ket{\psi}=\sum\limits _{n=0}^\infty \frac{1}{n!} \int \dd{\Phi_n(p_1,\dots,p_n)} \tilde{\psi}^{(n)}(p_1, \dots,p_n)\ket{p_1,\dots,p_n}$$
Where we use the notation for the [[Lorentz invariant measure]].
We call $\tilde{\psi}^{(n)}(p_1,\dots,p_n)$ the n-particle momentum space wave function. It is generally only defined in asymptotic states, considering well defined free non-interacting fields.  Usually as well we consider that:

 $$\tilde{\psi}^{(n)}(p_1,\dots,p_n)=\tilde{\psi}^{(n)}(\mathbf{p_1},\dots,\mathbf{p_n})=\prod \limits_{j=1}^n\tilde{f}_j(\mathbf{p_j})+\text{permutations}$$

that is, that the state is a product state and that we have eliminated the time dependence by putting things [[on-shell]] (i.e integrating over $t$ with the help of the positive energy enforcing delta function in the measure). Additionally we need that $\tilde{\psi}^{(n)}$ be square integrable and thus also the $\tilde{f}_j$.


The coordinate space wave functions $f_j(x)$ are defined as:

$$f_j(x)=\int \dd{\Phi(p)}\tilde{f}_j(\mathbf{p})\,e^{-\iunit p^\mu x_\mu}$$

If we take $x^\mu \to \infty$ then in the integrand  the exponential as a function of $\mathbf{p}$ will be rapidly oscillating. If additionally $\tilde{f}_j(\mathbf{p})$ is not a rapidly oscillating function of $\mathbf{p}$ then the integral will average out the exponential to zero and thus evaluate to zero. If however for certain values of $\mathbf{p}$ the exponential does not rapidly vary then those points will give a non-zero contribution to the integral. This is the [[stationary phase approximation]]. In this case the stationary phase point $\mathbf{p_c}$ is given by:

$$\begin{align*}
0=&\pdv{(-E_\mathbf{p_c}t+\mathbf{p_{c}\cdot \mathbf{x}})}{\mathbf{p_c}}\\
&=-\pdv{(\sqrt{m^2+\abs{\mathbf{p_c}}^2})}{\mathbf{p_c}}t+ \mathbf{x}\\
&=-\frac{\mathbf{p_{c}}t}{\sqrt{m^2+\abs{\mathbf{p_c}}^2}}+x\\
&=-\frac{\mathbf{p_c}t}{E_\mathbf{p_c}}+\mathbf{x}\end{align*}
$$

Thus $$\mathbf{p_{c}}=\frac{m\mathbf{x}\operatorname{sign}(t)}{\sqrt{t^2-\mathbf{x}^{2}} 
 } $$

And then $$E_\mathbf{p_c}=\frac{m \abs{t} }{\sqrt{t^2-m^2}}$$

Notice that the stationary phase condition only has a solution when $x=(t, \boldsymbol{x})$ is time-like or zero.

Usually we assume that the momentum space wave functions are sharply peaked around one specific value of momentum $\mathbf{p}=\mathbf{p_0}$. Then, given $t$, the coordinate-space wave function is largest when the stationary phase point is close to the maximum of the function $\tilde{f}_j(\boldsymbol{p})$, i.e., when $\boldsymbol{p}_{\mathrm{c}}=\boldsymbol{p}_{0}$, and thus when
$$
\boldsymbol{x} \simeq \frac{\boldsymbol{p}_{0} t}{E_{\boldsymbol{p}_{0}}}=\boldsymbol{v}_{0} t .
$$
This is the trajectory of a classical relativistic particle, which therefore, as expected, matches the overall propagation of the wave packet. The 3 -velocity is $\boldsymbol{v}_{0}=\boldsymbol{p}_{0} / E_{\boldsymbol{p}_{0}}$.