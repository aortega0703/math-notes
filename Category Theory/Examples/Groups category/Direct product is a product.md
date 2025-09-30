---
tags:
  - math/abstract_algebra
  - category_theory
  - theorem
related topics:
  - "[[Product]]"
  - "[[Notes/Category Theory/Examples/Groups category/Category of groups]]"
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
	$$So $\pi_1:G\times H\to G$ is a homomorphism, similarly $\pi_2:G\times H\to H$ is a homomorphism too. Therefore they are arrows in $\mathbf{Grp}$.
- $f\times g$ is an homomorphism:
	Let $x_1,x_2\in X$ for an arbitrary group $X$, and $f\times g$ as in the product in $\mathbf{Set}$. Then$$
	\begin{align}
		(f\times g)(x_1 \cdot x_2)
		&= \big(f(x_1\cdot x_2),\ g(x_1 \cdot x_2)\big)\\
		&= \big(f(x_1)\cdot f(x_2),\ g(x_1)\cdot g(x_2)\big)\\
		&= \big(f(x_1),\ g(x_1))\cdot \big(f(x_2),\ g(x_2)\big)\\
		&= (f\times g)(x_1) \cdot (f\times g)(x_2)
	\end{align}
	$$So $f\times g:X\to G\times H$ is an homomorphism, meaning it is an arrow in $\mathbf{Grp}$.
- It is a product:
	By [[Cartesian product is a product]].
Then, $G\times H$ is a product with $\pi_1$ and $\pi_2$.