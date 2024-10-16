---
tags:
  - abstract_algebra
  - definition
related topics:
  - "[[Group]]"
aliases:
  - Multiplicative Group of Integers Modulo n
reference:
  - "Gallian, J. A. Contemporary\r Abstract Algebra"
---
For $0<n\in \mathbb{Z}$, $U(n)=\{0<m<n\in\mathbb{Z}:\gcd(m,n)=1\}$ is a group under multiplication modulo $n$. This is called the group of units modulo $n$ or the multiplicative group of integers modulo $n$, also denoted by $(\mathbb{Z}/n\mathbb{Z})^\times$.
##### Proof:
For $U(n)$ to be a group it has to have
- Closure under multiplication:
	Let $a,b\in U(n)$, by [[Relative Primes Iff Linear Combination Equals 1]]
	$1=as+nt=bs'+nt'$ for some $s,s',t,t'\in\mathbb{Z}$. Then$$
	\begin{align}
		\begin{aligned}
			1&=as+nt\\
			as&=1-nt
		\end{aligned}
		&\quad\quad
		\begin{aligned}
			1&=bs'+nt'\\
			bs'&= 1 - nt'
		\end{aligned}\\
		(as)(bs') &= (1-nt)(1-nt')\\
		(ab)(ss') &= 1 - nt - nt' + n^2tt'\\
		(ab)(ss') + n(t+t'-ntt') &= 1
	\end{align}
	$$So $\gcd(ab,n) = 1$ and by [[Modulo Preserves GCD]] $\gcd(ab\ \operatorname{mod} n,n) = 1$, so $ab \ \operatorname{mod} n \in U(n)$.
- Associativity:
	By [[Modular multiplication]].
- Identity:
	$\gcd(1,n) = 1$ and $1a = a$, so $1\in U(n)$ is the identity.
- Inverses:
	Let $a\in U(n)$, so by [[Relative Primes Iff Linear Combination Equals 1]]$$
	\begin{align}
		1&=as+nt\quad\text{for some $s,t\in\mathbb{Z}$}\\
		1-nt &= as\\
		(1-nt)\!\mod n &= as\!\mod n\\
		1 &= as\!\mod n\\
		&= a\ (s\!\mod n)\!\mod n
	\end{align}$$And by [[Modulo Preserves GCD]] $\gcd(s\!\!\mod n,n)=1$. So there exists some $a^{-1}\in U(n)$ (namely $s\!\!\mod n$) that is the inverse of $a$.
