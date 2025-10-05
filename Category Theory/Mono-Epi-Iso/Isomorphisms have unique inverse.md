---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Isomorphism]]"
---
For an [[Isomorphism]] $f:A arrow.r.tilde B$, its inverse $f^{-1}: B -> A$ is unique.
##### Proof:
Let $g,h: B -> A$ be inverses of $f$, then$$

	op("id")_A &= op("id")_A\
	g compose f &= h compose f\
	g compose f  compose g &= h compose f  compose g\
	g compose op("id")_B &= f compose op("id")_B\
	g &= f

$$