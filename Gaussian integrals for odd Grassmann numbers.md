---
alias:
tags:
- qftII
---
To define a [[Gaussian integral|Gaußian integral]], we need at least two
[[Grassmann variables|Graßmann odd variables]],
otherwise the quadratic exponent would vanish by construction.
For the simplest Gaußian integral we obtain

$$
\int \dd{\theta_2}\dd{\theta_1} \exp(a \theta_1\theta_2)=a.
$$

To make this more reminiscent of a usual $n$-dimensional [[Gaussian integral#in n-dimensions|Gaußian integral]]
let us introduce a $2\times2$ matrix $A$

$$
A=\begin{pmatrix}0&+a\\-a&0\end{pmatrix}.
$$

The result can be expressed as^[The determinant of an anti-symmetric matrix $A$ is the square of the so-called Pfaffian $\operatorname{Pf} A$. The result of the Gaußian integral is thus the Pfaffian]

$$
\int \dd[n]{\theta} \exp(\frac{1}{2}\theta^\mathsf{T} A \theta)\sim\sqrt{\det(A)}.
$$

This result in fact applies to general fermionic Gaußian
integrals defined in terms of an $n\times n$ anti-symmetric matrix $A$.^[A fermionic Gaußian integral requires an even number of integration variables $n$ because the determinant of an odd-dimensional anti-symmetric matrix is zero.]

This expression is very similar to the bosonic $n$-dimensional [[Gaussian integral#in n-dimensions|Gaußian integral for a symmetric matrix]] $S$

$$
\int \dd[n]{x} \exp(- \frac{1}{2} x^\mathsf{T} S x)\sim\frac{1}{\sqrt{\det(S)}}.
$$

The crucial difference is that the determinant of the matrix
appears with positive rather than negative exponent.
Moreover, the matrix $A$ does not need to fulfil any positivity
requirements since the odd integral is always well-defined.