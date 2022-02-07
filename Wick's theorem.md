---
alias:
- wicks theorem
- Wicks theorem
- Wick contraction
---
If we can find an algorithm for turning a [[time-ordered|time ordered]] product of operators into a [[normal-ordered]] product of those operators, plus perhaps some c-number terms, we will have gone a long way in making the successive terms of this perturbation expansion easier to compute, and minimizing the amount of operator algebra we have to play with.

We need  [[contractions]]


$\require{physics} \op{a}{b}$
$\require{tikz}$
$\op{a}{b}$
$\wick{\c\phi A \c\phi}$
To prove the contraction is a c-number I will assume for the moment that $x_{0}>y_{0}$. The corresponding formula when $x_{0}<y_{0}$ will follow by the same reasoning. In this case,
$$
T(A(x) B(y))=A(x) B(y) \quad \text { (because } x_{0}>y_{0} \text { ) }
$$
Break each field up into its creation and annihilation parts,
$$
A(x)=A^{(+)}(x)+A^{(-)}(x) ; \quad B(y)=B^{(+)}(y)+B^{(-)}(y)
$$
where $A^{(-)}$and $B^{(-)}$contain each field's respective creation operators, while $A^{(+)}$and $B^{(+)}$ contain the annihilation operators (see the discussion following (3.33) on p. 39). Then
$$
T(A(x) B(y))=A^{(+)}(x) B^{(+)}(y)+A^{(-)}(x) B^{(+)}(y)+A^{(-)}(x) B^{(-)}(y)+A^{(+)}(x) B^{(-)}(y)
$$
There are four terms in the product $A(x) B(x)$, and three of them are already [[normal-ordered|normal ordered]]. The only one that is not [[normal-ordered|normal ordered]] is the last. Therefore the right-hand side is the [[normal-ordered|normal ordered]] product, plus a commutator:
$$
T(A(x) B(y))=: A(x) B(y):+\left[A^{(+)}(x), B^{(-)}(y)\right]
$$
The commutator is a c-number (see (3.38)):
$$
\left[A^{(+)}(x), B^{(-)}(y)\right]=\left\{\begin{array}{cc}
\Delta_{+}(x-y), & \text { if } A=B \\
0, & \text { if } A \neq B
\end{array}\right.
$$
A similar argument goes for $x_{0}<y_{0}$, so that we can write
$$
\begin{aligned}
\sqrt{A(x) A}(y) &=\theta\left(x_{0}-y_{0}\right)\left[A^{(+)}(x), A^{(-)}(y)\right]+\theta\left(y_{0}-x_{0}\right)\left[A^{(+)}(y), A^{(-)}(x)\right] \\
&=\theta\left(x_{0}-y_{0}\right) \Delta_{+}(x-y)+\theta\left(y_{0}-x_{0}\right) \Delta_{+}(y-x)
\end{aligned}
$$
$\wick{213}{A <1B CD <+E FG >1H IJ <xK LM >+O PQ >xR ST}$
That tells us that the contraction is a c-number.
We can write another expression for the contraction simply by taking the ground state expectation value of (8.14) above:
$$
\begin{aligned}
\overparen{A(x) B}(y) &=\langle 0|\overrightarrow{A(x) B}(y)| 0\rangle=\langle 0|T(A(x) B(y))| 0\rangle-\langle 0|: A(x) B(y):| 0\rangle \\
&=\langle 0|T(A(x) B(y))| 0\rangle
\end{aligned}
$$
because, by design, a [[normal-ordered|normal ordered]] product always has zero vacuum expectation value. Consequently,
$$
\overline{\phi(x) \phi}(y)=\langle 0|T(\phi(x) \phi(y))| 0\rangle
$$
By an amazing "coincidence", the right-hand side of this equation is something which you computed in your first homework (see Problem 1.3). I will save all of us the time to work it out again, and just remind you
$$
\langle 0|T(\phi(x) \phi(y))| 0\rangle=\lim _{\epsilon \rightarrow 0^{+}} \int \frac{d^{4} p}{(2 \pi)^{4}} e^{-i p \cdot(x-y)} \frac{i}{p^{2}-\mu^{2}+i \epsilon}
$$
Whenever I write an $\epsilon$ in the denominator in the future, you will need to remember that we are to take the expression in the limit $\epsilon \rightarrow 0^{+}$. Although you didn't do this for $\psi$, it's essentially the same calculation, and it's very easy to see that
$$
\overparen{\psi^{*}(x) \psi}(y)=\sqrt{\psi(x) \psi^{*}(y)}=\lim _{\epsilon \rightarrow 0^{+}} \int \frac{d^{4} p}{(2 \pi)^{4}} e^{-i p \cdot(x-y)} \frac{i}{p^{2}-m^{2}+i \epsilon}
$$
You get two equal terms from the $\phi^{1}$ and $\phi^{2}$, but that 2 is canceled by the $\sqrt{2}$ in the definitions of $\psi$ and $\psi^{*}$. All other contractions equal zero:
$$
\sqrt{\psi(x) \phi}(y)=\overline{\psi^{*}(x) \phi}(y)=\sqrt{\psi(x) \psi}(y)=\overline{\psi^{*}(x) \psi^{*}(y)}=0
$$
That's how it goes for two fields. Wick proved the same procedure works for a string of fields. We'll want two pieces of notation before diving into the proof. First, suppose we have a normal ordered string of fields, and want to contract two which are not immediately adjacent. Then
$$
: A ( x ) \longdiv { B ( y ) C ( z ) D } ( w ): \equiv: A(x) C(z): B(y) D(w)
$$
And, just for short, write
$$
\phi^{a_{1}}\left(x_{1}\right) \phi^{a_{2}}\left(x_{2}\right) \cdots \phi^{a_{n}}\left(x_{n}\right) \equiv \phi_{1} \phi_{2} \cdots \phi_{n}
$$

$$
\begC1{\phi_1}\conC{\phi_2\phi_3}\endC1{\phi_4}
$$
With those two conventions established, let's state Wick's Theorem:
$$
\begin{aligned}
T\left(\phi_{1} \phi_{2} \cdots \phi_{n}\right)=&: \phi_{1} \phi_{2} \cdots \phi_{n}: \\
&+: \emptyset_{1} \phi_{2} \cdots \phi_{n}:+\text { (all other terms with one contraction) } \\
&+: \emptyset_{1} \phi_{2} \phi_{3} \phi_{4} \cdots \phi_{n}:+\text { (all other terms with two contractions) } \\
&+\cdots+\text { (all terms with } \frac{1}{2} n \text { or } \frac{1}{2}(n-1) \text { contractions) } \\
\hline
\end{aligned}
$$
158
8. Wick diagrams
If $n$ is even, the last terms contain $\frac{1}{2} n$ contractions, otherwise they contain $\frac{1}{2}(n-1)$ contractions and a single field. It's perhaps not surprising that you obtain all the terms on the right-hand side of (8.28). A remarkable and graceful feature of the theorem is that each term appears exactly once, with coefficient $+1$.

Proof. The proof proceeds by induction on $n$. Let $W\left(\phi_{1} \phi_{2} \cdots \phi_{n}\right)$ denote the right-hand side of (8.28). It is trivially true that $T\left(\phi_{1}\right)=W\left(\phi_{1}\right)$, because both sides simply equal $\phi_{1}$. We've already established
$$
T\left(\phi_{1} \phi_{2}\right)=: \phi_{1} \phi_{2}:+: \emptyset_{1} \phi_{2}:=W\left(\phi_{1} \phi_{2}\right)
$$
By the induction hypothesis, assume $T\left(\phi_{1} \phi_{2} \cdots \phi_{n-1}\right)=W\left(\phi_{1} \phi_{2} \cdots \phi_{n-1}\right)$. If we can show $T\left(\phi_{1} \phi_{2} \cdots \phi_{n}\right)=W\left(\phi_{1} \phi_{2} \cdots \phi_{n}\right)$, we're done. Without loss of generality, we can relabel the fields, such that $x_{1}^{0} \geq x_{2}^{0} \geq x_{3}^{0} \geq \cdots \geq x_{n}^{0}$, and suppose we have then, by the induction hypothesis,
$$
T\left(\phi_{2} \phi_{3} \cdots \phi_{n}\right)=W\left(\phi_{2} \phi_{3} \cdots \phi_{n}\right)
$$
The job now is to show $T\left(\phi_{1} \phi_{2} \cdots \phi_{n}\right)=W\left(\phi_{1} \phi_{2} \cdots \phi_{n}\right)$. Multiply both sides of $(8.30)$ by $\phi_{1}$ :
$$
\phi_{1} T\left(\phi_{2} \phi_{3} \cdots \phi_{n}\right)=\phi_{1} W\left(\phi_{2} \phi_{3} \cdots \phi_{n}\right)
$$
The left-hand side of this equation is $T\left(\phi_{1} \phi_{2} \cdots \phi_{n}\right)$, because $x_{1}^{0}$ is larger than all the other times. The right-hand side is
$$
\begin{aligned}
\phi_{1} W\left(\phi_{2} \phi_{3} \cdots \phi_{n}\right) &=\left(\phi_{1}^{(+)}+\phi_{1}^{(-)}\right) W\left(\phi_{2} \phi_{3} \cdots \phi_{n}\right) \\
&=\phi_{1}^{(-)} W\left(\phi_{2} \phi_{3} \cdots \phi_{n}\right)+W\left(\phi_{2} \phi_{3} \cdots \phi_{n}\right) \phi_{1}^{(+)}+\left[\phi_{1}^{(+)}, W\left(\phi_{2} \phi_{3} \cdots \phi_{n}\right)\right]
\end{aligned}
$$
$W$ contains two types of elements, normal ordered strings and contractions. All of the terms in (8.32) are normal ordered. The first two terms on the right-hand side contain all contractions that do not involve $\phi_{1}$, as well as the remainder (if any) of uncontracted fields in normal order. Within the commutator, all the purely c-number terms, if any, will commute with $\phi_{1}^{(+)}$. The other terms will produce all the contractions that do involve $\phi_{1}$. Either a contraction involves $\phi_{1}$, or it does not. Therefore, the right-hand side of (8.32) is a normal ordered series containing all possible contractions of the $n$ fields: it is equal to $W\left(\phi_{1} \phi_{2} \cdots \phi_{n}\right)$. QED
I leave it as an exercise to show that Wick's theorem can also be written in the form
$$
T\left(\phi_{1} \phi_{2} \cdots \phi_{n}\right)=: \exp \left(\frac{1}{2} \sum_{i, j=1}^{n} \underset{\phi_{i} \phi_{j}}{\sigma} \frac{\partial}{\partial \phi_{i}} \frac{\partial}{\partial \phi_{j}}\right) \phi_{1} \phi_{2} \cdots \phi_{n}:
$$