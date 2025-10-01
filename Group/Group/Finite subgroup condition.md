---
related topics:
  - "[[Group]]"
  - "[[Subgroup]]"
tags:
  - theorem
  - math/abstract_algebra
---
For a [[Group]] $G$ and $H\subseteq G$ non-empty and finite, $H$ is a [[Subgroup]] of $G$ if and only if $H$ is closed under $\cdot$.
##### Proof:
- $\implies$:
	By hypothesis $H$ is a group so it is closed under $\cdot$.
- $\impliedby$:
	Let $a in H$, and consider the sequence $(a^n)_{n in  ZZ}$. As $H$ is finite there exist some $i> j$ such that $a^i = a^j$, then$$
	
		a^i a^{-j} &= e\
		a^{i-j} &= e\
		a^{i-j}a^{-1} &= a^{-1}\
		a^{i-j-1} &=  a^{-1}
	
	$$As $i>j$, then $i-j>0$ and $i-j-1 \geq 0$ so $a^{i-j-1}=a^{-1}  in H$ and by [[Subgroup criteria]] $H$ is a subgroup of $G$.