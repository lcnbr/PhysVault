Let us compute the first few terms of $Z[J]$ in
a model with cubic and quartic interactions

$$
S_\text{int}[\Psi]
\simeq
-\frac{1}{6}\kappa \,\Psi^3
-\frac{1}{24}\lambda \,\Psi^4
$$

In a graphical notation we could represent this as^[[Feynman graphical notation#Functional derivative]]

![[file:///C:/Users/Lucien/Documents/UNI/images/image70.png||300]]

where we have made the dependence on the
coupling constants $\kappa$ and $\lambda$ explicit
as an explicit means of power counting.
In position space, both vertices represent the integral
$-\iunit\int \dd{x}$.
The [[graph generating functional with interaction#^e033d4|generating functional]] $Z[J]$ can be
expanded in powers of $S_\text{int}$

$$
Z[J]
=
\pqty{1
+\iunit S_\text{int}\bqty*{\frac{-\iunit\delta}{\delta J}}
-\frac{1}{2} S_\text{int}\bqty*{\frac{-\iunit\delta}{\delta J}}^2
+\ldots}
Z_0[J].
$$

In the following we will discuss the individual terms arising
from this expression.
Evidently, the first term is just the free generating functional $Z_0[J]$.

The second term with a cubic interaction has three functional derivatives
$-\iunit\delta/\delta J$ acting on $Z_0[J]$.
Let each of the derivatives act on

$$ \begin{align}
&
-\frac{\iunit}{6}\kappa\int \dd{w}\pqty{\frac{-\iunit\delta}{\delta J_w}}^3Z_0[J]
\\
&=
-\frac{\iunit}{6}\kappa\int \dd{w}\dd{x}\pqty{\frac{-\iunit\delta}{\delta J_w}}^2\pqty{ G_{wx}J_x Z_0[J]}
\\
&=
-\frac{\iunit}{6}\kappa\int \dd{w}\dd{x}\dd{y}\pqty{\frac{-\iunit\delta}{\delta J_w}}\pqty{ G_{wx}J_x G_{wy}J_y Z_0[J]}
\\&
-\frac{1}{6}\kappa\int \dd{w}\pqty{\frac{-\iunit\delta}{\delta J_w}}\pqty{ G_{ww}  Z_0[J]}
\\
&=
-\frac{\iunit}{6}\kappa\int \dd{w}\dd{x}\dd{y}\dd{z} G_{wx}J_x G_{wy}J_y G_{wz}J_z Z_0[J]
\\
&
-\frac{3}{6}\kappa\int \dd{w}\dd{x} G_{ww} G_{wx}J_x Z_0[J].
\end{align}$$



We can also perform the calculation using diagrams.
We already understand the free generating functional $Z_0[J]$.
It can be [[graph generating functional#In a free theory|viewed as a bag of arbitrarily many propagators]]

![[file:///C:/Users/Lucien/Documents/UNI/images/image89.png||400]]


For the second term,
draw a triangle vertex with three source derivatives in front of the bag.
Pick some ordering (1,2,3) for the derivatives
and let them act on the bag and pull propagators


The construction for a single quartic interaction vertex is similar,
there are just many more (intermediate terms)

$$ \begin{align}
&
-\frac{\iunit}{24}\lambda\int \dd{w}\pqty{\frac{-\iunit\delta}{\delta J_w}}^4Z_0[J]
\\
&=
-\frac{\iunit}{24}\lambda\int \dd{w}\dd{x}\dd{y}\dd{z}\dd{u} G_{wx}J_x G_{wy}J_y G_{wz}J_z G_{wu}J_u Z_0[J]
\\
&
-\frac{6}{24}\lambda\int \dd{w}\dd{x}\dd{y} G_{ww} G_{wx}J_x G_{wy}J_y Z_0[J]
\\
&
+\frac{3\iunit}{24}\lambda\int \dd{w} G_{ww} G_{ww} Z_0[J]
\end{align}$$

or graphically

![[file:///C:/Users/Lucien/Documents/UNI/images/image93.png||400]]
 

Let us finally consider two cubic vertices

$$
\frac{\iunit^2 \kappa^2}{2\cdot 6^2}
\int \dd{v}\dd{w}\pqty{\frac{-\iunit\delta}{\delta J_v}}^3
\pqty{\frac{-\iunit\delta}{\delta J_w}}^3Z_0[J].
$$

We can start with the single cubic vertex as intermediate result


![[file:///C:/Users/Lucien/Documents/UNI/images/image83.png||250]]
![[file:///C:/Users/Lucien/Documents/UNI/images/image81.png||400]]


 
