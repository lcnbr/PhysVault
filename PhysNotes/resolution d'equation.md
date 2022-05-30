# Resolution d'equation

On cherche a resoudre une equation du type generale

$$\vec{f}(\vec{x})=\vec{g}(\vec{x})
$$

^eqEQ

Ou $\vec{f},\vec{g}$ sont des fonctions de $\mathbb{K}^m\to \mathbb{K}^n$, pour $\mathbb{K}$ un corps. Il y a plusieurs reformulations et cas particuliers de cette equation.

Une reformulation de [[#^eqEQ]] est une recherche de zeros. On peut definire $\vec{\tilde{f}}=\vec{f}-\vec{g}$, et [[#^eqEQ]] devient

$$
\vec{\tilde{f}}(\vec{x})=0
$$

^eqZero

Dans le cas ou $m=n$ on peut redefinir [[#^eqZero]], et ainsi [[#^eqEQ]] en equation de point fixe, si $\vec{h}(\vec{x})=\vec{\tilde{f}}(\vec{x})+\vec{x}$

$$
\vec{h}(\vec{x})=\vec{x}\iff \vec{h}(\vec{x})-\vec{x}=0\iff \vec{\tilde{f}}(\vec{x})=0
$$

^eqFix

Les methodes de resolution existent souvent pour des cas particuliers/simplifications de ces equations. On peut reduire les dimensions ou specifier le type de fonction.


## Simplification par dimension
Dans le cas particlulier de $m=n=1$ on a les methodes suivantes 

- Resolution de [[#^eqZero]]:
    - [[Méthode de dichotomie]]
    - [[Méthode de Newton]]
- Resolution de [[#^eqFix]]:
    - [[methode de point fixe]]

Dans le cas particulier de $m=n$ on peut encore utiliser la [[Méthode de Newton]]

## Simplification par type de fonction

### Polynomiale

Toujours en dimension $1=m=n$ si la fonction est polynomial le probleme  est reduit en une [[recherche de racine]]. 

### Lineaire



