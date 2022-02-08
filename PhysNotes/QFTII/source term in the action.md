---
alias:
- source
---
# source term in the action

We can always add this [[source term in the action|source term]] in the [[Action|action]]:
\footnote{The field $J(x)$ is the same source field
as discussed in QFT I in connection to propagators.}

$$
S_\text{src}[\Psi,J]:=
\int \dd[D]{x} \Psi(x) J(x).
$$

## Functional derivative
This source term has the simple property
that a [[functional derivative]] w.r.t.\ the source $J(x)$
produces precisely the [[Field|field]] $\Psi(x)$ at the same location

$$
\frac{\delta S_\text{src}[\Psi,J]}{\delta J(x)}
=
\int \dd[D]{y} \Psi(y) \delta^D(x-y)
=\Psi(x).
$$

When the source action is in the exponent,
the functional derivative brings down one power of $\Psi$
without altering the exponent

$$
\frac{-\iunit\delta}{\delta J(x)} \exp\pqty{\iunit S_\text{src}[\Psi,J]}
=
\Psi(x)
\exp\pqty{\iunit S_\text{src}[\Psi,J]}.
$$