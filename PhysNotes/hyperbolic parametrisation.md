---
aliases: 
tags: 
date created: Tuesday, May 10th 2022, 3:29:32 pm
date modified: Tuesday, May 10th 2022, 4:57:06 pm
---

A nice parametrisation to use when integrating over the [[Lorentz invariant measure]] is the following:
$$p^\mu = E(\cosh(\zeta),\sinh(\zeta)\hat{p}) \qqtext{where} \hat{p}=(\sin\theta\cos\phi,\sin \theta\sin\phi,\cos \theta)$$
with $\zeta$ running over $[0, \infty], \theta$ over $[0, \pi]$, and $\phi$ over $[0,2 \pi]$. Thus the measure  $\dd{\Phi(p)}$ can be written :[^1][^2]
            $$\dd{\Phi(p)}=\hat{\dd}E\,\hat{\dd}\zeta\,\hat{\dd}\theta\,\hat{\dd}\phi\,\hat{\delta}^{(+)}(E^2-m^2
            )E^{3} \sin(\theta) \sinh^{2}(\zeta)$$
and the integrating out the energy $E$ using [[delta function#^squares]] in combination with $\Theta(E)$ eliminates it and yields a factor of $\frac{1}{2m}$, and demands $E=m$ in the integrand:

$$\int f(p) \dd{\Phi(p)}=\frac{m^2}{2}\int\limits_0^\infty\hat{\dd}\zeta\,\sinh^{2}(\zeta)\int\limits_0^\pi \hat{\dd}\theta\,\sin(\theta)\int \limits_0^{2 \pi}\hat{\dd}\phi\,   \,f\pqty\big{m(\cosh(\zeta),\sinh(\zeta)\hat{p})}$$




[^1]: using sage:
    ```python
    E,z,t,ph=var('E,zeta,theta,phi')
    %display latex
    p=(E*cosh(z),E*sinh(z)*sin(t)*cos(ph),
    E*sinh(z)*sin(t)*sin(ph),E*sinh(z)*cos(t))
    jacobian(p, (E,z,t,ph)).determinant().simplify_full()
    ```
    
[^2]: note that $\hat{\dd{}}^{n}=\frac{\dd[4]}{(2 \pi)^n}$
