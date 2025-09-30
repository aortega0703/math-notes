---
tags:
  - definition
  - math/abstract_algebra
  - theorem
related topics:
  - "[[Group]]"
  - "[[Set Product]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
For groups $G,H$ their _direct product_ is a group on the [[Set]] $G\times H$ with the operation$$
\begin{align}
	\cdot: (G\times H)\times(G\times H) &\to (G\times H)\\
	\big((g_1,h_1),\ (g_2,h_2)\big) &\mapsto (g_1 g_2, h_1 h_2)
\end{align}
$$
---
$G\times H$ is a group.
##### Proof:
- Closed under multiplication:
	By the definition of the operation.
- Associative:
	Let $g_1,g_2,g_3\in G$ and $h_1,h_2,h_3\in H$ then$$
	\begin{align}
		\big((g_1,h_1)\cdot(g_2,h_2)\big)\cdot(g_3,h_3)
		&= (g_1g_2, h_1 h_2)\cdot (g_3, h_3)\\
		&= (g_1 g_2 g_3, h_1 h_2 h_3)\\
		&= (g_1,h_1)\cdot(g_2g_3, h_2h_3)\\
		&= (g_1,h_1)\cdot\big((g_2,h_2)\cdot(g_3, h_3)\big)\\
	\end{align}
	$$
	So multiplication on $G\times H$ is associative.
- Identity:
	Let $g\in G$ and $h\in H$, then$$
	\begin{align}
		(e_G,e_H)\cdot (g,h) 
		&= (e_G g, e_H h)\\
		&= (g, h)\\
		&= (g e_G, h e_H)\\
		&= (g,h)\cdot(e_G, e_H)
	\end{align}
	$$
	So $(e_G, e_H)\in G\times H$ is the identity.
- Inverses:
	Let $g\in G$ and $h\in H$, then $$
	\begin{align}
		(g,h)\cdot(g^{-1}, h^{-1})
		&=(g g^{-1}, hh^{-1})\\
		&=(e_G, e_H)\\
		&=(g^{-1}g,h^{-1}h)\\
		&=(g^{-1},h^{-1})\cdot(g,h)
	\end{align}
	$$
	So $(g,h)^{-1}=(g^{-1},h^{-1})$.
Then $G\times H$ is a group.