---
alias:
- Dirichlet conditions
- Dirichlet condition
- dirichlet boundaries
- dirichlet boundary
- dirichlet
---
$$
\delta X^{\mu}=0 \quad \text { at } \sigma=0, \pi
$$
This means that the end points of the string lie at some constant position, $X^{\mu}=$ $c^{\mu}$, in space.

Now consider [[Compactification and T-Duality|compactification]] for open strings. Again, this is almost the same as for closed strings. However, we have no [[winding modes]] because the open string can always unwind.

![](https://cdn.mathpix.com/cropped/2022_01_21_c2f821e442f23993db05g-3.jpg?height=94&width=617&top_left_y=1131&top_left_x=308)

# [[T-Duality]]. 
We apply [[T-duality]] to open strings and introduce the dual field $\tilde{X}^{25}$ by the relation

$$
X^{\prime 25}=\dot{\tilde{X}}^{25}, \quad \dot{X}^{25}=\tilde{X}^{\prime 25} .
$$

The boundary conditions translate to

$$
X^{\prime \mu}=0 \quad(\mu=0, \ldots, 24), \quad \dot{\tilde{X}}^{25}=0 .
$$

We obtain Dirichlet boundary condition for the dual coordinate $\tilde{X}^{25}$ while the [[Neumann boundary conditions]] remains for the remaining original coordinates $X^{\mu}$. The Dirichlet condition implies that the ends of the string are fixed to constant values in the coordinate $\tilde{X}^{25}$. This corresponds to the alternate choice of boundary e.o.m. where the variation is suppressed, $\delta \tilde{X}^{25}=0$.

![](https://cdn.mathpix.com/cropped/2022_01_21_c2f821e442f23993db05g-4.jpg?height=137&width=151&top_left_y=197&top_left_x=541)

We can show that the dual string actually starts and ends at the same $\tilde{X}^{25}$ coordinate

$$
\Delta \tilde{X}^{25}=\int \mathrm{d} \sigma \tilde{X}^{\prime 25}=\int \mathrm{d} \sigma \dot{X}^{25}=2 \pi \kappa^{2} p_{25}=\frac{2 \pi \kappa^{2} n}{R}=2 \pi n \tilde{R} .
$$

Here we have used that the momentum $p_{25}=n / R$ is quantised in KK modes. The end points are then identified by the compactification of the dual coordinate $\tilde{X}^{25} \equiv \tilde{X}^{25}+2 \pi \tilde{R}$.

![](https://cdn.mathpix.com/cropped/2022_01_21_c2f821e442f23993db05g-4.jpg?height=84&width=617&top_left_y=567&top_left_x=308)

Note that the Dirichlet boundary condition constrains the string end points which allows winding modes but prevents momentum flow along $\tilde{X}^{25}$ and thus KK modes. In conclusion, T-duality exchanges the roles of KK and winding modes just as for closed strings.

The Dirichlet condition modifies the oscillator relation

$$
\tilde{\alpha}_{n}^{\mathrm{L}, 25}=-\tilde{\alpha}_{n}^{\mathrm{R}, 25}=: \tilde{\alpha}_{n}^{25}
$$

such that the general solution reads

$$
\tilde{X}^{25}=\tilde{x}_{0}^{25}+\sum_{n \neq 0} \frac{i \kappa}{\sqrt{2} n} \tilde{\alpha}_{n}^{25}\left(-\exp \left(-i n \xi^{\mathrm{L}}\right)+\exp \left(-i n \xi^{\mathrm{R}}\right)\right) .
$$

Although the Dirichlet condition $X^{25}=$ const. may appear unnatural (why $X^{25} ?$ what value?), we find that it has to be part of (T-dual) string theory (on compact spaces).