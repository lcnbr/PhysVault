---
Alias:
- Legendre transformation
---
[[rowec-zotero#^d7ebeb]]

# 1-d
In one dimension we have $f^{*}(p)=f(x)-p x$, where $x=\left(f^{\prime}\right)^{-1}(p)$

# In several dimensions 
we have $f^{*}(p)=f(x)-p \cdot x$, where $x=(\nabla f)^{-1}(p)$

Suppose we start with a function $f (x_1, x_2,\dots, x_n)$ want to replace a subset$\left\{x_i, i = 1,\dots, j\right\}$ with different variables $u_i$ where:

$$u_i= \frac{\partial f}{\partial x_i} $$ ^e320f3

The [[Legendre transform]] transform of $f$ is:
 $$g(u_1,\dots, u_j,x_{j+1},\dots,x_n):=\sum\limits_{i=1}^{j}u_ix_i-f(x_1, x_2,\dots, x_n)$$ ^0bf46f
 
 Assuming that all the $x_i$ in the set $\left\{x_i, i = 1,\dots , j\right\}$ can be written as functions of $\left\{u_1,\dots, u_j,x_{j+1},\dots,x_n\right\}$
 Taking the derivative:
 
 $$\begin{aligned}
\frac{\partial g}{\partial u_{i}} &=x_{i}+\sum_{k=1}^{j}\left[u_{k} \frac{\partial x_{k}}{\partial u_{i}}-\frac{\partial f}{\partial x_{k}} \frac{\partial x_{k}}{\partial u_{i}}\right] \\
&=x_{i}+\sum_{k=1}^{j}\left[u_{k} \frac{\partial x_{k}}{\partial u_{i}}-u_{k} \frac{\partial x_{k}}{\partial u_{i}}\right] \\
&=x_{i}
\end{aligned}$$

^56190e
# For functionals (cont. dimensions)
In continuous dimensions we then should have $f^{*}(p)=f(x)-\langle p, x\rangle$, where $x=(\delta f)^{-1}(p)$ with $\delta f$
being the functional derivative of $f$.
In other notation:
$$
F^{*}[g]=F[f]-\int g(x) f(x) d x
$$
where $f(x)=\left(\frac{\delta F}{\delta f(x)}\right)^{-1}[g] .$


