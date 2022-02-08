# String Spectrum in [[light cone quantisation]]
The [[light cone quantisation#Mass]] of the string state depends on [[string level]]. Quantisation of [[string level]] leads to a quantisation of mass for string states. 
## Level matching
Since we have [[light cone quantisation#^f12d71]] we need to have Level matching:
$$
N^{\mathrm{L}}-a^{\mathrm{L}}=N^{\mathrm{R}}-a^{\mathrm{R}}
$$
String states at each level constitute a very-well known system: a harmonic oscillator.
# Vacuum State. 
Define vacuum state $|0 ; q\rangle$
$$
\vec{\alpha}_{n}^{\mathrm{L} / \mathrm{R}}|0 ; q\rangle=0 \quad \text { for } n>0
$$
This state is at level zero: $N^{\mathrm{L}}=N^{\mathrm{R}}=0 .$ It has spin zero. 
For a physical state we must require [[#Level matching]]:
$$
a^{\mathrm{R}}=a^{\mathrm{L}}=a, \quad M^{2}=-\frac{4 a}{\kappa^{2}}
$$
So far so good: We have a spin-0 particle with $M=2 \kappa^{-1} \sqrt{-a}$. For a physical particle we would have to require $a \leq 0 !$ Spatial extent of state: [[quantum harmonic oscillator|HO]] wave function $\sim \kappa$.

## First Level. 
Lowest excited state has $N=1 .$ [[#Level matching]] and $a^{\mathrm{L}}=a^{\mathrm{R}}$ from [[#Vacuum State]] implies $N^{\mathrm{L}}=N^{\mathrm{R}}=1$. One excitation $\vec{\alpha}_{-1}$ each from left/right movers
$$
|a b ; q\rangle=\alpha_{-1}^{\mathrm{L}, a} \alpha_{-1}^{\mathrm{R}, b}|0 ; q\rangle .
$$

^57efbd

We find $(D-2)^{2}$ states of mass $M=2 \kappa^{-1} \sqrt{1-a}$, as $a,b\in \{1,\dots,D-1\}$, c.f. [[light cone coordinates#In embedding space ambient space]].
What is their spin? Consider first the spin under $\operatorname{SO}(D-2)$ transverse rotations. There are three useful combinations:
$$
\begin{aligned}
|(a b) ; q\rangle &:=|a b ; q\rangle+|b a ; q\rangle-\frac{2 \delta_{a b}}{D-2}|c c ; q\rangle \\
|[a b] ; q\rangle &:=|a b ; q\rangle-|b a ; q\rangle \\
|1 ; q\rangle &:=|c c ; q\rangle
\end{aligned}
$$

^61e748

Transformation properties under $\mathrm{SO}(D-2)$ :


|            state             |       indices        | Young tab. | "spin" |
|:----------------------------:|:--------------------:|:----------:|:------:|
| $$\textbar(a b) ; q\rangle$$ | symmetric, traceless |     ◻      |   2    |
|  $\textbar[a b] ; q\rangle$  |    anti-symmetric    |     ◻      |   1    |
|    $\textbar1 ; q\rangle$    |       singlet        |     ∙      |   0    |

Compare this to classification of unitary representations of the Poincaré group Stabiliser (little group) for massive particle is $\mathrm{SO}(D-1)$. Can we fit these $\mathrm{SO}(D-2)$ representation into $\operatorname{SO}(D-1)$ representations? No!

The only way out: consider a massless particle where the stabiliser is $\mathrm{SO}(D-2)$. We have to set $a=a^{\mathrm{R}}=a^{\mathrm{L}}=1$.
Three types of particles:
- $|(\boldsymbol{a b}) ; \boldsymbol{q}\rangle:$ massless spin- 2 field. this is fine as free field.
Weinberg-Witten theorem: interactions are forbidden except for gravitational interactions. This particle must be the [[graviton]]! ^45d063
- $|[\boldsymbol{a b}] ; \boldsymbol{q}\rangle:$ massless 2-form field (Kalb-Ramond).
generalisation of electromagnetic field $A_{\mu}: B_{\mu \nu}$ with 1-form [[gauge symmetry]] $\delta B_{\mu \nu}=$ $\partial_{\mu} \epsilon_{\nu}-\partial_{\nu} \epsilon_{\mu} .$
- $|1 ; q\rangle:$ massless scalar particle (dilaton).
state different from string vacuum $|0 ; q\rangle$.

What we have learned so far:
- String theory contains [[graviton]] plus massless 2-form and scalar particles.
- Interacting string theory includes gravity!
- Spatial extent of particles $\sim \kappa ;$ practically point-like.
- $\kappa$ is the Planck scale (later).
- We must set $a=a^{\mathrm{R}}=a^{\mathrm{L}}=1$ for consistency (with physicality).
# Tachyon. 
Now revisit the [[#Vacuum State|string vacuum]] $|q, 0\rangle: M^{2}=-4 / \kappa^{2}<0$. This state is a [[tachyon]]!
Is this a problem? Not really, compare to spontaneous symmetry breaking mechanism:
- [[#Vacuum state]] was chosen at unstable local maximum of a potential. This leads to a tachyonic mode.
- Physical ground state should be situated at local minimum. No tachyon here!
- (Bosonic) string theory: Unclear if a global minimum exists. Unclear how to treat it in practice: Where is it? What are its properties?
- Let us ignore this shortcoming. Indeed, the tachyon is absent for superstrings (which are treated later)!

# Higher Levels. 
Levels zero and one work out. What about the higher levels? We have already used up all available freedom to adjust $a^{\mathrm{L}, \mathrm{R}}$, now self-consistency of the model is up to luck (or faith). The following table lists the representations for left-movers (equivalently right-movers)

|  level  |                            excitations                            |                                                                             SO(D-2)                                                                             |                                  SO(D-1)                                   |
|:-------:|:-----------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
|    0    |                              $\cdot$                              |                                                                            $\bullet$                                                                            |                                 $\bullet$                                  |
|    1    |                          $\alpha_{-1}^a$                          |                                                                      $\substack{\square}$                                                                       |                                  $\times$                                  |
|    2    |                   $\alpha_{-1}^a\alpha_{-1}^b$                    |                                                        $\substack{\square}\substack{\square}\ +\bullet$                                                         |                   $\substack{\square}\substack{\square}$                   |
|         |                          $\alpha_{-2}^a$                          |                                                                      $\substack{\square}$                                                                       |                                                                            |
|    3    |         $\alpha_{-1}^{a} \alpha_{-1}^{b} \alpha_{-1}^{c}$         |                                         $\substack{\square}\substack{\square}\substack{\square}\ + \substack{\square}$                                          |          $\substack{\square}\substack{\square}\substack{\square}$          |
|         |                 $\alpha_{-1}^{a} \alpha_{-2}^{b}$                 |                                           $\substack{\square}\substack{\square}+\substack{\square\\\square}+\bullet$                                            |                   $\substack{\square\\\square\\\square}$                   |
|         |                         $\alpha_{-3}^{a}$                         |                                                                      $\substack{\square}$                                                                       |                                                                            |
|    4    | $\alpha_{-1}^{a} \alpha_{-1}^{b} \alpha_{-1}^{c} \alpha_{-1}^{d}$ |                     $\substack{\square}\substack{\square}\substack{\square}\substack{\square}+\substack{\square}\substack{\square}+\bullet$                     | $\substack{\square}\substack{\square}\substack{\square}\substack{\square}$ |
|         |         $\alpha_{-1}^{a} \alpha_{-1}^{b} \alpha_{-2}^{c}$         | $\substack{\square}\substack{\square}\substack{\square}+\substack{\square\\\square}\substack{\square\\\phantom{\square}}+\substack{\square}+\substack{\square}$ |     $\substack{\square\\\square}\substack{\square\\\phantom{\square}}$     |
|         |                 $\alpha_{-2}^{a} \alpha_{-2}^{b}$                 |                                                         $\substack{\square}\substack{\square}+\bullet$                                                          |                   $\substack{\square}\substack{\square}$                   |
|         |                 $\alpha_{-3}^{a} \alpha_{-1}^{b}$                 |                                           $\substack{\square}\substack{\square}+\substack{\square\\\square}+\bullet$                                            |                                 $\bullet$                                  |
|         |                         $\alpha_{-4}^{a}$                         |                                                                      $\substack{\square}$                                                                       |                                                                            |
| $\dots$ |                              $\dots$                              |                                                                             $\dots$                                                                             |                                    $\dots$                                    |


All higher levels combine into proper $\operatorname{SO}(D-1)$ representations, for both left and right moving modes.

Furthermore, level matching implies we need to square the above representations for the correct particle spectrum.
Altogether:
- String describes collection of infinitely many particle types of different mass and spin.
- Various vibration modes might correspond to elementary particles. They include the massless [[graviton]]. 
- Intrinsic particle extent at Planck scale $\kappa$. Planck scale is much smaller than can be observed: String theory describes practically point-like particles! 
- String theory describes only a few massless particles; all others at Planck mass$1/\kappa$; one [[tachyon]]. 
- Proper treatment of [[tachyon]] could change picture altogether. 
- Very high excitations are long strings. They would mostly display classical behaviour, but are superheavy $M\gg1/\kappa$ 

 # Regge Trajectories. 

^b4fff2

 Maximum spin (all indices symmetric and traceless) increases linearly with level S =2N
 ![[Pasted image 20220120191118.png|300]]$$M^2=\frac{2S-4a}{\kappa}$$
This relationship is called the leading “Regge trajectory”: 
- $\alpha'=\kappa^2$ is called the Regge slope. 
- $2a$ is called the Regge intercept; spin of massless particle. 
Subleading trajectories have lower spins (indices anti-symmetric or have trace). Qualitative similarity to hadron spectrum: 
- Regge trajectories observed for hadronic resonances. 
- For a stringy description of QCD,$1/\kappa$ would have to be QCD scale $\simeq$ 1 GeV. 
- Intercept should be $a \approx  -\frac{1}{2}$ for QCD rather than $a =1$. 
- There is another problem (see later). 
- Strings provide a qualitative description of QCD flux tubes.
