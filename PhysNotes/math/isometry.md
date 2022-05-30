---
alias:
- isometries
---

# Idea

An _isometry_ is a function that preserves a metric, either in the sense of a metric space or in the sense of a Riemannian manifold.

# Metric spaces
An isometry $f:(X, d) \rightarrow\left(X^{\prime}, d^{\prime}\right)$ between metric spaces is a function $f: X \rightarrow X^{\prime}$ between the underyling sets that respects the metrics in that $d=f^{*} d^{\prime} \cdot$ More explicitly, $d^{\prime}(f(a), f(b))=d(a, b)$ for any points $a, b$ in $X$.
The same idea holds for extended quasi-pseudo-generalisations of metric spaces.
# Manifolds
An isometry $f:(X, g) \rightarrow\left(X^{\prime}, g^{\prime}\right)$ between Riemannian manifolds is a morphism $f: X \rightarrow X^{\prime}$ between the underlying manifolds that respects the metrics in that $g=f^{*} g^{\prime} \cdot$ More explicitly, $g^{\prime}\left(f_{*} v, f_{*} w\right)=g(v, w)$ for any $\underline{\text { tangent vectors }} v, w$ on $X$.
# Global isometries
Global isometries are the $\underline{\text { isomorphisms }}$ of metric spaces or Riemannian manifolds. An isometry is $\boldsymbol{g l o b a l}$ if it is a bijection whose inverse is also an isometry. Between metric spaces, isometries are necessarily injections and bijective isometries necessarily have isometries as inverses, so global isometries between metric spaces are also called surjective isometries; this does not work for Riemannian manifolds (where the inverse of an isometry need not be a morphism of manifolds), nor does it work for pseudometric spaces (where an isometry need not be injective).
# Infinitesimal isometries
see [[../GR/symmetries in GR|Killing vector]] field
# Isometries on normed vector spaces
In practice, isometries $E \rightarrow F$ between normed vector spaces tend to be affine maps. The following theorem gives a precise meaning to this.

A norm on a vector space is strictly convex if, whenever $\|u\|=1=\|v\|$, we have $\|t u+(1-t) v\|<1$ for some (hence all!) $t$ in the range $0<t<1$. In brief, no sphere contains a line segment. Examples of strictly convex spaces include spaces of type $L^{p}$ for $1<p<\infty$.
Theorem
Let $f: E \rightarrow F$ an isometry between normed vector spaces, and suppose $F$ is strictly convex. Then $f$ is affine.
Proof
To say that $f: E \rightarrow F$ is affine means that $f$ preserves linear combinations of the form $t x+(1-t) y$. It suffices to consider only the case where $0<t<1$ and, by continuity considerations, only the case of dyadic rationals between 0 and 1 . Continuing this train of thought, it suffices to prove that $f\left(\frac{1}{2}(x+y)\right)=\frac{1}{2}(f(x)+f(y))$ for all $x, y$.
In the case of strict convexity, midpoints $\frac{1}{2}(u+v)$ are determined in terms of the norm, as the unique point $w$ such that
$$
\|w-u\|=\frac{1}{2}\|u-v\|=\|w-v\| .
$$
The midpoint satisfies these equations for any normed vector space, but the uniqueness is a consequence of strict convexity. For if there were two such points $w, w^{\prime}$, then for some point $w$ '" on the line segment between them, we would have $\left\|w^{\prime \prime}-u\right\|<\frac{1}{2}\|u-v\|$, and $\left\|w^{\prime \prime}-v\right\| \leq \frac{1}{2}\|u-v\|$ by ordinary convexity. But these two inequalities taken together would violate the triangle inequality.

As a result, since $f$ is an isometry, $w=f\left(\frac{1}{2}(x+y)\right)$ is forced to be the midpoint between $f(x)$ and $f(y)$ if $F$ is strictly convex. This completes the proof.

If $F$ is not strictly convex, then isometries need not be affine. For example, consider $E=\mathbb{R}$, and $F=\mathbb{R}^{2}$ equipped with the $l_{\infty}$ (max) norm. For any contractive map $\phi: \mathbb{R} \rightarrow \mathbb{R}$, e.g., any smooth function with $\left|\phi^{\prime}\right| \leq 1$, the map $E \rightarrow F$ sending $x$ to $(x, \phi(x))$ is easily seen to be an isometry.

If however $f$ is a surjective isometry between normed vector spaces, then $f$ is affine, by the Mazur-Ulam theorem. Everything is linear instead of affine if $f(0)=0$.
## Linear isometry
Given two normed vector spaces $V$ and $W$, a linear isometry is a linear map $A: V \rightarrow W$ that preserves the norms:
$$
\|A v\|=\|v\|
$$
for all $v \in V_{\cdot}^{[7]}$ Linear isometries are distance-preserving maps in the above sense. They are global isometries if and only if they are surjective.


## [[inner product space]]


In an inner product space, the above definition reduces to
$$
\langle v, v\rangle=\langle A v, A v\rangle
$$
for all $v \in V$, which is equivalent to saying that $A^{\dagger} A=\mathrm{I}_{V}$. This also implies that isometries preserve inner products, as
$$
\langle A u, A v\rangle=\left\langle u, A^{\dagger} A v\right\rangle=\langle u, v\rangle .
$$
Linear isometries are not always unitary operators, though, as those require additionally that $V=W$ and $A A^{\dagger}=\mathrm{I}_{V}$.
