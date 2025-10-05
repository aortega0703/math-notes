---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Divisibility]]"
---
For any $n in ZZ$, the smallest $d>1$ that divides $n$ is prime.
##### Proof:
Suppose $d$ is not prime, then $d=ab$ for some $1<a,b<d$. As $d|n$ then$$

	n &= kd quad\text{for some $k in ZZ$}\
		&= kab\
		&= a(kb)

$$So $a|n$ which is a contradiction with $a<d$ as $d$ is chosen as the smallest divisor of $n$. Therefore $d$ is prime.