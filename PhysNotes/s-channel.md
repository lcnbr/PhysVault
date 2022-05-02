---
alias:
- channel I
tag:
- qft
---
![[s-channel 2022-04-29 14.44.24.excalidraw|100|left-wrap]]If we consider  $2 \to 2$ particle scattering with all incoming momenta then the s-channel corresponds to the two in states $1,2$ and two out states $3,4$. In the [[center of momentum frame|CM frame]] we can write:
$$\begin{array}{ll}
q_1=\pqty{E_1, \mathbf{p}_s}, & q_2=\pqty{E_2,-\mathbf{p}_s}, \\
q_3=\pqty{E_3,\mathbf{p}_s'}, & q_4=\pqty{E_4, \mathbf{p}_s'} ;
\end{array}$$
And from [[conserved total momentum]] we have: $E_1+E_2+E_3+E_4=0$. Generally we only want to consider positive energy on-shell states. If we have that our $\ket{\text{in}}$ system is made up of the generic momentum values $p_1$ and $p_2$, we have to impose that $E_1>0$ and $E_2>0$. This in turn, imposes a negative energy for the generic momenta $p_3$ and $p_4$. Since this is not physical we denote the momentum *of* particles 3 and 4 to be the additive inverse of $p_3$ and $p_4$ respectively[^1]: 
$$\begin{array}{ll}
p_{\text{in},1}^\mu=q_1^\mu=\pqty{E_1, \mathbf{p}_s}, & p_{\text{in},2}^\mu=q_2^\mu=\pqty{E_2,-\mathbf{p}_s}, \\
p_{\text{out},3}^\mu=-q_3^\mu=\pqty{-E_3,-\mathbf{p}_s'}^\mu=\pqty{E_{\text{out},3},-\mathbf{p}_s'}, & p_{\text{out},4}^\mu=-q_4^\mu=\pqty{-E_4, -\mathbf{p}_s'}=\pqty{E_{\text{out},4},\mathbf{p}_s'} ;
\end{array}$$
Now we remove the in and out labels and we can rewrite momentum conservation:

$$p_1^\mu+p_2^\mu=p_3^\mu+p_4^\mu\implies E_1+E_2=E_3+E_4>0$$
The definition of the [[Mandelstam invariants|s-variable]] is:![[Mandelstam invariants#^sInvariant]]
Rewriting in terms of our [[center of momentum frame|CM frame]] momenta:
$$s=E_s^2,\quad E_s=E_1+E_2=E_3+E_4$$
Thus invariant $s$ has a simple physical significance. It is the square of the total energy of the colliding particles $(1$ and 2$)$ in their [[center of momentum frame|centre-of-mass system]]. 

We can write the norm of the particles 3-momenta in the [[center of momentum frame|CM frame]] $\mathbf{p}_s^2$ and $\mathbf{p}_s'^2$ in terms of $s,m_1,m_2,m_3$ and $m_4$:[^2]

$$\begin{align*}
 \mathbf{p}_s^2=\frac{1}{4 s}\bqty{s-\pqty{m_1+m_2}^2}\bqty{s-\pqty{m_1-m_2}^2} \\
 \mathbf{p}_s^{\prime 2}=\frac{1}{4 s}\bqty{s-\pqty{m_3+m_4}^2}\bqty{s-\pqty{m_3-m_4}^2} 
\end{align*}$$
We can thus also write $E_i$ in terms of $s,m_1,m_2,m_3,m_4$:$$\begin{align*}
E_1&=\sqrt{m_1^2+\mathbf{p}_s^2}=\sqrt{\frac{1}{4s}\pqty\big{s^2+m_1^4+m_2^4-2m_1^2m_2^2-2s(m_2^2-m_1^2)}}\\
&=\frac{1}{2\sqrt{s}}\sqrt{\pqty\big{s-m_2^2+m_1^2}^2}=\frac{1}{2\sqrt{s}}\pqty\big{s-m_2^2+m_1^2}\\
E_2&=\frac{1}{2\sqrt{s}}\pqty\big{s-m_1^2+m_2^2}\\
E_3&=\frac{1}{2\sqrt{s}}\pqty\big{s-m_4^2+m_3^2}\\E_4&=\frac{1}{2\sqrt{s}}\pqty\big{s-m_3^2+m_4^2}\\
\end{align*}$$
Finally we can write $t$ and $u$ in terms of $s,m_1,m_2,m_3,m_4$ by plugging in:[^3]
$$t=(q_1+q_3)^2=(E_1-E_3)^2-(\mathbf{p}_s+\mathbf{p}_s')^2$$
[^1]: See also [[Mandelstam invariants#^ca96c7]]
[^2]: We use that the particles must be [[on-shell]], i.e. $p_i^2=m_i^2=q_i^2$ thus expanding out the definition of $s$ we have: $$s=q_1^2+2q_1^\mu q_{2,\mu} + q_2^2 =m_1^2+2(E_1E_2+\mathbf{p}_s^2)+m_2^2$$Since the particles are [[on-shell]] we also can write $E_i$ in terms of $\mathbf{p}_i$ and $m_i$: $E_i=\sqrt{m_i^2+\mathbf{p}_i^2}$ and inserting this we can now try to isolate $\mathbf{p}_s$:$$s=m_1^2+2(\sqrt{(m_1^2+\mathbf{p}_s^2)(m_2^2+\mathbf{p}_s^2)}+\mathbf{p}_s^2)+m_2^2$$isolating the square root and then squaring both sides yields:
$$4(m_1^2+\mathbf{p}_s^2)(m_2^2+\mathbf{p}_s^2)=(s-m_1^2-m_2^2-2\mathbf{p}_s^2)^2$$And expanding the squares, the $\mathbf{p}_s^4$ cancel:$$4m_1^2m_2^2+\bcancel{4\mathbf{p}_s^2(m_1^2+m_2^2)}+\cancel{4\mathbf{p}_s^4}=s^2+m_1^4+m_2^4+\cancel{4\mathbf{p}_s^4}-2s(m_1^2+m_2^2)+2m_1^2m_2^2-4s  \mathbf{p}_s^2+\bcancel{4\mathbf{p}_s^2(m_1^2+m_2^2)}$$And isolating $\mathbf{p}_s^2$:$$\mathbf{p}_s^2=\frac{1}{4s}\pqty\big{s^2+m_1^4+m_2^4-2m_1^2m_2^2-2s(m_1^2+m_2^2)}=\frac{1}{4 s}\bqty{s-\pqty{m_1+m_2}^2}\bqty{s-\pqty{m_1-m_2}^2}$$
[^3]: We have$$\begin{align*}
t=(q_1+q_3)^2&=(E_1-E_3)^2-(\mathbf{p}_s+\mathbf{p}_s')^2\\
&=\frac{1}{4s}(s-m_1+m_2-s+m_4-m_3)^2-\mathbf{p}_s^2-\mathbf{p}_s'^2-2\mathbf{p}_s \cdot \mathbf{p}_s'\\
&=\frac{1}{4s}(-m_1+m_2+m_4-m_3)^2-\frac{1}{4 s}\bqty{s-\pqty{m_1+m_2}^2}\bqty{s-\pqty{m_1-m_2}^2} 
 -\frac{1}{4 s}\bqty{s-\pqty{m_3+m_4}^2}\bqty{s-\pqty{m_3-m_4}^2} -2\mathbf{p}_s \cdot \mathbf{p}_s'
\end{align*}$$