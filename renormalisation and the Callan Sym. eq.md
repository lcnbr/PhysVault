Let us now show how regularisation and renormalisation of divergences leads to non-trivial coefficient functions $\beta(\lambda)$ and $\gamma(\lambda)$ in the Callan-Symanzik equation.

We start with some correlation function which we compute in the dimensional regularisation scheme. The bare result $\bar{G}$ in terms of the bare coupling constant $\bar{\lambda}$ is expressed as $\bar{G}\left(p_{k}, \bar{\lambda}, \mu, \epsilon\right)$.

We know that in dimensional regularisation the renormalisation scale $\mu$ appears in a very predictable fashion: Up to some potential rescalings it only appears in the combination $\lambda \mu^{2 \epsilon}$. This combination has a non-trivial mass dimension which we should compensate by some appropriate powers of the momenta $p_{k}$. Moreover the overall mass dimension of $\bar{G}$ is $n d$. We can thus write the most general result in the following form ${ }^{22}$
$$
\bar{G}(p, \bar{\lambda}, \mu, \epsilon)=p^{n d} \bar{F}\left((\mu / p)^{2 \epsilon} \bar{\lambda}, \epsilon\right) .
$$
It is straight-forward to confirm that this function obeys the [[running coupling]] with the bare parameter functions
$$
\bar{\beta}(\bar{\lambda})=-2 \epsilon \bar{\lambda}, \quad \bar{\gamma}(\bar{\lambda})=0
$$
The non-zero beta-function tells us that the coupling constant has an effective mass dimension which tends to zero when the regulator $\epsilon$ is removed.

The crucial point is that we cannot yet remove the regulator since the bare result $\bar{G}$ typically has a pole at $\epsilon=0$. This calls for renormalisation which takes the generic form
$$
\bar{G}_{n}\left(p_{k}, \bar{\lambda}, \mu, \epsilon\right)=N(\bar{\lambda})^{n} G_{n}\left(p_{k}, \lambda(\bar{\lambda}), \mu, \epsilon\right) .
$$
The renormalised result $G_{n}$ is now finite with divergences hidden in the field renormalisation $N(\bar{\lambda})$ and coupling constant renormalisation $\lambda(\bar{\lambda})$.

Assuming that the Callan-Symanzik equation holds in terms of the bare variables, it also holds for the renormalised variables with the renormalised functions given by the transformation
$$
\begin{aligned}
&\beta(\lambda(\bar{\lambda}))=\bar{\beta}(\bar{\lambda}) \frac{\partial \lambda}{\partial \bar{\lambda}}(\bar{\lambda}), \\
&\gamma(\lambda(\bar{\lambda}))=\bar{\gamma}(\bar{\lambda})+\frac{\bar{\beta}(\bar{\lambda})}{N(\bar{\lambda})} \frac{\partial N}{\partial \bar{\lambda}}(\bar{\lambda}) .
\end{aligned}
$$
Renormalisation therefore preserves the Callan-Symanzik equation with some set of deformed parameters.

Suppose in dimensional regularisation the renormalisation functions take the following generic form with poles at $\epsilon=0$
$$
\begin{aligned}
\lambda &=\bar{\lambda}+\bar{\lambda}^{2}\left(b_{1} / \epsilon+b_{2}+\ldots\right)+\ldots, \\
\bar{\lambda} &=\lambda-\lambda^{2}\left(b_{1} / \epsilon+b_{2}+\ldots\right)+\ldots, \\
N(\bar{\lambda}) &=1+\bar{\lambda}\left(c_{1} / \epsilon+c_{2}+\ldots\right)+\ldots
\end{aligned}
$$

Substituting these expansions into the above expressions we obtain perfectly regular expressions for $\beta$ and $\gamma$ at $\epsilon \rightarrow 0$
$$
\begin{aligned}
&\beta(\lambda)=-2 \epsilon \lambda-2 \lambda^{2}\left(b_{1}+b_{2} \epsilon+\ldots\right)+\ldots \\
&\gamma(\lambda)=-2 \lambda\left(c_{1}+c_{2} \epsilon+\ldots\right)+\ldots
\end{aligned}
$$
Taking the limit $\epsilon \rightarrow 0$, we find the renormalised expressions
$$
\beta(\lambda) \rightarrow-2 b_{1} \lambda^{2}+\ldots, \quad \gamma(\lambda) \rightarrow-2 c_{1} \lambda+\ldots
$$
Curiously, they are non-vanishing, so the renormalisation procedure has in fact achieved something non-trivial. This was only possible because of the divergences in the bare correlators. So the divergences are not just an inconvenient feature of QFT, they actually are related to non-trivial behaviour of the quantum model such as running coupling constants.

We should mention that the above functions $\beta$ and $\gamma$ are not uniquely defined: For example, we are free to perform a further finite perturbative redefinition of the coupling $\lambda \rightarrow \lambda^{\prime}=\lambda+\mathcal{O}\left(\lambda^{2}\right)$. This leaves the classical model unchanged, but it modifies the higher-loop contributions to $\beta$ and $\gamma$.