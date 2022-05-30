---
alias:
tags:
- qftII
---
The [[../math/defining representation of su(n|defining representation]].md) of $\mathfrak{s u}(N)$ maps elements of $\mathfrak{g}$ to $N \times N$ traceless anti-hermitian matrices. The representation $T_{a}^{\text {def }}$ of the basis $T_{a}$ therefore consists of traceless hermitian matrices ^[When $\mathfrak{s u}(N)$ is viewed as a matrix algebra, it makes sense to identify $T_{a}^{\text {def }}$ with $T_{a}$ and drop the label def from all matrices $T_{a}^{\text {def }}$ below for convenience.]
$$\left(T_{a}^{\text {def }}\right)^{+}=T_{a}^{\text {def }}, \quad \operatorname{Tr} T_{a}^{\text {def }}=0 .$$
The matrices $T_{a}^{\text {def }}$ are used to translate between the two standard formulations of unitary gauge theories: 
- One formulation assumes gauge fields to be traceless hermitian matrices $A$; 
- the other one uses real component fields $A^{a}$ in a basis of the Lie algebra. 

Consequently, the two are related by $A \sim T_{a}^{\text {def }} A^{a}$.

An important property of the representation matrices $T_{a}^{\text {def }}$ is that they also form a basis of $N \times N$ matrices (over the complex numbers) when supplemented with the unit matrix id. The completeness relation reads (using [[../math/structure constants#Killing form in basis]])
$$
k^{a b}\left(T_{a}^{\operatorname{def}}\right)^{i}{ }_{j}\left(T_{b}^{\operatorname{def}}\right)^{k}{ }_{l}=B^{\operatorname{def}}\left(\delta_{l}^{i} \delta_{j}^{k}-\frac{1}{N} \delta_{j}^{i} \delta_{l}^{k}\right) .
$$
It can be rephrased in terms of two trace identities which hold for any $N \times N$ matrix $X$
$$
\begin{aligned}
k^{a b} \operatorname{Tr}\left(T_{a}^{\mathrm{def}} X\right) T_{b}^{\mathrm{def}} &=B^{\mathrm{def}}\left(X-N^{-1} \operatorname{Tr} X\right) \\
k^{a b} T_{a}^{\mathrm{def}} X T_{b}^{\mathrm{def}} &=B^{\mathrm{def}}\left(\operatorname{Tr} X-N^{-1} X\right)
\end{aligned}
$$
These identities are useful in simplifying various expressions that appear in gauge theory.
We can express the structure constants as a trace
$$
\operatorname{Tr}\left(\left[T_{a}^{\text {def }}, T_{b}^{\text {def }}\right] T_{c}^{\text {def }}\right)=i B^{\text {def }} f_{a b c} .
$$
For example, the contractions of two structure constants then reads
$$
\begin{aligned}
&-\left(B^{\text {def }}\right)^{2} k^{c f} f_{a b c} f_{\text {def }} \\
=& k^{c f} \operatorname{Tr}\left(\left[T_{a}^{\text {def }}, T_{b}^{\text {def }}\right] T_{c}^{\text {def }}\right) \operatorname{Tr}\left(\left[T_{d}^{\text {def }}, T_{e}^{\text {def }}\right] T_{f}^{\text {def }}\right) \\
=& B^{\text {def }} \operatorname{Tr}\left(\left[T_{a}^{\text {def }}, T_{b}^{\text {def }}\right]\left[T_{d}^{\text {def }}, T_{e}^{\text {def }}\right]\right)
\end{aligned}
$$
The above completeness relation also has a useful graphical representation reminiscent of Feynman graphs and rules. Both identities can be written as
![[../math/Pasted image 20220126211944.png|400]]

Here a curly line depicts an algebra index and the directed straight line depicts the flow of the [[../math/defining representation of su(n|fundamental representation]].md). Inserting a matrix $X$ in two different places results in the above completeness relations which are thus equivalent.