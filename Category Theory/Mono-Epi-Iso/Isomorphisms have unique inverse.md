---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Isomorphism]]"
---
For an [[Isomorphism]] $f:A\overset{\sim}{\to} B$, its inverse $f^{-1}: B \to A$ is unique.
##### Proof:
Let $g,h: B\to A$ be inverses of $f$, then$$

	\operatorname{id}_A &= \operatorname{id}_A\
	g\circ f &= h \circ f\
	g\circ f \circ g &= h \circ f \circ g\
	g \circ \operatorname{id}_B &= f \circ \operatorname{id}_B\
	g &= f

$$