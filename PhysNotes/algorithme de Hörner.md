# Algorithme de Hörner 
pour evaluer un polynôme en $\alpha \in \mathbb{C}$  de manière efficace c.a.d. pour $P_{n}(x)=\sum_{i=0}^{n} a_{i} x^{i} \in \mathbb{R}[x]$ calculer: $P_{n}(\alpha)$

- je calcule $\alpha, \alpha^{2}, \ldots, \alpha^{n}$ (n-1 produits)
- ensuite $a_{1} \alpha, \ldots, a_{n} \alpha^{n}$ (n produits)
- ensuite je somme (n additions)

$\rightarrow$ total: 2n-1 produits et $n$ additions pour calculer $p_{n}(\alpha)$

On observe: 

$$P_{n}(x)=a_{0}+x\left(a_{1}+a_{2} x+\ldots+a_{n} x^{n-1}\right)=a_{0}+x\left(a_{1}+x\left(a_{2}+x\left(\ldots\left(a_{n-1}+a_{n} x\right) \ldots\right)\right.\right.$$

^eqStar

Avec cette formule, on calcule $P_{n}(\alpha)$ avec $n$ produits et $n$ sommes (par induction)

Écrit sous forme algorithmique:
```
b[n]:=a[n]
for k:=n-1 to 0 
    b[k]:=b[k+1]alpha+a[k]
endfor
b[0]=P_n(alpha) k
```
Le polynôme $a_{n-1}(x, z)=\sum_{i=1}^{n-1} b_{i} x^{i-1}$ est un polynôme de degré $n-1$ en $x$, dont les coéfficients $b_{i}=b_{i+1} z+a_{i}$ dépendent du paramètre $z$


# Division polynomiale

En divisant $P_{n}(x)$ par $(x-z)$ on obtient $P_{n}(x)=b_{0}+(x-z) q_{n-1}(x, z)$
En effet, $b_{0}+(x-z) a_{n-1}(x, z)=b_{0}+(x-z) \sum_{i=1}^{n} b_{i} x^{i-1}=b_{0}+\sum_{i=1}^{n} b_{i} x^{i}-\sum_{i=1}^{n} b_{i} z x^{i-1}=$
$$
=\sum_{i=0}^{n} b_{i} x^{i}+\sum_{i=0}^{n-1} b_{i+1} z x^{i}=\sum_{i=0}^{n-1}\left(b_{i}-z b_{i+1}\right) x^{i}+b_{n} x^{n}=\sum_{i=0}^{n} a_{i} x^{i}=P_{n}(x)
$$