---
alias: 
tag: GR physics
---

For a system with an energy-momentum tensor $T_{\mu\nu}$ the metric
$$
    g_{\mu\nu} = \eta_{\mu\nu} + h_{\mu\nu},
$$
in the weak field approximation is given by

![[solutions of the linearized field equations#^solInhomt]]

where

$$
    S_{\mu\nu}=T_{\mu\nu}-\frac{\eta_{\mu\nu}}{2}T\ind{\alpha}{\alpha}.
$$

^source

![[Pasted image 20220207134723.png#leftwrap|240]]We will restrict our study to "sources" $S_{\mu\nu}(\x^{\,\prime},t^\prime)$ which are localized to confined regions $|\x^{\,\prime}|\leq R$ and calculate the metric $h_{\mu\nu}(\x,t)$ at distances $|\x|\equiv r\gg R$.


Under these approximations we have
$$
\begin{split}
    |\x-\x^{\,\prime}| &= r\left(1-2\hat{x}\cdot\x^{\,\prime}+\frac{\x^{\,\prime2}}{r^2}\right)^{1/2} \\
    |\x-\x^{\,\prime}| &\approx r\left(1-\frac{\hat{x}\cdot\x^{\,\prime}}{r}\right)+\mathcal{O}\left(\frac{R^2}{r}\right).
\end{split}
$$
We can analyze the source $S_{\mu\nu}(\x,t)$ in Fourier space
$$
    S_{\mu\nu}(\x,t) = \int_0^\infty\dd{\omega}e^{-\im\omega t}S_{\mu\nu}(\x,\omega) + c.c.,
$$
where the $c.c.$ stands for the complex conjugate. Then the metric becomes 
$$
\begin{split}
    h_{\mu\nu}(\x,t) &= 4G\int_0^\infty\dd{\omega}\int\dd[3]{x'}\frac{S_{\mu\nu}(\x^{\,\prime},\omega)e^{-\im\omega(t-|\x-\x^{\,\prime}|)}}{|\x-\x^{\,\prime}|} +c.c. \\
    &= 4G\int_0^\infty\dd{\omega}\int\dd[3]{x'}\frac{S_{\mu\nu}(\x^{\,\prime},\omega)}{r}e^{-\im\left[\omega(t-r+\x^{\,\prime}\cdot\hat{x})+\mathcal{O}(\frac{\omega R^2}{r})\right]} + c.c. +\mathcal{O}\left(\frac{R}{r}\right) \\
    &\approx \int_0^\infty\dd{\omega}e^{-\im\omega(t-r)}\left[\frac{4G}{r}\int\dd[3]{x'}S_{\mu\nu}(\x^{\,\prime},\omega)e^{-\im\omega\hat{x}\cdot\x^{\,\prime}}\right] +c.c.
\end{split}
$$
In the above we make the assumptions that

-  $\omega r$ is substantial, i.e. $r\gg\frac{1}{\omega}$ (long wavelengths do not dominate),
-  $\frac{\omega R^2}{r}$ is small,
 -  $r\gg R$.

Combined we constrain our calculation to distances
$$
    r\gg\max\lbrace R,\omega R^2,\frac{1}{\omega}\rbrace.
$$
Let us define the wave vector
$$
    \vec{k}(\omega) \equiv\omega\hat{x}.
$$
Then $\omega r $
$$
\begin{split}
    h_{\mu\nu}&\approx\int_0^\infty\dd{\omega}e^{-\im(\omega t-\vec{k}\cdot\x)}\int\dd[3]{x'}S_{\mu\nu}(\x^{\,\prime},\omega)e^{-\im\x^{\,\prime}\cdot\vec{k}}\frac{4G}{r}+c.c. \\
    \Rightarrow\ h_{\mu\nu}&\approx\int_0^\infty\dd{\omega}e^{-\im(\omega t-\vec{k}\cdot\x)}\varepsilon_{\mu\nu}(\omega,\vec{k}) + c.c.,
\end{split}

$$
with the polarization tensor
$$
    \varepsilon_{\mu\nu}(\omega,\x)\equiv \frac{4G}{r}S_{\mu\nu}(\omega,\vec{k}),
$$
and
$$
    S_{\mu\nu}(\omega,\vec{k})=\int\dd[3]{x'}e^{-\im\vec{k}\cdot\x}S_{\mu\nu}(\omega,\x^{\,\prime}).
$$
We have found that at large distances the metric takes the form of superposition of (spherical, $\hat{k}=\hat{x}$) plane waves with a polarization tensor given by the above. We can now compute the energy-momentum tensor carried by the wave. We have carried out this computation assuming a monochromatic wave. However, in \eqref{eq:metric waves} we find a superposition of frequencies. The calculation of the energy-momentum tensor will then have additional "interference" terms of the form
$$
\begin{split}
    \frac{\partial h_{\alpha\beta}}{\partial h^\gamma}\frac{\partial h_{\mu\nu}}{\partial x^\rho} \to  \iint_0^\infty\dd{\omega}\dd{\omega}^\prime\,k_\gamma k\ind{\prime}{\rho}&\left[\varepsilon_{\alpha\beta}(k)e^{-\im(\omega t-\vec{k}\cdot\x)}-\varepsilon\ind{\ast}{\alpha\beta}(k)e^{+\im(\omega t-\vec{k}\cdot\x)}\right]\times \\
    &\left[\varepsilon_{\mu\nu}(k^\prime)e^{-\im(\omega^\prime t-\vec{k}^\prime\cdot\x)}-\varepsilon\ind{\ast}{\mu\nu}(k^\prime)e^{+\im(\omega^\prime t-\vec{k}^\prime\cdot\x)}\right].
\end{split}
$$
Integrating over time
$$
    \int\dd{t}\frac{\partial h_{\alpha\beta}}{\partial h^\gamma}\frac{\partial h_{\mu\nu}}{\partial x^\rho},
$$
results the following time integrals
$$
\begin{split}
    \int_{-\infty}^{+\infty}\dd{t}e^{\pm\im(\omega+\omega\prime)t}&=2\pi\delta(\omega+\omega^\prime) =0,\\
    \int_{-\infty}^{+\infty}\dd{t}e^{\pm\im(\omega-\omega\prime)t}&=2\pi\delta(\omega-\omega^\prime),
\end{split}
$$
which eliminates all contributions from $\omega\neq\omega^\prime$. Therefore, our result for the time averaged energy momentum tensor can be used here without worrying about interference of different frequencies
$$
    \int_{-\infty}^{+\infty}\dd{t}t^{\mu\nu} = \int_0^\infty\dd{\omega}\frac{k^\mu k^\nu}{16\pi G}\left(\varepsilon^{\ast\alpha\beta}\varepsilon_{\alpha\beta}-\frac{1}{2}\left|\varepsilon\ind{\alpha}{\alpha}\right|^2\right).
$$
We can now calculate the radiated energy
$$
    E = \int\dd{t}\frac{\diff E}{\diff t} = -\int\dd{S}n_it^{0i} = \int\dd{\omega}r^2(\hat{x}^it^{0i}).
$$
Written in differential form
$$
\begin{split}
    \frac{\diff E}{\dd{\omega}} &= r^2(\hat{x}^it^{0i})=\cdots \\ 
    &= 2G\int_0^\infty\dd{\omega}\omega^2\left[T^{\ast\mu\nu}(\vec{k},\omega)T_{\mu\nu}(\vec{k},\omega)-\frac{1}{2}\left|T\ind{\mu}{\mu}(\vec{k},\omega)\right|^2\right],
\end{split}
$$
where
$$
    T_{\mu\nu}(\vec{k},\omega)\equiv\int\dd[3]{x'}e^{-\im\vec{k}\cdot\x^\prime}T_{\mu\nu}(\x^\prime,\omega),
$$
and
$$
    T_{\mu\nu}(\x,t) = \int_0^\infty\dd{\omega}\left[e^{-\im\omega t}T_{\mu\nu}(\x,\omega)+e^{+\im\omega t}T\ind{\ast}{\mu\nu}(\x,\omega)\right].
$$

\underline{Application}

Consider $n$ particles moving with velocities $\v_n$ and carrying four-momenta $P^\mu_n\equiv(E_n,E_n\v_n)$ at times $t<0$ before they collide at $t=0$. After the collision the particles will have momenta $\Bar{P}^\mu_n\equiv(\Bar{E}_n,\Bar{E}_n\Bar{\v}_n)$. Due to momentum conservation we have
$$
    \sum_n(P_n-\Bar{P}_n)=0.
$$
The energy-momentum tensor is
$$
    T^{\mu\nu}(\x,t) = \sum_n\frac{P^\mu_nP^\nu_n}{E_n}\delta^{(3)}(\x-\v_nt)\Theta(-t) + \sum_n\frac{\Bar{P}^\mu_n\bar{P}^\nu_n}{\Bar{E}_n}\delta^{(3)}(\x-\bar{\v}_nt)\Theta(t).
$$
We can now employ the following representation of the $\Theta$-function
$$
    \Theta(x) = \lim_{\varepsilon\to0^+}\frac{1}{2\pi\im}\int_{-\infty}^{+\infty}\dd{\omega}\frac{e^{+\im\omega x}}{\omega-\im\varepsilon}.
$$
and the $\delta$-function
$$
    \delta^{(3)}(\x)=\int\frac{\diff^3k}{(2\pi)^3}e^{+\im\vec{k}\cdot\x}.
$$
Then
\begin{align}
    T^{\mu\nu}(\x,t) &= \int\frac{\dd{\omega}\diff^3k}{(2\pi)^4\im}\left[\sum_n\frac{P^\mu_nP^\nu_n}{E_n}e^{+\im\vec{k}\cdot(\x-\v_nt)}\frac{e^{+\im\omega(-t)}}{\omega-\im\varepsilon}-\sum_n\frac{\bar{P}^\mu_n\bar{P}^\nu_n}{\bar{E}_n}e^{+\im\vec{k}\cdot(\x-\bar{\v}_nt)}\frac{e^{-\im\omega t}}{\omega+\im\varepsilon}\right] \notag \\
    &= \int\frac{\dd{\omega}\diff^3k}{(2\pi)^4\im}\left[\sum_n\frac{P^\mu_nP^\nu_n}{E_n}\frac{e^{-\im[(\omega+\vec{k}\cdot\v_n)t-\vec{k}\cdot\x]}}{\omega-\im\varepsilon}-\sum_n\frac{\bar{P}^\mu_n\bar{P}^\nu_n}{\bar{E}_n}\frac{e^{-\im[(\omega+\bar{\v}_n\cdot\vec{k})t-\vec{k}\cdot\x]}}{\omega+\im\varepsilon}\right] \\
    &= \int\frac{\diff^3k}{(2\pi)^4}e^{+\im\vec{k}\cdot\x}\int_{-\infty}^{+\infty}\frac{\dd{\omega}}{\im}\left[\sum_n\frac{P^\mu_nP^\nu_n}{E_n}\frac{1}{\omega-\vec{k}\cdot\v_n-\im\varepsilon}-\sum_n\frac{\bar{P}^\mu_n\bar{P}^\nu_n}{\bar{E}_n}\frac{1}{\omega-\vec{k}\cdot\bar{\v}_n+\im\varepsilon}\right]e^{-\im\omega t}.\notag
\end{align}
We have that
$$
    T^{\mu\nu}(\vec{k},\omega) = \frac{1}{2\pi\im}\sum_n\frac{P^\mu_nP^\nu_n}{E_n(\omega-\vec{k}\cdot\v_n-\im\varepsilon)}-\frac{1}{2\pi\im}\sum_n\frac{\bar{P}^\mu_n\bar{P}^\nu_n}{\bar{E}_n(\omega-\vec{k}\cdot\bar{\v}_n+\im\varepsilon)}.
$$
Then, indeed,
$$
\begin{split}
    T^{\mu\nu}(\x,t) &= \int\frac{\diff^3k}{(2\pi)^3}e^{+\im\vec{k}\cdot\x}\int_{-\infty}^{+\infty}\dd{\omega}e^{\im\omega t}T^{\mu\nu}(\vec{k},\omega) \\
    &= \int\frac{\diff^3k}{(2\pi)^3}e^{+\im\vec{k}\cdot\x}\int_{0}^{+\infty}\dd{\omega}\left[e^{\im\omega t}T^{\mu\nu}(\vec{k},\omega)+e^{-\im\omega t}T^{\mu\nu}(\vec{k},-\omega)\right] \\
    &= \int_0^\infty\dd{\omega}\left[e^{+\im\omega t}\int\dd[3]{k}T^{\mu\nu}(\vec{k},\omega)e^{+\im\vec{k}\cdot\x} + e^{-\im\omega t}\int\dd[3]{k}T^{\mu\nu}(-\vec{k},-\omega)e^{-\im\vec{k}\cdot\x}\right] \\
    &= \int_0^\infty\dd{\omega}\left[e^{\im\omega t}T^{\mu\nu}(\x,\omega)+c.c.\right].
\end{split}
$$
Notice also that
$$
    P_n\cdot k = E_n\omega-\vec{k}\cdot E_n\v_n = E_n(\omega-\vec{k}\cdot\v_n),
$$
where we used $k^\mu = (\omega,\vec{k})$.
Thus
$$
    T^{\mu\nu}(\vec{k},\omega) = \frac{1}{2\pi\im}\sum_n\frac{P^\mu_nP^\nu_n}{P_n\cdot k-\im\varepsilon}-\frac{1}{2\pi\im}\sum_n\frac{\bar{P}^\mu_n\bar{P}^\nu_n}{\bar{P}_n\cdot k+\im\varepsilon}.
$$
We also notice that 
$$
    P_n\cdot k=E_n\omega(1-\v_n\cdot\hat{x}) = E\omega(1-v_n\cos\theta),
$$
never vanishes for massive particles. We can then drop the $\pm\im\varepsilon$ in the denominators. We can further compactify the expression as 
$$
    T^{\mu\nu}(\vec{k},\omega) = \frac{1}{2\pi\im}\sum_N\eta_N\frac{P^\mu_NP^\nu_N}{P_N\cdot k},
$$
where $N$ runs over the particles of both the initial and final state and 
$$
    \eta_N = \left\lbrace\begin{array}{ll}
        +1 & \text{initial state,} \\
        -1 & \text{final state.}
    \end{array}\right.
$$
Finally,
$$
\begin{split}
    T^{\mu\nu}T_{\mu\nu} &= \frac{1}{(2\pi)^2}\sum_{N,M}\eta_N\eta_M P^\mu_NP^\nu_NP_{M\mu}P_{M\nu}\frac{1}{(P_N\cdot k)(P_M\cdot k)} \\
    &= \sum_{N,M}\frac{\eta_N\eta_M}{(2\pi)^2}\frac{(P_N\cdot P_M)^2}{(P_n\cdot k)(P_M\cdot k)},
\end{split}
$$
and
$$
    \left|T\ind{\mu}{\mu}\right|^2 = \frac{1}{(2\pi)^2}\sum_{N,M}\frac{P_N^2P_M^2}{(P_N\cdot k)(P_M\cdot k)}.
$$
So, the total energy flux per solid angle is
$$
    \frac{\diff E}{\dd{\omega}} = \int\dd{\omega}\frac{G\omega^2}{2\pi^2}\sum_{N,M}\eta_N\eta_M\frac{(P_N\cdot P_M)^2-\frac{1}{2}m_N^2m_M^2}{(P_N\cdot k)(P_M\cdot k)}.
\label{eq:energy per solid angle}
$$

\underline{Observations}:

     - 1)] If $\bar{P}_n = P_n$ then $T_{\mu\nu}(\vec{k},\omega) =0$ and there is no radiation $\frac{\diff E}{\dd{\omega}}=0$.
    To produce gravitational radiation a particle needs to change momentum (be accelerated). This is also the case in electromagnetism, where radiation is produced by accelerated charges.
     - 2)] For massless particles $v_n=1$ and $P_N\cdot k=E_n\omega(1-\cos\theta)$. For $\theta=0$ this vanishes and seems to create a singularity in our expression for the energy. But this turns out to be a fake singularity. 
    
    \begin{minipage}{.45\textwidth}
    \begin{tikzpicture}
        \draw[gray,thick,->] (0,0) --  (5,0) node[right] {$P_M$};
        \draw[darkgray,thick,->] (0,0) -- (50:5) node[right] {$k$};
        \draw[thick,->] (0,0) --  (45:4) node[right] {$P_N$};
        \draw[dashed] (50:3.68) -- (45:4);
        \draw[dashed] (45:4) -- (.44,0);
        \draw[gray,thick,decoration={brace,mirror,raise=4pt},decorate] (0,0) -- node[below=6pt] {$\beta$} (.44,0);
        \draw[darkgray,thick,decoration={brace,raise=4pt},decorate] (0,0) -- node[above left=3pt] {$x$} (50:3.68);
        \node[lightgray] at(0,0) {$\odot$};
        \node[lightgray] at(-.35,-.27) {$P_N^\perp$};
    \end{tikzpicture}
    \end{minipage}\hfill
    \begin{minipage}{.49\textwidth}
    When we approach $P_N\parallel k$ we can write
$$
        P_N = \underbrace{x}_{\mathclap{\mathrm{large}}}k+\underbrace{\beta}_{\mathclap{\mathrm{small}}}P_M+\underbrace{P_N^\perp}_{\mathclap{\mathrm{small}}},
    $$
    and $P_N\cdot k=x\cancelto{0}{k^2}+\beta P_M\cdot k+\cancelto{0}{P_N^\perp\cdot k}$.
    \end{minipage}
    
    Then
$$
        \frac{P_N\cdot P_M}{P_N\cdot k} = \frac{P_M\cdot P_N}{\beta P_M\cdot P_N}=\frac{1}{\beta}\sim large,
    $$
    However, in the sum this singularity vanishes. From $P_N\approx xk$ we get $P_N\cdot P_M\approx xP_M\cdot k\ \Rightarrow\ x = \frac{P_N\cdot P_M}{P_M\cdot k}$ and
$$
    \begin{split}
        \sum_{N,M}\eta_N\eta_M\frac{(P_N\cdot P_M)^2}{(P_N\cdot k)(P_M\cdot k)}&\approx \sum_{N,M}\eta_N\eta_Mx\frac{P_N\cdot P_M}{P_N\cdot k} \\
        &= \sum_N\frac{\eta_N x}{P_N\cdot k}\underbrace{\left(\sum_M\eta_MP_M\right)}_{=0}\cdot P_N.
    \end{split}
    $$
    Above, due to momentum conservation the inner sum is zero and thus the singularity vanishes.
     - 3)] In \eqref{eq:energy per solid angle}, by substituting $\vec{k}=\hat{x}\omega$, we find
$$
    \begin{split}
        \frac{\diff E}{\dd{\omega}} &= \int_0^\infty\dd{\omega}\frac{G}{2\pi^2}\sum_{N,M}\eta_N\eta_M\frac{(P_NP_M)^2-\frac{1}{2}m_N^2m_M^2}{E_NE_M(1-\v_N\cdot\x)(1-\v_M\cdot\x)}\\
        \Rightarrow \frac{\diff E}{\dd{\omega}} &\propto \int_0^\infty\dd{\omega},
    \end{split}
    $$
    which is divergent. This divergence is removed if we assume that the collision does not happen instantaneously at $t=0$, but a finite interval $\Delta t$ is required for the transitioning from the initial to the final state. The behaviour of the integral is $\frac{\diff E}{\dd{\omega}}\propto\int_0^{1/\Delta t}\dd{\omega}$.
