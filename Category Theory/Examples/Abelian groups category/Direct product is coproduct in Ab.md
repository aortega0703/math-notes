---
tags:
  - theorem
  - math/abstract_algebra
  - math/category_theory
related topics:
  - "[[Category of abelian groups]]"
  - "[[Direct product]]"
  - "[[Coproduct]]"
---
For [[Abelian group|Abelian groups]] $A,B$, their [[Direct product]] $A times B$ is a [[Coproduct]] in $\mathbf{Ab}$ with the functions$$

	\begin{aligned}
		\iota_A : A & -> A times B\
		a & |-> (a, e_B)
	\end{aligned}\qquad
	\begin{aligned}
		\iota_B : B & -> A times B\
		b & |-> (e_A, b)
	\end{aligned}

$$
##### Proof:
![[coproduct.png]]

Consider homomorphisms $\phi: A -> X$ and $\psi: B -> X$ and the function$$

	\phi\cdot\psi : A times B & -> X\
    (a,b) & |-> \phi(a)\psi(b)

$$

- $\iota_A$ and $\iota_B$ are homomorphisms:
  Let $a_1,a_2 in A$, then$$
  
    \iota_A(a_1 a_2)
    &= (a_1 a_2, e_B)\
    &= (a_1, e_B)\cdot(a_2, e_B)\
    &= \iota_A(a_1)\cdot \iota_A(a_2)
  
  $$Which makes $\iota_A$ an homomorphism, similarly with $\iota_B$.
- $\phi\cdot\psi$ is an homomorphism:
  Let $a_1,a_2 in A$ and $b_1, b_2 in B$. Then$$
  
    (\phi\cdot\psi)\big((a_1,b_1)\cdot(a_2, b_2)\big)
    &= (\phi\cdot\psi)(a_1 a_2,b_1 b_2)\
    &= \phi(a_1 a_2) \psi(b_1 b_2)\
    &= \phi(a_1) \phi(a_2) \psi(b_1)\psi(b_2)\
    &= \phi(a_1) \psi(b_1) \phi(a_2) \psi(b_2)\
    &= (\phi\cdot\psi)(a_1,b_1) \cdot (\phi\cdot\psi)(a_2,b_2)
  
  $$making $\psi\cdot\psi$ an homomorphism. Note that this is not necessarily true when $X$ is no abelian as we need $\phi(a_2)$ and $\psi(b_1)$ to commute.
- $A times B$ is a coproduct:
  Let $a in A$, then$$
  
    (a)\iota_A(\phi\cdot\psi)
    &= (a,e_B)(\phi\cdot\psi)\
    &= \phi(a) \psi(e_B)\
    &= \phi(a) e_X\
    &= \phi(a)
  
  $$So by extensionality $\iota_A(\phi\cdot\psi) = \phi$. Similarly $\iota_B(\phi\cdot\psi) = \psi$.
Then $A times B$ is a coproduct in $\mathbf{Ab}$.
