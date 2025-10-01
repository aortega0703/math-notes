---
related topics:
  - "[[Group]]"
  - "[[Order]]"
tags:
  - theorem
  - math/abstract_algebra
mathLink: Criterion for $a^i = a^j$
---
For a [[Group]] $G$, $a in G$, and $i,j in  ZZ$:
- if $|a|\notin  ZZ$, then $a^i = a^j  <==> i=j$ 
- if $|a|  in  ZZ$, then $a^i=a^j  <==> |a| \bigg| i-j$
##### Proof:
- $|a| \notin  ZZ$:
	- $\implies$:
		Suppose $i > j$ , then$$
		
			a^i &= a^j\
			a^i a^{-j} &= e\
			a^{i-j} &= e
		$$
		As $i>j$ then $i-j>0$ and $a^{i-j}=e$ contradicts $|a| \notin  ZZ$, therefore $i=j$.
	- $\impliedby$:
		If $i=j$ then $a^i = a^j$ trivially.
- $|a|  in  ZZ$:
	- $\implies$:
		Let $|a| = n$, then$$
			
				a^i &= a^j\
				a^i a^{-j} &= e\
				a^{i-j} &= e
			
		$$
		By [[Order divides exponent]], $n|i-j$.
	- $\impliedby$:
		Let $|a| = n$ and $i-j = kn$ for some $k in  ZZ$, then by [[Order divides exponent]]$$
			
				e &= a^{i-j}\
					&= a^i a^{-j}\
				a^j &= a^i
			
		$$