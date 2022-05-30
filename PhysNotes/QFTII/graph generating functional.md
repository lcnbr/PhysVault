---
alias:
- generating functional
- path integral
tags:
- qftII
---

# Generating functional

Gladly there is a standard trick to insert factors
in front of the exponential factor using [[source term in the action|source]] terms.
We define the generating functional $Z[J]$

$$
Z[J]:=
\int \mathcal{D}{\Psi}\exp\pqty{\iunit  S[\Psi]+\iunit S_\text{src}[\Psi,J]}
$$

as a standard path integral but with an additional [[source term in the action]]. Since the [[source term in the action|source]] field does not appear in the original action, functional derivatives of $Z[J]$
w.r.t. the [[source term in the action|source]], insert factors of $\Psi(x)$ into the path integral

$$
\Psi(x) \simeq \frac{-\iunit\delta}{\delta J(x)}.
$$

For example, we express two insertions
as a double functional derivative of $Z[J]$

$$
\frac{-i\delta}{\delta J(x)}\frac{-\iunit\delta}{\delta J(y)}
Z[J] =
\int \mathcal{D}{\Psi}~\Psi(x)\Psi(y)\exp\pqty{\iunit  S[\Psi]+\iunit S_\text{src}[\Psi,J]}.
$$

^709167

Now we still need to get rid of the [[source term in the action|source]] term in the exponent
by setting $J=0$.
## time-ordered two-point correlator
The time-ordered two-point correlator
with proper normalisation term
finally takes the form

$$
\expval{\Psi(x)\Psi(y)}=
Z[J]^{-1}\eval*{\frac{-\iunit \delta}{\delta J(x)}
\frac{-\iunit\delta}{\delta J(y)} Z[J]}_{J=0}.
$$
## In interacting theory:

![[graph generating functional with interaction]]

# In [[Feynman graphical notation]]:

## In a free theory

Using the [[Free Scalar Field]] as an example we write:
![[Free Scalar Field#^2d84e1]]
With the [[connected graph generating functional#In feynman graphical notation]]:
![[image46.png]]

## Interacting theories

Using the [[cubic and quartic interaction generating functional]] example we extrapolate that the generating functional $Z[J]$ is a collection (sum) of Feynman graphs
whose legs are all saturated by source fields $J$
(monomials)

![[image86.png||250]]

To obtain a correlation function, all sources $J$ have to be saturated by
functional derivatives $-\iunit\delta/\delta J$ representing the fields $\Psi$
of the correlator.

Note that symmetry factors are usually different for terms of the
generating functional and for the corresponding correlation functions:


- All source fields $J$ are indistinguishable and can be freely permuted.
    - This results in large symmetry factors in $Z[J]$.
- The fields $\Psi(x)$, $\Psi(y)$ in some correlator and corresponding functional derivatives are well distinguishable due to the distinct positions $x,y$ in spacetime.
    - Hence correlation functions often have relatively small symmetry factors since the external legs cannot be permuted.
