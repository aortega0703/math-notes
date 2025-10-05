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
For a [[Group]] $G$, $a in G$ and $k in ZZ^+$, $\langle a^k\rangle = \langle a^{\operatorname{gcd}(|a|,k)}\rangle$ and $|a^k| = |a|/\operatorname{gcd}(|a|,k)$.
##### Proof:
- $\langle a^k\rangle = \langle a^{\operatorname{gcd}(|a|,k)}\rangle$:
	- $\langle a^k\rangle \subseteq \langle a^{\operatorname{gcd}(|a|,k)}\rangle$:
		By definition $k=q\operatorname{gcd}(k,|a|)$ for some $q in ZZ$, so for $n in ZZ$$$
		
			\left(a^k\right)^n 
				&= \left(a^{q\operatorname{gcd}(k,|a|)}\right)^n\
				&= \left(a^{\operatorname{gcd}(k,|a|)}\right)^{qn}\
			\left(a^k\right)^n 
				& in \left\langle a^{\operatorname{gcd}(k,|a|)} \right\rangle\
			\langle a^k\rangle &\subseteq \left\langle a^{\operatorname{gcd}(k,|a|)} \right\rangle\
		$$
	- $\langle a^{\operatorname{gcd}(|a|,k)}\rangle \subseteq \langle a^k\rangle$:
		By [[GCD is linear combination]] $\operatorname{gcd}(|a|,k) = |a|s + kt$ for some $s,t in ZZ$, then$$ 
		
			\left(a^{\operatorname{gcd}(|a|,k)}\right)^n
				&= \left(a^{|a|s+kt}\right)^n\
				&= \left(a^{|a|s}a^{kt}\right)^n\
				&= \left(a^{kt}\right)^n\tag{1}\
				&= \left(a^k\right)^nt\
			\left(a^{\operatorname{gcd}(|a|,k)}\right)^n
				& in \left\langle a^k\right\rangle\
			\left\langle a^{\operatorname{gcd}(|a|,k)}\right\rangle 
				&\subseteq \left\langle a^k\right\rangle
		$$Where $(1)$ is by [[Order divides exponent]].
	Therefore $\left\langle a^k\right\rangle = \left\langle a^{\operatorname{gcd}(|a|,k)}\right\rangle$.
- $|a^k| = |a|/\operatorname{gcd}(|a|,k)$:
	- If $d$ divides $|a|$ then $\left | a^d \right | = |a|/d$: 
		$|a|/d in ZZ$ since $d$ divides $|a|$, then$$
		
			\left(a^d\right)^{|a|/d} 
				&= a^{|a|}\
				&= e\
			\left|a^d\right| & lt.eq \frac{|a|}{d}
		$$
		$d(|a|/d) = |a|$ so $ds<|a|$ for $0<s<|a|/d$, implying $\left(a^d\right)^s != e$ . Therefore $\left | a^d \right | = |a|/d$.
	$\operatorname{gcd}(|a|,k)$ divides $|a|$ by definition, so$$
	
		\left|a^k\right| 
			&= \left|\left\langle
				a^k
			\right\rangle\right|
			\tag{1}\
			&= \left|\left\langle
				a^{\operatorname{gcd}(|a|,k)}
			\right\rangle\right|\
			&= \left|a^{\operatorname{gcd}(|a|,k)}
			\right|\tag{2}\
			&= \frac{|a|}{\operatorname{gcd}(|a|,k)}
	
	$$Where $(1)$ and $(2)$ are by [[Order of cyclic group is order of generator]].