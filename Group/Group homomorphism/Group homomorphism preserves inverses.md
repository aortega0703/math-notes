---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Group homomorphism]]"
---
For any [[Group homomorphism]] $\phi:G\to H$$$
	\phi(g^{-1})=\phi(g)^{-1}
$$
##### Proof:
Let $g\in G$, then by [[Group homomorphisms preverse identity]]$$
\begin{align}
	e_H &= \phi(e_G)\\
	&= \phi(gg^{-1})\\
	&= \phi(g)\phi(g^{-1})\\
	\phi(g)^{-1} &= \phi(g)^{-1}\phi(g)\phi(g^{-1})\\
	&= \phi(g^{-1})
\end{align}
$$