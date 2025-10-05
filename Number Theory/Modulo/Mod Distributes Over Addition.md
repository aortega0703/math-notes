---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Congruence under modulo]]"
  - "[[Division|Modulo]]"
mathLink: $a+b \equiv_n (a\ op("mod")\ n) + (b\ op("mod")\ n)$
---
For $a,b,n in ZZ$$$
a+b \equiv_n (a\ op("mod")\ n) + (b\ op("mod")\ n)$$
##### Proof:
Consider$$

	&\hspace{1.25em}(a+b)-\big((a\ op("mod")\ n) 
		+ (b\ op("mod")\ n)\big)\
	&=(a - a\ op("mod")\ n) + (b - b\ op("mod")\ n)\
	&=n q_a + n q_b\tag{$*$}\
	&= n(q_a + q_b)\
	n&\ \ |\ \ (a+b)-\big((a\ op("mod")\ n) 
		+ (b\ op("mod")\ n)\big)

$$Where $(*)$ is by [[Division algorithm]]. Therefore $a+b \equiv_n (a\ op("mod")\ n) + (b\ op("mod")\ n)$
