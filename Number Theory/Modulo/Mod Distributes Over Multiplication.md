---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Division|Modulo]]"
  - "[[Congruence under modulo]]"
mathLink: $ab \equiv_n (a\ \operatorname{mod}\ n)(b\ \operatorname{mod}\ n)$
---
For $a,b,n in ZZ$$$
ab \equiv_n (a\ \operatorname{mod}\ n)(b\ \operatorname{mod}\ n)$$
##### Proof:
Consider$$

	&\hspace{1.25em}
		ab-(a\ \operatorname{mod}\ n)(b\ \operatorname{mod}\ n)\
	&=(n q_a +r_a)(n q_b +r_b)
		- (a\ \operatorname{mod}\ n)(b\ \operatorname{mod}\ n)
		\tag{$*$}\
	&=(n^2 q_a q_b+ n q_a r_b + n q_b r_a + r_a r_b)
		- (a\ \operatorname{mod}\ n)(b\ \operatorname{mod}\ n)\
	&=n^2 q_a q_b+ n q_a r_b + n q_b r_a\
	&= n(nq_a q_b + q_a r_b+ q_b r_a)\
	n&\ \ |\ \ ab-(a\ \operatorname{mod}\ n)(b\ \operatorname{mod}\ n)

$$Where $(*)$ is by [[Division algorithm]]. Therefore $ab \equiv_n (a\ \operatorname{mod}\ n)(b\ \operatorname{mod}\ n)$.
