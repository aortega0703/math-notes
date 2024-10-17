---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Congruence under modulo|Congruence mod n]]"
  - "[[Modular addition]]"
---
In [[Integers modulo n (set)]] [[Modular addition]] has the following properties
- Commutativity.
- Associativity.
- Has identity $0$.
- Has inverses.
- Preserves [[Congruence under modulo]].
##### Proof:
- is commutative:
	By commutativity of addition $a+b=b+a$, then $(a+b)-(b+a)=0=0n$. Therefore $a+b\equiv b+a\ (\operatorname{mod}\ n)$.
- is associative:
	By associativity of addition $(a+b)+c=a+(b+c)$, then $\big((a+b)+c\big)-\big(a+(b+c)\big)=0=0n$. Therefore $(a+b)+c\equiv a+(b+c)\ (\operatorname{mod}\ n)$.
- has identity $0$:
	By identity of addition $a+0=a$, then $(a+0)-a=0=0n$. Therefore $a+0\equiv a\ (\operatorname{mod}\ n)$.
- has inverses:
	By existence of additive inverses $(a+(-a))-0=0=0n$. Therefore $a + (-a)\equiv 0\ (\operatorname{mod}\ n)$.
- preserves congruence modulo $n$:
	If $a\equiv b\ (\operatorname{mod}\ n)$ then $n\ |\ a-b=(a+c)-(b+c)$. Therefore $a+c\equiv b+c\ (\operatorname{mod}\ n)$.