---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Congruence under modulo|Congruence mod n]]"
  - "[[Equivalence relation]]"
aliases:
  - Congruence mod n is equivalence relation
---
For $n\in\mathbb{Z}$, [[Congruence under modulo|Congruence mod n]] $n$ is an [[Equivalence relation]].
##### Proof:
For $a,b,c\in\mathbb{Z}$
- Reflexivity:
	$a-a = 0 = 0n$, so $a\equiv a\ (\operatorname{mod}\ n)$.
- Commutativity:
	If $a\equiv b\ (\operatorname{mod}\ n)$ then $a-b=kn$ for some $k\in\mathbb{Z}$. So $b-a = (-k)n$ meaning $b\equiv a\ (\operatorname{mod}\ n)$.
- Transitivity:
	If $a\equiv b\ (\operatorname{mod}\ n)$ and $b\equiv c\ (\operatorname{mod}\ n)$ then $a-b = kn$ and $b-c=qn$ for some $k,q\in\mathbb{Z}$. So $a-c=(k+q)n$ meaning $a\equiv c\ (\operatorname{mod\ n})$.