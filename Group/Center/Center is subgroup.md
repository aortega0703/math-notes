---
related topics:
  - "[[Group]]"
  - "[[Center]]"
  - "[[Subgroup]]"
tags:
  - theorem
  - math/abstract_algebra
mathLink: $Z(G) \leq G$
---
For a [[Group]] $G$, its center $Z(G)$ is a [[Subgroup]] of $G$.
##### Proof:
By [[Subgroup criteria]] we only need to prove
- Non-emptiness:
	Let $x\in G$, then $xe=ex=e$ so $e\in G$.
- Closed under $\cdot$:
	Let $a,b\in Z(G)$ and $x\in G$, then$$
	\begin{align}
	x(ab) &= (xa)b\\
		&= (ax)b\\
		&= a(xb)\\
		&= a(bx)\\
		&= (ab)x
	\end{align}
	$$ So $ab\in Z(G)$.
- Closed under inverses:
	Let $a\in Z(G)$ and $x\in G$, then$$
	\begin{align}
	xa^{-1} &= exa^{-1}\\
		&= a^{-1}axa^{-1}\\
		&= a^{-1}xaa^{-1}\\
		&= a^{-1}x
	\end{align}$$So $a^{-1}\in Z(G)$.
Therefore $Z(G)$ is a subgroup of $G$.