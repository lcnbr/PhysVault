In [[Hamiltonian mechanics]], a '''canonical transformation''' is a change of [[canonical coordinates]] {{math|('''q''', '''p''', ''t'') → ('''Q''', '''P''', ''t'')}} that preserves the form of [[Hamilton's equations]]. This is sometimes known as '''form invariance'''. It need not preserve the form of the [[Hamiltonian mechanics|Hamiltonian]] itself. Canonical transformations are useful in their own right, and also form the basis for the [[Hamilton–Jacobi equation]]s (a useful method for calculating [[constant of motion|conserved quantities]]) and [[Liouville's theorem (Hamiltonian|Liouville's theorem]]) (itself the basis for classical [[statistical mechanics]]).

Since [[Lagrangian mechanics]] is based on [[../String/generalized coordinates]], transformations of the coordinates {{math|'''q''' → '''Q'''}} do not affect the form of [[Lagrangian mechanics|Lagrange's equations]] and, hence, do not affect the form of [[Hamilton's equations]] if we simultaneously change the momentum by a [[../math/Legendre transform|Legendre transformation]] into

$$P_i=\frac{\partial L}{\partial \dot{Q}_i}.$$

Therefore, coordinate transformations (also called '''point transformations''') are a ''type'' of canonical transformation. However, the class of canonical transformations is much broader, since the old generalized coordinates, momenta and even time may be combined to form the new generalized coordinates and momenta.  Canonical transformations that do not include the time explicitly are called '''restricted canonical transformations''' (many textbooks consider only this type).

For clarity, we restrict the presentation here to [[calculus]] and [[classical mechanics]].  Readers familiar with more advanced mathematics such as [[cotangent bundle]]s, [[exterior derivative]]s and [[symplectic manifold]]s should read the related [[symplectomorphism]] article.  (Canonical transformations are a special case of a symplectomorphism.)  However, a brief introduction to the modern mathematical description is included at the end of this article.

# Notation# 
Boldface variables such as {{math|'''q'''}} represent a list of {{mvar|N}} [[../String/generalized coordinates]] that need not transform like a [[Vector (geometric|vector]]) under [[rotation]], e.g.,

$$\mathbf{q} \equiv \left (q_{1}, q_{2}, \ldots, q_{N-1}, q_{N} \right ).$$

A dot over a variable or list signifies the time derivative, e.g.,

$$\dot{\mathbf{q}} \equiv \frac{d\mathbf{q}}{dt}.$$

The [[dot product]] notation between two lists of the same number of coordinates is a shorthand for the sum of the products of corresponding components, e.g.,

$$\mathbf{p} \cdot \mathbf{q} \equiv \sum_{k=1}^{N} p_{k} q_{k}.$$

The dot product (also known as an "[[../math/inner product]]") maps the two coordinate lists into one variable representing a single numerical value.

# Direct approach# 
The functional form of [[Hamilton's equations]] is

$$\begin{align}
\dot{\mathbf{p}} &= -\frac{\partial H}{\partial \mathbf{q}} \\
\dot{\mathbf{q}} &= \frac{\partial H}{\partial \mathbf{p}}
\end{align}$$

By definition, the transformed coordinates have analogous dynamics

$$\begin{align}
\dot{\mathbf{P}} &= -\frac{\partial K}{\partial \mathbf{Q}} \\
\dot{\mathbf{Q}} &= \frac{\partial K}{\partial \mathbf{P}}
\end{align}$$

where {{math|''K''('''Q''', '''P''')}} is a new Hamiltonian (sometimes called the Kamiltonian<ref>{{harvnb|Goldstein|1980|p=380}}</ref>) that must be determined.

In general, a  transformation {{math|('''q''', '''p''', ''t'') → ('''Q''', '''P''', ''t'')}} does not preserve the form of [[Hamilton's equations]].  For time independent transformations between {{math|('''q''', '''p''')}} and {{math|('''Q''', '''P''')}} we may check if the transformation is restricted canonical, as follows.  Since restricted transformations have no explicit time dependence (by definition), the time derivative of a new generalized coordinate {{math|''Q<sub>m</sub>''}} is

$$\begin{align}
\dot{Q}_{m} &= \frac{\partial Q_{m}}{\partial \mathbf{q}} \cdot \dot{\mathbf{q}} + \frac{\partial Q_{m}}{\partial \mathbf{p}} \cdot \dot{\mathbf{p}} \\
&= \frac{\partial Q_{m}}{\partial \mathbf{q}} \cdot \frac{\partial H}{\partial \mathbf{p}} - \frac{\partial Q_{m}}{\partial \mathbf{p}} \cdot \frac{\partial H}{\partial \mathbf{q}} \\
&= \lbrace Q_m , H \rbrace
\end{align}$$

where {{math|{⋅, ⋅} }} is the [[Poisson bracket]].

We also have the identity for the conjugate momentum ''P<sub>m</sub>''

$$\frac{\partial H}{\partial P_{m}} =  \frac{\partial H}{\partial \mathbf{q}} \cdot \frac{\partial \mathbf{q}}{\partial P_{m}} +  \frac{\partial H}{\partial \mathbf{p}} \cdot \frac{\partial \mathbf{p}}{\partial P_{m}}$$

If the transformation is canonical, these two must be equal, resulting in the equations

$$\begin{align}
\left( \frac{\partial Q_{m}}{\partial p_{n}}\right)_{\mathbf{q}, \mathbf{p}} &= -\left( \frac{\partial q_{n}}{\partial P_{m}}\right)_{\mathbf{Q}, \mathbf{P}} \\
\left( \frac{\partial Q_{m}}{\partial q_{n}}\right)_{\mathbf{q}, \mathbf{p}} &= \left( \frac{\partial p_{n}}{\partial P_{m}}\right)_{\mathbf{Q}, \mathbf{P}}
\end{align}$$

The analogous argument for the generalized momenta ''P<sub>m</sub>'' leads to two other sets of equations

$$\begin{align}
\left( \frac{\partial P_{m}}{\partial p_{n}}\right)_{\mathbf{q}, \mathbf{p}} &= \left( \frac{\partial q_{n}}{\partial Q_{m}}\right)_{\mathbf{Q}, \mathbf{P}} \\
\left( \frac{\partial P_{m}}{\partial q_{n}}\right)_{\mathbf{q}, \mathbf{p}} &= -\left( \frac{\partial p_{n}}{\partial Q_{m}}\right)_{\mathbf{Q}, \mathbf{P}}
\end{align}$$

These are the '''direct conditions''' to check whether a given transformation is canonical.

# Liouville's theorem# 
The direct conditions allow us to prove [[Liouville's theorem (Hamiltonian|Liouville's theorem]]), which states that the ''volume'' in  phase space is conserved under canonical transformations, i.e.,

$$ \int \mathrm{d}\mathbf{q}\, \mathrm{d}\mathbf{p} = \int \mathrm{d}\mathbf{Q}\, \mathrm{d}\mathbf{P}$$

By [[Integration by substitution#Substitution for multiple variables|calculus]], the latter integral must equal the former times the [[Jacobian matrix and determinant|Jacobian]] {{mvar|J}}

$$\int \mathrm{d}\mathbf{Q}\, \mathrm{d}\mathbf{P} = \int J\, \mathrm{d}\mathbf{q}\, \mathrm{d}\mathbf{p}$$

where the [[../math/Jacobian]] is the [[determinant]] of the [[matrix (mathematics|matrix]]) of [[partial derivative]]s, which we write as

$$J \equiv \frac{\partial (\mathbf{Q}, \mathbf{P})}{\partial (\mathbf{q}, \mathbf{p})}$$

Exploiting the "division" property of [[Jacobian matrix and determinant|Jacobian]]s yields

$$ J \equiv \frac{\partial (\mathbf{Q}, \mathbf{P})}{\partial (\mathbf{q}, \mathbf{P})} \left/ \frac{\partial (\mathbf{q}, \mathbf{p})}{\partial (\mathbf{q}, \mathbf{P})} \right. $$

Eliminating the repeated variables gives

$$J \equiv  \frac{\partial (\mathbf{Q})}{\partial (\mathbf{q})} \left/ \frac{\partial (\mathbf{p})}{\partial (\mathbf{P})} \right.$$

Application of the '''direct conditions''' above yields {{math|''J'' {{=}} 1}}.

# Generating function approach# 
{{main|Generating function (physics)}}
To ''guarantee'' a valid transformation between {{math|('''q''', '''p''', ''H'')}} and {{math|('''Q''', '''P''', ''K'')}}, we may resort to an indirect '''generating function''' approach. Both sets of variables must obey [[action (physics|Hamilton's principle]]). That is the [[Action Integral]] over the [[Lagrangian mechanics|Lagrangian]] <math>\mathcal{L}_{qp}=\mathbf{p} \cdot \dot{\mathbf{q}}  - H(\mathbf{q}, \mathbf{p}, t)$$ and <math>\mathcal{L}_{QP}=\mathbf{P} \cdot \dot{\mathbf{Q}} - K(\mathbf{Q}, \mathbf{P}, t)$$ respectively, obtained by the Hamiltonian via ("inverse") [[Legendre transformation]], both must be stationary (so that one can use the [[Euler–Lagrange equations]] to arrive at equations of the above-mentioned and designated form; as it is shown for example [[Hamilton equations#Deriving Hamilton's equations|here]]):

$$\begin{align}
\delta \int_{t_{1}}^{t_{2}} \left[ \mathbf{p} \cdot \dot{\mathbf{q}} - H(\mathbf{q}, \mathbf{p}, t) \right] dt &= 0 \\
\delta \int_{t_{1}}^{t_{2}} \left[ \mathbf{P} \cdot \dot{\mathbf{Q}} - K(\mathbf{Q}, \mathbf{P}, t) \right] dt &= 0
\end{align}$$

One way for both [[calculus of variations|variational integral]] equalities to be satisfied is to have

$$\lambda \left[ \mathbf{p} \cdot \dot{\mathbf{q}}  - H(\mathbf{q}, \mathbf{p}, t) \right] = \mathbf{P} \cdot \dot{\mathbf{Q}} - K(\mathbf{Q}, \mathbf{P}, t) + \frac{dG}{dt} $$

Lagrangians are not unique: one can always multiply by a constant {{mvar|λ}} and add a total time derivative {{math|{{sfrac|''dG''|''dt''}}}} and yield the same equations of motion (see for reference: [http://en.wikibooks.org/wiki/Classical_Mechanics/Lagrange_Theory#Is_the_Lagrangian_unique.3F]).

In general, the scaling factor {{mvar|λ}} is set equal to one; canonical transformations for which {{math|''λ'' ≠ 1}} are called '''extended canonical transformations'''. {{math|{{sfrac|''dG''|''dt''}}}} is kept, otherwise the problem would be rendered trivial and there would be not much freedom for the new canonical variables to differ from the old ones.

Here {{mvar|G}} is a [[generating function (physics|generating function]]) of one old [[canonical coordinates|canonical coordinate]] ({{math|'''q'''}} or {{math|'''p'''}}), one new [[canonical coordinates|canonical coordinate]] ({{math|'''Q'''}} or {{math|'''P'''}}) and (possibly) the time {{mvar|t}}.  Thus, there are four basic types of generating functions (although mixtures of these four types can exist), depending on the choice of variables. As will be shown below, the generating function will define a transformation from old to new [[canonical coordinates]], and any such transformation {{math|('''q''', '''p''') → ('''Q''', '''P''')}} is guaranteed to be canonical.

# =Type 1 generating function# =
The type 1 generating function {{math|''G''<sub>1</sub>}} depends only on the old and new generalized coordinates
$$G \equiv G_{1}(\mathbf{q}, \mathbf{Q}, t)$$
To derive the implicit transformation, we expand the defining equation above

$$ \mathbf{p} \cdot \dot{\mathbf{q}}  - H(\mathbf{q}, \mathbf{p}, t) = \mathbf{P} \cdot \dot{\mathbf{Q}} - K(\mathbf{Q}, \mathbf{P}, t) + \frac{\partial G_{1}}{\partial t} + \frac{\partial G_{1}}{\partial \mathbf{q}} \cdot \dot{\mathbf{q}} + \frac{\partial G_{1}}{\partial \mathbf{Q}} \cdot \dot{\mathbf{Q}}$$

Since the new and old coordinates are each independent, the following {{math|2''N'' + 1}} equations must hold

$$\begin{align}
\mathbf{p} &= \frac{\partial G_{1}}{\partial \mathbf{q}} \\
\mathbf{P} &= -\frac{\partial G_{1}}{\partial \mathbf{Q}} \\
K &= H + \frac{\partial G_{1}}{\partial t}
\end{align}$$

These equations define the transformation {{math|('''q''', '''p''') → ('''Q''', '''P''')}} as follows.   The ''first'' set of {{mvar|N}} equations

$$\mathbf{p} =\frac{\partial G_{1}}{\partial \mathbf{q}}$$

define relations between the new [[../String/generalized coordinates]] {{math|'''Q'''}} and the old [[canonical coordinates]] {{math|('''q''', '''p''')}}. Ideally, one can invert these relations to obtain formulae for each {{math|''Q<sub>k</sub>''}} as a function of the old [[canonical coordinates]].  Substitution of these formulae for the {{math|'''Q'''}} coordinates into the ''second'' set of {{mvar|N}} equations

$$\mathbf{P} = -\frac{\partial G_{1}}{\partial \mathbf{Q}}$$

yields analogous formulae for the new generalized momenta {{math|'''P'''}} in terms of the old [[canonical coordinates]] {{math|('''q''', '''p''')}}.  We then invert both sets of formulae to obtain the ''old'' [[canonical coordinates]] {{math|('''q''', '''p''')}} as functions of the ''new'' [[canonical coordinates]] {{math|('''Q''', '''P''')}}.  Substitution of the inverted formulae into the final equation 
$$K = H + \frac{\partial G_{1}}{\partial t}$$
yields a formula for {{mvar|K}} as a function of the new [[canonical coordinates]] {{math|('''Q''', '''P''')}}.

In practice, this procedure is easier than it sounds, because the generating function is usually simple.  For example, let 
$$
G_{1} \equiv \mathbf{q} \cdot \mathbf{Q}
$$
This results in swapping the generalized coordinates for the momenta and vice versa 
$$\begin{align}
\mathbf{p} &= \frac{\partial G_{1}}{\partial \mathbf{q}} = \mathbf{Q} \\
\mathbf{P} &= -\frac{\partial G_{1}}{\partial \mathbf{Q}} = -\mathbf{q}
\end{align}$$
and {{math|''K'' {{=}} ''H''}}.  This example illustrates how independent the coordinates and momenta are in the Hamiltonian formulation; they are equivalent variables.

# =Type 2 generating function# =
The type 2 generating function {{math|''G''<sub>2</sub>}} depends only on the old [[../String/generalized coordinates]] and the new generalized momenta
$$G \equiv -\mathbf{Q} \cdot \mathbf{P} + G_{2}(\mathbf{q}, \mathbf{P}, t)$$
where the <math>-\mathbf{Q} \cdot \mathbf{P}$$ terms represent a [[Legendre transformation]] to change the right-hand side of the equation below.  To derive the implicit transformation, we expand the defining equation above

$$ \mathbf{p} \cdot \dot{\mathbf{q}}  - H(\mathbf{q}, \mathbf{p}, t) =   -\mathbf{Q} \cdot \dot{\mathbf{P}} - K(\mathbf{Q}, \mathbf{P}, t) + \frac{\partial G_{2}}{\partial t} + \frac{\partial G_{2}}{\partial \mathbf{q}} \cdot \dot{\mathbf{q}} + \frac{\partial G_{2}}{\partial \mathbf{P}} \cdot \dot{\mathbf{P}}$$

Since the old coordinates and new momenta are each independent, the following {{math|2''N'' + 1}} equations must hold

$$\begin{align}
\mathbf{p} &= \frac{\partial G_{2}}{\partial \mathbf{q}} \\
\mathbf{Q} &= \frac{\partial G_{2}}{\partial \mathbf{P}} \\
K &= H + \frac{\partial G_{2}}{\partial t}
\end{align}$$

These equations define the transformation {{math|('''q''', '''p''') → ('''Q''', '''P''')}} as follows.   The ''first'' set of {{mvar|N}} equations

$$\mathbf{p} = \frac{\partial G_{2}}{\partial \mathbf{q}}$$

define relations between the new generalized momenta {{math|'''P'''}} and the old [[canonical coordinates]] {{math|('''q''', '''p''')}}. Ideally, one can invert these relations to obtain formulae for each {{math|''P<sub>k</sub>''}} as a function of the old [[canonical coordinates]].  Substitution of these formulae for the {{math|'''P'''}} coordinates into the ''second'' set of {{mvar|N}} equations

$$\mathbf{Q} = \frac{\partial G_{2}}{\partial \mathbf{P}}$$

yields analogous formulae for the new generalized coordinates {{math|'''Q'''}} in terms of the old [[canonical coordinates]] {{math|('''q''', '''p''')}}. We then invert both sets of formulae to obtain the ''old'' [[canonical coordinates]] {{math|('''q''', '''p''')}} as functions of the ''new'' [[canonical coordinates]] {{math|('''Q''', '''P''')}}.  Substitution of the inverted formulae into the final equation 
$$K = H + \frac{\partial G_{2}}{\partial t}$$
yields a formula for {{mvar|K}} as a function of the new [[canonical coordinates]] {{math|('''Q''', '''P''')}}.

In practice, this procedure is easier than it sounds, because the generating function is usually simple.  For example, let 
$$G_{2} \equiv \mathbf{g}(\mathbf{q}; t) \cdot \mathbf{P}$$
where {{math|'''g'''}} is a set of {{mvar|N}} functions.  This results in a point transformation of the generalized coordinates
$$\mathbf{Q} = \frac{\partial G_{2}}{\partial \mathbf{P}} = \mathbf{g}(\mathbf{q}; t)$$

# =Type 3 generating function# =
The type 3 generating function {{math|''G''<sub>3</sub>}} depends only on the old generalized momenta and the new generalized coordinates 
$$
G \equiv \mathbf{q} \cdot \mathbf{p} + G_{3}(\mathbf{p}, \mathbf{Q}, t)
$$
where the <math>\mathbf{q} \cdot \mathbf{p}$$ terms represent a [[Legendre transformation]] to change the left-hand side of the equation below.  To derive the implicit transformation, we expand the defining equation above

$$-\mathbf{q} \cdot \dot{\mathbf{p}}  - H(\mathbf{q}, \mathbf{p}, t) = \mathbf{P} \cdot \dot{\mathbf{Q}} - K(\mathbf{Q}, \mathbf{P}, t) + \frac{\partial G_{3}}{\partial t} + \frac{\partial G_{3}}{\partial \mathbf{p}} \cdot \dot{\mathbf{p}} + \frac{\partial G_{3}}{\partial \mathbf{Q}} \cdot \dot{\mathbf{Q}}$$

Since the new and old coordinates are each independent, the following {{math|2''N'' + 1}} equations must hold

$$\begin{align}
\mathbf{q} &= -\frac{\partial G_{3}}{\partial \mathbf{p}} \\
\mathbf{P} &= -\frac{\partial G_{3}}{\partial \mathbf{Q}} \\
K &= H + \frac{\partial G_{3}}{\partial t}
\end{align}$$

These equations define the transformation {{math|('''q''', '''p''') → ('''Q''', '''P''')}} as follows. The ''first'' set of {{mvar|N}} equations

$$ \mathbf{q} = -\frac{\partial G_{3}}{\partial \mathbf{p}}$$

define relations between the new [[../String/generalized coordinates]] {{math|'''Q'''}} and the old [[canonical coordinates]] {{math|('''q''', '''p''')}}.  Ideally, one can invert these relations to obtain formulae for each {{math|''Q<sub>k</sub>''}} as a function of the old [[canonical coordinates]].  Substitution of these formulae for the {{math|'''Q'''}} coordinates into the ''second'' set of {{mvar|N}} equations

$$\mathbf{P} = -\frac{\partial G_{3}}{\partial \mathbf{Q}}$$

yields analogous formulae for the new generalized momenta {{math|'''P'''}} in terms of the old [[canonical coordinates]] {{math|('''q''', '''p''')}}.  We then invert both sets of formulae to obtain the ''old'' [[canonical coordinates]] {{math|('''q''', '''p''')}} as functions of the ''new'' [[canonical coordinates]] {{math|('''Q''', '''P''')}}. Substitution of the inverted formulae into the final equation 
$$
K = H + \frac{\partial G_{3}}{\partial t}
$$
yields a formula for {{mvar|K}} as a function of the new [[canonical coordinates]] {{math|('''Q''', '''P''')}}.

In practice, this procedure is easier than it sounds, because the generating function is usually simple.

# =Type 4 generating function# =
The type 4 generating function <math>G_{4}(\mathbf{p}, \mathbf{P}, t)$$ depends only on the old and new generalized momenta
$$
G \equiv \mathbf{q} \cdot \mathbf{p} - \mathbf{Q} \cdot \mathbf{P} + G_{4}(\mathbf{p}, \mathbf{P}, t)
$$
where the <math>\mathbf{q} \cdot \mathbf{p} - \mathbf{Q} \cdot \mathbf{P}$$ terms represent a [[Legendre transformation]] to change both sides of the equation below.    To derive the implicit transformation, we expand the defining equation above

$$-\mathbf{q} \cdot \dot{\mathbf{p}}  - H(\mathbf{q}, \mathbf{p}, t) = -\mathbf{Q} \cdot \dot{\mathbf{P}} - K(\mathbf{Q}, \mathbf{P}, t) + \frac{\partial G_{4}}{\partial t} + \frac{\partial G_{4}}{\partial \mathbf{p}} \cdot \dot{\mathbf{p}} + \frac{\partial G_{4}}{\partial \mathbf{P}} \cdot \dot{\mathbf{P}} $$

Since the new and old coordinates are each independent, the following {{math|2''N'' + 1}} equations must hold

$$\begin{align}
\mathbf{q} &= -\frac{\partial G_{4}}{\partial \mathbf{p}} \\
\mathbf{Q} &= \frac{\partial G_{4}}{\partial \mathbf{P}} \\
K &= H + \frac{\partial G_{4}}{\partial t}
\end{align}$$

These equations define the transformation {{math|('''q''', '''p''') → ('''Q''', '''P''')}} as follows. The ''first'' set of {{mvar|N}} equations

$$
\mathbf{q} = -\frac{\partial G_{4}}{\partial \mathbf{p}}
$$

define relations between the new generalized momenta {{math|'''P'''}} and the old [[canonical coordinates]] {{math|('''q''', '''p''')}}.  Ideally, one can invert these relations to obtain formulae for each {{math|''P<sub>k</sub>''}} as a function of the old [[canonical coordinates]].  Substitution of these formulae for the {{math|'''P'''}} coordinates into the ''second'' set of {{mvar|N}} equations

$$\mathbf{Q} = \frac{\partial G_{4}}{\partial \mathbf{P}} $$

yields analogous formulae for the new generalized coordinates {{math|'''Q'''}} in terms of the old [[canonical coordinates]] {{math|('''q''', '''p''')}}.  We then invert both sets of formulae to obtain the ''old'' [[canonical coordinates]] {{math|('''q''', '''p''')}} as functions of the ''new'' [[canonical coordinates]] {{math|('''Q''', '''P''')}}.  Substitution of the inverted formulae into the final equation 
$$
K = H + \frac{\partial G_{4}}{\partial t}
$$
yields a formula for {{mvar|K}} as a function of the new [[canonical coordinates]] {{math|('''Q''', '''P''')}}.

# Motion as a canonical transformation# 
Motion itself (or, equivalently, a shift in the time origin) is a canonical transformation. If <math>\mathbf{Q}(t) \equiv \mathbf{q}(t+\tau)$$ and <math>\mathbf{P}(t) \equiv \mathbf{p}(t+\tau)$$, then [[action (physics|Hamilton's principle]]) is automatically satisfied

$$ \delta \int_{t_{1}}^{t_{2}} \left[ \mathbf{P} \cdot \dot{\mathbf{Q}} - K(\mathbf{Q}, \mathbf{P}, t) \right] dt = \delta \int_{t_{1}+\tau}^{t_{2}+\tau}  \left[ \mathbf{p} \cdot \dot{\mathbf{q}} - H(\mathbf{q}, \mathbf{p}, t+\tau) \right] dt = 0 $$

since a valid trajectory <math>(\mathbf{q}(t), \mathbf{p}(t))$$ should always satisfy [[action (physics|Hamilton's principle]]), regardless of the endpoints.

#  Examples # 
* The translation <math>\mathbf{Q}(\mathbf{q}, \mathbf{p})= \mathbf{q} + \mathbf{a}, \mathbf{P}(\mathbf{q}, \mathbf{p})= \mathbf{p} + \mathbf{b}$$ where <math>\mathbf{a}, \mathbf{b}$$ are two constant vectors is a canonical transformation. Indeed, the Jacobian matrix is the identity, which is symplectic: <math>I^\text{T}JI=J$$.
* Set <math>\mathbf{x}=(q,p)$$ and <math>\mathbf{X}=(Q,P)$$, the transformation <math>\mathbf{X}(\mathbf{x})=R \mathbf{x}$$ where <math>R \in SO(2)$$ is a rotation matrix of order 2 is canonical. Keeping in mind that special orthogonal matrices obey <math>R^\text{T}R=I$$ it's easy to see that the Jacobian is symplectic. Be aware that this example only works in dimension 2: <math>SO(2)$$ is the only special orthogonal group in which every matrix is symplectic.
* The transformation <math>(Q(q,p), P(q,p))=(q+f(p), p)$$, where <math>f(p)$$ is an arbitrary function of <math>p$$, is canonical. Jacobian matrix is indeed given by $$\frac{\partial X}{\partial x}=\begin{bmatrix} 1 & f'(p) \\ 0 & 1 \end{bmatrix}$$ which is symplectic.

# Modern mathematical description# 
In mathematical terms, [[canonical coordinates]] are any coordinates on the phase space ([[cotangent bundle]]) of the system that allow the [[canonical one-form]] to be written  as

$$\sum_i p_i\,dq^i$$

up to a total differential ([[exact form]]). The change of variable between one set of [[canonical coordinates]] and another is a '''canonical transformation'''.   The index of the [[generalized coordinate]]s {{math|'''q'''}} is written here as a ''superscript'' (<math>q^{i}$$), not as a ''subscript'' as done above (<math>q_{i}$$).  The superscript conveys the [[Covariance and contravariance of vectors|contravariant transformation properties]] of the generalized coordinates, and does ''not'' mean that the coordinate is being raised to a power.  Further details may be found at the [[symplectomorphism]] article.

# History# 
The first major application of the canonical transformation was in 1846, by [[Charles-Eugène Delaunay|Charles Delaunay]], in the study of the [[Earth-Moon-Sun system]]. This work resulted in the publication of a pair of large volumes as ''Mémoires'' by the [[French Academy of Sciences]], in 1860 and 1867.