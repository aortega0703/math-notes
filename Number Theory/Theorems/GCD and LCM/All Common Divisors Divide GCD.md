---
tags:
  - math/number_theory
  - theorem
related topics:
  - "[[Greatest Common Divisor|GCD]]"
---
For $a,b,d in ZZ$, if $d$ is a common divisor of $a,b$ then $d$ divides $\gcd(a,b)$.
##### Proof:
By [[Division algorithm]] for some $q,(0 lt.eq r < d) in ZZ$$$

	\gcd(a,b)&=qd+r\
	as+bt&=qd+r quad\text{for some $s,t in ZZ$}\tag{1}\
	0&\equiv r\ (\operatorname{mod}d)

$$Where $(1)$ is by [[GCD is linear combination]]. As $r<d$ then $r=0$ and therefore $d$ divides $\gcd(a,b)$.