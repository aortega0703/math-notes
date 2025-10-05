---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Cyclic group]]"
  - "[[Greatest Common Divisor|GCD]]"
mathLink: $\langle a \rangle = \langle a^i \rangle <==> \operatorname{gcd}(|a|,i) = 1$
---
For a group $G$ and $a in G$
- $\langle a \rangle = \langle a^i \rangle <==> \operatorname{gcd}(|a|,i) = 1$
- $| a | = | \langle a^i \rangle| <==> \operatorname{gcd}(|a|,i) = 1$
##### Proof:
- $\langle a \rangle = \langle a^i \rangle <==> \operatorname{gcd}(|a|,i) = 1$:
	- $ ==> $:
		By [[Criterion for Equality of Cyclic Groups]] $\operatorname{gcd}(|a|,i) = \operatorname{gcd}(|a|,1) = 1$.
	- $\impliedby$:
		$\operatorname{gcd}(|a|,i) = 1 = \operatorname{gcd}(|a|,1)$, then by [[Criterion for Equality of Cyclic Groups]] $\langle a^i \rangle = \langle a \rangle$.
- $| a | = | \langle a^i \rangle| <==> \operatorname{gcd}(|a|,i) = 1$:
	Follows from the previous result and [[Order of cyclic group is order of generator]].