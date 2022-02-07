---
alias:
tags:
- qftII
---
To define a fermionic path integral we need to understand how to integrate
over an  [[Grassmann variables#Grassmann odd numbers|odd Graßmann variable]] $\theta$

$$
\int \dd{\theta} f(\theta)=\mathord{?}.
$$

It makes sense to demand that the integral of a total derivative
vanishes
^[We disregard conceivable boundary terms;
[[Grassmann variables#Grassmann odd numbers|odd Graßmann numbers]] turn out to have trivial topology.]

$$
\int \dd{\theta} \frac{\partial}{\partial \theta} f(\theta)=0.
$$

Now due to anti-commutativity [[Grassmann variables#Grassmann odd numbers|odd Graßmann numbers]] square to zero, $\theta^2=0$,
and hence a generic function $f(\theta)$
can be expanded as $f(\theta)=f_0+\theta f_1$ with two coefficients $f_0$ and $f_1$.
We substitute this into the integral of a total derivative

$$
0=\int \dd{\theta} \frac{\partial}{\partial \theta} (f_0+\theta f_1)
=
\int \dd{\theta} f_1.
$$

It tells us that the integral of a constant must vanish.
We can now integrate a generic function

$$
\int \dd{\theta} (f_0+\theta f_1)=\pqty{\int \dd{\theta} \theta} f_1.
$$

The integral $\int \dd{\theta}\theta$ is some undetermined factor, we can define it as $1$.
The curious result is that integration of  [[Grassmann variables#Grassmann odd numbers|odd Graßmann variables]]
is equivalent to diferentiation
^[This implies that the integration measure $\dd{\theta}$
has the dimension of $\partial/\partial\theta$ or $1/\theta$.]

$$
\int \dd{\theta} f(\theta)=\frac{\partial}{\partial \theta}f(\theta).
$$


The so-called [[Berezin integral]] over  [[Grassmann variables#Grassmann odd numbers|odd Graßmann variables]] behaves in many other respects
like the standard bosonic integral.
For the path integral in quantum field theory,
the most important concepts are [[Fourier integrals for odd Grassmann numbers|Fourier integrals]], [[delta function for odd Grassmann numbers|delta functions]]
 and [[Gaussian integrals for odd Grassmann numbers|Gaußian integrals]]. 