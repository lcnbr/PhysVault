$1.1$ ![[topological n-manifold]]
1.1.1. Normal-
1.1.2. Metrizable -
1.1.3.![[Paracompact]]
1.1.4. Locally connected $-\forall x \in E$ and $\forall V$ open nhood of $x, \exists U$ open and connected s.t. $x \in U c V$
1.1.5. Locally compact - $\forall x \in E, \exists U$ open nhood of $x$ with $\bar{U}$ compact.
1.2. A coord. chart or coord nhood about $x \in E$ is a poir $(U, \varphi)$ where $U$ is an open nhood of $x$ and $\varphi: U \rightarrow \varphi(U)$ is a homeomorphism onto an open ball of $\mathbb{R}^{n}$.
1.2.1 To $x \in U$, we assign the local coordinates of $\varphi(x)$ in $\varphi(0) \subseteq \mathbb{R}^{n} \varphi(x)=\left(x^{4}(x), \ldots, x^{n}(x)\right)$
1.2.2 Transition fonctions: Let $(U, \varphi) \$(V, \Psi)$ be coord charts with $x \in U \cap V$ then: and $(U, \psi)$ are $C^{\infty}$-compatible if $U_{n} V \neq \varnothing$ implies:
1.3. $C^{\infty}$-compatiole- Let $M$ be a fopological n-manifold, the coordinate nhoods $(0, \varphi)$ and $(V, \psi)$ are conpatiole if $U_{n} V \neq \varnothing$ implies:
$$
\begin{aligned}
&\psi_{\circ} \varphi^{-1}: \varphi(U \cap V) \rightarrow \psi(U \cap V) \text { is } c^{\infty} \text { and } \\
&\varphi_{\circ} \psi^{-1}: \psi(U \cap V) \rightarrow \varphi(U \cap V) \text { is } c^{\infty}
\end{aligned}
$$
$1.4 C^{\infty}$-structure - on a topological n-menifold $M$ is a family $M=\left\{\left(U_{a}, \varphi_{a}\right) \mid \alpha \in A\right\}$ of coordinate nhoods such that:
$\left.\begin{array}{l}\text { i) } U_{\alpha \in A} U_{\alpha}=M \\ \text { ii) } \forall \alpha, B \in A,\left(U_{\alpha}, \varphi_{\alpha}\right) \text { and }\left(U_{B}, \varphi_{B}\right) \text { are } C^{\infty} \text {-compatible }\end{array}\right\}$ atlas $M$
iii) If $(v, \psi)$ is $c^{\infty}$-compatiole with everg $\left(u_{\alpha}, \psi_{\alpha}\right) \in \mathcal{U}$, then $(v, \psi) \in \mathbb{U}$
1.5 $C^{\infty}$-manifold - is a topological $n$-manifold enelowed with a $C^{\infty}$ structure 1.5.1 Open submonifold - the manifold obtained by creating atlas $N$ on an open subset U of the mfold $M$, with coord. nhoods. : $\left(U \cap V,\left.\psi\right|_{U n}\right)$ where $(V, \psi)$ is a chart on $M$ 1.5.2 Product manifold- If $M$ is a $C^{\infty}-n$-mfold and $N$ is a $C^{\infty}-m-m f_{0} l d$ then $M \times N$ is a $C^{\infty}-(m+n)-m f_{0} 1 d$ with coord nhoods $\left(U \times V, \varphi_{x} \psi\right)$ for $(U, \varphi) \in M$ and $(V, \psi) \in \mathcal{N}$, where $\left(\varphi_{x} \psi\right)(x, y)=(\varphi(x), \varphi(y)) \in \varphi(u) \times \varphi(V) \subseteq \mathbb{R}^{n+m}$
$2.0$ Projection- Let $E$ be a topological space and $\sim$ be an equivalence relation on $E$. We denote the projection by: $\pi: E \rightarrow E / \sim \quad x \mapsto[x]$
$2.1$ Quoffent topology - on $E / \sim$ is defined by $U c E / v$ is open $\Leftrightarrow \pi^{-1}(U)$ is opon in $E$ $2.2$ Cone - Given a sobset $A C E$, we define $C(A) \subset E$ as $C(A)=\pi^{-1}(\pi(A))$ the cone over $A$. In other words, $C(A)$ is the set of ekments of $E$ equivalent to elements of $A$. $2.3$ Open- An equivalence relation $\sim$ on a top. space $E$ is said to be open if AcE open implies $C(A) C E$ open.

