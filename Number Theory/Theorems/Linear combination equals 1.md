---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Greatest Common Divisor|GCD]]"
  - "[[Greatest Common Divisor|Relative Prime]]"
mathLink: $1=as+bt \iff \gcd(a,b)=1$
---
For $a,b\in\mathbb{Z}$, $a$ and $b$ are relative primes if and only if $1=as+bt$ for some $s,t\in\mathbb{Z}$.
##### Proof:
- $\implies$:
	Trivially by [[GCD is linear combination]].
- $\impliedby$:
	By [[GCD is linear combination]] $\gcd(a,b)$ is the smallest positive integer of the form $as' + bt'$, and $as+bt=1$ is the smallest positive integer, therefore $1=\gcd(a,b)$.