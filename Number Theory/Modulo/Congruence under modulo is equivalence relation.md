---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Equivalence relation]]"
  - "[[Congruence under modulo]]"
mathLink: $\equiv_n$ is equivalence relation
---
For $n in ZZ$, [[Congruence under modulo|Congruence mod n]] $n$ is an [[Equivalence relation]].
##### Proof:
For $a,b,c in ZZ$
- Reflexivity:
	$a-a = 0 = 0n$, so $a\equiv a\ (op("mod")\ n)$.
- Commutativity:
	If $a\equiv b\ (op("mod")\ n)$ then $a-b=kn$ for some $k in ZZ$. So $b-a = (-k)n$ meaning $b\equiv a\ (op("mod")\ n)$.
- Transitivity:
	If $a\equiv b\ (op("mod")\ n)$ and $b\equiv c\ (op("mod")\ n)$ then $a-b = kn$ and $b-c=qn$ for some $k,q in ZZ$. So $a-c=(k+q)n$ meaning $a\equiv c\ (op("mod\ n"))$.