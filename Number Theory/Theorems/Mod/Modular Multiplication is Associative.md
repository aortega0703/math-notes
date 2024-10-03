---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Division|Modulo]]"
---
For $a,c,b,(n>0)\in\mathbb{Z}$, $(a * b \ \operatorname{mod} n) * c \ \operatorname{mod} n = a * (b * c \ \operatorname{mod} n) \ \operatorname{mod} n = abc \!\mod n$.
##### Proof:
- $(a * b \ \operatorname{mod} n) * c \ \operatorname{mod} n = abc \ \operatorname{mod} n$:
	By [[Division algorithm]] let $ab=q_1n + r_1$ and $(ab\!\mod n)c = r_1 c=q_2n+r_2$. Then$$
	\begin{align}
		ab &= q_1n + r_1\\
		abc &= (q_1n + r_1)c\\
			&= q_1nc + r_1c\\
			&= q_1nc + q_2n + r_2\\
			&= (q_1c + q_2)n + r_2
	\end{align}$$So $abc\!\mod n = (ab\!\mod n) c\!\mod n$.
- $a * (b * c \ \operatorname{mod} n) \ \operatorname{mod} n = abc \ \operatorname{mod} n$:
	By [[Division algorithm]] let $bc=q_1n + r_1$ and $a(bc\!\mod n) = a r_1 =q_2n+r_2$. Then$$
	\begin{align}
		bc &= q_1n + r_1\\
		abc &= a(q_1n + r_1)\\
			&= aq_1n + a r_1\\
			&= aq_1n + q_2n + r_2\\
			&= (aq_1 + q_2)n + r_2
	\end{align}$$So $abc \!\mod n = a(bc\!\mod n)\!\mod n$.
Therefore $(a * b \ \operatorname{mod} n) * c \ \operatorname{mod} n = a * (b * c \ \operatorname{mod} n) \ \operatorname{mod} n = abc \!\mod n$.