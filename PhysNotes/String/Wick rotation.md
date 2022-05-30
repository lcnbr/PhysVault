---
alias:
tags:
- qftII
- stringTheory
---
> In physics, **Wick rotation**, named after Italian physicist Gian Carlo Wick, is a method of finding a solution to a mathematical problem in Minkowski space from a solution to a related problem in Euclidean space by means of a transformation that substitutes an imaginary-number variable for a real-number variable. This transformation is also used to find solutions to problems in quantum mechanics and other areas.
>
> [Wikipedia](https://en.wikipedia.org/wiki/Wick%20rotation)

Wick rotation is motivated by the observation that the [Minkowski metric](https://en.wikipedia.org/wiki/Minkowski_metric "Minkowski metric") in natural units (with [metric signature](https://en.wikipedia.org/wiki/Metric_signature "Metric signature") (−1, +1, +1, +1) [[1 Intro and Motivation/1.1 Point to string/Conventions]])

![[dt^{2}\right)+dx^{2}+dy^{2}+dz^{2}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/04dc2ca3d71d46992aa7d4e07865f5fd47a22fc5|{\displaystyle ds^{2}=-\left(dt^{2}\right)+dx^{2}+dy^{2}+dz^{2}}]]

and the four-dimensional Euclidean metric

![ds^{2}=d\tau ^{2}+dx^{2}+dy^{2}+dz^{2}](https://wikimedia.org/api/rest_v1/media/math/render/svg/3822141f73cf2a944b7fe8d26fb72590832db8a2)

are equivalent if one permits the coordinate t to take on [imaginary](https://en.wikipedia.org/wiki/Imaginary_number "Imaginary number") values. The Minkowski metric becomes Euclidean when t is restricted to the [imaginary axis](https://en.wikipedia.org/wiki/Imaginary_number "Imaginary number"), and vice versa. Taking a problem expressed in Minkowski space with coordinates x, y, z, t, and substituting _t_ = −_iτ_ sometimes yields a problem in real Euclidean coordinates x, y, z, τ which is easier to solve. This solution may then, under reverse substitution, yield a solution to the original problem.

# In [[7 CFT/conformal field theory|CFT]]
In the context of [[7 CFT/conformal field theory]], the [[worldsheet]] is conventionally taken to have [[euclidean signature]]. In order to get there, perform the [[.md|Wick rotation]] $\tau=-i \tilde{\tau}$ (now $\tilde{\tau}$ is real) and define

$$
\exp \left(i \xi^{\mathrm{L}}\right)=\exp (\tilde{\tau}-i \sigma)=: \bar{z}, \quad \exp \left(i \xi^{\mathrm{R}}\right)=\exp (\tilde{\tau}+i \sigma)=: z .
$$

The result of this change are cylindrical coordinates for the (euclidean) string:

![[Wick rotation_2022-01-22 12.38.41.excalidraw||center]]

The radius $|z|$ denotes the exponential euclidean time $\tilde{\tau}$, while $\sigma$ is mapped to the (naturally periodic) angular coordinate. These coordinates are the standard ones for a euclidean quantum field theory: the [[worldsheet]] coordinates $z$ and $\bar{z}$ are complex conjugates and the fields are functions $f(z, \bar{z})$ of complex $z$. 
## [[worldsheet#Embedding]]


[[3 Classical Bosonic String/Polyakov action#^b37d90|Splitting of the string coordinates]] into a [[light cone coordinates#In the worldsheet|right and a left part]] is replaced by considering a holomorphic and a anti-holomorphic part:

$$
X(z, \bar{z})=X(z)+\bar{X}(\bar{z}) \text {. }
$$

Why is it favourable to use this language? Firstly, [[conformal transformations]] preserve holomorphicity, that is, they do not mix the functions $X(z)$ and $\bar{X}(\bar{z})$. Secondly (and most importantly) one can now employ the powerful tools of complex functional analysis, e.g. residue theorems.

The derivatives are now denoted: $\partial_\mathrm{R}\rightarrow\partial = \frac{\partial}{\partial z}$ and $\partial_\mathrm{L}\rightarrow\bar{\partial} = \frac{\partial}{\partial \bar{z}}$ 

## [[conformal transformations#Action on Coordinates|^|]] 
are now: 
+ infinitesimal boosts $\delta(z, \bar{z})=\left(\epsilon z^{2}, \bar{\epsilon} \bar{z}^{2}\right)$
+ scaling: $(z, \bar{z}) \rightarrow(z +s z, \bar{z}+\bar{s} \bar{z})$ with $s\in \mathbb{R}$
    + Infinistesimally: $\delta(z, \bar{z})=(\epsilon z, \bar{\epsilon} z)$ with $\epsilon\in \mathbb{R}$
+ Rotation: $(z, \bar{z}) \rightarrow(z +r z, \bar{z}+\bar{r} \bar{z})$ with $r\in \mathring\imath\mathbb{R}$ that is fully imaginary
    + Infinistesimally: $\delta(z, \bar{z})=(\epsilon z, \bar{\epsilon} z)$ with $\epsilon\in \mathring\imath\mathbb{R}$
