---
alias:
- tensor
- contract
tag: SR GR physics
---
We can define objects with multiple indices that we call tensors
$$
T^{\mu_{1} \mu_{2} \cdots}{ }_{\nu_{1} \nu_{2} \cdots} .
$$
Tensors include products of vectors and transform as such under a [[../String/Lorentz transformation]]
$$
(T^{ \mu_{1} \mu_{2} \cdots}{ }_{\nu_{1} \nu_{2} \cdots})'=\Lambda^{\mu_{1}}{ }_{\alpha_{1}} \Lambda^{\mu_{2}}{}_{\alpha_{2}} \cdots \Lambda_{\nu_{1}}{ }^{\beta_{1}} \Lambda_{\nu_{2}}{ }^{\beta_{2}} \cdots T^{\alpha_{1} \alpha_{2} \cdots}{ }_{\beta_{1} \beta_{2} \cdots} .
$$

# Forming tensors from other tensors

- **Linear Combinations:** A linear combination of tensors with the same upper and lower indices is a tensor with these indices. For instance, if $R_{\beta}^{\alpha}$ and $S_{\beta}^{x}$ are tensors, and $a$ and $b$ are scalars, and we define
$$
T^{\alpha}{}_{\beta} \equiv a R^{\alpha}{ }_{\beta}+b B^{\alpha}{ }_{\beta}
$$
then $T^{\alpha}{}_{\beta}$ is a tensor, that is,
$$
\begin{aligned}
(T^{\alpha}{}_{\beta})' & \equiv a (R^\alpha{}_{\beta})^{\prime }+b (B^{\alpha}{ }_{\beta})' \\
&=a \Lambda^\alpha{}_\mu \Lambda_\beta{}^\nu R^\mu{}_{\nu}+b \Lambda^\alpha{}_\mu \Lambda_\beta{}^\nu B^{\alpha}{ }_{\beta} \\
&=\Lambda^\alpha{}_\mu \Lambda_\beta{}^\nu T^{\mu}{}_{\nu}
\end{aligned}
$$
-  **Direct Products:** The product of the components of two tensors yields a tensor whose upper and lower indices consist of all the upper and lower indices of the two original tensors. For instance, if $A^{\alpha}{}_{\beta}$ and $B^{\gamma}$ are tensors, and$$
T^\alpha{}_{\beta}{}^\gamma \equiv A^{\alpha}{}_{\beta} B^{\gamma}
$$then $T^\alpha{}_{\beta}{}^\gamma$ is a tensor, that is,
$$
\begin{aligned}
(T^\alpha{}_{\beta}{}^\gamma)^\prime &=(A^{\alpha}{}_{\beta} )' (B^{\gamma})'\\
&=\Lambda^\alpha{}_\mu \Lambda_\beta{}^\nu  \Lambda^\gamma{}_\rho T^{\mu}{}_{\nu}{}^{\rho}
\end{aligned}
$$
- **Contraction:** Setting an upper and lower index equal and summing it over its values $0,1,2,3$, yields a tensor with these two indices absent. For instance, if $T^\alpha{}_\beta{}^\gamma{}^\delta$ is a tensor and
$$
T^\alpha{}^\gamma=T^\alpha{}_\mathbf{\beta}{}^\gamma{}^{\beta}
$$
then $T^{\alpha \gamma}$ is a tensor, that is,$$(T^{\alpha \gamma})'=(T^\alpha{}_\beta{}^\gamma{}^\beta)'=\Lambda^\alpha{}_\mu \underbracket{\Lambda_\beta{}^\nu} \Lambda^\gamma{}_\rho \overbracket{ \Lambda^\beta{}_\sigma} T^\mu{}_\nu{}^\rho{}^\sigma=\Lambda^\alpha{}_\mu \Lambda^\gamma{}_\rho \delta^\nu_\sigma T^\mu{}_\nu{}^\rho{}^\sigma=\Lambda^\alpha{}_\mu \Lambda^\gamma{}_\rho T^{\mu \rho}$$
- **Differentiation:** The derivative $\partial / \partial x^{\alpha}$ of any tensor is a tensor with one additional lower index $\alpha$. For instance, if $T^{\beta \gamma}$ is a tensor and
$$
T_{\alpha}{ }^{\beta \gamma} \equiv \pdv{}{ x^{\alpha}} T^{\beta \gamma}
$$
then $T_{\alpha}{}^{\beta \gamma}$ is a tensor, that is,
$$(T_{\alpha}{}^{\beta \gamma})'= \pdv{}{ (x^{\alpha})'} (T^{\beta \gamma})'=\Lambda_\alpha{}^\mu \pdv{x^\mu} \Lambda^\beta{}_\nu \Lambda^\gamma{}_\rho T^{\nu \rho}=\Lambda_\alpha{}^\mu  \Lambda^\beta{}_\nu \Lambda^\gamma{}_\rho T_\mu{}^{\nu \rho}$$


