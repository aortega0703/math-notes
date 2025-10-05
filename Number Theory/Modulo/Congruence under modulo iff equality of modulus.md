---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Congruence under modulo|Congruence mod n]]"
  - "[[Division|Modulo]]"
mathLink: $a\equiv b\ (op("mod")\ n) <==> a\ op("mod")\ n = b\ op("mod") n$
---
For $a,b,n in ZZ$$$
	a\equiv b\ (op("mod")\ n)
	 <==> a\ op("mod")\ n 
		= b\ op("mod") n
$$
##### Proof:
- $ ==> $:
	If $a\equiv b\ (op("mod")\ n)$ then$$
	
		a-b&=kn
			&\text{for some $k in ZZ$}\
		a &= kn + b\
		&= kn + (q_b n+ r_b)\tag{$*$}\
		&= (k+q_b)n + r_b
	$$Where $(*)$ is by [[Division algorithm]]. As $r_b$ is unique, $a\ op("mod")\ n = r_b = b\ op("mod")\ n$.
- $\impliedby$:
	$a = q_a n + r$ and $b= q_b n + r$, then $a-b = (q_a - q_b)n$. Therefore $a\equiv b\ (op("mod")\ n)$.