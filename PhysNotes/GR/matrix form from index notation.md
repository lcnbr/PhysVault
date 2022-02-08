---
alias:
- matrix form
tags: GR SR physics LA
---
Index notation, where [[Einstein summation]] is used (only on one raised indices and one lower indices), makes ordering of elements in an equation irrelevant. One can translate a matrix equation into a component equation and then commute elements around without discretion. However if one wants to translate back to matrices, graet care is needed. In particular index placement, (vertical **and** horizontal) is crucial. Then we use the following dictionary:

|                   Matrix operation                   |                 index notation                  |
|:----------------------------------------------------:|:-----------------------------------------------:|
|             $\underline{\underline{A}}$              | $A^\mu{}_\nu$ or $A^{\mu \nu}$ or $A_{\mu \nu}$ |
|       $\underline{\underline{A}}\underline{v}$       |               $A^\mu{}_\nu v^\nu$               |
| $\underline{\underline{A}}\underline{\underline{B}}$ |         $A^\mu{}_\alpha B^\alpha{}_\nu$         |
|           $\underline{\underline{A}}^\top$           |        $(A^\top)^\mu{}_\nu=A_\nu{}^\mu$         |                                                     |                                                 |

We still can use the [[metric tensor]] to raise and lower indices. To extract the matrix order one needs to order the coefficients to  be summing over indices that are next to each other, where we can exchange the order between indices using the transpose.