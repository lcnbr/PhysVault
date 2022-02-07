If we are over-confident we could now postulate the Feynman rules for Yang-Mills theory. 

When reading them off from a straight-forward non-abelian generalisation of the [[gauge fixing action for EM]],
$$
\mathrm{Z}[J]=\text { const } \cdot \int \mathrm{D} A \exp \left(i S_{\mathrm{YM}}[A, J]+i S_{\mathrm{gf}}[A]\right)
$$
we run into some problems. These can be seen in several ways:

![[Pasted image 20220126230408.png|400]]

We can consider the process of two matter particles annihilating into two vector particles

In the abelian process the resulting photons automatically have only physical polarisation vectors. This turns out not to hold in the nonabelian generalisation, some of the produced vector particles have unphysical polarisations. They arise from from the **third diagram which is not present for abelian gauge theory** (no gauge interaction). Such unphysical behaviour in a process is a reliable sign that something is wrong.

To some extent we may choose to ignore such contributions by projecting the external states to physical polarisations. This makes sense because the above construction applied to gauge-invariant quantities and configurations only. Nevertheless, this interpretation causes problems w.r.t. unitarity: The optical theorem relates the square of the above tree process to the imaginary part of a loop process.
![[Pasted image 20220126230635.png|300]]
- All the fields of the gauge-fixed formulation of the model propagate in loops. This includes the unphysical polarisation of the vector field.
- The truncated tree process discards the unphysical polarisations.
Consequently, unitarity fails or the loop contributions predicted by the path integral do not accurately describe quantum effects in YangMills theory.

A further clue is provided by the loop correction to the effective vertex of two gluons
![[Pasted image 20220126231628.png|400]]
In the abelian theory, the result turns out to be properly transverse and thus gauge-invariant
$$
M_{\mu \nu}^{(1)}(p)=M^{(1)}(p)\left(p^{2} \eta_{\mu \nu}-p_{\mu} p_{\nu}\right), \quad p^{v} M_{\mu \nu}^{(1)}(p)=0 .
$$

The non-abelian result, however, is not transverse
$$
M_{\mu \nu}^{(1)}(p)=M_{1}^{(1)}(p) p^{2} \eta_{\mu \nu}+M_{2}^{(1)}(p) p_{\mu} p_{\nu}, \quad p^{v} M_{\mu \nu}^{(1)}(p) \neq 0
$$
The violation of transversality can actually be traced to the second diagram involving only gluons.

It turns out that indeed loop effects are not correctly captured by a naive postulation of Feynman rules. We have to reinvestigate the quantisation and properly generalise it to non-abelian gauge theory.