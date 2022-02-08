---
alias:
tags:
- qftII
- stringTheory
---
In [[mathematics]], the 'beta function', also called the [[Euler integral]] of the first kind, is a [[special function]] that is closely related to the [[gamma function]] and to [[binomial coefficient]]s.  It is defined by the [[integral]]

$$ B(x,y) = \int_0^1 t^{x-1}(1-t)^{y-1}\,dt$$

for [[complex number]] inputs$x,y$ such that $\mathrm{Re}(x)>0, ~\mathrm{Re}(y)>0$.

The beta function was studied by [[Leonhard Euler|Euler]] and [[Adrien-Marie Legendre|Legendre]] and was given its name by [[Jacques Philippe Marie Binet|Jacques Binet]]; its symbol $B$ is a [[Greek alphabet|Greek]] capital [[Beta (letter)|beta]].

# Properties
The beta function is [[symmetric function|symmetric]], meaning that

$$ B(x,y) = B(y,x)$$

for all inputs $x,y$.

A key property of the beta function is its close relationship to the [[gamma function]]: one has that

$$ B(x,y)=\frac{\Gamma(x)\,\Gamma(y)}{\Gamma(x+y)}.$$


The beta function is also closely related to [[binomial coefficient]]s.  When $x$ (or $y$, by symmetry) is a positive integer, it follows from the definition of the [[gamma function]] $\Gamma$

$$ B(x,y) =\dfrac{(x-1)!}{(x+y-1)_x} = \frac{x + y}{xy} \Bigg/ \binom{x + y}{x}. $$