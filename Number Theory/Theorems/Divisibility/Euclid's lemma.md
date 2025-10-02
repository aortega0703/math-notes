---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Divisibility]]"
  - "[[Divisibility|Prime]]"
aliases:
  - p Divides Product Implies p Divides Factors
mathLink: $p|ab \implies p|a \lor p|b$
---
For $a,b,p in ZZ$, if $p$ is a prime that divides $ab$ then $p|a$ or $p|b$.
##### Proof:
It is given that $ab=kp$ for some $k in ZZ$. Suppose $p$ does not divide $a$, then by [[Relative Primes Iff Linear Combination Equals 1]]$$

	1 &= ps + at quad\text{for some $s,t in ZZ$}\
	b &= b(ps + at)\
		&= bps + abt\
		&= bps + kpt\
		&= p(bs + kt)
$$So $p|b$. By symmetry if $p$ does not divides b it must divide $a$. Therefore $p$ divides either $a$ or $b$.