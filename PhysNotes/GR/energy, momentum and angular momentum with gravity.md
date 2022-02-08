---
alias:
- modified energy-momentum tensor
tag: GR physics
---

In [[special relativity]] we could define the [[energy-momentum tensor in SR|energy/momentum]] of isolated systems from the conservation equation of the energy-momentum tensor $\partial_{\mu} T^{\mu \nu}=0$. In General Relativity the [[energy-momentum tensor in GR|energy-momentum tensor]] in the right-hand side of [[Einstein's field equations|Einstein's equations]]

![[Einstein's field equations#^EinsteinfieldEq|Einstein's equation]]

is not conserved in the traditional way. Instead we have (see [[energy-momentum tensor in GR#^contEq|energy-momentum tensor]])
$$
T^{\mu \nu}{}_{; \mu}=0
$$
in which the [[covariant derivative]] includes the effects of gravitation in a concealed way. We want to define an energy-momentum tensor which includes explicitly gravitation, let us call it $t_{\mu \nu}$, that is traditionally conserved
$$
\partial_{\mu} t^{\mu \nu}=0
$$
We will do that for gravitational systems which are confined within some finite volume. The spacetime metric at large distances, where we assume that gravity falls off, will approach the [[Minkowski metric|Minkowskian]] limit. We can then decompose
$$
g_{\mu \nu}=\eta_{\mu \nu}+h_{\mu \nu}
$$
where $h_{\mu \nu} \rightarrow 0$ as $r \rightarrow \infty$, but it can be large at finite distances. Let us now separate the part of the left-hand side of Einstein's equations which is linear in $h_{\mu \nu}$. Namely ($\Lambda=0$)
$$
G^{\mu \nu} \equiv R^{(1) \mu \nu}-g^{\mu \nu} \frac{R^{(1)}}{2}=G^{(1) \mu \nu}+\Delta G^{\mu \nu}
$$

We have from [[Ricci tensor#weak field approximation]]:
![[Ricci tensor#^weeakApprox]]
which we represent as
![[Pasted image 20220206160122.png#center|400]]
also the  linear [[Ricci scalar]]:
![[Pasted image 20220206160225.png#center|400]]
In total
$$G^{(1) \mu \nu}=R^{(1) \mu \nu}-\eta^{\mu \nu} \frac{R^{(1)}}{2}$$

![[Pasted image 20220206160253.png#center|400]]


$$=\frac{\partial}{\partial x^{\rho}}\left(A^{\mu \nu \rho}-A^{\mu \rho \nu}\right)$$
with
![[Pasted image 20220206160314.png#center|400]]
or, explicitly (note we raise and lower with [[Minkowski metric]] instead of the generic [[metric tensor|metric]])
$$
A^{\mu \nu \rho}=\frac{1}{2}\left\{\eta^{\nu \beta} \eta^{\mu \rho} \frac{\partial h^{\alpha}{ }_{\alpha}}{\partial x^{\beta}}+\frac{\partial h^{\mu \nu}}{\partial x^{\beta}} \eta^{\rho \beta}+\eta^{\mu \nu} \frac{\partial h^{\rho \alpha}}{\partial x^{\alpha}}\right\} .
$$
Thus

$$
G^{(1) \mu \nu} \equiv R^{(1) \mu \nu}-\frac{\eta^{\mu \nu}}{2} R^{(1)}=\frac{\partial}{\partial x^{\rho}}\left(A^{\mu \nu \rho}-A^{\mu \rho \nu}\right) .
$$

^LinG

Differentiating with $\frac{\partial}{\partial x^{\nu}}$, we have
$$
\frac{\partial G^{(1) \mu \nu}}{\partial x^{\nu}} \equiv \frac{\partial}{\partial x^{\nu}}\left(R^{(1) \mu \nu}-\frac{\eta^{\mu \nu} R^{(1)}}{2}\right)=\underbrace{\frac{\partial^{2}}{\partial x^{\nu} \partial x^{\rho}}}_{\text {sym. }} \underbrace{\left(A^{\mu \nu \rho}-A^{\mu \rho \nu}\right)}_{\text {antisym. }}=0 .
$$
Let us now return to Einstein's equations and rewrite them as follows (still setting $\Lambda=0$ )

$$
\begin{align}
G^{\mu \nu} & \equiv R^{\mu \nu}-\frac{g^{\mu \nu}}{2} R=-8 \pi G T^{\mu \nu} \\
\iff G^{(1) \mu \nu} &=-8 \pi G T^{\mu \nu}+G^{(1) \mu \nu}-G^{\mu \nu} 

\end{align}
$$
Thus we have our rewritten [[Einstein's field equations#^EinsteinfieldEq|Einstein's equations]]:

$$ G^{(1) \mu \nu} =-8 \pi G t^{\mu \nu}$$

^newEinstein

with [[#^LinG]] and
$$
t^{\mu \nu}=T^{\mu \nu}+\frac{1}{8 \pi G}\left(G^{\mu \nu}-G^{(1) \mu \nu}\right)=T^{\mu \nu}+\frac{1}{8 \pi G} \Delta G^{\mu \nu} 
$$

^newT

Differentiating the rewritten Einstein's equations [[#^newEinstein]] we obtain
$$
\begin{aligned}
\frac{\partial}{\partial x^{\nu}} G^{(1) \mu \nu} &=-8 \pi G \frac{\partial}{\partial x^{\nu}} t^{\mu \nu} \\
0 &=-8 \pi G \frac{\partial}{\partial x^{\nu}} t^{\mu \nu} \\
\end{aligned}
$$

Thus

$$
\frac{\partial}{\partial x^{\nu}} t^{\mu \nu} =0
$$

^tCons

showing that $t^{\mu \nu}$ is conserved. It is composed of the energy-momentum tensor of matter and electromagnetic and other forces (other than gravity) and the term $\Delta G^{\mu \nu}=G^{\mu \nu}-G^{(1) \mu \nu}$ in which the part of $G^{\mu \nu}$ which is linear in $h_{\mu \nu}$ is removed. Therefore $\Delta G$ is quadratic in $h_{\mu \nu}$. In a particle physics interpretation, such nonlinear terms correspond to "self-interaction" of particles, which in this case are the gravitons.


# [[Newtonian limit]]

At large distances, we assume that $h_{\mu \nu}$ approaches the [[Newtonian limit]]. It should then behave as the Newtonian potential, falling off as
$$
h_{\mu \nu} \stackrel{r \rightarrow \infty}{\longrightarrow} \frac{1}{r} .
$$
The derivatives of $h_{\mu \nu}$ should behave as
$$
\frac{\partial h_{\mu \nu}}{\partial x^{\nu}} \stackrel{r \rightarrow \infty}{\longrightarrow} \frac{1}{r^{2}},
$$
and thus
$$
\Delta G^{\mu \nu} \stackrel{r \rightarrow \infty}{\longrightarrow} \frac{1}{r^{4}} .
$$
With these scalings in mind, which guarantee convergence, the integral of the continuity equation over some large volume $V$ bounded by a surface $S$ very far towards infinity. We have
$$
\int_{V} \dd[3]{x} \frac{\partial t^{\mu 0}}{\partial t}=-\int_{V} \dd[3]{x} \frac{\partial t^{\mu j}}{\partial x^{j}}=-\int_{S} \dd{S} n_{j} t^{\mu j} .
$$
On the left-hand side, we identify the time derivative of the momentum of the system
$$
P^{\mu}=\int_{V} \dd[3]{x} t^{\mu 0} .
$$
On the right-hand side we identify the momentum flux. For the momentum we have
$$
\begin{aligned}
8 \pi G P^{\mu} &=\int_{V} \dd[3]{x} \frac{\partial}{\partial x^{\rho}}\left(A^{\mu 0 \rho}-A^{\mu \rho 0}\right) \\
&=\int_{V} \dd[3]{x} \frac{\partial}{\partial x^{j}}\left(A^{\mu 0 j}-A^{\mu j 0}\right) \\
&=\int_{S} \dd{S} n_{j}\left(A^{\mu 0 j}-A^{\mu j 0}\right),
\end{aligned}
$$

where we used the divergence theorem in the last step. For $\mu=0$
$8 \pi G P^{0}=\int_{S} \dd{S} n_{j}\left(A^{00 j}-A^{0 j 0}\right)$,
which after plugging in previous results for $A^{\mu \nu \rho}$ gives
$$
P^{0}=\frac{1}{16 \pi G} \int_{S} \dd{S} n_{j}\left[\frac{\partial h^{j k}}{\partial x^{k}}-\frac{\partial h^{k k}}{\partial x^{j}}\right] .
$$
For $\mu=i=1,2,3$ we have
$$
8 \pi G P^{i}=\int_{S} \dd{S} n_{j}\left(A^{i 0 j}-A^{i j 0}\right),
$$
which similarly gives
$$
P^{i}=\frac{1}{16 \pi G} \int_{S} \mathrm{~d} S n_{j}\left[\frac{\partial h^{i j}}{\partial t}+\frac{\partial h^{i 0}}{\partial x^{j}}-\delta_{i j}\left(\frac{\partial h^{0 k}}{\partial x^{k}}+\frac{\partial h^{k k}}{\partial t}\right)\right]
$$
Angular momentum is derived similarly. As $t^{\mu \nu}$ is symmetric, the following [[tensor fields in GR|tensor]] is conserved
$$
M^{\mu \nu \rho}=t^{\mu \nu} x^{\rho}-t^{\mu \rho} x^{\nu}
$$
Then
$$
\begin{aligned}
\frac{\partial}{\partial x^{\mu}} M^{\mu \nu \rho} &
=\cancel{\frac{\partial t^{\mu \nu}}{\partial x^{\mu}} x^{\rho}}
+t^{\mu \nu} \delta_{\mu}^{\rho}
-\cancel{\frac{\partial t^{\mu \rho}}{\partial x^{\mu}} x^{\nu}}
-t^{\mu \rho} \delta_{\mu}^{\nu} \\

&=t^{\rho \nu}-t^{\nu \rho}=0 .
\end{aligned}
$$
And the following quantities (identified with angular momentum) are conserved
$$
J^{\rho \nu}=\int \mathrm{d}^{3} x M^{0 \rho \nu} .
$$
which is equivalent to Einstein's theory. We are thus led back to the remark at the beginning of this chapter, that the major difference between the electromagnetic and gravitational fields is that the source of the electromagnetic potential $A^{\alpha}$ is a conserved current $J^{\alpha}$ that does not involve $A^{\alpha}$ because the electromagnetic field is not itself charged, whereas the source of the gravitational field $h_{\mu \kappa}$ is a conserved "[[tensor fields in GR|tensor]]" $\tau^{\mu \kappa}$ that must involve $h_{\mu \kappa}$ because the gravitational field does carry energy and momentum.