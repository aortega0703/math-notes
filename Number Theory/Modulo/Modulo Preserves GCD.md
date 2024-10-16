---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Greatest Common Divisor|GCD]]"
  - "[[Division|Modulo]]"
mathLink: $\gcd(a,n) = \gcd(a\ \operatorname{mod}\ n,\ n)$
---
For $a,n\in\mathbb{Z}$$$
\gcd(a,n) = \gcd(a\ \operatorname{mod}\ n,\ n)
$$
##### Proof:
By [[Division algorithm]], $a = qn + b$ for some $q\in\mathbb{Z}$
- $\gcd(b,n) \leq \gcd(a,n)$:$$
\begin{align}
	a &= qn + b\\
		&= qc\gcd(b,n) + c'\gcd(b,n)\quad\text{for some $c,c'\in\mathbb{Z}$}\\
		&= (qc+c')\gcd(b,n)\\
	\gcd(b,n)&\ \ \big|\ \ a\\
	\gcd(b,n) &\leq \gcd(a,n)
\end{align}
$$
- $\gcd(b,n) \geq \gcd(a,n)$:$$
	\begin{align}
		b &= a - qn\\
			&= c\gcd(a,n) - qc'\gcd(a,n)\quad\text{for some $c,c'\in\mathbb{Z}$}\\
			&= (c-qc')\gcd(a,n)\\
		\gcd(a,n) &\ \ \big|\ \ b\\
		\gcd(a,n) &\leq \gcd(b,n)
	\end{align}$$
Therefore $\gcd(a,n) = \gcd(b,n)$.