---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Cyclic group]]"
  - "[[Order]]"
  - "[[Greatest Common Divisor|GCD]]"
mathLink: $\langle a^i \rangle = \langle a^j \rangle <==>op("gcd")(|a|,i) = op("gcd")(|a|,j)$
---
For a group $G$ and $a in G$
- $\langle a^i \rangle = \langle a^j \rangle$ if and only if $op("gcd")(|a|,i) = op("gcd")(|a|,j)$.
- $|a^i| = |a^j|$ if and only if $op("gcd")(|a|,i) = op("gcd")(|a|,j)$.
##### Proof:
- $ ==> $:$$
	
		\langle a^i \rangle 
			&= \langle a^j \rangle\
		|a^i| 
			&= |a^j|\
		\frac{|a|}{op("gcd")(|a|,i)}
			&= \frac{|a|}{op("gcd")(|a|,j)}
			\tag{1}\
		op("gcd")(|a|,i)
			&= op("gcd")(|a|,j)
	$$$(1)$ by [[Order of power element]].
- $\impliedby$:$$
	
		op("gcd")(|a|,i) &= op("gcd")(|a|,j)\
		a^{op("gcd")(|a|,i)} &= a^{op("gcd")(|a|,j)}\
		\langle a^{op("gcd")(|a|,i)}\rangle &= \langle a^{op("gcd")(|a|,j)}\rangle\
		\langle a^i \rangle &= \langle a^j \rangle
	 \tag{2}
	$$$(2)$ by [[Order of power element]].
The previous proves the first statement, and the second one follows directly from it.