

# Definition in classical mechanics
In [[classical mechanics]], '''canonical coordinates''' are coordinates $q^i$ and $p_i$ in [[phase space]] that are used in the [[Hamiltonian mechanics|Hamiltonian]] formalism. The canonical coordinates satisfy the fundamental [[Poisson bracket]] relations:

$$\left\{q^i, q^j\right\} = 0 \qquad \left\{p_i, p_j\right\} = 0 \qquad \left\{q^i, p_j\right\} = \delta_{ij}$$

A typical example of canonical coordinates is for $q^i$ to be the usual [[Cartesian coordinates]], and $p_i$ to be the components of [[momentum]]. Hence in general, the $p_i$ coordinates are referred to as "[[Conjugate momenta|conjugate momenta]]."

Canonical coordinates can be obtained from the [[generalized coordinates]] of the [[Lagrangian mechanics|Lagrangian]] formalism by a [[Legendre transformation]], or from another set of canonical coordinates by a [[canonical transformation]].

# Definition on cotangent bundles
Canonical coordinates are defined as a special set of [[coordinates]] on the [[cotangent bundle]] of a [[manifold]]. They are usually written as a set of $\left(q^i, p_j\right)$ or $\left(x^i, p_j\right)$ with the ''x'' 's or ''q'' 's denoting the coordinates on the underlying manifold and the ''p'' 's denoting the '''conjugate momentum''', which are [[1-form]]s in the cotangent bundle at point ''q'' in the manifold.

A common definition of canonical coordinates is any set of coordinates on the cotangent bundle that allow the [[canonical one-form]] to be written in the form
$$\sum_i p_i\,\mathrm{d}q^i$$

up to a total differential. A change of coordinates that preserves this form is a [[canonical transformation]]; these are a special case of a [[symplectomorphism]], which are essentially a change of coordinates on a [[symplectic manifold]].

In the following exposition, we assume that the manifolds are real manifolds, so that cotangent vectors acting on tangent vectors produce real numbers.

# Formal development# 
Given a manifold {{mvar|Q}}, a [[vector field]] {{mvar|X}} on {{mvar|Q}} (a [[section (fiber bundle)|section]] of the [[tangent bundle]] {{math|''TQ''}}) can be thought of as a function acting on the [[cotangent bundle]], by the duality between the tangent and cotangent spaces.  That is, define a function

$$P_X: T^*Q \to \mathbb{R}$$

such that

$$P_X(q, p) = p(X_q)$$

holds for all cotangent vectors {{mvar|p}} in $T_q^*Q$. Here, $X_q$ is a vector in $T_qQ$, the tangent space to the manifold {{mvar|Q}} at point {{mvar|q}}.  The function $P_X$ is called the ''momentum function'' corresponding to {{mvar|X}}.

In [[atlas (topology)|local coordinates]], the vector field {{mvar|X}} at point {{mvar|q}} may be written as

$$X_q = \sum_i X^i(q) \frac{\partial}{\partial q^i}$$

where the $$\partial /\partial q^i$$ are the coordinate frame on {{mvar|TQ}}. The conjugate momentum then has the expression

$$P_X(q, p) = \sum_i X^i(q)\; p_i$$

where the $$p_i$$ are defined as the momentum functions corresponding to the vectors $$\partial /\partial q^i$$:

$$p_i = P_{\partial /\partial q^i}$$

The $q^i$ together with the $p_j$ together form a coordinate system on the cotangent bundle $T^*Q$; these coordinates are called the ''canonical coordinates''.

# Generalized coordinates# 
In [[Lagrangian mechanics]], a different set of coordinates are used, called the [[generalized coordinates]].  These are commonly denoted as $\left(q^i, \dot{q}^i\right)$ with $q^i$ called the '''generalized position''' and $\dot{q}^i$ the '''generalized velocity'''.  When a [[symplectic vector field|Hamiltonian]] is defined  on the cotangent bundle, then the generalized coordinates are related to the canonical coordinates by means of the [[Hamilton–Jacobi equation]]s.



In [[mathematics]] and [[classical mechanics]], '''canonical coordinates''' are sets of [[coordinates]] on [[phase space]] which can be used to describe a physical system at any given point in time. Canonical coordinates are used in the [[Hamiltonian mechanics|Hamiltonian formulation]] of [[classical mechanics]]. A closely related concept also appears in [[quantum mechanics]]; see the [[Stone–von Neumann theorem]] and [[canonical commutation relation]]s for details.

As [[Hamiltonian]] mechanics are generalized by [[symplectic geometry]] and [[canonical transformation]]s are generalized by [[contact transformation]]s, so the 19th century definition of canonical coordinates in classical mechanics may be generalized to a more abstract 20th century definition of coordinates on the [[cotangent bundle]] of a [[manifold]] (the mathematical notion of phase space).