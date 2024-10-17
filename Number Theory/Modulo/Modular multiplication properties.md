---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Congruence under modulo|Congruence mod n]]"
  - "[[Modular multiplication]]"
---
In [[Integers modulo n (set)]] [[Modular multiplication]] has the following properties
- Commutativity.
- Associativity.
- Has identity $1$.
- Preserves [[Congruence under modulo]].
##### Proof:
- is commutative:
	By commutativity of multiplication $ab=ba$, then $(ab)-(ba)=0=0n$. Therefore $ab\equiv ba\ (\operatorname{mod}\ n)$.
- is associative:
	By associativity of multiplication $(ab)c=a(bc)$, then $\big((ab)c\big)-\big(a(bc)\big)=0=0n$. Therefore $(ab)c\equiv a(bc)\ (\operatorname{mod}\ n)$.
- has identity $1$:
	By identity of multiplication $1a=a$, then $(1a)-a=0=0n$. Therefore $1a\equiv a\ (\operatorname{mod}\ n)$.
- preserves congruence modulo $n$:
	If $a\equiv b\ (\operatorname{mod}\ n)$ then $a-b=kn$ for some $k$, meaning $ac-bc=(kc)n$. Therefore $ac\equiv bc\ (\operatorname{mod}\ n)$.
	