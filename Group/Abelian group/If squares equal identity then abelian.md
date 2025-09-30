---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Abelian group]]"
---
If $G$ is a [[Group]] such that $a^2=e$ for all $a\in G$, then $G$ is [[Abelian group|Abelian]].
##### Proof:
$a^2=e$ implies $a=a^{-1}$, then$$
\begin{align}
	(ab)^2 
	&= e\\
	ab &= (ab)^{-1}\\
	ab &= b^{-1} a^{-1}\tag{$*$}\\
	ab &= ba
\end{align}
$$Where ($*$) is by [[Socks-shoes property]]. Then $G$ is Abelian.