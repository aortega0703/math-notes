---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Abelian group]]"
  - "[[Group isomorphism]]"
---
For [[Group|groups]] $G\cong H$, $G$ is commutative if and only if $H$ is commutative.
##### Proof:
Let $\phi: G\to H$ be an isomorphism.
- $G$ commutative $\implies H$ commutative:
	Let $h_1,h_2\in H$, then$$
	\begin{align}
		h_1h_2
		&= \phi(g_1)\phi(g_2)
			&\text{for some $g_1,g_2\in G$}\\
		&= \phi(g_1g_2)\\
		&= \phi(g_2g_1)\\
		&= \phi(g_2)\phi(g_1)\\
		&= h_2h_1
	\end{align}
	$$
	Then $H$ is commutative.
The proof that the commutativity of $H$ implies the commutativity of $G$ is analogous (changing the use of $\phi$ with $\phi^{-1}$). Therefore $G$ is commutative if and only if $H$ is commutative.