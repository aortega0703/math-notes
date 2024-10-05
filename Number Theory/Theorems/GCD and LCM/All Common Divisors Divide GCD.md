---
tags:
  - exercise
  - number_theory
related topics:
  - "[[Greatest Common Divisor|GCD]]"
---
For $a,b,d\in\mathbb{Z}$, if $d$ is a common divisor of $a,b$ then $d$ divides $\gcd(a,b)$.
##### Proof:
By [[Division algorithm]] for some $q,(0\leq r < d)\in\mathbb{Z}$$$
\begin{align}
	\gcd(a,b)&=qd+r\\
	as+bt&=qd+r\quad\text{for some $s,t\in\mathbb{Z}$}\tag{1}\\
	0&\equiv r\ (\operatorname{mod}d)
\end{align}
$$Where $(1)$ is by [[GCD is linear combination]]. As $r<d$ then $r=0$ and therefore $d$ divides $\gcd(a,b)$.