---
tags:
  - abstract_algebra
  - category_theory
  - theorem
related topics:
  - "[[Product]]"
  - "[[Category of groups]]"
---
For groups $G,H$ their [[Direct product]] $G\times H$ is a [[Product]].
##### Proof:
- Projections are [[Group homomorphism|homomorphisms]]:
	Let $g_1,g_2\in G$ and $h_1,h_2\in H$, then$$
	\begin{align}
		\pi_1\big((g_1,h_1)\cdot(g_2,h_2)\big)
		&= \pi_1(g_1g_2,h_1h_2)\\
		&= g_1g_2\\
		&= \pi_1(g_1,h_1)\cdot\pi_1(g_2,h_2)
	\end{align}
	$$So $\pi_1:G\times H\to G$ is a homomorphism, similarly $\pi_2:G\times H\to H$ is a homomorphism too.
- It is a product:
	By [[Cartesian product is a product]].
Then, $G\times H$ is a product with $\pi_1$ and $\pi_2$.