---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Congruence under modulo]]"
  - "[[Division|Modulo]]"
mathLink: $a+b \equiv_n (a\ \operatorname{mod}\ n) + (b\ \operatorname{mod}\ n)$
---
For $a,b,n in ZZ$$$
a+b \equiv_n (a\ \operatorname{mod}\ n) + (b\ \operatorname{mod}\ n)$$
##### Proof:
Consider$$

	&\hspace{1.25em}(a+b)-\big((a\ \operatorname{mod}\ n) 
		+ (b\ \operatorname{mod}\ n)\big)\
	&=(a - a\ \operatorname{mod}\ n) + (b - b\ \operatorname{mod}\ n)\
	&=n q_a + n q_b\tag{$*$}\
	&= n(q_a + q_b)\
	n&\ \ |\ \ (a+b)-\big((a\ \operatorname{mod}\ n) 
		+ (b\ \operatorname{mod}\ n)\big)

$$Where $(*)$ is by [[Division algorithm]]. Therefore $a+b \equiv_n (a\ \operatorname{mod}\ n) + (b\ \operatorname{mod}\ n)$
