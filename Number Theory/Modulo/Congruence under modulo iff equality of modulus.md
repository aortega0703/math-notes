---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Congruence under modulo|Congruence mod n]]"
  - "[[Division|Modulo]]"
---
For $a,b,n\in\mathbb{Z}$$$
	a\equiv b\ (\operatorname{mod}\ n)
	\iff a\ \operatorname{mod}\ n 
		= b\ \operatorname{mod} n
$$
##### Proof:
- $\implies$:
	If $a\equiv b\ (\operatorname{mod}\ n)$ then$$
	\begin{align}
		a-b&=kn
			&\text{for some $k\in\mathbb{Z}$}\\
		a &= kn + b\\
		&= kn + (q_b n+ r_b)\tag{$*$}\\
		&= (k+q_b)n + r_b
	\end{align}$$Where $(*)$ is by [[Division algorithm]]. As $r_b$ is unique, $a\ \operatorname{mod}\ n = r_b = b\ \operatorname{mod}\ n$.
- $\impliedby$:
	$a = q_a n + r$ and $b= q_b n + r$, then $a-b = (q_a - q_b)n$. Therefore $a\equiv b\ (\operatorname{mod}\ n)$.