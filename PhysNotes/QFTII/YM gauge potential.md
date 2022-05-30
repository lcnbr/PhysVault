# Gauge potential

Since the [[YM covariant derivative]] is [[YM covariant derivative#^dbef82|gauge covariant]],
The gauge potential $A_{\mu}$ must therefore transform according to

$$
A_{\mu}^{\prime}=U A_{\mu} U^{-1}+i U\left(\partial_{\mu} U^{-1}\right)
$$


This shows that the gauge potential itself must be an $N \times N$ matrix. However, we can restrict it further by imposing a reality condition. The reality condition must be compatible with the gauge transformation rule. We make use of the [[../math/unitary matrix|unitary properties]] of $U$ and write the transformation of the hermitian conjugate of the potential $A^{\mu}$
$$
\left(A_{\mu}^{\prime}\right)^{\dagger}=U A_{\mu}^{\dagger} U^{-1}-i\left(\partial_{\mu} U\right) U^{-1} .
$$
We note that $0=\left(\partial_{\mu}\left(U U^{-1}\right)\right)=\left(\partial_{\mu} U\right) U^{-1}+U\left(\partial_{\mu} U^{-1}\right) .$ Altogether it shows that $A_{\mu}^{\dagger}$ transforms exactly as $A_{\mu}$ itself, and therefore the gauge transformation is consistent with the assumption of a hermitian gauge potential
$$
A_{\mu}^{\dagger}=A_{\mu}
$$
Consequently, it makes sense to impose this property on the gauge field in order to reduce its independent components to a minimum.