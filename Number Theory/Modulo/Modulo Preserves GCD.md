---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Greatest Common Divisor|GCD]]"
  - "[[Division|Modulo]]"
mathLink: $\gcd(a,n) = \gcd(a\ op("mod")\ n,\ n)$
---
For all $a,b,n in ZZ$
$$
a\equiv b\ (\text{mod }n) ==> \gcd(a,n) = \gcd(b,n)
$$
##### Proof:
- $\gcd(a,n) lt.eq\gcd(b,n)$:
	Let $d in ZZ$ such that $d\ |\ a$ and $d\ |\ n$, so $a=a_d d$ and $n=n_d d$ for some $a_d$ and $n_d$, then$$
	
		a&\equiv b quad (\text{mod }n)\
		n&\ \ |\ \ a-b\
		a - b &= kn
			&\text{for some $k$}\
		a_dd -b &= n_d d\
		b &= a_dd-n_dd\
		&= (a_d-n_d)d\
		d&\ \ |\ \ b
	
	$$As every common divisor of $a$ and $n$ is also a common divisor of $b$ and $n$, then $\gcd(a,n) lt.eq\gcd(b,n)$.
- $\gcd(a,n)\geq\gcd(b,n)$:
	Let $d in ZZ$ such that $d\ |\ b$ and $d\ |\ n$, so $b=b_d d$ and $n=n_d d$ for some $b_d$ and $n_d$, then$$
	
		a&\equiv b quad (\text{mod }n)\
		n&\ \ |\ \ a-b\
		a - b &= kn
			&\text{for some $k$}\
		a - b_dd &= n_d d\
		a &= b_dd+n_dd\
		&= (b_d+n_d)d\
		d&\ \ |\ \ a
	
	$$As every common divisor of $b$ and $n$ is also a common divisor of $a$ and $n$, then $\gcd(a,n)\geq\gcd(b,n)$.
Therefore $\gcd(a,n)=\gcd(b,n)$.