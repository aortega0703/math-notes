---
tags:
  - theorem
  - math/abstract_algebra
  - math/category_theory
related topics:
  - "[[Category of abelian groups]]"
  - "[[Exponential object]]"
---
For any [[Abelian group]] $G$ and set $A$, $G^A = \text{Hom}_\mathbf{Set}(A, G)$ is an abelian group with the operation $$

	+:G^A times G^A & -> G^A\
	f,g& |-> f(\_)\cdot g(\_)

$$
##### Proof:
- $G^A$ is a [[Group]]:
	By [[Exponentials in category of groups]].
- Commutativity:
	Let $f,g in G^A$ and $a in A$, then$$
	
		(f+g)(a)
		&= f(a)\cdot g(a)\
		&= g(a)\cdot f(a)\
		&= (g+f)(a)
	
	$$which by [[Set|Extensionality]] implies $f+g=g+f$, so $G^A$ is an abelian group.