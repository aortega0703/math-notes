---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Equivalence relation]]"
  - "[[Congruence under modulo]]"
mathLink: $\equiv_n$ is equivalence relation
---
For $n in ZZ$, [[Congruence under modulo|Congruence mod n]] $n$ is an [[Equivalence relation]].
##### Proof:
For $a,b,c in ZZ$
- Reflexivity:
	$a-a = 0 = 0n$, so $a\equiv a\ (\operatorname{mod}\ n)$.
- Commutativity:
	If $a\equiv b\ (\operatorname{mod}\ n)$ then $a-b=kn$ for some $k in ZZ$. So $b-a = (-k)n$ meaning $b\equiv a\ (\operatorname{mod}\ n)$.
- Transitivity:
	If $a\equiv b\ (\operatorname{mod}\ n)$ and $b\equiv c\ (\operatorname{mod}\ n)$ then $a-b = kn$ and $b-c=qn$ for some $k,q in ZZ$. So $a-c=(k+q)n$ meaning $a\equiv c\ (\operatorname{mod\ n})$.