---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Cyclic group]]"
  - "[[Greatest Common Divisor|GCD]]"
mathLink: $\langle a \rangle = \langle a^i \rangle <==> op("gcd")(|a|,i) = 1$
---
For a group $G$ and $a in G$
- $\langle a \rangle = \langle a^i \rangle <==> op("gcd")(|a|,i) = 1$
- $| a | = | \langle a^i \rangle| <==> op("gcd")(|a|,i) = 1$
##### Proof:
- $\langle a \rangle = \langle a^i \rangle <==> op("gcd")(|a|,i) = 1$:
	- $ ==> $:
		By [[Criterion for Equality of Cyclic Groups]] $op("gcd")(|a|,i) = op("gcd")(|a|,1) = 1$.
	- $\impliedby$:
		$op("gcd")(|a|,i) = 1 = op("gcd")(|a|,1)$, then by [[Criterion for Equality of Cyclic Groups]] $\langle a^i \rangle = \langle a \rangle$.
- $| a | = | \langle a^i \rangle| <==> op("gcd")(|a|,i) = 1$:
	Follows from the previous result and [[Order of cyclic group is order of generator]].