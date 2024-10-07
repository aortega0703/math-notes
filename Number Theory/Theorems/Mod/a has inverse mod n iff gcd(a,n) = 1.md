---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Division|Modulo]]"
  - "[[Greatest Common Divisor|GCD]]"
mathLink: $ax\equiv 1\ \operatorname{mod}n \iff \gcd(a,n)=1$
---
For $a,(n>0)\in\mathbb{Z}$, $ax\equiv 1$ has a solution for $x$ if and only if $a$ and $n$ are relative primes.
##### Proof:
- $\implies$:
	By definition$$
	\begin{align}
		ax &= qn + 1\quad\text{for some $q\in\mathbb{Z}$}\\
		ax - qn &= 1\\
		ax + n(-q) &= 1
	\end{align}
	$$So by [[Relative Primes Iff Linear Combination Equals 1]] $a$ and $n$ are relative primes.
- $\impliedby$:
	By definition$$
	\begin{align}
		1 &= as + nt\quad\text{for some $s,t\in\mathbb{Z}$}\\
		1 &\equiv as\ (\operatorname{mod} n)
	\end{align}
	$$So $x=s$ is the solution for the expression.