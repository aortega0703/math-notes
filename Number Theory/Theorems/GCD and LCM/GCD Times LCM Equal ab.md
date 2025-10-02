---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Least common multiple|LCM]]"
  - "[[Greatest Common Divisor|GCD]]"
mathLink: $ab=\gcd(a,b)\operatorname{lcm}(a,b)$
---
For positive $a,b in ZZ$, $ab=\gcd(a,b)\operatorname{lcm}(a,b)$.
##### Proof:
Let $a=a'\gcd(a,b)$ and $b=b'\gcd(a,b)$, then $\gcd(a,b)$ divides $ab$ trivially. Then for some $q in ZZ$$$

	ab &= q\gcd(a,b)\
	\begin{aligned}
		a'\gcd(a,b)b &= q\gcd(a,b)\
		a'b &= q
	\end{aligned}&\qquad
	\begin{aligned}
		ab'\gcd(a,b) &= q\gcd(a,b)\
		ab' &= q
	\end{aligned}

$$So $q$ is a multiple of $a$ and $b$. Now let $m$ be another multiple of $a$ and $b$. Then for some $c in ZZ$$$

	m&=ac\
	&=a'\gcd(a,b)c\
	b&\ \  |\ \ a'\gcd(a,b)c quad\text{(by hypothesis $b$ divides $m$)}\
	b'\gcd(a,b)&\ \ |\ \ a'\gcd(a,b)c\
	b'&\ \ |\ \ a'c\
	b'&\ \ |\ \ c\tag{1}\
	b' & lt.eq c\
	ab' & lt.eq ac\
	q & lt.eq m

$$Where $(1)$ is by [[Euclid's lemma]] and [[GCD Factors Into Relative Primes]]. Therefore $q=\operatorname{lcm}(a,b)$.