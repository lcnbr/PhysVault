---
alias:
tags:
- qftII
---
Let us now compute $\expval{\Psi(x)\Psi(y)}$. We use [[graph generating functional#time-ordered two-point correlator]] and perform the two functional derivatives
^[There are two equivalent factors of $J$ in the exponent of $Z[J]$,
so the functional derivative acting on them produces a factor
of $2$ to be cancelled by the prefactor of $\frac{1}{2}$.]
$$\begin{align} & \frac{-\iunit \delta}{\delta J(y)}\frac{-\iunit \delta}{\delta J(x)} Z[J] \\ 
&= \frac{-\iunit \delta}{\delta J(y)} \int \dd[D]{z} G_\text{F}(x-z)\underbracket[1pt][3pt]{J(z)}_{1} \underbracket[1pt][3pt]{Z[J]}_{2} \\ 
&= \overbracket[1pt][3pt]{-\iunit G_\text{F}(x-y)Z[J] }^{1}\\ 
& +\overbracket[1pt][3pt]{\int \dd[D]{z} \dd[D]{z'{}} G_\text{F}(x-z)J(z) G_\text{F}(y-z')J(z') Z[J]}^{2} . \end{align}$$
Now divide by $Z[J]$ and set $J=0$ to obtain the correlator
$$
\expval{\phi(x)\phi(y)}=-\iunit G_\text{F}(x-y)
$$
This is precisely the expected result.

We can also perform the exercise with more than two fields.
The result agrees with [[Wick's theorem]].
In fact the form of $Z[J]$ as the exponent of $W[J]$
which is a quadratic monomial of $J$
can be viewed as the functional formulation of Wick's theorem:

- The first derivative knocks down a linear term $\delta W/\delta J$
from the quadratic exponent. In [[Feynman graphical notation]], using [[graph generating functional#In feynman graphical notation]]:    ![|500](file:///C:/Users/Lucien/Documents/UNI/images/image149.png) then 
![|500](file:///C:/Users/Lucien/Documents/UNI/images/image145.png)


- Subsequent derivatives can knock further linear terms $\delta W/\delta J$
from the exponent. They can also hit the remaining $J$ in some $\delta W/\delta J$
leaving behind a Feynman propagator $\delta^2W/\delta J^2\simeq-\iunit G_\text{F}(x_k-x_l)$. Again with [[Feynman graphical notation]]: ![|500](file:///C:/Users/Lucien/Documents/UNI/images/image142.png)
thus
![|500](file:///C:/Users/Lucien/Documents/UNI/images/image152.png)
- Any first derivative term $\delta W/\delta J$ that remains after the functional derivatives cause the expression to vanish when $J=0$.
- As every<mark style="background: #FF5582A6;"> exponent requires two functional derivatives, all fields $\phi(x_k)$ must be Wick contracted to some other field.</mark> 
- The product rule of derivatives takes care of the sum of all combinations.
- Setting $J=0$ in the end corresponds to the time-ordered correlator; it removes all non-trivial normal ordered terms.




