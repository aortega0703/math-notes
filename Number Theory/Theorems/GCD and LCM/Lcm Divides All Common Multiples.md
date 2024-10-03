---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Least common multiple]]"
  - "[[Set]]"
---
For a finite set of integers $S$, every (positive) common multiple of $S$ is a multiple of $\operatorname{lcm}(S)$.
##### Proof:
Let $(m>0)\in \mathbb{Z}$ such that $s | m$ for all $s\in S$, then by [[Division algorithm]]
$$
\begin{align}
	\exists (0\leq r<\operatorname{lcm}(S)),q\in\mathbb{Z}.\quad 
	m &= q\operatorname{lcm}(S) + r\\
	\forall s\in S.\exists c,k\in\mathbb{Z}.\quad
	c s &= q(k s) + r\\
	c s - q(k s) &= r\\
	(c - qk) s &= r\\
	s &\ \ |\ \ r
\end{align}
$$
So $r$ is a multiple of all $s\in S$ but is also less than $\operatorname{lcm}(S)$, so it must be $0$. Therefore $m$ is a multiple of $\operatorname{lcm}(S)$.