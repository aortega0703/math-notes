---
tags:
  - theorem
  - category_theory
related topics:
  - "[[Notes/Category Theory/Morphism/Isomorphism]]"
---
For an [[Notes/Category Theory/Morphism/Isomorphism]] $f:A\overset{\sim}{\to} B$, its inverse $f^{-1}: B \to A$ is unique.
##### Proof:
Let $g,h: B\to A$ be inverses of $f$, then$$
\begin{align}
	\operatorname{id}_A &= \operatorname{id}_A\\
	g\circ f &= h \circ f\\
	g\circ f \circ g &= h \circ f \circ g\\
	g \circ \operatorname{id}_B &= f \circ \operatorname{id}_B\\
	g &= f
\end{align}
$$