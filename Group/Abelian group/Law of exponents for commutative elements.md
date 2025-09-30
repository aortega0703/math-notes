---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Abelian group]]"
---
If $G$ is a [[Group]] and $a,b\in G$, if $ab=ba$ then $(ab)^n=a^nb^n$.
##### Proof:
- Step $n=0$:
	$(ab)^0=e=ee=a^0 b^0$.
- Step $n+1$:$$
	\begin{align}
		(ab)^{n+1}
		&= (ab)^n(ab)\\
		&= a^n b^n ab
			&\text{by induction}\\
		&= a^n a b^nb\\
		&=a^{n+1}b^{n+1}
	\end{align}
	$$
So $(ab)^n=a^nb^n$ for all $n$.
