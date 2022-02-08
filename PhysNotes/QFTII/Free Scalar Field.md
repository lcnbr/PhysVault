# Free Scalar Field

The [[Lagrangian Density#Free scalar field|action]] with [[source term in the action|source]] term reads

$$
S_\text{free}[\phi]+S_\text{src}[\phi,j]=\int \dd[D]{x}\pqty{-\frac{1}{2} (\partial \phi)^2-\frac{1}{2} m^2 \phi^2+j\phi }.
$$

By partial integration we can make all the derivatives act on a single
field

$$
S_\text{free}[\phi]+S_\text{src}[\phi,j]=\int \dd[D]{x}\pqty{\frac{1}{2} \phi(\partial^2-m^2) \phi+\phi j }.
$$

This is a [[Gaussian integral]] which can be performed
by shifting the integration variable $\phi$.
A complication is that the kernel of the [[Gaussian integral|Gaußian function]] 
is the derivative operator $(-\partial^2+m^2)$,
and result of the integral depends on its inverse.
We have already determined its inverse in QFT I,
it is the propagator $G_\text{F}(x-y)$ satisfying
^[Due to the tilting of the time axis into the complex plane,
we have to choose the Feynman propagator.]

$$
(-\partial^2+m^2)G_\text{F}(x-y)=\delta^D(x-y).
$$

Hence we shift the field

$$
\phi(x)=\tilde\phi(x)+\int \dd[D]{y} G_\text{F}(x-y) j(y).
$$

and substitute it into the action
$$
\begin{align}
S_\text{free}[\phi]+S_\text{src}[\phi,j]
&=
\int \dd[D]{x}
\frac{1}{2} \tilde\phi(x)(\partial^2-m^2)\tilde\phi(x)
+W_0[j]
.
\\
W_0[j]
&=
\int \dd[D]{x}\dd[D]{y}\frac{1}{2} j(x) G_\text{F}(x-y) j(y)
.
\end{align}
$$

^c25ae2

As $\tilde \phi$ and $j$ are now well-separated,
we can perform the integral over $\tilde \phi$.
Moreover, the integration measure does not change $\mathcal{D}{\phi}=\mathcal{D}{\tilde\phi}$
when the integration variable is merely shifted.
Up to the overall constant $Z_0[0]$ we thus get

$$
Z_0[j]=Z_0[0]\exp\pqty{\iunit W_0[j]}.
$$

^2d84e1

A derivation in momentum space
is somewhat simpler because the Gaußian kernel is automatically diagonal.
The momentum-space version of $W_0[j]$ is
^[The factor of $\vfrac{1}{2}$ compensates the
double-counting of $|j(p)|=|j(-p)|$
for a real field $\phi^*(x)=\phi(x)$.]

$$
W_0[j]
=
\int \frac{\dd[D]{p}}{(2\pi)^D}\frac{\frac{1}{2}  j(p)j(-p)}{p^2+m^2-\iunit\epsilon}
=
\int \frac{\dd[D]{p}}{(2\pi)^D}\frac{\frac{1}{2}  \vqty{j(p)}^2}{p^2+m^2-\iunit\epsilon} .
$$

Formally, the prefactor reads
^[This statement is more or less tautological in QFT
since the determinant of an operator is commonly defined
via a Gaußian integral.
Here, $Z_0[0]$ is a constant (independent of the other fields)
and can therefore be ignored.]

$$
Z_0[0]\sim \frac{1}{\sqrt{\text{Det}\qty(-\partial^2+m^2-\iunit\epsilon)}}.
$$