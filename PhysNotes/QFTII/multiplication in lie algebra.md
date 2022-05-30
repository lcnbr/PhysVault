---
alias:
tags:
- qftII
---
# Multiplication
The exponential map allows to pull back the group multiplication to the [[../math/Lie algebras|Lie algebra]]. Define a smooth map $m: \mathfrak{g} \times \mathfrak{g} \rightarrow \mathfrak{g}$ (more precisely on some neighbourhoods of 0 in $\mathfrak{g}$ ) such that
$$
\underbracket{\exp (a) \exp (b)}_{\text{in G}}=: \exp (\underbracket{m(a, b)}_{\text{in }\mathfrak{g}}) .
$$

Now it is clear that $m(a, 0)=m(0, a)=a$ hence
$$
m(a, b)=a+b+\mathcal{O}(a) \mathcal{O}(b) .
$$
We see that the pull back is approximated by vector addition. Addition is a natural operation for vector spaces, and the result is evident from smoothness properties. Consequently, this composition law is not very interesting since it tells nothing about multiplication in the underlying Lie group.

Let us therefore understand the deviation from linearity. We write explicitly the terms quadratic and of higher orders in $a, b$ as
$$
m(a, b)=a+b+m_{2}(a, b)+m_{\geq 3}(a, b) .
$$
From the above discussion we know that $m_{2}$ must be [[../math/bilinear form|bilinear]]. We furthermore know that $m(a, a)=2 a$. This implies that $m_{2}(a, a)=0$. Together with bilinearity we conclude that $m_{2}$ is [[../math/bilinear form#^antisym|anti-symmetric]]
$$
0=m_{2}(a+b, a+b)-m_{2}(a, a)-m_{2}(b, b)=m_{2}(a, b)+m_{2}(b, a)
$$

^69185d
