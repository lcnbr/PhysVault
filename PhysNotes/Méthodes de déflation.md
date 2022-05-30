Si $\alpha$ est une racine de $P_{n}(x)\in \mathbb{R}[x]^{\leq n}$, alors on peut diviser $P_{n}(x)$ par $(x-\alpha)$ et la [[algorithme de Hörner|division polynomiale]]  n'aura pas de reste. Par l'[[algorithme de Hörner]] on obtient le quotient, qu'on note $q_{n-1}(x,\alpha)$:

$$P_{n}(x)=(x-\alpha) q_{n-1}(x, \alpha)$$

Les racines de $P_{n}(x)$ sont donc $\alpha$ et celles de $q_{n-1}(x, \alpha)$. On peut donc chercher les racines du polynôme $q_{n-1}(x, \alpha)$ de degré $n-1$.

> [!def] Méthode de déflation
>
>**Méthode de déflation** pour $m=n, n-1, \ldots, 1$
> 1) Trouver une racine $r_{m}$ de $P_{m}(x)$
> 2)  Calculer $q_{m-1}\left(x, r_{m}\right)$
> 3) Poser $P_{m-1}(x)=q_{m-1}\left(x, r_{m}\right)$