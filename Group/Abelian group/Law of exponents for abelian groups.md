---
tags:
  - theorem
  - abstract_algebra
related topics:
  - "[[Abelian group]]"
---
If $G$ is [[Abelian group]] and $a,b\in G$, then $(ab)^n=a^nb^n$.
##### Proof:
- Step $n=0$:
	$(ab)^0=e=a^0 b^0$.
- Step $n+1$:$$
	\begin{align}
		(ab)^{n+1}
		&= (ab)^n(ab)
			&\text{by induction}\\
		&= a^n b^n ab\\
		&= a^n a b^nb\\
		&=a^{n+1}b^{n+1}
	\end{align}
	$$
So $(ab)^n=a^nb^n$ for all $n$.
