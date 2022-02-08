---
alias:
- insert
tags:
- qftII
---
---
# Single Insertion
 ![|300](file:///C:/Users/Lucien/Documents/UNI/images/image67.png)

We insert one quantum operator $\hat O = O(\hat q,\hat p)$ at time $t_\text{o}$ with $t_\text{f}>t_\text{o}>t_\text{i}$ into the [[transition amplitude]]^[Here we have used the Heisenberg and Schrödinger pictures
of the operator related by
$\hat O(t_\text{o})=
\hat U(t_\text{ref},t_\text{o})\hat O\hat U(t_\text{o},t_\text{ref})$.]

$$
A_\text{f,o,i}=
\bra{q_\text{f},t_\text{f}}\hat O(t_\text{o})\ket{q_\text{i},t_\text{i}}
=\bra{q_\text{f}}\hat U(t_\text{f},t_\text{o})\hat O\hat U(t_\text{o},t_\text{i})\ket{q_\text{i}}.
$$


As [[Path Integral for Transition Amplitude#Time Slices|before]], we evaluate this expression by inserting a [[position eigenstate#Complete set|complete set of position eigenstates]]

$$
A_\text{f,o,i}
=
\int \dd{q_\text{o}}\dd{q'_\text{o}}
A_\text{f,o}\bra{q_\text{o}}\hat O\ket{q'_\text{o}}A_\text{o',i}.
$$

Here we should replace the quantum operator $\hat O$ by $O(\bar q_\text{o},\hat p)$ where $\bar q_\text{o}$ is a suitable combination of $q_\text{o}$ and $q'_\text{o}$. To evaluate the momentum operator $\hat p$ we insert a [[momentum eigenstate#Complete set|complete set of momentum eigenstates]]

$$\begin{align}
A_\text{f,o,i}
&=
\int \dd{q_\text{o}}\dd{q'_\text{o}}\frac{\dd{p_\text{o}}}{2\pi \hbar}
A_\text{f,o}\bra{q_\text{o}}O(\bar q_\text{o},\hat p)\ket{p_\text{o}}\braket{p_\text{o}}{q'_\text{o}}A_\text{o',i}.
\\
&=
\int \dd{q_\text{o}}\dd{q'_\text{o}}\frac{\dd{p_\text{o}}}{2\pi \hbar}
\exp\pqty{\frac{\iunit}{ \hbar}p_\text{o}(q_\text{o}-q'_\text{o})}
A_\text{f,o}O(\bar q_\text{o},p_\text{o})  A_\text{o',i}.
\end{align}$$
Continuing^[Note that we assumed the two consecutive times
$t_\text{o},t_\text{o'}$
before and after the operator insertion as
identified $t_\text{o}=t_\text{o'}$.
This explains the absence of [[Hamiltonian]] contribution
$-(t_\text{o}-t_\text{o'})H$ at the operator insertion.],

$$
A_\text{f,o,i}
=
\int \prod_{k=1}^{n-1} \dd{q_k}\prod_{k=1}^{n} \frac{\dd{p_k}}{2\pi \hbar}
O(\bar q_\text{o},p_\text{o})
\exp(\frac{\iunit}{ \hbar}S_{n,0}[q,p]).
$$
As a continuous path integral it takes the form
$$
A_\text{f,o,i}
=
\int \mathcal{D}{q} \mathcal{D}{p}
O(q(t_\text{o}),p(t_\text{o}))
\exp\pqty{\frac{\iunit}{ \hbar}S_\text{f,i}[q,p]}.
$$