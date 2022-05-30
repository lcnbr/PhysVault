# Méthode de la dichotomie (ou bissection)
![[Pasted image 20220526154729.png#leftwrap|140]]
Soit $f:[a, b] \rightarrow \mathbb{R}$ continue telle que $f(a) f(b)<0$. Par le TVI, $\exists a \in[a, b]$ t.q $f(\alpha)=0$ On pose $a^{(0)}=a, b^{(0)}=b, I^{(0)}=[a, b], x^{(0)}=\frac{a+b}{2}$. À chaque étape $k \geqslant 1$, on choisit le sous-intervalle $I^{(k)}=\left[a^{(k)}, b^{(k)}\right] \subseteq I^{(k-1)}$ comme suit:
- donnés $a^{(k-1)}, b^{(k-1)}, x^{(k-1)}=\frac{a^{(k-1)}+b^{(k-1)}}{2}$
- $\rightarrow$ si $f\left(x^{(k-1)}\right)=0$ alors $\alpha=x^{(k-1)}$
- sinon si $f\left(x^{(k-1)}\right) f\left(a^{(k-1)}\right)<0$ on pose $a^{(k)}=a^{(k-1)}$, $x^{(K)}=\frac{a^{(K)}+b^{(K)}}{2}$
- sinon on pose $a^{(k)}=x^{(k-1)}, b^{(k)}=b^{(k-1)}, x^{(k)}=\frac{a^{(k)}+b^{(k)}}{2}$

Ainsi, nous avons $x^{(k)}, K \geqslant 0, x^{(k)}$ est le point milieu de $I^{(k)},\left|I^{(k)}\right|=\frac{b-a}{2^{k}}$ et $I^{(k)}$ contient (par le TvI) un zéro 
>[!Lmm] 
>
>$\left|I^{(K)}\right|=b^{(K)}-a^{(K)}=\frac{b-a}{2^{K}} \quad \forall k \geqslant 0$. On suppose $f(a) f(b) \neq 0$. L'erreur $e^{(k)}$ à l'étape $k$ vérifie $\left|e^{(k)}\right|<\frac{b-a}{2 K+1} \quad \forall K \geqslant 0$.

>[!Prf]-
>Par déf., $\left|e^{(k)}\right|=\left|x^{(k)}-\alpha\right|$. On montre $\mid a$ theise par induction sur $k \geqslant 0$ $K=0\left|I^{(0)}\right|=|[a, b]|=b-a$ et $\left|x^{(0)}-\alpha\right|=\left|\frac{b-a}{2}-\alpha\right|<\frac{b-a}{2}$
>

> [!rmk]-
> - Soit $\varepsilon>0$ une tolerance donneee. Pour s'assurer que $\left|e^{(k)}\right|<\varepsilon$ il suffit de choisir kt.q $\frac{b-a}{2^{k+1}} \leqslant \varepsilon \Leftrightarrow 2^{k+1} \geqslant \frac{b-a}{\varepsilon} \Leftrightarrow k+1 \geqslant \log _{2}\left(\frac{b-a}{\varepsilon}\right)$. On doit donc choisir $\bar{k}=\left\lceil\log _{2}\left(\frac{b \cdot a}{\varepsilon}\right)\right]-1$
> - La formule pour $\bar{k}$ ne dépend pas de f. Par ex., nous pouvons pas calculer le zéro d'une fonction linēaire en une seule étape (pas optimal)

