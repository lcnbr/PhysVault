# Path integral

We split up the action into a free part (e.g [[Free Scalar Field]])
and interaction terms

$$
S[\Psi]=S_0[\Psi]+S_\text{int}[\Psi].
$$

The free part $S_0$ is quadratic in the fields
and can therefore be integrated exactly (e.g. [[Free Scalar Field]]).
The interaction part $S_\text{int}$ contains all the remaining terms.
^[As discussed in QFT I, the interaction part may as well contain
quadratic terms. These terms can be used to counterbalance loop effects
such that the free action $S_0=S_\text{asymp}$
describes physical particles accurately in the absence of interactions.]
The path integral for the [[graph generating functional]] then reads

$$
Z[J]=\int \mathcal{D}{\Psi}\exp\pqty{\iunit S_0[\Psi]+\iunit S_\text{int}[\Psi]+\iunit S_\text{src}[\Psi,J]}.
$$

We now split up the exponential into
interactions and free terms including sources.
We can then replace the field $\Psi$ in the
interaction part by a functional derivative w.r.t.\ the [[source term in the action|source]] $J$
$$
\begin{align}
Z[J]
&=\int \mathcal{D}{\Psi}\exp\pqty{\iunit S_\text{int}[\Psi]}
\exp\pqty{\iunit S_0[\Psi]+\iunit S_\text{src}[\Psi,J]}
\\
&=\int \mathcal{D}{\Psi}\exp\pqty{\iunit S_\text{int}\bqty{\frac{-\iunit\delta}{\delta J}}}
\exp\pqty{\iunit S_0[\Psi]+\iunit S_\text{src}[\Psi,J]}.
\end{align}
$$
Now the integration variable $\Psi$ appears only in the free and [[source term in the action|source]] contributions
whereas the interactions are formulated in terms of the [[source term in the action|source]] field $J$.
We can thus pull the interactions out of the integral and perform
the free integral as described above
$$
\begin{align}
Z[J]
&=\exp\pqty{\iunit S_\text{int}\bqty{\frac{-\iunit\delta}{\delta J}}}Z_0[J],
\\
Z_0[J]
&=
\int \mathcal{D}{\Psi}\exp\pqty{\iunit S_0[\Psi]+\iunit S_\text{src}[\Psi,J]}.
\end{align}$$

^e033d4


# Examples

[[cubic and quartic interaction generating functional]]