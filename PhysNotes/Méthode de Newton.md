# Une dimension 
![[Pasted image 20220526155521.png#leftwrap|200]]La droite tangente à $y=f(x)$ en $\left(x^{(k)}, f\left(x^{(k)}\right)\right)$ est d'équation $y=f\left(x^{(k)}\right)+f^{\prime}\left(x^{(k)}\right)\left(x-x^{(K)}\right)$ On cherche $x^{(k+1)}$ avec la propriété que $f\left(x^{(k+1)}\right)=0$; si on remplace la fct et la tangente en un voisinage on trouve:
$$
0=f\left(x^{(k)}\right)+f^{\prime}\left(x^{(k)}\right)\left(x^{(k+1)}-x^{(k)}\right) \Rightarrow x^{(k+1)}=x^{(k)}-\frac{f\left(x^{(k)}\right)}{f^{\prime}\left(x^{(k)}\right)}
$$
> [!rmk]-
>  Si $f$ linéaire, $x^{(1)}=\alpha, \alpha=$ zéro de $f$ En général, la méthode marche bien si $x^{(0)}$ est suffisamment proche de $\alpha$.Normalement, on regarde le graphe de $y=f(x)$ ou sinon on fait
un certain nombre d'itérations dans l'algorithme de bissection. Cela nous aide à choisir $x^{(0)}$ proche de $\alpha$.


> [!prop]
> Supposons $f \in C^{2}$ en un voisinage de $\alpha$ t.q. $f(\alpha)=0, f^{\prime}(\alpha)=0$. Alors $\lim _{K \rightarrow \infty} \frac{x^{(k+1)}-\alpha}{\left(x^{(K)}-\alpha\right)^{2}}=\frac{f^{\prime \prime}(\alpha)}{2 f^{\prime}(\alpha)}$ si $x^{(k)} \longrightarrow \alpha($ càd si la méthode

> [!prf]-
> La formule de Taylor donne:
> $$x^{(k+1)}-\alpha=x^{(k)}-\frac{f\left(x^{(k)}\right)}{f^{\prime}\left(x^{(k)}\right)}-\alpha=x^{(k)}-\alpha-\left(x^{(k)}-\alpha\right)+\frac{1}{2}\left(x^{(k)}-\alpha\right)^{2} \frac{f^{\prime \prime}(y)}{f^{\prime}\left(x^{(k)}\right)}$$
> Ainsi $$\frac{x^{(k+1)}-\alpha}{\left(x^{(k)}-\alpha\right)^{2}}=\frac{f^{\prime \prime}(y)}{2 f^{\prime}\left(x^{(k)}\right)} \longrightarrow \frac{f^{\prime \prime}(\alpha)}{2 f^{\prime}(\alpha)} \leftarrow \begin{gathered}\text { Comme } y \rightarrow \alpha \\ \text { et } f^{\prime \prime}(y)\end{gathered}$$

>[!rmk]-
>pour $k>0, e^{(k+1)} \sim c\left(e^{(k)}\right)^{2}, c \in \mathbb{R}$ (l'erreur décroit vite)

>[!def]
>Une suite $\left\{x^{(k)}\right\}_{k \geqslant 0}$ converge a l'ordre $p \geqslant 1 s^{\prime} \exists c \in \mathbb{R}, c>0, t$.q. $\exists k_{0}: \frac{\left|x^{(k+1)}-\alpha\right|}{\left|x^{(K)}-\alpha\right|^{p}} \leqslant C \quad \forall k \geqslant k_{0}$. Dans ce cas, on dit que la méthode converge a I'ordre p. Si $p=1$, on a la convergence $x^{(k)} \rightarrow \alpha$ si $c<1$.

>[!rmk]-
> Si les hypothèses de la prop. Sont verifiées, la méthode converge quadratiquement (a l'ordre 2).

# Plusieurs dimensions


