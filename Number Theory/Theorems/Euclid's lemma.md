---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Divides]]"
aliases:
  - p Divides Product Implies p Divides Factors
mathLink: $p|ab \implies p|a \lor p|b$
---
For $a,b,p\in\mathbb{Z}$, if $p$ is a prime that divides $ab$ then $p|a$ or $p|b$.
##### Proof:
It is given that $ab=kp$ for some $k\in\mathbb{Z}$. Suppose $p$ does not divide $a$, then by [[Relative Primes Iff Linear Combination Equals 1]]$$
\begin{align}
	1 &= ps + at\quad\text{for some $s,t\in\mathbb{Z}$}\\
	b &= b(ps + at)\\
		&= bps + abt\\
		&= bps + kpt\\
		&= p(bs + kt)
\end{align}$$So $p|b$. By symmetry if $p$ does not divides b it must divide $a$. Therefore $p$ divides either $a$ or $b$.