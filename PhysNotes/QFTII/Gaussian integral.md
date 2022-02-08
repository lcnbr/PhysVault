---
alias:
- Gaußian integral
---
-$$\int_{-\infty}^{+\infty} \dd{p} \exp\qty(-\frac{1}{2} ap^2+bp+c)=\sqrt{\frac{2\pi}{a}}\exp\qty(\frac{b^2}{2a}+c).$$

# in n-dimensions

If $A$ is a symmetric positive-definite matrix, then (assuming all are colomn vectors)

$$\int \exp\left(-\frac{1}{2}\sum_{i,j=1}^{n}A_{ij} x_i x_j+\sum_{i=1}^{n}B_i x_i\right) d^n x
=\int e^{-\frac{1}{2}\vec{x}^\mathsf{T} \mathbf{A} \vec{x}+\vec{B}^\mathsf{T} \vec{x}} d^n x
= \sqrt{ \frac{(2\pi)^n}{\det{A}} }e^{\frac{1}{2}\vec{B}^\mathsf{T}\mathbf{A}^{-1}\vec{B}}$$