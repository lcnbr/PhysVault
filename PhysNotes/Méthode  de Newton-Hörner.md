# Méthode de Newton-Hörner
Elle consiste en une [[Méthodes de déflation|procédure de déflation]], ou la racine $r_{m}$ est calculée à l'aide de la [[Méthode de Newton]].

Nous avons: $P_{n}^{\prime}(x)=q_{n-1}(x, z)+(x-z) q_{n-1}^{\prime}(x, z)$ donc $P_{n}^{\prime}(z)=q_{n-1}(z, z)$ Étant donné une estimation initiale $r^{(0)}$ d'une racine $r$ de $P_{n}(x)$, on calcule pour $k \geqslant 0$
$$r^{(k+1)}=r^{(k)}-\frac{P_{n}\left(r^{(k)}\right)}{P_{n}^{\prime}\left(r^{(k)}\right)}=r^{(k)}-\frac{P_{n}\left(r^{(k)}\right)}{q_{n-1}\left(r^{(k)}, r^{(k)}\right)}$$
Après avoir trouvé une racine $r$ de $P_{n}(x)$, on passe a la recherche d'une racine de $P_{n-1}(x)$ t.q. $P_{n}(x)=(x-r) P_{n-1}(x)$. Pour calculer $P_{n-1}(x)$ nous utilisons la méthode de Hörner et $P_{n-1}(x)=q_{n-1}(x, r)$.
On repète jusqu'à calculer toutes les racines.

# Remarques: 
- Il faut commencer avec un $r^{(0)} \in \mathbb{C} \mid \mathbb{R}$, car si on commence avec $r^{(0)} \in \mathbb{R}$, alors $r^{(k)} \in \mathbb{R} \forall k \geqslant 0$ et on trouve que les racines reelles
- Dans ce cas, on passe directement $\dot{a} P_{n-2}(x)=q_{n-2}(x, \bar{r})$(sans regarder $P_{n-1}(x)=q_{n-1}(x, r)$ )
- Accumulation de l'erreur