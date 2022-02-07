---
alias:
tag: GR physics
---

Recall the relations
$$
    A_\mu(x) = \varepsilon_\mu(x)e^{-\im k\cdot x}+\varepsilon\ind{\ast}{\mu}(x)e^{+\im k\cdot x},
$$

$$
    \left.\begin{array}{r}
        \Box^2 A_\mu =0 \\
        \partial_\mu A^\mu =0
    \end{array}\right\rbrace\rightarrow \begin{array}{r}
        k^2 =0\phantom{,}  \\
        k_\mu\varepsilon^\mu =0,
    \end{array}
$$

$$
\begin{split}
    A_\mu&\to A_\mu+\partial_\mu\phi, \\
    \phi(x) &= \im\varepsilon e^{+\im k\cdot x}-\im\varepsilon^\ast e^{-\im k\cdot x}.
\end{split}
$$
Then
$$
    A_\mu(x)\to A\ind{\prime}{\mu}(x)=\varepsilon\ind{\prime}{\mu}e^{\im k\cdot x}+\varepsilon\ind{\prime\ast}{\mu}e^{-\im k\cdot x},
$$
with
$$
    \varepsilon\ind{\prime}{\mu} = \varepsilon_\mu-\varepsilon k_\mu.
$$
For $k^\mu=k(1,0,0,1)$
$$
    \varepsilon_\mu k^\mu =0\ \Rightarrow\ \varepsilon^0-\varepsilon^3=0\ \Rightarrow\ \varepsilon_0=-\varepsilon_3.
$$
Also, by
$$
    \varepsilon_\mu\to\varepsilon\ind{\prime}{\mu}=\varepsilon_\mu-\varepsilon k_\mu,
$$
we get
$$
\begin{split}
    \varepsilon\ind{\prime}{0} &= \varepsilon_0 -\varepsilon k \\
    \varepsilon\ind{\prime}{3} &= \varepsilon_3 +\varepsilon k = -\varepsilon_0 + \varepsilon k \\
    \varepsilon\ind{\prime}{1} &= \varepsilon_1 \\
    \varepsilon\ind{\prime}{2} &= \varepsilon_2.
\end{split}
$$
Setting $\varepsilon=\frac{\varepsilon_0}{k}$ we get
$$
    \varepsilon\ind{\prime}{0}=0,\ \varepsilon\ind{\prime}{3}=0,
$$
and only $\varepsilon_1$ and $\varepsilon_2$ are physical.

Under a rotation
$$
    \varepsilon\ind{\prime}{\mu} = R\invind{\mu}{\nu}(\theta)\varepsilon_\nu = \begin{pmatrix}
    1 & 0 & 0 & 0 \\
    0 & \cos\theta & \sin\theta & 0 \\
    0 & -\sin\theta & \cos\theta & 0 \\
    0 & 0 & 0 & 0
    \end{pmatrix}\begin{pmatrix}
    \varepsilon_0 \\ \varepsilon_1 \\ \varepsilon_2 \\ \varepsilon_3
    \end{pmatrix} = \begin{pmatrix}
    \varepsilon_0 \\ \varepsilon_1\cos\theta+\varepsilon_2\sin\theta \\ -\varepsilon_1\sin\theta+\varepsilon_2\cos\theta \\ \varepsilon_3
    \end{pmatrix}.
$$
Thus 
$$
    \left.\begin{array}{r}
        \varepsilon\ind{\prime}{0}=\varepsilon_0 \\
        \varepsilon\ind{\prime}{1}=\varepsilon_1
    \end{array}\right\rbrace\rightarrow\ \text{scalar,}
$$
and with
$$
    \varepsilon_\pm = \frac{\varepsilon_1\mp\im\varepsilon_2}{2},\ \varepsilon_++\varepsilon_-=\varepsilon_1,\ \varepsilon_+-\varepsilon_-=\im\varepsilon_2,
$$
we have
$$
    \varepsilon\ind{\prime}{\pm}=\frac{\varepsilon\ind{\prime}{1}\mp\im\varepsilon\ind{\prime}{2}}{2}=e^{\pm\im\theta}\varepsilon_\pm,
$$
the only physical degrees of freedom have helicity $\pm1$.