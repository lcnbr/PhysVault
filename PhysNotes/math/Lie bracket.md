---
alias:
- Jacobi identity
- Lie brackets
tags:
- qftII
- string theory
---
-The leading deviation $2 m_{2}(a, b)$ from linearity in [[../QFTII/multiplication in lie algebra#^69185d]] is called the Lie bracket $[\![ a, b ]\!]$.

We can thus compute it as the limit of a commutator of Lie group elements
$$
[\![ a, b ]\!]=\lim _{\epsilon \rightarrow 0} \frac{1}{\epsilon^{2}} \exp ^{-1}[\exp (\epsilon a) \exp (\epsilon b) \exp (-\epsilon a) \exp (-\epsilon b)] .
$$
The Lie bracket has the following properties:
- It is [[bilinear form|bilinear]].

- It is [[bilinear form#^antisym|anti-symmetric]]
$$
[\![ a, b ]\!]=-[\![ b, a ]\!] .
$$

- It satisfies the Jacobi identity$$[\![ [\![ a, b ]\!], c ]\!]+[\![ [\![ b, c]\!], a ]\!]+[\![ [\![ c, a ]\!], b ]\!]=0 .$$ 
^jacobi


The latter property follows from the Hall-Witt identity for three group elements $x, y, z$ and their inverses $\bar{x}, \bar{y}, \bar{z}$
$$
\begin{aligned}
1=& \bar{y}((y \bar{x} \bar{y} x) \bar{z}(\bar{x} y x \bar{y}) z) y \\
& \cdot \bar{z}((z \bar{y} \bar{z} y) \bar{x}(\bar{y} z y \bar{z}) x) z \\
& \cdot \bar{x}((x \bar{z} \bar{x} z) \bar{y}(\bar{z} x z \bar{x}) y) x .
\end{aligned}
$$

^a02fc1

The leading order (cubic) contribution of each line equals one of the three terms of the Jacobi identity. Note that the conjugation of the double commutator does not affect the leading order terms, but it is necessary to make the identity hold for generic groups upon dropping all brackets.