---
tags:
  - theorem
  - number_theory
  - to_do
related topics:
  - "[[Division|Modulo]]"
---
For $a,b,(n>0)\in\mathbb{Z}$, $ab\mod n = (a\mod n)(b\mod n)\mod n$.
##### Proof:
By [[Division algorithm]] let $a=q_1n + r_1$, $b=q_2n+r_2$, and $(a\mod n)(b\mod n)=r_1r_2=q_3n+r_3$, then$$
\begin{align}
	ab &= (q_1n + r_1)(q_2n + r_2)\\
		&= q_1q_2n^2 + q_1r_2n + q_2r_1 n + r_1r_2\\
		&= q_1q_2n^2 + q_1r_2n + q_2r_1 n + q_3n + r_3\\
		&= (q_1q_2n + q_1r_2 + q_2r_1 + q_3)n + r_3\\
\end{align}$$So $ab\mod n = (a\mod n)(b\mod n)\mod n$.