
So far we have discussed [[closed string]]s. The alternative choice is open boundary conditions which leads to some interesting new objects in string theory.

For [[open string]]s we conventionally choose the range of the spatial coordinate $\sigma$ as $0 \leq \sigma \leq$ $\pi$, and we should discuss the boundaries at $\sigma=0, \pi$. We start again in conformal gauge

$$
S=\frac{1}{2 \pi \kappa^{2}} \int \mathrm{d} \xi^{2} \frac{1}{2} \eta^{a b} \partial_{a} X \cdot \partial_{b} X .
$$
involves an integration by parts. Let's consider the string evolving from some initial configuration at $\tau=\tau_{i}$ to some final configuration at $\tau=\tau_{f}$ :
$$
\begin{aligned}
\delta S &=\frac{1}{2 \pi \kappa^{2}} \int \mathrm{d} \xi^{2} \eta^{a b} \partial_{a} \delta X \cdot \partial_{b} X \\
&=\frac{1}{2 \pi \kappa^{2}} \int \mathrm{d} \xi^{2}\left(\partial^{\alpha} \partial_{\alpha} X\right)  \cdot\delta X+\text { total derivative }
\end{aligned}
$$
For an open string the total derivative picks up the boundary contributions
$$
\frac{1}{2 \pi \kappa^{2}}\left[\int_{\tau_{i}}^{\tau_{f}} \mathrm{d}\tau~ \dot{X} \cdot \delta X\right]_{\tau=\tau_{i}}^{\tau=\tau_{f}}-\frac{1}{2 \pi \kappa^{2}}\left[\int_{0}^{\pi} \mathrm{d} \sigma ~ X^{\prime} \cdot \delta X\right]_{\sigma=0}^{\sigma=\pi}
$$
The first term is the kind that we always get when using the principle of least action. The equations of motion are derived by requiring that $\delta X^{\mu}=0$ at $\tau=\tau_{i}$ and $\tau_{f}$ and so it vanishes. However, the second term is novel. In order for it too to vanish, we require
$$
X^{\prime} \cdot \delta X=\partial_{\sigma} X^{\mu} \delta X_{\mu}=0 \quad \text { at } \sigma=0, \pi
$$
There are two different types of boundary conditions that we can impose to satisfy this:
- [[Neumann boundary conditions]]
- [[Dirichlet boundary conditions]]

We can, as we did for the [[closed string spectrum|closed string]] compute the [[open string spectrum]] imposing [[Neumann boundary conditions|Neumann conditions]].


![[string interactions]]


# [[Dp-branes|D-Branes]]. 
Now we take the [[Dirichlet boundary conditions|Dirichlet condition]] seriously. At each string boundary we can choose

- [[Neumann boundary conditions|Neumann condition]] $X^{\prime \mu}=0$ or

- [[Dirichlet boundary conditions|Dirichlet condition]] $X^{\mu}=$ fixed.

We can make this choice for each direction $\mu$ individually.

Geometrical picture: String ends are confined to so-called " [[Dp-branes]]".



![[multiple branes]]