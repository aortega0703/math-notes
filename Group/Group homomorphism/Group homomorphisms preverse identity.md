---
tags:
  - theorem
  - abstract_algebra
related topics:
  - "[[Group homomorphism]]"
---
For any [[Group homomorphism]] $\phi:G\to H$$$
	\phi(e_G) = e_H
$$
##### Proof:
Let $g\in G$, then$$
\begin{align}
	\phi(g) = \phi(g e_G) &= \phi(g) \phi(e_G)\\
	\phi(g)^{-1}\phi(g) &= \phi(g)^{-1}\phi(g)\phi(e_G)\\
	e_H &= \phi(e_G)
\end{align}
$$