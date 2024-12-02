---
tags:
  - theorem
  - abstract_algebra
  - category_theory
related topics:
  - "[[Category of abelian groups]]"
---
For [[Abelian group|abelian groups]] $G,H$, their [[Direct product]] $G\times H$ is also abelian. This means that $\mathbf{Ab}$ has products.
##### Proof:
Let $(g_1,h_1),\ (g_2,h_2)\in G\times H$, then$$
\begin{align}
	(g_1,h_1)(g_2,h_2)
	&= (g_1 g_2, h_1 h_2)\\
	&= (g_2 g_1, h_2 h_1)\\
	&= (g_2, h_2)(g_1, h_1)
\end{align}
$$Then $G\times H$ is abelian.