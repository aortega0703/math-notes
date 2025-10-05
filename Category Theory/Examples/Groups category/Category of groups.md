---
tags:
  - definition
  - math/category_theory
related topics:
  - "[[Group]]"
  - "[[Group homomorphism]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
The [[Category]] of [[Group|groups]] $\mathbf{Grp}$ is defined by
- $\text{Obj}(\mathbf{Grp})=$ the collection of all groups.
- $\text{Hom}_\mathbf{Grp}(G,H)=$ the collection of [[Group homomorphism|group homomorphisms]] $G -> H$.
- $ compose =$ [[Function|Function composition]].
---
This data does describe a [[Category]].
##### Proof:
- Closed under $ compose $:
	Let $G\overset{\phi}{ -> } H\overset{\psi}{ -> } K$ be [[Group homomorphism|group homomorphisms]]. This gives the following diagram
	![[Grp composition.png]]
	As the inner squares commute so does the outer rectangle. Then $\mathbf{Grp}$ is closed under composition.
- Identities:
	Let $H$ be a group, then $\text{id}_H: H -> H$ is trivially a group homomorphism. Let $G\overset{\phi}{ -> } H\overset{\psi}{ -> } K$, then$$
	
		\begin{aligned}
			(g)(\phi\,; \text{id}_H) &= ((g)\phi)\text{id}_H\
				&=(g)\phi\
			\phi\,; \text{id}_H &= \phi
		\end{aligned} quad
		\begin{aligned}
			(h)(\text{id}_H\,;\psi) &= ((h)\text{id}_H)\psi\
				&=(h)\psi\
			\text{id}_H\,;\psi &= \psi
		\end{aligned}
	
	$$So $\text{id}_H$ is the identity of $H$.
- Associativity:
	By [[Function composition is associative]].
Then $\mathbf{Grp}$ is a category.