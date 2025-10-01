---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Division|Modulo]]"
  - "[[Greatest Common Divisor|GCD]]"
mathLink: $ax\equiv 1\ \operatorname{mod}n  <==> \gcd(a,n)=1$
---
For $a,n in ZZ$, $ax\equiv 1\ (\operatorname{mod}\ n)$ has a solution for $x$ if and only if $a$ and $n$ are [[Greatest Common Divisor|Relative Primes]].
##### Proof:
- $\implies$:
	By definition$$
	
		ax &= qn + 1 quad\text{for some $q in ZZ$}\
		ax - qn &= 1\
		ax + n(-q) &= 1
	
	$$So by [[Relative Primes Iff Linear Combination Equals 1]] $a$ and $n$ are relative primes.
- $\impliedby$:
	By definition$$
	
		1 &= as + nt quad\text{for some $s,t in ZZ$}\
		1 &\equiv as\ (\operatorname{mod} n)
	
	$$So $x=s$ is the solution for the expression.