---
related topics:
  - "[[Group]]"
  - "[[Centralizer]]"
  - "[[Subgroup]]"
tags:
  - theorem
  - math/abstract_algebra
mathLink: $C(x) \leq G$
---
For a [[Group]] $G$ and $x\in G$, the [[Centralizer]] $C(x)$ is a [[Subgroup]] of $G$.
##### Proof:
By [[Subgroup criteria]] we only need to prove
- Non-emptiness:
	$ex=xe=x$ so $e\in C(a)$.
- Closed under $\cdot$:
	Let $a,b\in C(x)$, then$$
	\begin{align}
		(ab)x &= a(bx)\\
			&= a(xb)\\
			&= (ax)b\\
			&= (xa)b\\
			&= x(ab)
	\end{align}$$
	So $ab\in C(x)$.
- Closed under inverses:
	Let $a\in C(x)$, then$$
	\begin{align}
		a^{-1}x &= a^{-1}x e\\
			&= a^{-1}xaa^{-1}\\
			&= a^{-1}axa^{-1}\\
			&= xa^{-1}
	\end{align}$$So $a^{-1}\in C(x)$.
Therefore $C(x)$ is a subspace of $G$.