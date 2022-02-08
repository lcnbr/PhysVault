---
alias:
- Grassmann number
- odd Grassmann number
- Grassmann odd number
- odd Grassmann numbers
- Grassmann odd numbers
- Grassmann variable
- Graßmann variables
- Graßmann variable
- Graßmann number
- Graßmann numbers

tags:
- qftII
---
---
The distinction between bosonic and fermionic fields
in QFT is that the former obey commutation relations
while the latter obey anti-commutation relations.
For the path integral we work with classical fields:
In the classical limit, bosonic fields commute with each other,
and they are represented by ordinary numbers.
Correspondingly, classical fermionic fields anti-commute with each other.
Fermionic fields therefore should take values in
anti-commuting numbers, the so-called odd [[Grassmann variables|Grassmann numbers]].

Let us briefly review [[Grassmann variables|Grassmann numbers]]:
- A Graßmann number $a$ can be either:
    -  even ($\mathbb{Z}_2$-grading $|a|=0$)
    -  odd ($\mathbb{Z}_2$-grading $|a|=1$).
- [[Grassmann variables|Grassmann numbers]] can be added as usual.
- The products of two [[Grassmann variables|Grassmann numbers]] is commutative unless both factors are odd in which case the product is anti-commutative.

# Grassmann odd numbers

Consider a set of odd [[Grassmann variables|Graßmann variables]] $\theta_k$.
They mutually anti-commute
$$
\theta_j \theta_k = -\theta_k \theta_j.
$$
For each variable $\theta_k$ we can define a derivative $\partial/\partial \theta_k$.
The derivatives themselves are odd Graßmann quantities
$$
\frac{\partial}{\partial \theta_j}\frac{\partial}{\partial \theta_k} =
-\frac{\partial}{\partial \theta_k}\frac{\partial}{\partial \theta_j}.
$$
The defining property of derivatives of [[Grassmann variables#Grassmann odd numbers|odd Grassmann numbers]] is
$$
\frac{\partial}{\partial \theta_j}\theta_k
+\theta_k\frac{\partial}{\partial \theta_j}
=\delta^j_k.
$$