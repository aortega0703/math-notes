---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Congruence under modulo|Congruence mod n]]"
  - "[[Modular addition]]"
---
In [[Integers modulo n (set)]] [[Modular addition]] has the following properties
- Commutativity:$$
	 a + b \equiv b + a quad(\text{mod}\ n)
	$$
- Associativity:$$
		(a + b) + c \equiv a + (b + c) quad(\text{mod}\ n)
	$$
- Has identity $0$:$$
		a + 0 \equiv a quad(\text{mod}\ n)
	$$
- Has inverses:$$
	(\forall a in ZZ/n)(\exists b in ZZ/n): a + b \equiv 0 quad(\text{mod}\ n)
	$$
- Preserves [[Congruence under modulo]]:$$
		(a\equiv_n b) \land (a'\equiv_n b') ==> a+a'\equiv_n b+b'
	$$
##### Proof:
- is commutative:
	By commutativity of addition $a+b=b+a$, then $(a+b)-(b+a)=0=0n$. Therefore $a+b\equiv b+a\ (\operatorname{mod}\ n)$.
- is associative:
	By associativity of addition $(a+b)+c=a+(b+c)$, then $\big((a+b)+c\big)-\big(a+(b+c)\big)=0=0n$. Therefore $(a+b)+c\equiv a+(b+c)\ (\operatorname{mod}\ n)$.
- has identity $0$:
	By identity of addition $a+0=a$, then $(a+0)-a=0=0n$. Therefore $a+0\equiv a\ (\operatorname{mod}\ n)$.
- has inverses:
	By existence of additive inverses $(a+(-a))-0=0=0n$. Therefore $a + (-a)\equiv 0\ (\operatorname{mod}\ n)$.
- preserves congruence modulo $n$:$$
	
		\begin{aligned}
			a &\equiv b quad(\text{mod}\ n)\
			n&\ \ |\ \ a-b\
			a-b &= kn
		\end{aligned}&\qquad
		\begin{aligned}
			a' &\equiv b' quad(\text{mod}\ n)\
			n&\ \ |\ \ a'-b'\
			a'-b' &= k'n\
		\end{aligned}\
		a-b + a'-b' &= kn + k'n\
		(a+a')-(b+b') &= (k + k')n\
		n &\ \ |\ \ (a+a')-(b+b')\
		a + a'&\equiv b + b' quad(\text{mod}\ n)
	
	$$