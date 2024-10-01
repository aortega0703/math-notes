---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Greatest Common Divisor|GCD]]"
  - "[[Division|Modulo]]"
mathLink: $a = b\ (\operatorname{mod} n)\implies\gcd(a,n) = \gcd(b,n)$
---
For $a,b,(n>0)\in\mathbb{Z}$, if $a = b\ (\operatorname{mod} n)$ then $\gcd(a,n) = \gcd(b,n)$.
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