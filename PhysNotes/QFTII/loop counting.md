---
aliases: 
tags: 
sources:
date created: Saturday, February 19th 2022, 9:45:03 am
date modified: Monday, May 23rd 2022, 12:07:53 pm
---

Next let us understand the role of the quantum parameter $\hbar$
in QFT better.
We reinstate $\hbar$ in the [[graph generating functional with interaction]]^[Of course the action $S[\Psi]$ may also implicitly depend on Planck's constant which would spoil the counting scheme outlined below. Therefore we set $\hbar=1$ and only put the (new) constant $\hbar$ in front of the action in the exponent. This $\hbar$ is the formal parameter to count loops.]
$$
\require{color}
\definecolor{light-yellow}{rgb}{1,0.98,0.77}
\definecolor{dark-yellow}{RGB}{255, 249, 196}
\definecolor{light-green}{RGB}{197, 225, 165}
\definecolor{dark-green}{rgb}{.58,.69,.46}
\definecolor{light-blue}{rgb}{.75,0.87,0.98}
\definecolor{dark-blue}{RGB}{138, 172, 200}
\definecolor{light-purple}{rgb}{.88,0.75,0.91}
\definecolor{dark-purple}{RGB}{175, 142, 181}
\definecolor{light-orange}{rgb}{1,0.88,0.7}
\definecolor{dark-orange}{RGB}{203, 174, 130}
\definecolor{light-red}{rgb}{.94,0.6,0.6}
\definecolor{dark-red}{RGB}{186, 107, 108}
\begin{align}
Z[J]
&=\int \mathcal{D}{\Psi}\exp\pqty{\iunit {\color{dark-red}\hbar^{-1}}S[\Psi]+\iunit{\color{dark-red}\hbar^{-1}}S_\text{src}[\Psi,J]},
\\
&=\exp\pqty{{\iunit}{\color{dark-blue}\hbar^{-1}}S_\text{int}\bqty{{\color{dark-orange}\hbar}\frac{-\iunit\delta}{\delta J}}}Z_0[J],
\\
Z_0[J]
&=
\exp \pqty{ \frac{\iunit}{2}{\color{dark-green}\hbar^{-1}} \int \dd[D]{x}\dd[D]{y} J(x) J(y) G_\text{F}(x,y) }.
\end{align}
$$

^bd49ba

The above expression for the generating functional
shows clearly where powers of $\hbar$ appear within [[graph generating functional#Interacting theories|graphs]] :
- <mark style="background: #BBDEFBA6;">Each interaction vertex contributes a power of $\hbar^{-1}$</mark>.
- <mark style="background: #C5E1A5A6;">Each line contributes a power of $\hbar^{-1}$</mark> .
- <mark style="background: #FFE0B2A6;">Each junction between a vertex and a line originating from the functional derivative $-\iunit\hbar\delta/\delta J$ contributes a power of $\hbar^{+1}$.</mark> 

Consider now a graph with
- $I$ internal lines (connecting two vertices),
- $E$ external lines (connecting to one vertex only),
- $V$ interaction vertices,
- $N$ connection components,
- $L$ loops.


For the counting of powers of $\hbar$ we need to count
the vertices, lines and junctions.
The latter is not immediately given by the graph parameters,
but it can be expressed in terms of the number of
internal and external lines:
- Each internal line contributes $\hbar^{-1}$ for the line itself times $\hbar^{+2}$ from the two junctions with vertices.
- ![[image37.png#center|200]]
- Each external line contributes $\hbar^{-1}$ for the line itself times $\hbar^{+1}$ from a single junction to a vertex.
![[image27.png#center|200]]
- Each interaction vertex contributes $\hbar^{-1}$.
![[image58.png#center|200]]


Altogether we obtain the total power of $\hbar$ associated to the graph
$$
\hbar^{I-V}.
$$

We can reexpress this combination using the number of
non-trivial momentum integrals, i.e.\ the number of loops of the graph.
Consider the number of undetermined momenta within a graph:
- one free momentum for each internal and external line (integral),
 - one constraint for each vertex ([[delta function]]),
 - one constraint for each external line (fixed by momentum inflow),
 - relax one constraint for the external lines within each connection component (the constraints due to the vertices already imply overall momentum conservation within this component which determines one of the external momenta in terms of the others).

Performing all trivial momentum integrals which contain delta functions
thus leaves the following number of momentum integrals undetermined
$$
L=I+E-V-E+N=I-V+N.
$$

This combination is the number $L$ of non-trivial
momentum integrals, i.e. the number of loops of the graph.

Altogether the powers of $\hbar$ now read

$$
\hbar^{I-V} = \hbar^{L-N}.
$$

This means that each momentum loop is
suppressed by one power of $\hbar$.
The leading contribution at $L=0$
is considered to represent
classical physics.
Moreover the number of connection components $N$ plays a role.
We shall soon return to this result.
