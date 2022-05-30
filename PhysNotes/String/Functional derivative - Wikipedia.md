In the [calculus of variations](https://en.wikipedia.org/wiki/Calculus_of_variations "Calculus of variations"), a field of [mathematical analysis](https://en.wikipedia.org/wiki/Mathematical_analysis "Mathematical analysis"), the **functional derivative** (or **variational derivative**)[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-GiaquintaHildebrandtP18-1]] relates a change in a [functional](https://en.wikipedia.org/wiki/Functional_(mathematics) "Functional (mathematics)") (a functional in this sense is a function that acts on functions) to a change in a [function](https://en.wikipedia.org/wiki/Function_(mathematics) "Function (mathematics)") on which the functional depends.

In the calculus of variations, functionals are usually expressed in terms of an [integral](https://en.wikipedia.org/wiki/Integral "Integral") of functions, their [arguments](https://en.wikipedia.org/wiki/Argument_of_a_function "Argument of a function"), and their [derivatives](https://en.wikipedia.org/wiki/Derivative "Derivative"). In an integral _L_ of a functional, if a function _f_ is varied by adding to it another function _δf_ that is arbitrarily small, and the resulting integrand is expanded in powers of _δf_, the coefficient of _δf_ in the first order term is called the functional derivative.

For example, consider the functional

![[\,x,f(x),f\,'(x)\,)\,dx\ ,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/68be973ffd7b1b84391c61f2dcacd0ecf74ca766|{\displaystyle J[f]]

where _f_ ′(_x_) ≡ _df/dx_. If _f_ is varied by adding to it a function _δf_, and the resulting integrand _L_(_x, f +δf, f '+δf_ ′) is expanded in powers of _δf_, then the change in the value of _J_ to first order in _δf_ can be expressed as follows:[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-GiaquintaHildebrandtP18-1]][[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-2]]

![[{\frac {\partial L}{\partial f}}\delta f(x)+{\frac {\partial L}{\partial f'}}{\frac {d}{dx}}\delta f(x)\right)\,dx\,=\int _{a}^{b}\left({\frac {\partial L}{\partial f}}-{\frac {d}{dx}}{\frac {\partial L}{\partial f'}}\right)\delta f(x)\,dx\,+\,{\frac {\partial L}{\partial f'}}(b)\delta f(b)\,-\,{\frac {\partial L}{\partial f'}}(a)\delta f(a)\,}](https://wikimedia.org/api/rest_v1/media/math/render/svg/0a158226d573ac9354c92c290fb21e7c6830e566|{\displaystyle \delta J=\int _{a}^{b}\left({\frac {\partial L}{\partial f}}\delta f(x)+{\frac {\partial L}{\partial f'}}{\frac {d}{dx}}\delta f(x)\right)\,dx\,=\int _{a}^{b}\left({\frac {\partial L}{\partial f}}-{\frac {d}{dx}}{\frac {\partial L}{\partial f'}}\right)\delta f(x)\,dx\,+\,{\frac {\partial L}{\partial f'}}(b)\delta f(b)\,-\,{\frac {\partial L}{\partial f'}}(a)\delta f(a)\,}]]

where the variation in the derivative, _δf_ ′ was rewritten as the derivative of the variation (_δf_) ′, and [integration by parts](https://en.wikipedia.org/wiki/Integration_by_parts "Integration by parts") was used.

## Definition\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=1 "Edit section: Definition")\]

In this section, the functional derivative is defined. Then the functional differential is defined in terms of the functional derivative.

### Functional derivative\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=2 "Edit section: Functional derivative")\]

Given a [manifold](https://en.wikipedia.org/wiki/Manifold "Manifold") _M_ representing ([continuous](https://en.wikipedia.org/wiki/Continuous_function_(topology) "Continuous function (topology)")/[smooth](https://en.wikipedia.org/wiki/Smooth_function "Smooth function")) functions _ρ_ (with certain [boundary conditions](https://en.wikipedia.org/wiki/Boundary_condition "Boundary condition") etc.), and a [functional](https://en.wikipedia.org/wiki/Functional_(mathematics) "Functional (mathematics)") _F_ defined as

![F\colon M \rightarrow \mathbb{R} \quad \mbox{or} \quad F\colon M \rightarrow \mathbb{C} \, ,](https://wikimedia.org/api/rest_v1/media/math/render/svg/619e4ea211514bac49c0fbf890ba895cf0e8b358)

the **functional derivative** of _F_\[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-ParrYangP246A.2-3]]

![[x)\phi (x)\;dx&=\lim _{\varepsilon \to 0}{\frac {F[\rho +\varepsilon \phi ]-F[\rho ]}{\varepsilon }}\\&=\left[{\frac {d}{d\varepsilon }}F[\rho +\varepsilon \phi ]\right]_{\varepsilon =0},\end{aligned}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/132e1da8f763ed918cb58f7d83cd4c108acc888f|{\displaystyle {\begin{aligned}\int {\frac {\delta F}{\delta \rho }}(x)\phi (x)\;dx&=\lim _{\varepsilon \to 0}{\frac {F[\rho +\varepsilon \phi ]]

where ![\phi ](https://wikimedia.org/api/rest_v1/media/math/render/svg/72b1f30316670aee6270a28334bdf4f5072cdde4) is an arbitrary function. The quantity ![{\displaystyle \varepsilon \phi }](https://wikimedia.org/api/rest_v1/media/math/render/svg/d985d11fd66f00c42d03a6925abb23d8ae319292) is called the variation of _ρ_.

In other words,

![{\displaystyle \phi \mapsto \left[{\frac {d}{d\varepsilon }}F[\rho +\varepsilon \phi ]\right]_{\varepsilon =0}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/8b1ada65ccea3070c2f498355c7e01f1a82b1fb7)

is a linear functional, so one may apply the [Riesz–Markov–Kakutani representation theorem](https://en.wikipedia.org/wiki/Riesz%E2%80%93Markov%E2%80%93Kakutani_representation_theorem "Riesz–Markov–Kakutani representation theorem") to represent this functional as integration against some [measure](https://en.wikipedia.org/wiki/Measure_(mathematics) "Measure (mathematics)"). Then _δF_/_δρ_ is defined to be the [Radon–Nikodym derivative](https://en.wikipedia.org/wiki/Radon%E2%80%93Nikodym_derivative "Radon–Nikodym derivative") of this measure.

One thinks of the function _δF_/_δρ_ as the gradient of _F_ at the point _ρ_ and

![[x) \phi(x) \; dx](https://wikimedia.org/api/rest_v1/media/math/render/svg/50360a6873c3b76ccb1bf161fedf5ec9728e205f|\int \frac{\delta F}{\delta\rho}(x) \phi(x) \; dx]]

as the directional derivative at point _ρ_ in the direction of _ϕ_. Then analogous to vector calculus, the inner product with the gradient gives the directional derivative.

### Functional differential\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=3 "Edit section: Functional differential")\]

The differential (or variation or first variation) of the functional ![{\displaystyle F\left[\rho \right]}](https://wikimedia.org/api/rest_v1/media/math/render/svg/b5f2b97341e91c7e096b9fdb0cfa2cd7294b2afc) is [[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-ParrYangP246A.1-4]] [[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-5]]

![[x)\ \phi (x)\ dx\ .}](https://wikimedia.org/api/rest_v1/media/math/render/svg/1d7e377793bd3f8a8deb912eb0199638f4c2975a|{\displaystyle \delta F[\rho ;\phi ]]

Heuristically, ![\phi ](https://wikimedia.org/api/rest_v1/media/math/render/svg/72b1f30316670aee6270a28334bdf4f5072cdde4) is the change in ![\rho ](https://wikimedia.org/api/rest_v1/media/math/render/svg/1f7d439671d1289b6a816e6af7a304be40608d64), so we 'formally' have ![\phi =\delta \rho ](https://wikimedia.org/api/rest_v1/media/math/render/svg/072cafb6fc9caf296796ed601c8bc2bdcd3e99e1), and then this is similar in form to the [total differential](https://en.wikipedia.org/wiki/Total_differential "Total differential") of a function ![[\rho _{1},\rho _{2},\dots ,\rho _{n})}](https://wikimedia.org/api/rest_v1/media/math/render/svg/71fc74ad4256da18bb0aa5b452f488ba10ddf6d2|{\displaystyle F(\rho _{1},\rho _{2},\dots ,\rho _{n})}]],

![ dF =   \sum_{i=1} ^n  \frac {\partial F} {\partial \rho_i} \ d\rho_i  \ ,](https://wikimedia.org/api/rest_v1/media/math/render/svg/d42e2d895d30e7b4d8888ee7b6f6ffc6a1e8dc52)

where ![{\displaystyle \rho _{1},\rho _{2},\dots ,\rho _{n}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/18e9dfc44cd0a2ab384e0f5ba57fe40959545ca7) are independent variables. Comparing the last two equations, the functional derivative ![[x)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/fe130f00d494d704fe53af2533436aee5a1f8f26|{\displaystyle \delta F/\delta \rho (x)}]] has a role similar to that of the partial derivative ![{\displaystyle \partial F/\partial \rho _{i}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/609308f616a84019fcea5797e0936c6c3859f3c0), where the variable of integration ![x](https://wikimedia.org/api/rest_v1/media/math/render/svg/87f9e315fd7e2ba406057a97300593c4802b53e4) is like a continuous version of the summation index ![i](https://wikimedia.org/api/rest_v1/media/math/render/svg/add78d8608ad86e54951b8c8bd6c8d8416533d20).[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-ParrYangP246-6]]

## Properties\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=4 "Edit section: Properties")\]

Like the derivative of a function, the functional derivative satisfies the following properties, where _F_\[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-7]]

-   Linearity:[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-ParrYangP247A.3-8]]

![[\lambda F+\mu G)[\rho ]}{\delta \rho (x)}}=\lambda {\frac  {\delta F[\rho ]}{\delta \rho (x)}}+\mu {\frac  {\delta G[\rho ]}{\delta \rho (x)}},](https://wikimedia.org/api/rest_v1/media/math/render/svg/a3855d2be1b75c59c9da233cf9c8c71eeed66eaf|{\frac  {\delta (\lambda F+\mu G)[\rho ]]

where _λ_, _μ_ are constants.

-   Product rule:[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-ParrYangP247A.4-9]]

![[FG)[\rho ]}{\delta \rho (x)}}={\frac  {\delta F[\rho ]}{\delta \rho (x)}}G[\rho ]+F[\rho ]{\frac  {\delta G[\rho ]}{\delta \rho (x)}}\,,](https://wikimedia.org/api/rest_v1/media/math/render/svg/ee0421ecdfb105f4b62dcbd729c20e8ca587bda2|{\frac  {\delta (FG)[\rho ]]

-   Chain rules:

If _F_ is a functional and _G_ another functional, then[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-10]]

![[y)}  = \int dx \frac{\delta F[G]}{\delta G(x)}_{G = G[\rho]}\cdot\frac {\delta G[\rho](x|\displaystyle\frac{\delta F[G[\rho]]} {\delta\rho(y)} \ . ](https://wikimedia.org/api/rest_v1/media/math/render/svg/0e0aabc7b3b65317e5567d152a86c9c3adefc3fc)

If _G_ is an ordinary differentiable function (local functional) _g_, then this reduces to[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-11]]

![[\rho )]}{\delta \rho (y)}}={\frac {\delta F[g(\rho )]}{\delta g[\rho (y)]}}\ {\frac {dg(\rho )}{d\rho (y)}}\ .}](https://wikimedia.org/api/rest_v1/media/math/render/svg/2ceb8c9983e83b468694e9eb59635b8ff9ea924a|{\displaystyle \displaystyle {\frac {\delta F[g(\rho )]]

## Determining functional derivatives\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=5 "Edit section: Determining functional derivatives")\]

A formula to determine functional derivatives for a common class of functionals can be written as the integral of a function and its derivatives. This is a generalization of the [Euler–Lagrange equation](https://en.wikipedia.org/wiki/Euler%E2%80%93Lagrange_equation "Euler–Lagrange equation"): indeed, the functional derivative was introduced in [physics](https://en.wikipedia.org/wiki/Physics "Physics") within the derivation of the [Lagrange](https://en.wikipedia.org/wiki/Joseph-Louis_Lagrange "Joseph-Louis Lagrange") equation of the second kind from the [principle of least action](https://en.wikipedia.org/wiki/Principle_of_least_action "Principle of least action") in [Lagrangian mechanics](https://en.wikipedia.org/wiki/Lagrangian_mechanics "Lagrangian mechanics") (18th century). The first three examples below are taken from [density functional theory](https://en.wikipedia.org/wiki/Density_functional_theory "Density functional theory") (20th century), the fourth from [statistical mechanics](https://en.wikipedia.org/wiki/Statistical_mechanics "Statistical mechanics") (19th century).

### Formula\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=6 "Edit section: Formula")\]

Given a functional

![[ \boldsymbol{r}, \rho(\boldsymbol{r}), \nabla\rho(\boldsymbol{r}) )\, d\boldsymbol{r},](https://wikimedia.org/api/rest_v1/media/math/render/svg/984500e18fa20fadb9f03147b92b046a166aafc7|F[\rho]]

and a function _ϕ_(**_r_**) that vanishes on the boundary of the region of integration, from a previous section [[https://en.wikipedia.org/wiki/Functional_derivative#Definition "Functional derivative"]],

![
\begin{align}
\int \frac{\delta F}{\delta\rho(\boldsymbol{r})} \, \phi(\boldsymbol{r}) \, d\boldsymbol{r}  
&  = \left [ \frac{d}{d\varepsilon} \int f( \boldsymbol{r}, \rho + \varepsilon \phi, \nabla\rho+\varepsilon\nabla\phi )\, d\boldsymbol{r} \right ]_{\varepsilon=0} \\
&  = \int \left( \frac{\partial f}{\partial\rho} \, \phi + \frac{\partial f}{\partial\nabla\rho} \cdot \nabla\phi \right) d\boldsymbol{r} \\
&  = \int \left[ \frac{\partial f}{\partial\rho} \, \phi + \nabla \cdot \left( \frac{\partial f}{\partial\nabla\rho} \, \phi \right) - \left( \nabla \cdot \frac{\partial f}{\partial\nabla\rho} \right) \phi \right] d\boldsymbol{r} \\
&  = \int \left[ \frac{\partial f}{\partial\rho} \, \phi - \left( \nabla \cdot \frac{\partial f}{\partial\nabla\rho} \right) \phi \right] d\boldsymbol{r} \\
&  = \int \left( \frac{\partial f}{\partial\rho} -  \nabla \cdot \frac{\partial f}{\partial\nabla\rho} \right) \phi(\boldsymbol{r}) \ d\boldsymbol{r} \, .
\end{align}
](https://wikimedia.org/api/rest_v1/media/math/render/svg/364480cb1cb7bbad967750d4f4c2b2baa061f134)

The second line is obtained using the [total derivative](https://en.wikipedia.org/wiki/Total_derivative "Total derivative"), where _∂f_ /_∂∇__ρ_ is a [[https://en.wikipedia.org/wiki/Matrix_calculus#Scalar-by-vector "Matrix calculus"]].[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-12]]

The third line was obtained by use of a [[https://en.wikipedia.org/wiki/Divergence#Properties "Divergence"]]. The fourth line was obtained using the [divergence theorem](https://en.wikipedia.org/wiki/Divergence_theorem "Divergence theorem") and the condition that _ϕ_\=0 on the boundary of the region of integration. Since _ϕ_ is also an arbitrary function, applying the [fundamental lemma of calculus of variations](https://en.wikipedia.org/wiki/Fundamental_lemma_of_calculus_of_variations "Fundamental lemma of calculus of variations") to the last line, the functional derivative is

![
\frac{\delta F}{\delta\rho(\boldsymbol{r})} = \frac{\partial f}{\partial\rho} - \nabla \cdot \frac{\partial f}{\partial\nabla\rho} 
](https://wikimedia.org/api/rest_v1/media/math/render/svg/22ee5ae13b023dfb79c4ce74ae1c462d0df9b8c0)

where _ρ_ = _ρ_(**_r_**) and _f_ = _f_ (**_r_**, _ρ_, ∇_ρ_). This formula is for the case of the functional form given by _F_\[[https://en.wikipedia.org/wiki/Functional_derivative#Coulomb_potential_energy_functional "Functional derivative"]].)

The above equation for the functional derivative can be generalized to the case that includes higher dimensions and higher order derivatives. The functional would be,

![
F[\rho(\boldsymbol{r})] = \int f( \boldsymbol{r}, \rho(\boldsymbol{r}), \nabla\rho(\boldsymbol{r}), \nabla^{(2)}\rho(\boldsymbol{r}), \dots, \nabla^{(N)}\rho(\boldsymbol{r}))\, d\boldsymbol{r},
](https://wikimedia.org/api/rest_v1/media/math/render/svg/e8d2a74e6ffc8d130e6540ae052afa4431152535)

where the vector _**r**_ ∈ ℝ_n_, and ∇(_i_) is a tensor whose _ni_ components are partial derivative operators of order _i_,

![[i)} \right ]_{\alpha_1 \alpha_2 \cdots \alpha_i} = \frac {\partial^{\, i}} {\partial r_{\alpha_1}  \partial r_{\alpha_2} \cdots \partial r_{\alpha_i} } \qquad \qquad \text{where} \quad  \alpha_1, \alpha_2, \cdots, \alpha_i = 1, 2, \cdots , n \ . ](https://wikimedia.org/api/rest_v1/media/math/render/svg/56d037aa2a7b100d82e701c7c784e8fc1c4db99f| \left [ \nabla^{(i)} \right ]][[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-13]]

An analogous application of the definition of the functional derivative yields

![
\begin{align}
\frac{\delta F[\rho]}{\delta \rho} &{} = \frac{\partial f}{\partial\rho} - \nabla \cdot \frac{\partial f}{\partial(\nabla\rho)} + \nabla^{(2)} \cdot \frac{\partial f}{\partial\left(\nabla^{(2)}\rho\right)} + \dots + (-1)^N \nabla^{(N)} \cdot \frac{\partial f}{\partial\left(\nabla^{(N)}\rho\right)} \\
&{} =   \frac{\partial f}{\partial\rho} + \sum_{i=1}^N (-1)^{i}\nabla^{(i)} \cdot \frac{\partial f}{\partial\left(\nabla^{(i)}\rho\right)} \ .
\end{align}
](https://wikimedia.org/api/rest_v1/media/math/render/svg/5e309ee6857a3699070ebbbb3e9380ededa6572d)

In the last two equations, the _ni_ components of the tensor ![[\nabla^{(i)}\rho\right)} ](https://wikimedia.org/api/rest_v1/media/math/render/svg/c1bfbfa0573912d3a2d6dfb4267e7bb7d75dfb5f| \frac{\partial f}{\partial\left(\nabla^{(i)}\rho\right)} ]] are partial derivatives of _f_ with respect to partial derivatives of _ρ_,

![[\nabla^{(i)}\rho \right ) } \right ]_{\alpha_1 \alpha_2 \cdots \alpha_i} = \frac {\partial f} {\partial \rho_{\alpha_1 \alpha_2 \cdots \alpha_i} } \qquad \qquad \text{where} \quad \rho_{\alpha_1 \alpha_2 \cdots \alpha_i} \equiv \frac {\partial^{\, i}\rho} {\partial r_{\alpha_1} \, \partial r_{\alpha_2} \cdots \partial r_{\alpha_i} }   \ ,   ](https://wikimedia.org/api/rest_v1/media/math/render/svg/75a055a108cb726caf3543357d6e379254a09dbf| \left [ \frac {\partial f} {\partial \left (\nabla^{(i)}\rho \right ) } \right ]]

and the tensor scalar product is,

![[i)} \cdot \frac{\partial f}{\partial\left(\nabla^{(i)}\rho\right)} = \sum_{\alpha_1, \alpha_2, \cdots, \alpha_i = 1}^n \ \frac {\partial^{\, i} } {\partial r_{\alpha_1} \, \partial r_{\alpha_2} \cdots \partial r_{\alpha_i} }  \ \frac {\partial f} {\partial \rho_{\alpha_1 \alpha_2 \cdots \alpha_i} }   \  .  ](https://wikimedia.org/api/rest_v1/media/math/render/svg/dd5095d63edbd303f91b2a2a25dc1feddaefba0f| \nabla^{(i)} \cdot \frac{\partial f}{\partial\left(\nabla^{(i)}\rho\right)} = \sum_{\alpha_1, \alpha_2, \cdots, \alpha_i = 1}^n \ \frac {\partial^{\, i} } {\partial r_{\alpha_1} \, \partial r_{\alpha_2} \cdots \partial r_{\alpha_i} }  \ \frac {\partial f} {\partial \rho_{\alpha_1 \alpha_2 \cdots \alpha_i} }   \  .  ]] [[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-14]]

### Examples\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=7 "Edit section: Examples")\]

#### Thomas–Fermi kinetic energy functional\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=8 "Edit section: Thomas–Fermi kinetic energy functional")\]

The [Thomas–Fermi model](https://en.wikipedia.org/wiki/Thomas%E2%80%93Fermi_model "Thomas–Fermi model") of 1927 used a kinetic energy functional for a noninteracting uniform [electron gas](https://en.wikipedia.org/wiki/Free_electron_model "Free electron model") in a first attempt of [density-functional theory](https://en.wikipedia.org/wiki/Density-functional_theory "Density-functional theory") of electronic structure:

![[\mathbf{r}) \, d\mathbf{r} \, .](https://wikimedia.org/api/rest_v1/media/math/render/svg/805e085a9d15321704c17fcea9c5c2f3a1f8924b|T_\mathrm{TF}[\rho]]

Since the integrand of _T_TF\[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-ParrYangP247A.6-15]]

![
\begin{align}
\frac{\delta T_{\mathrm{TF}}}{\delta \rho (\boldsymbol{r}) } 
& = C_\mathrm{F} \frac{\partial \rho^{5/3}(\mathbf{r})}{\partial \rho(\mathbf{r})}  \\
& = \frac{5}{3} C_\mathrm{F}  \rho^{2/3}(\mathbf{r}) \, .
\end{align}
](https://wikimedia.org/api/rest_v1/media/math/render/svg/4752d7fd2521305935cf0d80fb730accdbbcb30f)

#### Coulomb potential energy functional\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=9 "Edit section: Coulomb potential energy functional")\]

For the **electron-nucleus potential**, Thomas and Fermi employed the [Coulomb](https://en.wikipedia.org/wiki/Coulomb%27s_law "Coulomb's law") potential energy functional

![[\boldsymbol{r})}{|\boldsymbol{r}|} \ d\boldsymbol{r}.](https://wikimedia.org/api/rest_v1/media/math/render/svg/2c1593ae52b426aa72244fda7d98ac6aab5a6fd4|V[\rho]]

Applying the definition of functional derivative,

![
\begin{align}
\int \frac{\delta V}{\delta \rho(\boldsymbol{r})} \ \phi(\boldsymbol{r}) \ d\boldsymbol{r} 
& {} = \left [ \frac{d}{d\varepsilon}  \int \frac{\rho(\boldsymbol{r}) + \varepsilon \phi(\boldsymbol{r})}{|\boldsymbol{r}|} \ d\boldsymbol{r} \right ]_{\varepsilon=0} \\
& {} =  \int  \frac {1} {|\boldsymbol{r}|} \, \phi(\boldsymbol{r}) \ d\boldsymbol{r} \, .
\end{align}
](https://wikimedia.org/api/rest_v1/media/math/render/svg/c5feda7981e551ab3ef736601c97d676b5c93eeb)

So,

![[\boldsymbol{r})} = \frac{1}{|\boldsymbol{r}|} \ . ](https://wikimedia.org/api/rest_v1/media/math/render/svg/1c1cee60ee7e8ff1b8ce269836ddb38a45629fd6| \frac{\delta V}{\delta \rho(\boldsymbol{r})} = \frac{1}{|\boldsymbol{r}|} \ . ]]

For the classical part of the **electron-electron interaction**, Thomas and Fermi employed the [Coulomb](https://en.wikipedia.org/wiki/Coulomb%27s_law "Coulomb's law") potential energy functional

![[\mathbf{r}) \rho(\mathbf{r}')}{\vert \mathbf{r}-\mathbf{r}' \vert}\, d\mathbf{r} d\mathbf{r}' \, .](https://wikimedia.org/api/rest_v1/media/math/render/svg/2a6d16f5ade6b1bc0c8c78a03ff33b386221d068|J[\rho]]

From the [[https://en.wikipedia.org/wiki/Functional_derivative#Functional_derivative "Functional derivative"]],

![
\begin{align}
\int \frac{\delta J}{\delta\rho(\boldsymbol{r})} \phi(\boldsymbol{r})d\boldsymbol{r}  
& {} = \left [ \frac {d \ }{d\epsilon} \, J[\rho + \epsilon\phi] \right ]_{\epsilon = 0} \\
& {} = \left [ \frac {d \ }{d\epsilon} \, \left ( \frac{1}{2}\iint \frac {[\rho(\boldsymbol{r}) + \epsilon \phi(\boldsymbol{r})] \,  [\rho(\boldsymbol{r}') + \epsilon \phi(\boldsymbol{r}')]  }{\vert \boldsymbol{r}-\boldsymbol{r}' \vert}\, d\boldsymbol{r} d\boldsymbol{r}'  \right ) \right ]_{\epsilon = 0} \\
& {} =  \frac{1}{2}\iint \frac {\rho(\boldsymbol{r}') \phi(\boldsymbol{r})  }{\vert \boldsymbol{r}-\boldsymbol{r}' \vert}\, d\boldsymbol{r} d\boldsymbol{r}' +
\frac{1}{2}\iint \frac {\rho(\boldsymbol{r}) \phi(\boldsymbol{r}')  }{\vert \boldsymbol{r}-\boldsymbol{r}' \vert}\, d\boldsymbol{r} d\boldsymbol{r}'   \\
\end{align}
](https://wikimedia.org/api/rest_v1/media/math/render/svg/604d9921f18f63a32115a37490f300325c7fafcb)

The first and second terms on the right hand side of the last equation are equal, since _**r**_ and _**r′**_ in the second term can be interchanged without changing the value of the integral. Therefore,

![[\boldsymbol{r})} \phi(\boldsymbol{r})d\boldsymbol{r} = \int \left ( \int \frac {\rho(\boldsymbol{r}') }{\vert \boldsymbol{r}-\boldsymbol{r}' \vert} d\boldsymbol{r}' \right )  \phi(\boldsymbol{r}) d\boldsymbol{r}  ](https://wikimedia.org/api/rest_v1/media/math/render/svg/a37ec62be367efd27e812fb1168b1dca8d1f27ee| \int \frac{\delta J}{\delta\rho(\boldsymbol{r})} \phi(\boldsymbol{r})d\boldsymbol{r} = \int \left ( \int \frac {\rho(\boldsymbol{r}') }{\vert \boldsymbol{r}-\boldsymbol{r}' \vert} d\boldsymbol{r}' \right )  \phi(\boldsymbol{r}) d\boldsymbol{r}  ]]

and the functional derivative of the electron-electron coulomb potential energy functional _J_\[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-ParrYangP248A.11-16]]

![[\boldsymbol{r})} = \int \frac {\rho(\boldsymbol{r}') }{\vert \boldsymbol{r}-\boldsymbol{r}' \vert} d\boldsymbol{r}' \, . ](https://wikimedia.org/api/rest_v1/media/math/render/svg/f39bc784298e5fd4f7f7503aeff0c0638d2621ad| \frac{\delta J}{\delta\rho(\boldsymbol{r})} = \int \frac {\rho(\boldsymbol{r}') }{\vert \boldsymbol{r}-\boldsymbol{r}' \vert} d\boldsymbol{r}' \, . ]]

The second functional derivative is

![\frac{\delta^2 J[\rho]}{\delta \rho(\mathbf{r}')\delta\rho(\mathbf{r})}  = \frac{\partial}{\partial \rho(\mathbf{r}')} \left ( \frac{\rho(\mathbf{r}')}{\vert \mathbf{r}-\mathbf{r}' \vert} \right ) = \frac{1}{\vert \mathbf{r}-\mathbf{r}' \vert}.
](https://wikimedia.org/api/rest_v1/media/math/render/svg/2e5d2633d38d32e3ec5d142181697543d6b17aea)

#### Weizsäcker kinetic energy functional\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=10 "Edit section: Weizsäcker kinetic energy functional")\]

In 1935 [von Weizsäcker](https://en.wikipedia.org/wiki/Carl_Friedrich_von_Weizsacker "Carl Friedrich von Weizsacker") proposed to add a gradient correction to the Thomas-Fermi kinetic energy functional to make it suit better a molecular electron cloud:

![[\mathbf{r}) \cdot \nabla\rho(\mathbf{r})}{ \rho(\mathbf{r}) } d\mathbf{r} =  \int t_\mathrm{W} \ d\mathbf{r} \, ,](https://wikimedia.org/api/rest_v1/media/math/render/svg/0eafe31ae78208f4c75df2c3147f18c61ed02e29|T_\mathrm{W}[\rho]]

where

![[\boldsymbol{r}) \ .  ](https://wikimedia.org/api/rest_v1/media/math/render/svg/6ba8b6c7fe84535137fe832d2b552d3ee4d237f0| t_\mathrm{W} \equiv  \frac{1}{8}  \frac{\nabla\rho \cdot \nabla\rho}{ \rho } \qquad \text{and} \ \ \rho = \rho(\boldsymbol{r}) \ .  ]]

Using a previously derived [[https://en.wikipedia.org/wiki/Functional_derivative#Formula "Functional derivative"]] for the functional derivative,

![
\begin{align}
\frac{\delta T_\mathrm{W}}{\delta \rho(\boldsymbol{r})} 
& = \frac{\partial t_\mathrm{W}}{\partial \rho} - \nabla\cdot\frac{\partial t_\mathrm{W}}{\partial \nabla \rho} \\
& = -\frac{1}{8}\frac{\nabla\rho \cdot \nabla\rho}{\rho^2} - \left ( \frac {1}{4} \frac {\nabla^2\rho} {\rho} -  \frac {1}{4} \frac {\nabla\rho \cdot \nabla\rho} {\rho^2} \right ) \qquad \text{where} \ \ \nabla^2 = \nabla \cdot \nabla \ ,
\end{align}
](https://wikimedia.org/api/rest_v1/media/math/render/svg/7606a5a837e42b5c6fef0dc4f579708e225a4fce)

and the result is,[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-ParrYangP247A.9-17]]

![[\boldsymbol{r})} =  \ \ \, \frac{1}{8}\frac{\nabla\rho \cdot \nabla\rho}{\rho^2} - \frac{1}{4}\frac{\nabla^2\rho}{\rho} \ . ](https://wikimedia.org/api/rest_v1/media/math/render/svg/baa84f1f6ef2c83d9e6f447b2c48ccdd01430759| \frac{\delta T_\mathrm{W}}{\delta \rho(\boldsymbol{r})} =  \ \ \, \frac{1}{8}\frac{\nabla\rho \cdot \nabla\rho}{\rho^2} - \frac{1}{4}\frac{\nabla^2\rho}{\rho} \ . ]]

#### Entropy\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=11 "Edit section: Entropy")\]

The [entropy](https://en.wikipedia.org/wiki/Information_entropy "Information entropy") of a discrete [random variable](https://en.wikipedia.org/wiki/Random_variable "Random variable") is a functional of the [probability mass function](https://en.wikipedia.org/wiki/Probability_mass_function "Probability mass function").

![
\begin{align}
H[p(x)] = -\sum_x p(x) \log p(x)
\end{align}
](https://wikimedia.org/api/rest_v1/media/math/render/svg/96861966ca600ab501ab12eb13a187562581cff1)

Thus,

![
\begin{align}
\sum_x \frac{\delta H}{\delta p(x)} \, \phi(x) 
& {} = \left[ \frac{d}{d\epsilon} H[p(x) + \epsilon\phi(x)] \right]_{\epsilon=0}\\
& {} = \left [- \, \frac{d}{d\varepsilon}  \sum_x \, [p(x) + \varepsilon\phi(x)] \ \log [p(x) + \varepsilon\phi(x)] \right]_{\varepsilon=0} \\
& {} = \displaystyle -\sum_x \, [1+\log p(x)] \ \phi(x) \, .
\end{align}
](https://wikimedia.org/api/rest_v1/media/math/render/svg/7a13f6bab84e66aadc5f4d0b41d6af651a2825b7)

Thus,

![
\frac{\delta H}{\delta p(x)} = -1-\log p(x).
](https://wikimedia.org/api/rest_v1/media/math/render/svg/2c2dfd3f28b5e7eee63464be7360ff93f9461764)

#### Exponential\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=12 "Edit section: Exponential")\]

Let

![[x)]= e^{\int \varphi(x) g(x)dx}.](https://wikimedia.org/api/rest_v1/media/math/render/svg/8cf62da868a4878d3d5c56043e0e7947d1a3789f| F[\varphi(x)]]

Using the [[../math/delta function]] as a test function,

![
\begin{align}
\frac{\delta F[\varphi(x)]}{\delta \varphi(y)} 
& {} = \lim_{\varepsilon\to 0}\frac{F[\varphi(x)+\varepsilon\delta(x-y)]-F[\varphi(x)]}{\varepsilon}\\
& {} = \lim_{\varepsilon\to 0}\frac{e^{\int (\varphi(x)+\varepsilon\delta(x-y)) g(x)dx}-e^{\int \varphi(x) g(x)dx}}{\varepsilon}\\
& {} = e^{\int \varphi(x) g(x)dx}\lim_{\varepsilon\to 0}\frac{e^{\varepsilon \int \delta(x-y) g(x)dx}-1}{\varepsilon}\\
& {} = e^{\int \varphi(x) g(x)dx}\lim_{\varepsilon\to 0}\frac{e^{\varepsilon g(y)}-1}{\varepsilon}\\
& {} = e^{\int \varphi(x) g(x)dx}g(y).
\end{align}
](https://wikimedia.org/api/rest_v1/media/math/render/svg/ec4bb807430d52bf84582815526969c5182132bb)

Thus,

![[x)]}{\delta \varphi(y)} = g(y) F[\varphi(x)]. ](https://wikimedia.org/api/rest_v1/media/math/render/svg/e78f30af55466f2e117b3dc25af74e86a2db308c| \frac{\delta F[\varphi(x)]]

This is particularly useful in calculating the [correlation functions](https://en.wikipedia.org/wiki/Correlation_function_(quantum_field_theory) "Correlation function (quantum field theory)") from the [partition function](https://en.wikipedia.org/wiki/Partition_function_(quantum_field_theory) "Partition function (quantum field theory)") in [quantum field theory](https://en.wikipedia.org/wiki/Quantum_field_theory "Quantum field theory").

#### Functional derivative of a function\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=13 "Edit section: Functional derivative of a function")\]

A function can be written in the form of an integral like a functional. For example,

![[\boldsymbol{r}) = F[\rho] = \int \rho(\boldsymbol{r}') \delta(\boldsymbol{r}-\boldsymbol{r}')\, d\boldsymbol{r}'.](https://wikimedia.org/api/rest_v1/media/math/render/svg/d4a462a8d7648c751791e624f6bb5abdfa985733|\rho(\boldsymbol{r}) = F[\rho]]

Since the integrand does not depend on derivatives of _ρ_, the functional derivative of _ρ_(_**r**_) is,

![
\begin{align} 
\frac {\delta \rho(\boldsymbol{r})} {\delta\rho(\boldsymbol{r}')} \equiv \frac {\delta F} {\delta\rho(\boldsymbol{r}')} 
& = \frac{\partial \ \ }{\partial \rho(\boldsymbol{r}')} \, [\rho(\boldsymbol{r}') \delta(\boldsymbol{r}-\boldsymbol{r}')] \\
& = \delta(\boldsymbol{r}-\boldsymbol{r}').
\end{align}
](https://wikimedia.org/api/rest_v1/media/math/render/svg/1583fde0b7d6e164506aced9aa3781e502395d53)

#### Functional derivative of iterated function\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=14 "Edit section: Functional derivative of iterated function")\]

The functional derivative of the iterated function ![[f(x))}](https://wikimedia.org/api/rest_v1/media/math/render/svg/f11f1c1b426c8f37ee0d2c5b9a60e413d8793913|{\displaystyle f(f(x))}]] is given by:

![[f(x))}{\delta f(y)}}=f'(f(x))\delta (x-y)+\delta (f(x)-y)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/08cee11f422cb7194e8da8f41adc48919e5a1ced|{\displaystyle {\frac {\delta f(f(x))}{\delta f(y)}}=f'(f(x))\delta (x-y)+\delta (f(x)-y)}]]

and

![[f(f(x)))}{\delta f(y)}}=f'(f(f(x))(f'(f(x))\delta (x-y)+\delta (f(x)-y))+\delta (f(f(x))-y)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/54c2245f3b3a5ccb7f3f581cbbca60731f909460|{\displaystyle {\frac {\delta f(f(f(x)))}{\delta f(y)}}=f'(f(f(x))(f'(f(x))\delta (x-y)+\delta (f(x)-y))+\delta (f(f(x))-y)}]]

In general:

![[x)}{\delta f(y)}}=f'(f^{N-1}(x)){\frac {\delta f^{N-1}(x)}{\delta f(y)}}+\delta (f^{N-1}(x)-y)}](https://wikimedia.org/api/rest_v1/media/math/render/svg/8b2c2f80661a94f479f5a9eff3640049d01ea097|{\displaystyle {\frac {\delta f^{N}(x)}{\delta f(y)}}=f'(f^{N-1}(x)){\frac {\delta f^{N-1}(x)}{\delta f(y)}}+\delta (f^{N-1}(x)-y)}]]

Putting in N=0 gives:

![[x)}{\delta f(y)}}=-{\frac {\delta (f^{-1}(x)-y)}{f'(f^{-1}(x))}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/c59e61027e20323d8cd7cbf298f472f6c0af14d7|{\displaystyle {\frac {\delta f^{-1}(x)}{\delta f(y)}}=-{\frac {\delta (f^{-1}(x)-y)}{f'(f^{-1}(x))}}}]]

## Using the [[../math/delta function]] as a test function\[[edit]] as a test function")\]

In physics, it is common to use the [Dirac delta function](https://en.wikipedia.org/wiki/Dirac_delta_function "Dirac [delta function](../math/delta%20function.md)") ![[x-y)](https://wikimedia.org/api/rest_v1/media/math/render/svg/caadbaf86974aa6db3aaf6f3566c6eb8d762f3e5|\delta(x-y)]] in place of a generic test function ![[x)](https://wikimedia.org/api/rest_v1/media/math/render/svg/546b660b2f3cfb5f34be7b3ed8371d54f5c74227|\phi (x)]], for yielding the functional derivative at the point ![y](https://wikimedia.org/api/rest_v1/media/math/render/svg/b8a6208ec717213d4317e666f1ae872e00620a0d) (this is a point of the whole functional derivative as a [partial derivative](https://en.wikipedia.org/wiki/Partial_derivative "Partial derivative") is a component of the gradient):[[https://en.wikipedia.org/wiki/Functional_derivative#cite_note-18]]

![\frac{\delta F[\rho(x)]}{\delta \rho(y)}=\lim_{\varepsilon\to 0}\frac{F[\rho(x)+\varepsilon\delta(x-y)]-F[\rho(x)]}{\varepsilon}.
](https://wikimedia.org/api/rest_v1/media/math/render/svg/b01a2033e8c8afc08ec56de9981c0e29042885f6)

This works in cases when ![[x)+\varepsilon f(x)]](https://wikimedia.org/api/rest_v1/media/math/render/svg/b979a338aa9020b6c02e0bcae441aaa605ec2a20|F[\rho(x)+\varepsilon f(x)]] formally can be expanded as a series (or at least up to first order) in ![\varepsilon ](https://wikimedia.org/api/rest_v1/media/math/render/svg/a30c89172e5b88edbd45d3e2772c7f5e562e5173). The formula is however not mathematically rigorous, since ![[x)+\varepsilon\delta(x-y)]](https://wikimedia.org/api/rest_v1/media/math/render/svg/659a52b75b432c570f6c2a7415fc5b4334bf3618|F[\rho(x)+\varepsilon\delta(x-y)]] is usually not even defined.

The definition given in a previous section is based on a relationship that holds for all test functions ![[x)](https://wikimedia.org/api/rest_v1/media/math/render/svg/546b660b2f3cfb5f34be7b3ed8371d54f5c74227|\phi (x)]], so one might think that it should hold also when ![[x)](https://wikimedia.org/api/rest_v1/media/math/render/svg/546b660b2f3cfb5f34be7b3ed8371d54f5c74227|\phi (x)]] is chosen to be a specific function such as the [delta function](https://en.wikipedia.org/wiki/Dirac_delta_function "[Dirac delta function](../math/delta%20function.md)"). However, the latter is not a valid test function (it is not even a proper function).

In the definition, the functional derivative describes how the functional ![[x)]}](https://wikimedia.org/api/rest_v1/media/math/render/svg/c7fab43f9b14ba7f5581e7767857988b966692be|{\displaystyle F[\rho (x)]] changes as a result of a small change in the entire function ![[x)](https://wikimedia.org/api/rest_v1/media/math/render/svg/0f32a26d8795457b2f5c2bdc078758dcbbc71b30|\rho (x)]]. The particular form of the change in ![[x)](https://wikimedia.org/api/rest_v1/media/math/render/svg/0f32a26d8795457b2f5c2bdc078758dcbbc71b30|\rho (x)]] is not specified, but it should stretch over the whole interval on which ![x](https://wikimedia.org/api/rest_v1/media/math/render/svg/87f9e315fd7e2ba406057a97300593c4802b53e4) is defined. Employing the particular form of the perturbation given by the delta function has the meaning that ![[x)](https://wikimedia.org/api/rest_v1/media/math/render/svg/0f32a26d8795457b2f5c2bdc078758dcbbc71b30|\rho (x)]] is varied only in the point ![y](https://wikimedia.org/api/rest_v1/media/math/render/svg/b8a6208ec717213d4317e666f1ae872e00620a0d). Except for this point, there is no variation in ![[x)](https://wikimedia.org/api/rest_v1/media/math/render/svg/0f32a26d8795457b2f5c2bdc078758dcbbc71b30|\rho (x)]].

## Notes\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=16 "Edit section: Notes")\]

1.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-2 "Jump up"]]** According to [[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFGiaquintaHildebrandt1996]], p. 18, this notation is customary in [physical](https://en.wikipedia.org/wiki/Physics "Physics") literature.
2.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-5 "Jump up"]]** Called _differential_ in ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFParrYang1989]], p. 246), _variation_ or _first variation_ in ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFCourantHilbert1953]], p. 186), and _variation_ or _differential_ in ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFGelfandFomin2000]], p. 11, § 3.2).
3.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-7 "Jump up"]]** Here the notation ![[x)\equiv {\frac {\delta {F}}{\delta \rho (x)}}}](https://wikimedia.org/api/rest_v1/media/math/render/svg/151e3a56bb44d7a18ea72ecd4d316ff49e1055a9|{\displaystyle {\frac {\delta {F}}{\delta \rho }}(x)\equiv {\frac {\delta {F}}{\delta \rho (x)}}}]] is introduced.
4.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-12 "Jump up"]]** For a three-dimensional cartesian coordinate system,
    
    ![
    \begin{align}
    \frac{\partial f}{\partial\nabla\rho} =   \frac{\partial f}{\partial\rho_x}  \mathbf{\hat{i}}   + \frac{\partial f}{\partial\rho_y}  \mathbf{\hat{j}} + \frac{\partial f}{\partial\rho_z}  \mathbf{\hat{k}}\, ,  \qquad 
    & \text{where} \ \rho_x = \frac{\partial \rho}{\partial x}\, ,  \ \rho_y = \frac{\partial \rho}{\partial y}\, , \ \rho_z = \frac{\partial \rho}{\partial z}\, \\
    & \text{and} \ \ \mathbf{\hat{i}}, \ \mathbf{\hat{j}}, \ \mathbf{\hat{k}} \ \ \text {are unit vectors along the x, y, z axes.}
    \end{align}
    ](https://wikimedia.org/api/rest_v1/media/math/render/svg/17e7ed61ed5dccd09100ee7792ffe6a997bd2c14)
    
5.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-13 "Jump up"]]** For example, for the case of three dimensions (_n_ = 3) and second order derivatives (_i_ = 2), the tensor ∇(2) has components,
    
    ![[2)} \right ]_{\alpha \beta} = \frac {\partial^{\,2}} {\partial r_{\alpha} \, \partial r_{\beta}} \qquad \qquad \text{where} \quad \alpha, \beta = 1, 2, 3 \, . ](https://wikimedia.org/api/rest_v1/media/math/render/svg/78cbff2c145d8b1d793a8318a07d6f72883d2f3d| \left [ \nabla^{(2)} \right ]]
    
6.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-14 "Jump up"]]** For example, for the case _n_ = 3 and _i_ = 2, the tensor scalar product is,
    
    ![[2)} \cdot \frac{\partial f}{\partial\left(\nabla^{(2)}\rho\right)} = \sum_{\alpha, \beta = 1}^3 \ \frac {\partial^{\, 2} } {\partial r_{\alpha} \, \partial r_{\beta} }  \ \frac {\partial f} {\partial \rho_{\alpha \beta} }    \qquad \text{where} \ \ \rho_{\alpha \beta} \equiv \frac {\partial^{\, 2}\rho} {\partial r_{\alpha} \, \partial r_{\beta} } \ . ](https://wikimedia.org/api/rest_v1/media/math/render/svg/8614c20390d2fe431b437a27daaae4aa9851b10d| \nabla^{(2)} \cdot \frac{\partial f}{\partial\left(\nabla^{(2)}\rho\right)} = \sum_{\alpha, \beta = 1}^3 \ \frac {\partial^{\, 2} } {\partial r_{\alpha} \, \partial r_{\beta} }  \ \frac {\partial f} {\partial \rho_{\alpha \beta} }    \qquad \text{where} \ \ \rho_{\alpha \beta} \equiv \frac {\partial^{\, 2}\rho} {\partial r_{\alpha} \, \partial r_{\beta} } \ . ]]
    

## Footnotes\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=17 "Edit section: Footnotes")\]

1.  ^ [[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-GiaquintaHildebrandtP18_1-0]] [[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-GiaquintaHildebrandtP18_1-1]] ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFGiaquintaHildebrandt1996]], p. 18)
2.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-ParrYangP246A.2_3-0 "Jump up"]]** ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFParrYang1989]], p. 246, Eq. A.2).
3.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-ParrYangP246A.1_4-0 "Jump up"]]** ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFParrYang1989]], p. 246, Eq. A.1).
4.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-ParrYangP246_6-0 "Jump up"]]** ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFParrYang1989]], p. 246).
5.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-ParrYangP247A.3_8-0 "Jump up"]]** ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFParrYang1989]], p. 247, Eq. A.3).
6.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-ParrYangP247A.4_9-0 "Jump up"]]** ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFParrYang1989]], p. 247, Eq. A.4).
7.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-10 "Jump up"]]** ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFGreinerReinhardt1996]], p. 38, Eq. 6).
8.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-11 "Jump up"]]** ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFGreinerReinhardt1996]], p. 38, Eq. 7).
9.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-ParrYangP247A.6_15-0 "Jump up"]]** ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFParrYang1989]], p. 247, Eq. A.6).
10.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-ParrYangP248A.11_16-0 "Jump up"]]** ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFParrYang1989]], p. 248, Eq. A.11).
11.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-ParrYangP247A.9_17-0 "Jump up"]]** ([[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFParrYang1989]], p. 247, Eq. A.9).
12.  **[[https://en.wikipedia.org/wiki/Functional_derivative#cite_ref-18 "Jump up"]]** [[https://en.wikipedia.org/wiki/Functional_derivative#CITEREFGreinerReinhardt1996]], p. 37

## References\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=18 "Edit section: References")\]

-   [Courant, Richard](https://en.wikipedia.org/wiki/Richard_Courant "Richard Courant"); [Hilbert, David](https://en.wikipedia.org/wiki/David_Hilbert "David Hilbert") (1953). "Chapter IV. The Calculus of Variations". _Methods of Mathematical Physics_. Vol. I (First English ed.). New York, New York: [Interscience Publishers](https://en.wikipedia.org/wiki/Interscience_Publishers "Interscience Publishers"), Inc. pp. 164–274. [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [978-0471504474](https://en.wikipedia.org/wiki/Special:BookSources/978-0471504474 "Special:BookSources/978-0471504474"). [MR](https://en.wikipedia.org/wiki/MR_(identifier) "MR (identifier)") [0065391](https://www.ams.org/mathscinet-getitem?mr=0065391). [Zbl](https://en.wikipedia.org/wiki/Zbl_(identifier) "Zbl (identifier)") [0001.00501](https://zbmath.org/?format=complete&q=an:0001.00501). .
-   Frigyik, Béla A.; Srivastava, Santosh; Gupta, Maya R. (January 2008), [_Introduction to Functional Derivatives_](https://web.archive.org/web/20170217025324/https://www2.ee.washington.edu/techsite/papers/documents/UWEETR-2008-0001.pdf) (PDF), UWEE Tech Report, UWEETR-2008-0001, Seattle, WA: Department of Electrical Engineering at the University of Washington, p. 7, archived from [the original](https://www.ee.washington.edu/techsite/papers/documents/UWEETR-2008-0001.pdf) (PDF) on 2017-02-17, retrieved 2013-10-23.
-   [Gelfand, I. M.](https://en.wikipedia.org/wiki/Israel_Gelfand "Israel Gelfand"); [Fomin, S. V.](https://en.wikipedia.org/wiki/Sergei_Fomin "Sergei Fomin") (2000) \[1963\], [_Calculus of variations_](http://store.doverpublications.com/0486414485.html), translated and edited by Richard A. Silverman (Revised English ed.), Mineola, N.Y.: [Dover Publications](https://en.wikipedia.org/wiki/Dover_Publications "Dover Publications"), [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [978-0486414485](https://en.wikipedia.org/wiki/Special:BookSources/978-0486414485 "Special:BookSources/978-0486414485"), [MR](https://en.wikipedia.org/wiki/MR_(identifier) "MR (identifier)") [0160139](https://www.ams.org/mathscinet-getitem?mr=0160139), [Zbl](https://en.wikipedia.org/wiki/Zbl_(identifier) "Zbl (identifier)") [0127.05402](https://zbmath.org/?format=complete&q=an:0127.05402).
-   [Giaquinta, Mariano](https://en.wikipedia.org/wiki/Mariano_Giaquinta "Mariano Giaquinta"); Hildebrandt, Stefan (1996), _Calculus of Variations 1. The Lagrangian Formalism_, Grundlehren der Mathematischen Wissenschaften, **310** (1st ed.), Berlin: [Springer-Verlag](https://en.wikipedia.org/wiki/Springer-Verlag "Springer-Verlag"), [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [3-540-50625-X](https://en.wikipedia.org/wiki/Special:BookSources/3-540-50625-X "Special:BookSources/3-540-50625-X"), [MR](https://en.wikipedia.org/wiki/MR_(identifier) "MR (identifier)") [1368401](https://www.ams.org/mathscinet-getitem?mr=1368401), [Zbl](https://en.wikipedia.org/wiki/Zbl_(identifier) "Zbl (identifier)") [0853.49001](https://zbmath.org/?format=complete&q=an:0853.49001).
-   [Greiner, Walter](https://en.wikipedia.org/wiki/Walter_Greiner "Walter Greiner"); Reinhardt, Joachim (1996), ["Section 2.3 – Functional derivatives"](https://archive.org/details/fieldquantizatio0000grei/page/36), _Field quantization_, With a foreword by D. A. Bromley, Berlin–Heidelberg–New York: Springer-Verlag, pp. [36–38](https://archive.org/details/fieldquantizatio0000grei/page/36), [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [3-540-59179-6](https://en.wikipedia.org/wiki/Special:BookSources/3-540-59179-6 "Special:BookSources/3-540-59179-6"), [MR](https://en.wikipedia.org/wiki/MR_(identifier) "MR (identifier)") [1383589](https://www.ams.org/mathscinet-getitem?mr=1383589), [Zbl](https://en.wikipedia.org/wiki/Zbl_(identifier) "Zbl (identifier)") [0844.00006](https://zbmath.org/?format=complete&q=an:0844.00006).
-   Parr, R. G.; Yang, W. (1989). "Appendix A, Functionals". [_Density-Functional Theory of Atoms and Molecules_](https://books.google.com/books?id=mGOpScSIwU4C&q=Density-Functional+Theory+of+Atoms+and+Molecules). New York: Oxford University Press. pp. 246–254. [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier) "ISBN (identifier)") [978-0195042795](https://en.wikipedia.org/wiki/Special:BookSources/978-0195042795 "Special:BookSources/978-0195042795").

## External links\[[edit](https://en.wikipedia.org/w/index.php?title=Functional_derivative&action=edit&section=19 "Edit section: External links")\]

-   ["Functional derivative"](https://www.encyclopediaofmath.org/index.php?title=Functional_derivative), _[Encyclopedia of Mathematics](https://en.wikipedia.org/wiki/Encyclopedia_of_Mathematics "Encyclopedia of Mathematics")_, [EMS Press](https://en.wikipedia.org/wiki/European_Mathematical_Society "European Mathematical Society"), 2001 \[1994\]