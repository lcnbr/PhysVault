---
alias:
tag: 
- ED
- qft
---
# Free real vector field
Consider a real [[vector fields in QFT|vector field]], since the complex case is a trivial extension. [[Field]]

The most general quadratic (s.t the [[equations of motion|e.o.m.s]] are that of a free particle) [[Lagrangian Density|lagrangian]] with no more than two derivatives is given by   ^[see ![[@colemanQUANTUMFIELDTHEORY2018#26 1 The free real vector field zotero open-pdf 0_4E7XKTS3 598]]]

$$\mathcal{L}=\pm \frac{1}{2}\left[\left(\partial_{\mu} A_{\nu}\right)\left(\partial^{\mu} A^{\nu}\right)+a\left(\partial_{\mu} A^{\mu}\right)\left(\partial_{\nu} A^{\nu}\right)+b A_{\nu} A^{\nu}\right]$$

The [[equations of motion|e.o.m.s]] are :
$$-\partial^{\mu} \partial_{\mu} A_{\nu}-a \partial_{\nu} \partial_{\mu} A^{\mu}+b A_{\nu}=0$$

For a plane wave ansatz ($A_{\nu}=\varepsilon_{\nu} e^{-i k \cdot x}$) this is:
$$
+k^{2} \varepsilon_{\nu}+a k_{\nu} \varepsilon \cdot k+b \varepsilon_{\nu}=0
$$
We could write this as a $4 \times 4$ matrix in $k$ acting on the vectors $\varepsilon_{\mu}$, and find the eigenvectors in the usual way. Instead, we'll just read them off. This equation has two kinds of solutions: longitudinal solutions, where $\varepsilon_{\mu}$ is aligned along $k_{\mu}$; and transverse solutions, with $\varepsilon_{\mu}$ perpendicular to $k_{\mu}$.
-  Longitudinal: $\varepsilon_{\nu} \propto k_{\nu}$.$$
\left[k^{2}+a k^{2}+b\right] k_{\nu}=0 ; \quad k^{2} \equiv \mu_{L}^{2}=-\frac{b}{1+a}
$$where $\mu_{L}$ is the mass of the longitudinal mode;
-  Transverse: $\varepsilon \cdot k=0$.$$
k^{2} \varepsilon_{\nu}+b \varepsilon_{\nu}=0 ; \quad k^{2} \equiv \mu_{T}^{2}=-b
$$where $\mu_{T}$ is the mass of the transverse mode.

Ideally we remove the longitudinal modes (only 1 deg of freedom -> scalar) thus  if, $a=-1$ and $b=-\mu^{2} \neq 0$, the Lagrangian becomes
$$
\mathcal{L}=\pm \frac{1}{2}\left[\left(\partial_{\mu} A_{\nu}\right)\left(\partial^{\mu} A^{\nu}\right)-\left(\partial_{\mu} A^{\mu}\right)\left(\partial_{\nu} A^{\nu}\right)-\mu^{2} A_{\nu} A^{\nu}\right]
$$
Remember: the middle term is equivalent to $-\left(\partial_{\mu} A_{\nu}\right)\left(\partial^{\nu} A^{\mu}\right)$, plus surface terms. This Lagrangian is so simple I can't resist introducing notation to make it look obscure. Define the field strength tensor
$$
F_{\mu \nu} \equiv \partial_{\mu} A_{\nu}-\partial_{\nu} A_{\mu}
$$
This is the convention in modern high energy physics literature. Then
$$
\mathcal{L}=\pm\left[\frac{1}{4} F_{\mu \nu} F^{\mu \nu}-\frac{1}{2} \mu^{2} A_{\nu} A^{\nu}\right]
$$

^freeVectLag

The [[equations of motion|e.o.m.]] then obtained is the [[Proca equation]]
To have massless scalars we can now take $\mu^2\rightarrow0$. This will be problematic when quantising in QED.