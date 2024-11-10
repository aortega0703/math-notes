---
tags:
  - definition
  - category_theory
related topics:
  - "[[Group]]"
  - "[[Group homomorphism]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
The [[Category]] of [[Group|groups]] $\mathbf{Grp}$ is defined by
- $\text{Obj}(\mathbf{Grp})=$ the collection of all groups.
- $\text{Hom}_\mathbf{Grp}(G,H)=$ the collection of [[Group homomorphism|group homomorphisms]] $G\to H$.
- $\circ=$ [[Function|Function composition]].
---
This data does describe a [[Category]].
##### Proof:
- Closed under $\circ$:
	Let $G\overset{\phi}{\to} H\overset{\psi}{\to} K$ be [[Group homomorphism|group homomorphisms]]. This gives the following diagram
	![[Grp composition.png]]
	As the inner squares commute so does the outer rectangle. Then $\mathbf{Grp}$ is closed under composition.
- Identities:
	Let $H$ be a group, then $\text{id}_H: H \to H$ is trivially a group homomorphism. Let $G\overset{\phi}{\to} H\overset{\psi}{\to} K$, then$$
	\begin{align}
		\begin{aligned}
			(g)(\phi\,; \text{id}_H) &= ((g)\phi)\text{id}_H\\
				&=(g)\phi\\
			\phi\,; \text{id}_H &= \phi
		\end{aligned}\quad
		\begin{aligned}
			(h)(\text{id}_H\,;\psi) &= ((h)\text{id}_H)\psi\\
				&=(h)\psi\\
			\text{id}_H\,;\psi &= \psi
		\end{aligned}
	\end{align}
	$$So $\text{id}_H$ is the identity of $H$.
- Associativity:
	By [[Function composition is associative]].
Then $\mathbf{Grp}$ is a category.