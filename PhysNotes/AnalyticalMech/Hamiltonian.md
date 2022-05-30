dddddddd---
alias:
tags:
- qftII
---
# For [[../String/Classical Particle Mechanics]]
The [[.md|Hamiltonian]] is the [[../math/Legendre transform]] of the [[Lagrangian]]:

$$
H(q, p)= p_a \dot{q}^a-L(q, \dot{q})
$$

Where $p_a$ are [[Conjugate momenta]] to $q^a$

The [[equations of motion|eoms]] are then given by [[../math/Legendre transform#^56190e]] i.e:

$$\frac{\partial H}{\partial p_a}=\dot{q}^a$$

And using [[../math/Legendre transform#^e320f3]]

$$
\begin{aligned}
\frac{\partial H}{\partial q^a} &= p_b \frac{\partial \dot{q}^b}{\partial q^a}-\frac{\partial L}{\partial q^a}-\frac{\partial L}{\partial \dot{q}_b} \frac{\partial \dot{q}_b}{\partial q^a} \\
&= p_b \frac{\partial \dot{q}^b}{\partial q^a}-\frac{\partial L}{\partial q^a}-p_b \frac{\partial \dot{q}_b}{\partial q^a} \\

&=-\frac{\partial L}{\partial q^a} \\
&=-\frac{d}{d t} \frac{\partial L}{\partial \dot{q}^a} \\
&=-\dot{p}_a
\end{aligned}
$$

^db7790

Where  we used [[../GR/Einstein summation]] everywhere  and the [[Euler-Lagrange equations]] in the fourth line. Altogether we have
## Hamilton's equations
$$
\boxed{
\begin{align}
\dot{q}^a&=\frac{\partial H}{\partial p_a} \\
-\dot{p}_{i}&=\frac{\partial H}{\partial q^a}
\end{align}}
$$

# For [[../FT/Classical Field Theory]]

We define the [[Hamiltonian Density]].

![[Hamiltonian Density]]


# Common [[.md|Hamiltonian]]s

## Quadratic momentum

$$H(q,p)=\frac{p^2}{2M(q)}+p K(q) + V(q).$$

### Free Particle
$$H(q,p)=\frac{p^2}{2m}.$$