2.3.1 Real projective space $-\mathbb{P}_{n}$ is the n-dim projetive space: let $\left.E=\mathbb{R}^{n+1} \backslash \varepsilon_{0}\right\}$ and $\sim$ the equivalence relation on $E$ defined by $\vec{x} \sim \vec{y} \Leftrightarrow \exists t \in \mathbb{R}^{*}$ st. $\vec{y}=t \bar{x}$ then $\mathbb{P}_{n}=E / \sim=$ the set of lines through $\vec{O}$ in $\mathbb{R}^{n+1}$ with $\vec{O}$ removed.
$2.3 .2 G_{\text {rassmann }} m f_{\text {old }}-G(k, n)$, consider $F(k, n)=\{$ ordered $k+$ tuples of lin. indep. vectors in $\mathbb{R}^{n} \xi=\left\{k\right.$-frames in $\left.\mathbb{R}^{n}\right\}$. K-frame is repesented by: $\left(\vec{x}_{1} \cdots \vec{x}_{k}\right)^{\top}=(\quad)=\chi$ a metrix of renk $K$. Detine $\sim$ by $X \sim Y \Leftrightarrow Y=A X$ for $A \in G L(k, \vec{R})$ and $G(k, n)=F(k, n) / \sim$
$\underline{3.1 C^{\infty}}-A$ map $f: W_{f} C M \rightarrow \mathbb{R}\left(W_{f}\right.$ openin $\left.M\right)$ is $C^{\infty}$ if $\forall x \in W_{f}$ and $\forall$ charts $(U, \varphi)$ s.t. $x \in U$ the map $f \circ \varphi^{-1}: \varphi\left(U \cap \omega_{f}\right) \subset \mathbb{R}^{n} \rightarrow \mathbb{R}$ is $C^{\infty}$![[Pasted image 20220122103058.png]]
$\underline{3.2 C^{\infty}}-A$ map $f: M \rightarrow N$ is $c^{\infty}$ if $\forall x \in M, \exists$ coordinate neighbors $(U, \varphi) d(V, \psi)$ with $x \in U$ and $f(x) \in V$ on $M$ and $N$ resp. (Assume wolG $f(U) \subset V$ ) s.t. $\psi \circ f \circ \varphi^{-1}, \varphi(U) \subseteq \mathbb{R}^{n} \rightarrow \psi(V) \subseteq \mathbb{R}^{m} \quad(n=\operatorname{dim} N, m=\operatorname{dim} M)$ is a $c^{\infty} \operatorname{map}$ of evelidean spaces.![[Pasted image 20220122103114.png]]
$\underline{3.3 R_{\text {ank }}}$ - the rank of $f$ at $x:(r k f)_{x}=r k\left(\left.\frac{\partial y^{i}}{\partial x_{i}}\right|_{\varphi(x)}\right)$

$4.0 .1$ Germ - Let $M$ be a $C^{\infty}$ manifold, $x \in M$ and fig, be $C^{\infty}$ functions, $\mathbb{R}$-valued, defined in a nhood of $x$. We say frg if $\exists U$ open nhood of $x$ s.t. $f(y)=g(y)$ \forallyeU [f] is called germ of $f$ at $x$
$4.0 .2$ Algebra of gems - denote by $C^{\infty}(M,\{x\}, \mathbb{R})$ the real algebra of germs of $C^{\infty}$ - function at $x$.
$\underline{4.1}$ Tangent vector - at $x \in M$ is a map $X_{x}: c^{\infty}(M,\{x\}, \mathbb{R}) \rightarrow \mathbb{R}$ s.t if $(U, \varphi)$ is
a chart about $x \in M$ with coord $\left(x^{1}, \ldots, x^{n}\right), \exists\left(a^{1}, \ldots, a^{9}\right) \in \mathbb{R}^{n}$,
$$
X_{x}([f])=\left.\sum_{i=1}^{n} a^{i} \frac{\partial}{\partial x^{i}}\right|_{\varphi(x)}\left(f \circ \varphi^{-1}\right) \underset{\mathbb{R}}{\longrightarrow \atop x^{4}, \ldots, x^{n}} \stackrel{M}{\varphi}
$$
![[Pasted image 20220122103214.png]]
4.1.1 Derivation $-X_{x}$ is a derivation of $C^{\infty}(M,\{x\}, \mathbb{R})$ :
i) $x_{x}([f]+[g])=x_{x}([f])+x_{x}([g])$
ii) $x_{x}(\lambda[f])=\lambda x_{x}([f])$
iii) $X_{x}([f] \cdot[g])=X_{x}([\in]) g(x)+f(x) X_{x}([g])$
$4.2$ Tangent space - The vector space of tangent vectors at $x$ is colled the tangent space to $M$ at $x$ and is denoted by $T_{x} M$. Basis: $\left\{\frac{\partial}{\partial x^{x}} I_{x}, 1 \leq i \leq n\right\}$
$4.2 .1$ Tangent bundle-TM of $M$ is $\frac{11}{x \in M} T_{x} M \quad \| \prod \Pi(Y$
$42.2$ Fibers $-\pi^{-1}(\{x\})$ where $\pi: T M \rightarrow M, X_{x} \mapsto x$
$4.2 .3 P_{\text {ush }}-$ forward $-$ (denivative) of $f: M \rightarrow N$ at $x$ denoted ty $\left.f_{*}\right|_{x}$ is:
$$
\begin{aligned}
\left.f_{*}\right|_{x}: & T_{x} M \rightarrow T_{f(x)} N, X_{x} \mapsto\left(\left.f_{*}\right|_{x} X_{x}\right) \in T_{f(x)} N \text { where } \\
\left(f_{*} X\right)[g] &=X([g \circ f]) \quad \forall[g] \in C^{\infty}\left(N_{f}(x), \mid R\right)
\end{aligned}
$$

$4.2 .4$ Cotangent space $-T_{x}^{*} M=\left(T_{x} M\right)^{*} \quad$ basis $\left\{\left.\underset{\text { Lsymbolic }}{\{}\right|_{x}, 1 \leqslant i \leqslant n\right\} \omega^{-}$
where $\left.d x^{i}\right|_{x}\left(\frac{\partial}{\partial x^{j}} j_{x}\right)=\delta_{i j}$
4.2.5 Cotangent bundle $-T^{x} M=\frac{11}{x \in M} T_{x}^{*} M$
$4.3 C^{\infty}$ vector field $-X$ on $M$ is a $C^{\infty}$ mop $X: M \rightarrow T M$ s.t. $\pi \circ X=i d_{M}$, which in a chart $(U, \varphi)$ is of the form: $X(x)=\left.\sum_{i=1}^{n} X^{i}(x) \frac{\partial}{\partial x^{i}}\right|_{x}$. The set of is denoted by $\Gamma(T M), \mathcal{f}(M)$.
$4.4 C^{\infty} 1-$ form $-\omega$ on $M$ is a $C^{\infty}$ map $\omega: M \rightarrow T^{*} M$ s.t. $\pi o w=i d_{M}$, set of denoted by $\Gamma\left(T^{*} M\right), \Omega .$ In a chart $(0, \varphi) \quad \omega \in \Gamma\left(T^{*} U\right): \omega=\sum_{i=1}^{n} a_{i}\left(x^{4}, \ldots, x^{n}\right) d x^{i}$
5.1.1 Immersion- $A C_{\text {map }}^{\infty} f: M \rightarrow N$ is an immersion if $f_{*}: T_{x} M \rightarrow T_{f(x)} M$ is an injective linear mapping at every $x \in M$.
5.1.2 Immersed Submanifold - of a manifold $M$ is a pair $(N, f)$ where $f: N \rightarrow M$ is an injective immersion
$5.1 .3$ Embedded submanifold - of $M$ is an immersed submanifold (N,f) s.f. $f: N \rightarrow f(N)$ is a homeomorphism, where $f(N)$ is endowed with the topology induced by $M$.
5.1.4 Diffeomorphism $-f: M \rightarrow N$ is a diffeomorphism if $f$ is a $C^{\infty}$ homeomorphism and $f^{-1}$ is $C^{\infty}$
5.2 Lie Group - is a $C^{\infty}$-manifold $G$ endowed with a group structure for which the maps $m: G_{x} G \rightarrow G:(x, y) \mapsto x \cdot y$ and $i G \rightarrow G: x \mapsto x^{-1}$ are $C^{\infty}$
5.2.1 K-th exterior power - Let $V$ be a real vectorspace with $\operatorname{dim} V=n$. Let $V^{*}$ denote the dual of $V$. We define for $o \leqslant k \leqslant n$ the $k$ th exterior power $\Lambda^{k}\left(V^{x}\right)$ of $V^{*}$ by: $\Lambda^{0}\left(V^{*}\right)=\mathbb{R}, \quad{\Lambda^{k}}\left(V^{*}\right)=\{w: \underbrace{V^{n} X \cdots}_{k \text { times }} V^{n} \longrightarrow \mathbb{R}$ s.t. $w$ is $k$-linear and alternating $\}$
5.2.2 Altemating $-\omega$ is alternating if $\omega\left(\pi\left(v_{1}\right), \ldots, \pi\left(v_{k}\right)\right)=(-1)^{1 \pi 1} \omega\left(v_{1}, \ldots, v_{k}\right)$ for $\pi \in S_{k}$ (permutation set

$5.2 .3$ wedge product $-\Lambda: \Lambda^{k}\left(V^{*}\right) \times \Lambda^{l}\left(V^{*}\right) \rightarrow \Lambda^{k+l}\left(V^{*}\right),(\omega, \tau) \mapsto \omega \wedge \tau$ where $(\omega \wedge \tau)\left(v_{1}, \ldots, v_{k+e}\right)=\frac{1}{(k+e) !} \sum_{\pi \in S_{k+e}} \omega\left(v_{\pi(1)}, \ldots, v_{\pi(k)}\right) \tau\left(v_{\pi(k+1)}, \ldots, v_{\pi(k+e)}\right)$ This endows $\Lambda^{*}\left(V^{*}\right)=\bigoplus_{k=0}^{n} \Lambda^{k}\left(V^{*}\right)$ with a graded algebra structure
$6.1 C^{\infty} k$-form - on $M$ is a $C^{\infty}$ section of the sondle $\Lambda^{k}\left(T^{*} M\right)$, that is a $C^{\infty}$ map $\omega \cdot M \rightarrow \Lambda^{k}\left(T^{*} M\right)$ such that $\pi o w=i d_{M}$. In a coord. chart $(U, \varphi)$ $w=\sum_{1 \leqslant i_{1}} a_{c} \ldots i_{i}\left(x_{k}^{1}, \ldots, x^{n}\right) d x^{i,} \wedge \ldots \wedge d x^{i k}$, where $a_{i, \ldots, i_{k}}\left(x^{1}, \ldots, x^{n}\right) \in C^{\infty}\left(\mathbb{R}^{n}\right)$
6.1.1 Module of differential forms- The set of $C^{\infty} k$-forms on $m$ is a module aver the ring $C^{\infty}(M, \mathbb{R})$. We denote it by $\Omega^{k}(M)=\Gamma\left(\Lambda^{k}\left(T^{*} M\right)\right)$ and the module of differential forms is $\Omega^{*}(M)=\underset{k=0}{\oplus} \Omega^{k}(M)$
6.1.2 $d: \Omega^{0}(M) \rightarrow \Omega{ }^{1}(M)-\left.d f\right|_{x}\left(X_{x}\right)=X_{x}([f])$
$6.1 .3 \mathrm{du}^{-}$- for $M$ covered by a single chart we define:
$$
\begin{aligned}
&d_{U}: \Omega^{*}(U) \rightarrow \Omega^{*}(U) \text { by } \\
&d_{U} \omega=\sum_{i,<\cdots<i_{k}} \sum_{R} \frac{\partial}{\partial x} R\left(a_{i, \ldots i_{k}}\right) d x^{R} \wedge d x^{i_{1}} \wedge \cdots \wedge d x^{i_{k}}
\end{aligned}
$$
6.2.1 K-cocycle - is a $C^{\infty} k$-form we $\Omega^{k}($ (u) s.t. $d \omega=0$
$$
Z_{d R}^{k}=\left\{\omega \in \Omega^{k}(M) \mid \omega \text { is a } k \text {-co-cycle }\right\}
$$
$\underline{6.2 .2 k \text {-coooundary }-\text { is a } C^{\infty} k \text {-form } \omega \in \Omega^{k}(M) \text { s.t. } \exists \eta \in \Omega^{k-1}(M)}$ with $w=d \eta$.
$B_{d R}^{k}=\left\{w \in \Omega^{k}(M) l w\right.$ is a $k$-cobeundery $\}$
6.3.1 $K_{\text {th }}$ de Rahm conomology space $-H_{d R}^{k}(M)$ is defined as the quotient space. $\quad H_{d R}^{k}(\omega)=Z_{d Q}^{k}(M) / B_{d R}^{k}(M)$

6.3.2 $k$-th Getti number - of $M, 6_{k}(m):=\operatorname{dim}\left(H_{d R}^{k}(m)\right)$ if $<\infty$
$6.4 \mathrm{de}-\operatorname{Ranm}$ cohomolog algebra - of $M$ is defined as $H_{\mathrm{dR}}^{*}(M)$ endowed with the graded product
$$
\Lambda: H_{d R}^{k}(M) \times H_{d R}^{e}(M) \rightarrow H_{d R}^{k+e}(M) \quad([\omega],[\tau]) \mapsto[\omega] \wedge[\tau]
$$
6.3.3 Pull back - given f:M $\rightarrow N, C^{\infty}$ map, define $f^{*}: \Omega^{*}(N) \rightarrow \Omega^{*}(M)$ as follows: on o-forms ge $\Omega^{\circ}(N): c^{\infty}(N, \mathbb{R}) \quad f^{*} g=g \circ f$
$$
M \stackrel{f}{\rightarrow} N
$$
$$
\begin{aligned}
&f_{g}^{*} \underset{\mathbb{R}}{\downarrow} \text { g and on } k \text {-forms, with } k \geqslant 1 \text { : } \\
&\left(f^{*} \omega\right)\left(\left.X_{1}\right|_{x}, \ldots,\left.X_{k}\right|_{x}\right)=\omega\left(\left.f_{*}\left(X_{1}\right)\right|_{f(x)}, \ldots,\left.f_{*}\left(X_{k}\right)\right|_{f(x)}\right)
\end{aligned}
$$
$6.3 .4$ Lagrangian Map - a map
s.t. $\mathcal{L}^{*} \Omega=0 . \quad \mathcal{L}:\left(x^{1}, \ldots, x^{n}\right) \mapsto\left(x^{1}, \ldots, x^{n}, y^{n}=f^{1}\left(x_{1}^{*}, \ldots, x^{n}\right), \ldots, y^{n}=f^{n}\left(x^{n}, \ldots, x^{n}\right)\right)$
$7.0$ Homotopy operator $-$ is a linear operator $K: \Omega^{*}\left(\mathbb{R}^{n} \times \mathbb{R}\right) \rightarrow \Omega^{*}\left(\mathbb{R}^{n} \times \mathbb{R}\right)$ suen that $\quad i d_{\Omega^{*}\left(\mathbb{R}^{n} \times \mathbb{R}\right)}-\pi^{*} \circ s^{*}=\pm d k \pm k d$
( $\pi$ is the projection $\mathbb{R}^{n} \times \mathbb{R} \rightarrow \mathbb{R}^{n}$ and $s$ the coo section: $s: \mathbb{R}^{n} \rightarrow \mathbb{R}^{n} \times \mathbb{R} \quad \underline{x} \mapsto(x, 0)$
$8.1$ Partion of unity- of a fopological space $X$ is a set $R$ of continuous functions of $x \rightarrow[0,1]$ s.t. $\forall x \in X$ : $\exists U$ open nhood of $x$ s.t. all bot finite arount of functions of R ore 0 and $\sum_{f \in R} f(x)=1$.
$8.2$ cochain complex - let $A=\prod_{i=0}^{n} A_{i}$ where $A_{i}$ is a finitedim. vector space then if $d_{A}: A_{i} \rightarrow A_{i+1}$ is s.t. $d_{A} \circ d_{A}=0$ then $\left(A, d_{A}\right)$ is a cochain complex

8.3 cochain map-A map $f:\left(A, d_{A}\right) \rightarrow\left(B, d_{B}\right)$ is a cochain map if every square:
$8.4$ Exact sequence $-G_{0} \stackrel{f_{1}}{\rightarrow} G_{1} \stackrel{f_{2}}{\longrightarrow} G_{3} \rightarrow \ldots$ where $f_{i}$ is a group and $f_{i}$ a howomorphism then the sequence is exact if $\operatorname{im}\left(f_{k}\right)=\operatorname{ker}\left(f_{k+1}\right)$. Thus: Monomorphism (oneto-one /njective) : $0 \rightarrow A C^{t} B$ is exact $\Leftrightarrow f$ is a monomorphism Epinorphism (onto / surjective): $\quad B \stackrel{f}{\rightarrow} C \rightarrow 0$ is exact $\Leftrightarrow f$ is an epinorphism bimorphism ( isonorpnism almost): $0-A \hookrightarrow B \rightarrow 0$ is exact $\Leftrightarrow f$ is a binorphism if isor $\quad A \stackrel{\sim}{\rightarrow} B$
$8.5$ Mayer-Vietoris sequence - Let $U, V$ be open subsets $, M=U_{n} V:$
$$
\begin{aligned}
0 \rightarrow \Omega^{*}(u \cup V) & \stackrel{f}{\rightarrow} \Omega^{*}(u) \oplus \Omega^{*}(V) \stackrel{g}{\rightarrow} \Omega^{*}\left(U_{n} V\right) \rightarrow 0 \\
\omega &\left.\omega_{u} \oplus \omega\right|_{V} \\
\mu &\left.\oplus \stackrel{g}{\longmapsto} \tau\right|_{U n V}-\left.\mu\right|_{U n V}
\end{aligned}
$$
$9.1$ Good cover - an open corer $U=\left\{U_{\alpha} \mid \alpha \in A\right\}$ of a $C^{\infty}$ manifold is called a good cover if all non-empty finite intersections of open sets of $U$ are difteomorphic to $\mathbb{R}^{n}$.
9.2 Finite type manifold $-A C^{\infty}$ manifold $M$ is said to be of finite type if it odmits a finite good cover
9.3 Poincare Polynomial-Let $M$ a manifold odmitting a finite good, cover. The poincarre polynomial of $M, P_{M}(t)$ is defined by:
$$
P_{m}(t)=\sum_{k=0}^{\operatorname{dim}(M)=n} b_{k}(M) t^{k}, k+h \text { tetti number of } M
$$

10.1 Orientable- $A C^{\infty}$ manifold $M$ is orientable if $\exists$ atlas $\left\{\left(U_{\alpha}, \varphi_{\alpha}\right) \mid \alpha \in A\right\}$ s.t.
$$
\varphi_{B} \circ \varphi_{A}^{-r}: \varphi_{\alpha}\left(U_{\alpha} \cap U_{B}\right) \rightarrow \varphi_{B}\left(U_{\alpha} \cap U_{B}\right)
$$
has positive Jacobian determinant for all $\alpha, \beta \in A$.
$$
\left(\varphi_{\beta} \circ \varphi_{A}^{-1}\right)\left(d x_{\beta} \wedge \cdots \wedge d x_{\beta}^{n}\right)=J\left(\frac{x_{B}}{x_{\alpha}}\right)\left(d x_{\alpha}^{\wedge} \wedge \ldots \wedge d x_{\alpha}^{n}\right)
$$
$10.2$ Orientation-An orientation on $M$ is an equivalence class [w] where $\omega \in \Omega^{n}(M)$ and $\omega_{1} \sim \omega_{2} \Leftrightarrow \omega_{1}=f \omega_{2}, f>0$, an orientation is denoted by [M]
10.3 Integral- let $\tau \in \Omega_{c}^{n}(M)$, then:
$$
\int_{[M]} \tau:=\sum_{\alpha \in A} \int_{U_{\alpha}} \rho_{\alpha} \tau:=\sum_{\alpha \in A} \int_{\mathbb{R}^{n}}\left(\varphi_{\alpha}^{-1}\right)^{*}\left(\rho_{\alpha} \tau\right)
$$
where $\left\{\left.\left(U_{\alpha}, Q_{\alpha}\right)\right|_{\mathrm{~ Y o u ~ a r e ~ m u t e d . ~ P r e s s ~ A l t ~ A ~ A ~ t e ~ A n s ~}~\right.$ and $\left\{\rho_{\alpha} \mid \alpha \in A\right\}$ is a partion of hold the SPACE key to temporarily unm