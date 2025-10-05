---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Abelian group]]"
mathLink: $ab=ba <==> (ab)^{-1}=a^{-1}b^{-1}$
---
For a [[Group]] $G$, $G$ is [[Group|Abelian]] if and only if $(ab)^{-1}=a^{-1}b^{-1}$.
##### Solution:
- $ ==> $:
	By [[Socks-shoes property]]$$
	
		(ab)^{-1}
		&= b^{-1}a^{-1}\
		&= a^{-1} b^{-1}
	
	$$
- $\impliedby$:$$
	
		e &= (ba)(ba)^{-1}\
		&= (ba)(a^{-1}b^{-1})\tag{$*$}\
		&= (ba)(ab)^{-1}\
		ab &= ba
	
	$$Where ($*$) is by [[Socks-shoes property]].
