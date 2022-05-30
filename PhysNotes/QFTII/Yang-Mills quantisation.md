---
alias:
tags:
- qftII
---

We are now prepared to apply to the path integral quantisation to the vector fields of Yang-Mills theory. Here some further complications arise due to the non-abelian nature of the gauge group. These lead to the introduction of further fields.

[[some puzzles]]
[[YM gauge fixing]]
[[Faddeev-Popov ghosts]]

# Discussion. 
We observe that the proper quantisation of the Yang-Mills action requires the introduction of additional scalar fermionic fields, so-called [[Faddeev-Popov ghosts]]. These fields are called ghosts because they obey the wrong statistics for scalar fields.

Usually such fields would violate basic properties of QFT. In this situation it actually solves a problem since the gauge potential itself has some unphysical modes. The unphysical behaviour of these two fields conspires to cancel each other out precisely.

For example, the one-loop contribution to the two-point effective vertex receives another contribution from a [[Faddeev-Popov ghosts|ghost]] loop (dotted line)

![[Pasted image 20220126234431.png|400]]
This [[Faddeev-Popov ghosts|ghost]] has precisely the same unphysical behaviour as the pure gauge loop. Since it is a fermion loop, it receives an extra minus sign, so that the two unphysical contributions cancel exactly. The final result for the one-loop two-point effective vertex therefore has a proper polarisation structure.

Note, however, that unphysical polarisations do remain for asymptotic vector fields as do the [[Faddeev-Popov ghosts|ghost]] fields. In the above example of two matter fields annihilating we thus have an extra contribution producing a pair of ghosts
![[Pasted image 20220126234505.png|400]]
As we shall see later, the unphysical particles can now be projected out safely without violating unitarity.

Note that the [[Faddeev-Popov ghosts]] are not required for all gauges. For example, the light cone gauge is typically formulated in terms of the gauge field only. The point is that the vector field in the [[../String/Light Cone Gauge]] has no unphysical modes, hence no ghosts are needed to cancel their effects.

Another example where no ghosts are needed is the abelian theory. Here the gauge field never forms closed loops on its own. Consequently, the [[Faddeev-Popov ghosts|ghost field]] does not couple to the gauge field.