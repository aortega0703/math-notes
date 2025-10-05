---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Group]]"
  - "[[Order]]"
  - "[[Cyclic group]]"
mathLink: $\langle a^k\rangle = \langle a^{gcd(|a|,k)}\rangle$ and $|a^k| = |a|/gcd(|a|,k)$
---
For a [[Group]] $G$, $a in G$ and $k in ZZ^+$, $\langle a^k\rangle = \langle a^{op("gcd")(|a|,k)}\rangle$ and $|a^k| = |a|/op("gcd")(|a|,k)$.
##### Proof:
- $\langle a^k\rangle = \langle a^{op("gcd")(|a|,k)}\rangle$:
	- $\langle a^k\rangle subset.eq \langle a^{op("gcd")(|a|,k)}\rangle$:
		By definition $k=qop("gcd")(k,|a|)$ for some $q in ZZ$, so for $n in ZZ$$$
		
			\left(a^k\right)^n 
				&= \left(a^{qop("gcd")(k,|a|)}\right)^n\
				&= \left(a^{op("gcd")(k,|a|)}\right)^{qn}\
			\left(a^k\right)^n 
				& in \left\langle a^{op("gcd")(k,|a|)} \right\rangle\
			\langle a^k\rangle & subset.eq \left\langle a^{op("gcd")(k,|a|)} \right\rangle\
		$$
	- $\langle a^{op("gcd")(|a|,k)}\rangle subset.eq \langle a^k\rangle$:
		By [[GCD is linear combination]] $op("gcd")(|a|,k) = |a|s + kt$ for some $s,t in ZZ$, then$$ 
		
			\left(a^{op("gcd")(|a|,k)}\right)^n
				&= \left(a^{|a|s+kt}\right)^n\
				&= \left(a^{|a|s}a^{kt}\right)^n\
				&= \left(a^{kt}\right)^n\tag{1}\
				&= \left(a^k\right)^nt\
			\left(a^{op("gcd")(|a|,k)}\right)^n
				& in \left\langle a^k\right\rangle\
			\left\langle a^{op("gcd")(|a|,k)}\right\rangle 
				& subset.eq \left\langle a^k\right\rangle
		$$Where $(1)$ is by [[Order divides exponent]].
	Therefore $\left\langle a^k\right\rangle = \left\langle a^{op("gcd")(|a|,k)}\right\rangle$.
- $|a^k| = |a|/op("gcd")(|a|,k)$:
	- If $d$ divides $|a|$ then $\left | a^d \right | = |a|/d$: 
		$|a|/d in ZZ$ since $d$ divides $|a|$, then$$
		
			\left(a^d\right)^{|a|/d} 
				&= a^{|a|}\
				&= e\
			\left|a^d\right| & lt.eq \frac{|a|}{d}
		$$
		$d(|a|/d) = |a|$ so $ds<|a|$ for $0<s<|a|/d$, implying $\left(a^d\right)^s != e$ . Therefore $\left | a^d \right | = |a|/d$.
	$op("gcd")(|a|,k)$ divides $|a|$ by definition, so$$
	
		\left|a^k\right| 
			&= \left|\left\langle
				a^k
			\right\rangle\right|
			\tag{1}\
			&= \left|\left\langle
				a^{op("gcd")(|a|,k)}
			\right\rangle\right|\
			&= \left|a^{op("gcd")(|a|,k)}
			\right|\tag{2}\
			&= \frac{|a|}{op("gcd")(|a|,k)}
	
	$$Where $(1)$ and $(2)$ are by [[Order of cyclic group is order of generator]].