Now we have already encountered some [[.md|tensors]] for example:
- Metric $\eta_{\mu \nu}$ : This is a covariant tensor, as can be seen from the definition of the [[../String/Lorentz transformation]]
$$
(\eta_{\rho \sigma})^{\prime}=\eta_{\mu \nu} \Lambda^{\mu}{ }_{\rho} \Lambda^{\nu}{ }_{\sigma}=\eta_{\rho \sigma} .
$$
- Kronecker-delta: This is a tensor with one contravariant and one covariant index. Indeed,

$$
\begin{aligned}
\delta^{\mu}_{\nu} \rightarrow (\delta^{ \mu}_{\nu})' &=\Lambda^{\mu}{ }_{\rho} \Lambda_{\nu}{ }^{\sigma} \delta^{\rho}_{\sigma} \\
&=\underbracket{\Lambda^{\mu}{ }_{\rho} \Lambda_{\nu}{ }^{\rho}}_{\mathbb{1}}=\delta^{\mu}_{\nu} .
\end{aligned}
$$
- Levi-Civita tensor: This is defined as a fully antisymmetric tensor with
$$
\varepsilon^{\alpha \beta \gamma \delta}=\left\{
\begin{aligned}
+1 & \quad \text{if }\alpha \beta \gamma \delta  \text { is an even permutation of } 0123 \\
-1 & \quad \text{if }\alpha \beta \gamma \delta \text { is an odd permutation of } 0123 \\
0 & \quad \text { otherwise. }
\end{aligned}\right.
$$
The Levi-Civita symbol is a tensor. Let us transform it accordingly,
$$
\varepsilon^{\alpha \beta \gamma \delta} \rightarrow (\varepsilon^{\alpha \beta \gamma \delta})'=\Lambda^{\alpha}{}{}_{\mu} \Lambda^{\beta}{}_{\nu} \Lambda^{\gamma}{}_{\rho}\Lambda^{\delta}{}_{\sigma} \varepsilon^{\mu \nu \rho \sigma}
$$
The right-hand-side is fully antisymmetric in the $\alpha \beta \gamma \delta$ indices and thus:$$ \Lambda^{\alpha}{}{}_{\mu} \Lambda^{\beta}{}_{\nu} \Lambda^{\gamma}{}_{\rho}\Lambda^{\delta}{}_{\sigma} \varepsilon^{\mu \nu \rho \sigma}\propto\varepsilon^{\alpha \beta \gamma \delta}$$ Let us calculate it concretely for $\alpha \beta \gamma \delta=0123$
$$
\Lambda^{0}{}_{\mu} \Lambda^{1}{}_{\nu} \Lambda^{2}{}_{\rho}\Lambda^{3}{}_{\sigma} \varepsilon^{\mu \nu \rho \sigma},
$$
and for $\alpha \beta \gamma \delta=1023$
$$
\Lambda^{1}{}_{\mu} \Lambda^{0}{}_{\nu} \Lambda^{2}{}_{\rho}\Lambda^{3}{}_{\sigma} \varepsilon^{\mu \nu \rho \sigma}=-\Lambda^{0}{}_{\mu} \Lambda^{1}{}_{\nu} \Lambda^{2}{}_{\rho}\Lambda^{3}{}_{\sigma} \varepsilon^{\mu \nu \rho \sigma} 
$$
Thus: 
$$
\begin{aligned}
\Lambda^{1}{}_{\mu} \Lambda^{0}{}_{\nu} \Lambda^{2}{}_{\rho}\Lambda^{3}{}_{\sigma} \varepsilon^{\mu \nu \rho \sigma} &=\text { constant } \cdot \varepsilon^{0123} \\
\rightarrow \operatorname{det} \Lambda &=\text { constant } \cdot(+1)
\end{aligned}
$$
Since we are only considering proper [[../String/Lorentz transformation|Lorentz transformations]] $\operatorname{det} \Lambda=1$ and we have
$$
\varepsilon^{\prime \alpha \beta \gamma \delta}=\Lambda_{\mu}^{\alpha} \Lambda_{\nu}^{\beta} \Lambda_{\rho}^{\gamma} \Lambda_{\sigma}^{\delta} \varepsilon^{\mu \nu \rho \sigma}=\varepsilon^{\alpha \beta \gamma \delta} .
$$
Notice that for [[general coordinate transformation|general coordinate transformations]] that will be needed in General Relativity $\operatorname{det} \Lambda$ cis not necessarily 1 and the Levi-Civita symbol is no longer a tensor. (rather a "[[densities|tensor density]]".)