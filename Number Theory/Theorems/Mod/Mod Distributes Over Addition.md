---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Division|Modulo]]"
mathLink: $(a+b)\mod n = \big((a\mod n) + (b\mod n)\big)\mod n$
---
For $a,b,(n>0)\in\mathbb{Z}$, $(a+b)\mod n = \big((a\mod n) + (b\mod n)\big)\mod n$.
##### Proof:
By [[Division algorithm]] let $a = q_a n + r_a$, $b = q_b n + r_b$ and $(a\operatorname{ mod } n) + (b\operatorname{ mod } n) = r_a + r_b = q_{a+b} n + r_{a+b}$, then$$
\begin{align}
	a+b &= (q_a n + r_a) + (q_b n + r_b)\\
	&= (q_a + q_b) n + (r_a + r_b)\\
	&= (q_a + q_b) n + q_{a+b} n + r_{a+b}\\
	&= (q_a + q_b + q_{a+b}) n + r_{a+b}
\end{align}
$$So $(a+b)\mod n = \big((a\mod n) + (b\mod n)\big)\mod n$.