---
tags:
  - theorem
  - math/number_theory
related topics:
  - "[[Congruence under modulo|Congruence mod n]]"
  - "[[Modular multiplication]]"
---
In [[Integers modulo n (set)]] [[Modular multiplication]] has the following properties
- Commutativity:$$
		 ab \equiv ba quad(\text{mod}\ n)
	$$
- Associativity:$$
			(ab)c \equiv a(bc) quad(\text{mod}\ n)
	$$
- Has identity $1$:$$
			a1 \equiv a  quad(\text{mod}\ n)
	$$
- Preserves [[Congruence under modulo]]:$$
			(a\equiv_n b) \land (a'\equiv_n b')\implies aa'\equiv_n bb'
	$$
##### Proof:
- is commutative:
	By commutativity of multiplication $ab=ba$, then $(ab)-(ba)=0=0n$. Therefore $ab\equiv ba\ (\operatorname{mod}\ n)$.
- is associative:
	By associativity of multiplication $(ab)c=a(bc)$, then $\big((ab)c\big)-\big(a(bc)\big)=0=0n$. Therefore $(ab)c\equiv a(bc)\ (\operatorname{mod}\ n)$.
- has identity $1$:
	By identity of multiplication $1a=a$, then $(1a)-a=0=0n$. Therefore $1a\equiv a\ (\operatorname{mod}\ n)$.
- preserves congruence modulo $n$:
	$$
	
		\begin{aligned}
			a &\equiv b quad(\text{mod}\ n)\
			n&\ \ |\ \ a-b\
			a-b &= kn\
			a &= kn + b
		\end{aligned}\hspace{-3em}&\hspace{5em}
		\begin{aligned}
			a' &\equiv b' quad(\text{mod}\ n)\
			n&\ \ |\ \ a'-b'\
			a'-b' &= k'n\
			a'&= k'n + b'
		\end{aligned}\
		aa' &= (kn + b)(k'n+b')\
		&= kk'n^2 + knb' + k'nb + bb'\
		aa' - bb' &= n(kk'n + kb' + k'b)\
		n&\ \ |\ \ aa'-bb'\
		aa' &\equiv bb'  quad(\text{mod }n)
	
	$$
	