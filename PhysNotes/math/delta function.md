---
alias:
- Dirac delta function
tags:
- qftII
---
> In mathematics, the Dirac delta distribution (δ distribution), also known as the unit impulse symbol, is a generalized function or distribution over the real numbers, whose value is zero everywhere except at zero, and whose integral over the entire real line is equal to one.The current understanding of the impulse is as a linear functional that maps every continuous function to its value at zero, or as the weak limit of a sequence of bump functions, which are zero over most of the real line, with a tall spike at the origin. Bump functions are thus sometimes called "approximate" or "nascent" delta distributions.
>
> The **delta function** was introduced by physicist Paul Dirac as a tool for the normalization of state vectors.  It also has uses in probability theory and signal processing.  As it is (or rather, was) not a true mathematical function, some mathematicians objected to it as nonsense until Laurent Schwartz developed the theory of distributions where it is defined as a linear form acting on bump functions. 
>
> The Kronecker delta function, which is usually defined on a discrete domain and takes values 0 and 1, is the discrete analog of the Dirac delta function.
>
> [Wikipedia](https://en.wikipedia.org/wiki/Dirac%20delta%20function)


![](https://upload.wikimedia.org/wikipedia/commons/thumb/4/48/Dirac_distribution_PDF.svg/2560px-Dirac_distribution_PDF.svg.png)

# Definitions

The Dirac delta can be loosely thought of as a function on the real line
which is zero everywhere except at the origin, where it is infinite,

:   $\delta(x) = \begin{cases} +\infty, & x = 0 \ 0, & x \ne 0 \end{cases}$

and which is also constrained to satisfy the identity

$$\int_{-\infty}^\infty \delta(x) \, dx = 1.$$

This is merely a [heuristic] characterization. The Dirac delta is not a
function in the traditional sense as no function defined on the real
numbers has these properties.
Dirac delta function can be rigorously defined either as a
[distribution] or as a [measure].

Originally: 
$$\begin{align}
f(x)&=\frac{1}{2\pi} \int_{-\infty}^\infty e^{ipx}\left(\int_{-\infty}^\infty e^{-ip\alpha }f(\alpha)\,d \alpha \right) \,dp \\[4pt]
&=\frac{1}{2\pi} \int_{-\infty}^\infty \left(\int_{-\infty}^\infty e^{ipx} e^{-ip\alpha } \,dp \right)f(\alpha)\,d \alpha =\int_{-\infty}^\infty \delta (x-\alpha) f(\alpha) \,d \alpha,
\end{align}$$

where the *δ*-function is expressed as

$$\delta(x-\alpha)=\frac{1}{2\pi} \int_{-\infty}^\infty e^{ip(x-\alpha)}\,dp \ .$$

# Properties

# Scaling and symmetry 

The delta function satisfies the following scaling property for a
non-zero scalar $\alpha$

$$\int_{-\infty}^\infty \delta(\alpha x)\,dx
=\int_{-\infty}^\infty \delta(u)\,\frac{du}{|\alpha|}
=\frac{1}{|\alpha|}$$

and so
$$\delta(\alpha x) = \frac{\delta(x)}{|\alpha|}.$$

Proof:

$$\begin{align}
\delta(\alpha x) &= \lim_{a \to 0} \frac{1}{|a|\sqrt{\pi}}e^{-(\alpha x/a)^2} \qquad \text{since } a \text{ is a dummy variable, we set } a=\alpha b \
&=\lim_{b \to 0} \frac{1}{|\alpha b|\sqrt{\pi}}e^{-(\alpha x/(\alpha b))^2} \
&=\lim_{b \to 0} \frac{1}{|\alpha|} \frac{1}{|b|\sqrt{\pi}}e^{-(x/b)^2} = \frac{1}{|\alpha|} \delta(x)
\end{align}$$

In particular, the delta function is an [even] distribution, in the
sense that

$$\delta(-x) = \delta(x)$$

which is [homogeneous] of degree −1.

## Algebraic properties 

The [distributional product] of $\delta$ with $x$ is equal to zero:

$$x\delta(x) = 0.$$

Conversely, if $1=xf(x) = xg(x)$,
where *f* and *g* are distributions, then

$$f(x) = g(x) +c \delta(x)$$

for some constant
$c$.

## Translation

The integral of the time-delayed Dirac delta is[^1]

$$\int_{-\infty}^\infty f(t) \delta(t-T)\,dt = f(T).$$

This is sometimes referred to as the *sifting property* or the
*sampling property*. The delta function is said to \"sift out\" the
value at $t=T$.

It follows that the effect of [convolving] a function $f(t)$ with the
time-delayed Dirac delta $\delta_T(t) = \delta(t-T)$ is to time-delay $f(t)$ by the same amount:

$$\begin{align} 
(f * \delta_T)(t) &= \int_{-\infty}^\infty f(\tau)
\delta(t-T-\tau)  \dd{\tau} \\ 
&= \int_{-\infty}^\infty f(\tau)
\delta(\tau-(T-t)) \dd{\tau}\\
&= f(t-T) \end{align}$$

This holds under the precise condition that *f* be a [tempered
distribution] (see the discussion of the Fourier transform [below]). As
a special case, for instance, we have the identity (understood in the
distribution sense)

$$\int_{-\infty}^\infty \delta (\xi-x) \delta(x-\eta) \, dx = \delta(\eta-\xi).$$

## Composition with a function 

More generally, the delta distribution may be [composed] with a smooth
function $g(x)$ in such a way that the familiar change of variables
formula holds, that

$$\int_{\mathbb{R}} \delta\bigl(g(x)\bigr) f\bigl(g(x)\bigr) \left|g'(x)\right| dx = \int_{g(\mathbb{R})} \delta(u)f(u)\, du$$

provided that $g$ is a [continuously differentiable] function with $g'$
nowhere
zero.
That is, there is a unique way to assign meaning to the distribution
$\delta\circ g$ so that this identity holds for all compactly supported
test functions $f$. Therefore, the domain must be broken up to exclude
the $g′ = 0$ point. This distribution satisfies
$1=δ(g(x)) = 0$ if *g* is nowhere zero,
and otherwise if *g* has a real [root] at *x*~0~, then

$$\delta(g(x)) = \frac{\delta(x-x_0)}{|g'(x_0)|}.$$

It is natural therefore to *define* the composition *δ*(*g*(*x*)) for
continuously differentiable functions *g* by

$$\delta(g(x)) = \sum_i \frac{\delta(x-x_i)}{|g'(x_i)|}$$

where the sum extends over all roots (i.e., all the different ones) of
*g*(*x*), which are assumed to be [simple]. Thus, for example

$$\delta\left(x^2-\alpha^2\right) = \frac{1}{2|\alpha|} \Big[\delta\left(x+\alpha\right)+\delta\left(x-\alpha\right)\Big].$$

In the integral form, the generalized scaling property may be written as

$$\int_{-\infty}^\infty f(x) \, \delta(g(x)) \, dx = \sum_{i}\frac{f(x_i)}{|g'(x_i)|}.$$

## Properties in *n* dimensions 

The delta distribution in an *n*-dimensional space satisfies the
following scaling property instead,

$$\delta(\alpha\mathbf{x}) = |\alpha|^{-n}\delta(\mathbf{x}) ~,$$ so
that *δ* is a [homogeneous] distribution of degree −*n*.

Under any [reflection] or [rotation] ρ, the delta function is invariant,

$$\delta(\rho \mathbf{x}) = \delta(\mathbf{x})~.$$

As in the one-variable case, it is possible to define the composition of
*δ* with a [bi-Lipschitz function]$\mathbb{R}^n\rightarrow \mathbb{R}^n$

## Fourier transform

The delta function is a [tempered distribution], and therefore it has a
well-defined [Fourier transform]. Formally, one finds[^1]

$$\widehat{\delta}(\xi)=\int_{-\infty}^\infty e^{-2\pi i x \xi}\delta(x)\,dx = 1.$$

Properly speaking, the Fourier transform of a distribution is defined by
imposing [self-adjointness] of the Fourier transform under the duality
pairing $\langle\cdot,\cdot\rangle$ of tempered distributions with
[Schwartz functions]. Thus $\widehat{\delta}$ is defined as the unique
tempered distribution satisfying

$$\langle\widehat{\delta},\varphi\rangle = \langle\delta,\widehat{\varphi}\rangle$$

for all Schwartz functions $\varphi$. And indeed it follows from this
that $\widehat{\delta}=1.$

As a result of this identity, the [convolution] of the delta function
with any other tempered distribution *S* is simply *S*:

$$S*\delta = S.$$

That is to say that *δ* is an [identity element] for the convolution on
tempered distributions, and in fact, the space of compactly supported
distributions under convolution is an [associative algebra] with
identity the delta function. This property is fundamental in [signal
processing], as convolution with a tempered distribution is a [linear
time-invariant system], and applying the linear time-invariant system
measures its [impulse response]. The impulse response can be computed to
any desired degree of accuracy by choosing a suitable approximation for
*δ*, and once it is known, it characterizes the system completely. 

The inverse Fourier transform of the tempered distribution *f*(*ξ*) = 1
is the delta function. Formally, this is expressed

$$\int_{-\infty}^\infty 1 \cdot e^{-2\pi i x\xi}\,d\xi = \delta(x)$$

and more rigorously, it follows since

$$\langle 1, \widehat{f}\rangle = f(0) = \langle\delta,f\rangle$$

for all Schwartz functions *f*.

In these terms, the delta function provides a suggestive statement of
the orthogonality property of the Fourier kernel on **$\mathbb{R}$**. Formally, one
has

$$\int_{-\infty}^\infty e^{i 2\pi \xi_1 t}  \left[e^{i 2\pi \xi_2 t}\right]^*\,dt = \int_{-\infty}^\infty e^{-i 2\pi (\xi_2 - \xi_1) t} \,dt = \delta(\xi_2 - \xi_1).$$

This is, of course, shorthand for the assertion that the Fourier
transform of the tempered distribution

$$f(t) = e^{i2\pi\xi_1 t}$$

is

$$\widehat{f}(\xi_2) = \delta(\xi_1-\xi_2)$$

which again follows by imposing self-adjointness of the Fourier
transform.

By [analytic continuation] of the Fourier transform, the [Laplace
transform] of the delta function is found to
be:   $$\int_{0}^{\infty}\delta (t-a)e^{-st} \, dt=e^{-sa}.$$