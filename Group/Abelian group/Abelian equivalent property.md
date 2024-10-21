---
tags:
  - theorem
  - abstract_algebra
related topics:
  - "[[Abelian group]]"
mathLink: $ab=ba \iff (ab)^{-1}=a^{-1}b^{-1}$
---
For a [[Group]] $G$, $G$ is [[Group|Abelian]] if and only if $(ab)^{-1}=a^{-1}b^{-1}$.
##### Solution:
- $\implies$:
	By [[Socks-shoes property]]$$
	\begin{align}
		(ab)^{-1}
		&= b^{-1}a^{-1}\\
		&= a^{-1} b^{-1}
	\end{align}
	$$
- $\impliedby$:$$
	\begin{align}
		e &= (ba)(ba)^{-1}\\
		&= (ba)(a^{-1}b^{-1})\tag{$*$}\\
		&= (ba)(ab)^{-1}\\
		ab &= ba
	\end{align}
	$$Where ($*$) is by [[Socks-shoes property]].
