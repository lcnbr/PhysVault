
On cherche les racines d'un polynôme $p_{n}(x)=\sum_{i=0}^{n} a_{i} x^{i} \in \mathbb{R}[x]$, ou $n \geqslant 2$

Rappel: 
- si $\alpha \in \mathbb{C}, p_{n}(\alpha)=0$, alors $p_{n}(\bar{\alpha})=0 \quad \bar{\alpha}=$ conjugué complexe de $\alpha$
- Il n'y a pas de formule explicite pour les racines si $n \geqslant 5$ (thēorie de Galois)

Remarque: Le choix du $x^{(0)}$ ou de l'intervalle de recherche d'une racine est très important pour la réussite de la méthode.

# Nombre de racines et localisation
## 
>[!thm] Règle des signes de Descartes
>
>Soit $\eta$ le nombre de changements de signe des coefficients $a_{0}, \ldots, a_{n}$ et $k l e$ nombre de racines reeelles positives de $P_{n}(x)=\sum_{i=0}^{n} a_{i} x^{i}$
>Alors $k \leqslant \eta$ et $\eta-k$ est pair.


>[!expl]-
>$P_{6}(x)=x^{6}-2 x^{5}+5 x^{4}-6 x^{3}+2 x^{2}+8 x-8$ a $\eta=5$ et racines $\pm 1, \pm 2 i, 1 \pm i$, donc $k=1$

>[!thm] Théorème (cauchy) 
>
>Les zéros de $p_{n}(x)$ sont inclus dans
>$$
\Gamma=\left\{z \in \mathbb{C}:\|z\| \leqslant 1+\max _{i=0, \ldots, n-1}\left|\frac{a_{i}}{a_{n}}\right|\right\}
>$$


> [!expl]- 
> Pour $P_{6}(x), \max _{i=0, \ldots, n-1}\left|a_{i}\right|=8$

# Evaluation efficace

L'[[algorithme de Hörner]] permet l'evaluation efficace de polynomes.

# Methode de recherche

Les methodes de recherche de racine sont generalement construites comme [[Méthodes de déflation]]. Ainsi la [[Méthode  de Newton-Hörner]] consiste en une methode de déflation qui applique a chaque sous problème la [[Méthode de Newton]].