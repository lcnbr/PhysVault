
---
alias:
- tree functional
- tree generating functional
---
There is a generating functional for
the leading classical contributions.
This turns out to generate precisely the tree graphs,
i.e. those without momentum loops.

The leading classical contributions are the most relevant
contributions when $\hbar$ is very small.
The quantum constant appears as the inverse $\hbar^{-1}$
    in the prefactor to the action in the exponent (c.f. [[loop counting#^bd49ba]]).
In the path integral this causes a strongly oscillating integrand.
All contributions cancel out almost perfectly
unless the exponent is *stationary*

$$
\frac{\delta S[\Psi]}{\delta \Psi(x)}
+
\frac{\delta S_\text{src}[\Psi,J]}{\delta \Psi(x)}=
\frac{\delta S[\Psi]}{\delta \Psi(x)}
+
J(x)=0.
$$

Let us assume that there is a single stationary contribution
for each source field configuration $J$
^[At least formally and perturbatively we can make this assumption.]
which we shall denote by $\Psi=\Psi[J]$.
At small $\hbar$ the path integral is dominated by
this contribution (up to some irrelevant prefactor)

$$
Z[J]
\approx \exp\pqty{\iunit \hbar^{-1}T[J]},
$$

where we have introduced the functional $T[J]$ for the leading contribution to the exponent

$$
T[J]:=S[\Psi[J]]+\int \dd[D]{x} J(x) \,\Psi[J](x).
$$

What can we say about $T[J]$?

# Generates trees

First of all $T[J]$ is defined as the leading classical contribution to $W[J]$.$$
T[J]=\lim_{\hbar\to 0} W[J].
$$As such $T[J]$ generates a subclass of the connected graphs.

 Furthermore, we have learned that the contributions to $Z[J]$
depend on $\hbar$ as $\hbar^{L-N}$ (c.f. [[loop counting]]).
For connected graphs we have $N=1$,
and therefore the graphs in $W[J]$ scale as $\hbar^L$.
The limit $\hbar\to 0$ then restricts to graph with $L=0$,
i.e. the graphs in $T[J]$ have no momentum loops.

Therefore $T[J]$ generates precisely the
*subclass of connected tree graphs* within $Z[J]$ or $W[J]$.

# Is the legendre transform

Another important observation is that
$T[J]$ formally is the [[Legendre transform|Legendre transformation]] of the action $S[\Psi]$, since 
The source $J$ is defined as the functional derivative of $S[\Psi]$ (c.f. [[graph generating functional with interaction]])

$$
J(x)=-\frac{\delta S[\Psi]}{\delta \Psi(x)}.
$$

Moreover, $T[J]$ equals $S[\Psi]$ plus a term $J\cdot\Psi$ evaluated
at the inverse $\Psi=\Psi[J]$ of the above relation:

$$T[J]:=S[\Psi[J]]- \int\dd[D]{x} J(x) \Psi[J(x)]$$

Putting the above insights together,
we conclude that the Legendre transformation of
some generating functional $S[\Psi]$
is a functional $T[J]$ which generates connected trees
from the lines and vertices encoded by $S_0[\Psi]$ and $S_\text{int}[\Psi]$, respectively

 ![|400](file:///C:/Users/Lucien/Documents/UNI/images/image1.png)

# Example
Let us consider this transformation explicitly
for the example of a theory with a cubic interaction

![|300](file:///C:/Users/Lucien/Documents/UNI/images/image170.png)

The source field $J$ is then defined in terms of the field $\Psi$
 ![|300](file:///C:/Users/Lucien/Documents/UNI/images/image171.png)

We need to find the inverse functional $\Psi[J]$


 ![|450](file:///C:/Users/Lucien/Documents/UNI/images/image169.png)


One can confirm by substitution that these two functions are mutually inverse
by using the graphical relationship

![[Pasted image 20220125183156.png|250]]

We obtain

![[Pasted image 20220125190307.png|450]]

Now substitute $\Psi[J]$ into the two terms of the action $S[\Psi]$
and the Legendre transformation term $S_\text{src}[\Psi,J]$


 ![|400](file:///C:/Users/Lucien/Documents/UNI/images/image167.png) 
 ![|400](file:///C:/Users/Lucien/Documents/UNI/images/image168.png)

The sum of these terms yields the Legendre transform

 ![|400](file:///C:/Users/Lucien/Documents/UNI/images/image160.png)

 The various prefactors in the above conspire to yield the canonical symmetry factors of the tree graphs