the action S, defined as a functional of the paths that can be followed, is an extremum^[[[zotero-843-Annotations#^266b73]]].  The condition that S be an extremum is specified by requiring $\delta S = 0$ ^[[[zotero-843-Annotations#^a3b30e]]]

# From least action to [[Euler-Lagrange equations]]

Varying the action and using the [[chain rule]]^[[[zotero-843-Annotations#^b26c54]]] for [[functional derivatives]]  we obtain

[$$\begin{align*}
\delta S &= \delta \int\limits_{t_{1}}^{t_{2}}\! L~ \mathrm{d}t \\
&=  \int\limits_{t_{1}}^{t_{2}}\! \delta L~ \mathrm{d}t\\
&= \int\limits_{t_{1}}^{t_{2}}\! \frac{\partial L}{\partial q_{i}}\delta q_{i}+\frac{\partial L}{\partial \dot{q_{i}}}\delta\dot{q_i}~ \mathrm{d}t\\
&= \int\limits_{t_{1}}^{t_{2}}\! \frac{\partial L}{\partial q_{i}}\delta q_{i}+\frac{\partial L}{\partial \dot{q_{i}}}\frac{d(\delta (q_{i}))}{d t}~ \mathrm{d}t
\end{align*}$$](zotero-843-Annotations#^8311af)

Here [[Einstein summation]] is used. Integrating by parts yields^[[zotero-843-Annotations#^5b3394]]:

[$$\delta S=   \int\limits_{t_{1}}^{t_{2}}\! 
\frac{\partial L}{\partial q_{i}}\delta q_{i}~\mathrm{d}t+
\left. 
\frac{\partial L}{\partial \dot{q_{i}}}\delta q_i\right|_{t_{1}}^{t_{2}} -\int\limits_{t_{1}}^{t_{2}}\! \frac{d}{d t}\left(\frac{\partial L}{\partial \dot{q_{i}}}\right) \delta q_i~\mathrm{d}t=0$$
](zotero-843-Annotations#^867192)^bb3857

$q_i(t_1)$ and $q_i (t_2)$ are fixed means that $\delta q_i = 0$ at the limits of integration, so the middle term is zero. Thus:

$$\delta S =  \int\limits_{t_{1}}^{t_{2}}\! 
\left[\frac{\partial L}{\partial q_{i}}-\frac{d}{d t}\left(\frac{\partial L}{\partial \dot{q_{i}}}\right)\right] \delta q_{i}~\mathrm{d}t=0 \quad \forall \delta q_{i}\implies\boxed{\frac{\partial L}{\partial q_{i}}-\frac{d}{d t}\left(\frac{\partial L}{\partial \dot{q_{i}}}\right)=0}$$

The boxed part are the [[Euler-Lagrange equations]] for [[Classical Particle Mechanics]].

If instead we were using a [[Lagrangian Density]] then [[principle of least action#^bb3857|this equation]] would become:
[$$\delta S  = \int\limits_{\Omega}\! 
\left[\frac{\partial \mathcal{L}}{\partial \phi}-\frac{\partial}{\partial q^\mu}\left(\frac{\partial \mathcal{L}}{\partial \phi_{,\mu}}\right)\right] \delta \phi~\mathrm{d^4}q+\int\limits_{\Omega}\! 
\frac{\partial}{\partial q^\mu}\left[\frac{\partial \mathcal{L}}{\partial \phi_{,\mu}}\delta \phi \right]~\mathrm{d^4}q=0 $$](zotero-843-Annotations#^d3367a)

The last term is the integral of a 4-d divergence over a 4-d volume, which becomes a surface integral (gauss' thm) over a vanishing boundary, thus once again we obtain:


[$$\delta S  =  \int\limits_{\Omega}\! 
\left[\frac{\partial \mathcal{L}}{\partial \phi}-\frac{\partial}{\partial q^\mu}\left(\frac{\partial \mathcal{L}}{\partial \phi_{,\mu}}\right)\right] \delta \phi~\mathrm{d^4}q =0\quad \forall \delta q_{i}\implies\boxed{\frac{\partial \mathcal{L}}{\partial \phi}-\frac{\partial}{\partial q^\mu}\left(\frac{\partial \mathcal{L}}{\partial \phi_{,\mu}}\right)=0}$$](zotero-843-Annotations#^caea84)

The boxed part are the [[Euler-Lagrange equations]] for [[Classical Field Theory]].
# Further to the [[Hamiltonian]] formalism
By defining [[Conjugate momenta]] and performing a [[Legendre transform]] we obtain

 