REPRÉSENTATION DES NOMBRES
$\mathbb{F} \subset \mathbb{R} \quad x \in \mathbb{F}$ nombre à virgule flottante, $x=(-1)^{5}\left(0 . a_{1} \ldots a_{+}\right) \cdot \beta^{e}=(-1)^{5} \cdot m \cdot \beta^{e-t}$ $s \in \mathbb{F}_{2}=\{0,1\}$ est un bit, $\beta \geqslant 2$ base $\beta \in \mathbb{Z}_{+}, 0 \leqslant a_{i} \leqslant \beta-1, m=a_{1} \ldots a_{+}$mantisse
Rem: $t=$ nombre max de chiffres stockées, $e \in \mathbb{Z}$ exposant t.q. $L \leqslant e \leqslant U$ (typiquement $L<0$ et $U>0$ )
- "flottante" $\leftrightarrow$ la position de la virgule n'est pas fixée
- $a_{1}, \ldots, a_{t}$ s'appellent chiffres
- on suppose $a_{1} \neq 0$ pour avoir l'unicité de la représentation
Ex: $1.2345=(-1)^{\circ}(0.12345) \cdot 10^{\prime}=(-1)^{\circ}(0,012345) \cdot 10^{2}$
$\tau$ pas une représentation valide car $a_{1}=0$
On écrit $\mathbb{F}(\beta, t, L, U)=\{0\} \cup\left\{x \in \mathbb{R}: x=(-1)^{s} \beta^{e} \sum_{i=1}^{t} a_{i} \beta^{-i}, L \leqslant e \leqslant U, s \in\{0,1\}\right\}$ pour l'ens. des nombres à virgule flottante $\dot{a} t$ chiffres, base $\beta$ et exposant $L \leqslant e \leqslant U$.

Déf./Ex: (norme IEEE754) deux standards pour le calcul numérique:
- précision simple: $\beta=2$, mantisse $=24$ bits $(t=23) \quad \begin{array}{r}\text { car } a_{1} \neq 0 \Rightarrow \\ a_{1}=1\end{array}$ exposant $=8$ bits $\left(\begin{array}{lll}-126 & \dot{a} & 127\end{array}\right)$
TOTAL: 32 bits
- precision double: $\beta=2,53$ bits de mantisse $(t=52)$.
exposant $=11$ bits ( $-1022$ à 1023 )
TOTAL : 64 bits
scilab utilise la précision double $2^{53} \sim 10^{15}$
53 chiffres binaires $\leftrightarrow 15$ chiffes décimaux

Rem: $\quad \mathbb{F} \neq \mathbb{R}, \quad|\mathbb{F}|<\infty, \quad x \in \mathbb{F} \Leftrightarrow-x \in \mathbb{F}$