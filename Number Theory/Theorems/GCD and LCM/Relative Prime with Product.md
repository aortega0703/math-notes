---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Greatest Common Divisor|Relative Prime]]"
mathLink: $\gcd(a,bc)=1  <==> \gcd(a,b)=\gcd(a,c)=1$
---
For $a,b,c in ZZ$, $\gcd(a,bc)=1$ if and only if $\gcd(a,b)=\gcd(a,c)=1$.
##### Proof:
- $\gcd(a,bc)=1 \implies \gcd(a,b)=\gcd(a,c)=1$:
	By [[Relative Primes Iff Linear Combination Equals 1]] $1 = as + (bc)t$ for some $s,t in ZZ$. Then $1 = as + b(ct) = as + c(bt)$ so by [[Relative Primes Iff Linear Combination Equals 1]] $a$ is a relative prime of $b$ and $c$.
- $\gcd(a,b)=\gcd(a,c)=1 \implies \gcd(a,bc)=1$:
	Let $p$ be a prime such that $p|a$ and $p|bc$. By [[Euclid's lemma]] $p|b$ or $p|c$, so $p$ is a common divisor of $a$ and $b$ or a common divisor of $a$ and $c$. In either case as $\gcd(a,b)=\gcd(a,c)=1$ then $p=1$ implying $\gcd(a,bc)=1$.