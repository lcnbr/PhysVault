The path integral  generalises straight-forwardly to fields
(we set $\hbar=1$ for convenience).
$$
\begin{align}
&
\bra{\Psi_\text{f},t_\text{f}}\text{T}(\hat O_1 \ldots \hat O_n)
\ket{\Psi_\text{i},t_\text{i}}
\\
&=
\int \mathcal{D}{\Psi}~
O_1[\Psi]\ldots O_n[\Psi]
\exp\pqty{\iunit S_\text{f,i}[\Psi]}.
\end{align}
$$
Here $\Psi_\text{i,f}$ are the spatial fields at the initial
and final time slices,
whereas $\Psi$ is a field in spacetime which
interpolates between the fields $\Psi_\text{i}=\Psi(t_\text{i})$ and $\Psi_\text{f}=\Psi(t_\text{f})$.
The [[../AnalyticalMech/Action]] can be written as an integral over the [[density)](../AnalyticalMech/Lagrangian Density.md|Lagrangian (density)]]
$$
S_\text{f,i}[\Psi]:=
\int_{t_\text{i}}^{t_\text{f}} \mathcal{D}{t} ~L\bqty{\Psi(t),\dot\Psi(t)}
=
\int_\text{i}^\text{f} \dd[D]{x}\mathcal{L}\pqty{\Psi(x),\partial_\mu\Psi(x)}.
$$

This expression is almost covariant, but it still makes reference to
two particular time slices.
Moreover, we are usually not so much interested in
[[transition amplitude]]s between particular field configurations,
but rather in time-ordered correlators
$$
\expval{O_1 \ldots O_n}:=
\bra{0}\text{T}\bqty{\hat O_1 \ldots \hat O_n}\ket{0}.
$$
To solve these problems, we can apply a trick we have
learned in QFT I: A generic state
such as $\ket{\Psi_\text{i},t_\text{i}}$ can be expected to have some overlap with
the ground state $\ket{0}$.
Letting the state evolve for some time while adding some friction
(let the time have a small imaginary component)
makes the state decay to its lowest-energy contribution,
i.e.\ the ground state.

We therefore take the limit $t_\text{f,i}\to \pm \infty(1-\iunit\epsilon)$
and obtain a familiar expression for the time-ordered correlator
$$
\expval{O_1 \ldots O_n}=\frac{\displaystyle
\int \mathcal{D}{\Psi}~O_1[\Psi]\ldots O_n[\Psi]\exp\pqty{\iunit  S[\Psi]}
}{\displaystyle
\int \mathcal{D}{\Psi}\exp\pqty{\iunit  S[\Psi]}
}.
$$
Here the path integrals integrate over [[../AnalyticalMech/Field|fields]] $\Psi$ defined for all of [[spacetime]],
and the [[../AnalyticalMech/Action]] is the integral of the [[../AnalyticalMech/Lagrangian Density]] over all
of [[spacetime]]
$$
S[\Psi]=\int \dd[D]{x}\mathcal{L}\pqty{\Psi(x),\partial_\mu\Psi(x)}.
$$
The term in the denominator accounts for the
overlap of the initial and final states with the ground state.
It evidently takes care of proper normalisation $\expval{1}=1$.
Even more, it conveniently eliminates any constant factor
in the integration measure $\mathcal{D}{\Psi}$ allowing us to
be somewhat sloppy in defining the latter.

As discussed in QFT I, the slight tilting of the time axis
into the complex plane selects Feynman propagators as Green functions.
When we keep this in mind, we do not to consider the tilting anymore.
The path integral expression for time-ordered
^[Here time ordering can be interpreted as causality
since fields commute outside the light-cone.]
correlators is thus perfectly relativistic.

The main application of the path integral
in quantum field theory is to
compute time-ordered vacuum expectation values.
It may also be used to compute different quantities
by specifying alternative boundary conditions
for the integration over fields $\Psi$.