---
alias:
- connected functional
- connected generating functional

tags:
- qftII
---

# generating functional of connected graphs

The connected generating functional $W[J]$
is defined as the logarithm of $Z[J]$
^[This is a pretty general relationship for generating functionals of graphs which also holds in different contexts.]

$$
W[J]=-\iunit\hbar\log Z[J],
\quad
Z[J]=\exp\pqty{\iunit \hbar^{-1}W[J]}.
$$

Just like any other generating functional,
$W[J]$ can be represented in terms
of a sum over Feynman graphs.
The difference w.r.t. $Z[J]$ is that
$W[J]$ encodes precisely all *connected* Feynman graphs.


How can this relationship be proved?
It is a simple consequence of the symmetry
factors of disconnected Feynman graphs.
The symmetry factor is the product of


 - the symmetry factors of the connected components and
 - a factor of $1/n!$ for $n$ equivalent connected components.


More explicitly, consider a disconnected graph $\Gamma$ consisting of connected subgraphs $\Gamma_k$ with
multiplicity $n_k$. The contribution to $Z[J]$ reads
^[Here, the symbol $X\in Y$ is means “$X$ is a term of the polynomial $Y$”.]

$$
\frac{\Gamma[J]}{S(\Gamma)}=
\prod_k \frac{1}{n_k!}
\pqty{\frac{\Gamma_k[J]}{S(\Gamma_k)}}^{n_k}
\in Z[J]

$$

Here $S(\Gamma)$ denotes the symmetry factor associated to the graph $\Gamma$.
The above term actually arises as one term in the multinomial
and exponential

$$
\frac{\Gamma}{S(\Gamma)}
\in
\frac{1}{n!}\pqty{\sum\nolimits_k\frac{\Gamma_k}{S(\Gamma_k)}}^n
\in
\exp\pqty{\sum\nolimits_k\frac{\Gamma_k}{S(\Gamma_k)}}.
$$


This means that exponentiating the sum of all connected graphs with
appropriate symmetry factors
yields the sum of all connected and disconnected graphs with
precisely the right symmetry factors.
In terms of graphs we can write $Z[J]$ in terms of $W[J]$ as
 
![[file:///C:/Users/Lucien/Documents/UNI/images/image12.png||500]]

# For the free action
## In [[Feynman graphical notation]]

Using the [[Free Scalar Field]] as an example, we use [[Free Scalar Field#^c25ae2]] and write it using the [[Feynman graphical notation#Feynman Propagator|Feynman propagator]] and [[Feynman graphical notation#Source|source integral]]: 
![[file:///C:/Users/Lucien/Documents/UNI/images/image139.png||200]]