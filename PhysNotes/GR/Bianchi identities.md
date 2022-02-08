---
alias: 
- Bianchi identity
tag: GR physics
---
# Bianchi identities


You can prove the following Bianchi identity
$$
R_{\mu \nu \rho \sigma ; \tau}+R_{\mu \nu \tau \rho ; \sigma}+R_{\mu \nu \sigma \tau ; \rho}=0 .
$$
We can now multiply with $g^{\mu \rho}$. As we have that $g^{\mu \rho}{ }_{; \beta}=0$, we arrive at
$$
\begin{gathered}
R^\rho{}_{\nu \rho \sigma ; \tau}
+R^\rho{ }_{\nu \tau \rho ; \sigma}
+R^\rho{}_{\nu \sigma \tau ; \rho}=0 \\

R^{\rho}{ }_{\nu \rho \sigma ; \tau}
-R^\rho{}_{\nu \rho \tau ; \sigma}
+R^\rho{}_{\nu \sigma \tau ; \rho}=0 \\

\implies R_{\nu \sigma ; \tau}
-R_{\nu \tau ; \sigma}
+R^\rho{}_{\nu \sigma \tau ; \rho}=0
\end{gathered}
$$
Multiplying with $g^{\nu \sigma}$ we now get
$$
\begin{array}{r}
R_{; \tau}
-R^\sigma{}_{\tau ; \sigma}
+g^{\rho \beta} g^{\nu \sigma} R_{\beta \nu \sigma \tau ; \rho}=0 \\
R_{; \tau}
-R^\sigma{}_{\tau ; \sigma}
-g^{\rho \beta} g^{\nu \sigma} R_{\nu \beta \sigma \tau ; \rho}=0 \\
R_{; \tau}
-R^\sigma{}_{\tau ; \sigma}
+g^{\rho \beta} R_{\beta \tau ; \rho}=0 \\

2 R^\sigma{}_{\tau ; \sigma}-R_{; \tau}=0 \\

R_{\tau ; \sigma}^{\sigma}
-\frac{1}{2}\left(\delta^{\sigma}{ }_{\tau} R\right)_{; \sigma}=0 \\

\implies \left(R^\sigma{}_{\tau}
-\frac{1}{2} \delta^{\sigma}{ }_{\tau} R\right)_{; \sigma}=0
\end{array}
$$
Or equivalently:


$$\left(R^{\mu \nu}-\frac{1}{2} g^{\mu \nu} R\right)_{; \mu}=0$$