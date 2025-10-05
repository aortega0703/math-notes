---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Greatest Common Divisor|GCD]]"
mathLink: $\operatorname{gcd}(a,b)=as+bt$
---
For $a,b in ZZ$ with $a,b != 0$, there exist $s,t in ZZ$ such that $\operatorname{gcd}(a,b)=as+bt$. Moreover $\operatorname{gcd}(a,b)$ is the smallest positive integer of the form $as+bt$.
##### Proof:
Let $S=\{d=as+bt: s,t in ZZ, d>0\}$ and by [[Well ordering principle]] let $d=\operatorname{min}(S)$.
- $d$ is a common divisor: 
	By [[Division algorithm]] there exist unique $q,r in ZZ$ such that $a=qd+r$ with $0 lt.eq r < d$. To show that $r=0$ suppose $r>0$, then$$
	
		r &= a - qd\
			&= a - q(as + bt) quad\text{for some $s,t in ZZ$}\
			&= a(1-qs) + b(-qt)\
		r & in S
	$$Which is a contradiction with $r<g$ since $g$ is the smallest element in $S$. Therefore $r=0$ and $d$ divides $a$.
- $d$ is the greatest common divisor:
	Suppose there is another common divisor $d'$ such that $a=nd'$ and $b=md'$, then$$
	
		d &= as + bt quad\text{for some $s,t in ZZ$}\
			&= (nd')s + (md')t\
			&= (ns + mt)d'
	$$If $ns + mt<0$ then $d'<0$ so $d'< d$. If $ns + mt > 0$ then $d' lt.eq d$. Finally $ns + mt != 0$ as it would make $g=0$. Therefore $d \geq d'$ for all divisors $d'$.