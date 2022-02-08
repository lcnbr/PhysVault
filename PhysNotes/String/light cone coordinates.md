
# In the [[worldsheet]]
$$\xi^{\mathrm{L} / \mathrm{R}}=\tau \mp \sigma, \quad \partial_{\mathrm{L} / \mathrm{R}}=\frac{1}{2}\left(\partial_{\tau} \mp \partial_{\sigma}\right)$$

They imply the [[spacetime interval]] is written:

$$
\mathrm{d} s^{2}=-\mathrm{d} \tau^{2}+\mathrm{d} \sigma^{2}=-\mathrm{d} \xi^{\mathrm{L}} \mathrm{d} \xi^{\mathrm{R}}
$$ 
## [[worldsheet#Embedding]] coordinates
We then write a separable function:
$$
X^{\mu}\left(\xi^{\mathrm{L}}, \xi^{\mathrm{R}}\right)=X_{\mathrm{L}}^{\mu}\left(\xi^{\mathrm{L}}\right)+X_{\mathrm{R}}^{\mu}\left(\xi^{\mathrm{R}}\right)
$$
# In [[embedding space|ambient space]]

Let us introduce light cone coordinates in [[worldsheet#Embedding]] space
$$
X^{\pm}=X^{0} \pm X^{D-1}
$$
where $\vec{X}$ denotes the transverse components $1 \ldots(D-2)$. 

Note that this choice picks out a particular time direction and a particular spatial direction. It means that any calculations that we do involving X± will not be manifestly Lorentz invariant. You might think that we needn’t really worry about this. We could try to make the following argument: “The equations may not look Lorentz invariant but, since we started from a Lorentz invariant theory, at the end of the day any physical process is guaranteed to obey this symmetry”. Right?! Well, unfortunately not. One of the more interesting and subtle aspects of quantum field theory is the possibility of [[anomaly|anomalies]]: these are symmetries of the classical theory that do not survive the journey of quantization. When we come to the quantum theory, if our equations don’t look Lorentz invariant then there’s a real possibility that it’s because the underlying physics actually isn’t Lorentz invariant. Later we will need to spend some time figuring out under what circumstances our quantum theory keeps the classical Lorentz symmetry. ^fff8df

 
In lightcone coordinates, the [[spacetime]] [[Minkowski metric]] reads
$$
d s^{2}=-2 d X^{+} d X^{-}+\sum_{i=1}^{D-2} d X^{i} d X^{i}
$$
This means that indices are raised and lowered with $A_{+}=-A^{-}$and $A_{-}=-A^{+}$and $A_{i}=A^{i} .$ The product of [[spacetime]] vectors reads $A \cdot B=-A^{+} B^{-}-A^{-} B^{+}+A^{i} B^{i} .$ ^a95469