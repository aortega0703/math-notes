---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Isomorphism]]"
---
For an [[Isomorphism]] $f:A -> B$ and its inverse $f^{-1}:B -> A$
- $f^{-1}$ is an isomorphism.
- $(f^{-1})^{-1} = f$.
##### Proof:
- $f^{-1}$ is isomorphism:
	$f f^{-1}= \operatorname{id}_B$ and $f^{-1}f = \operatorname{id}_A$, so $f$ is left and right inverse of $f^{-1}$ making it an isomorphism.
- $(f^{-1})^{-1} = f$:
	$$
	
		(f^{-1})^{-1} f^{-1}&= \operatorname{id}_B\
		(f^{-1})^{-1} f^{-1} f &= \operatorname{id}_B f\
		(f^{-1})^{-1} \operatorname{id}_A &= \operatorname{id}_B f\
		(f^{-1})^{-1} &= f
	
	$$