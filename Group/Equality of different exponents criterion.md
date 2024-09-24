---
related topics:
  - "[[Group]]"
  - "[[Order]]"
tags:
  - theorem
  - abstract_algebra
mathLink: Criterion for $a^i = a^j$
---
For a [[Group]] $G$, $a\in G$, and $i,j\in \mathbb{Z}$:
- if $|a|\notin \mathbb{N}$, then $a^i = a^j \iff i=j$ 
- if $|a| \in \mathbb{N}$, then $a^i=a^j \iff |a| \bigg| i-j$
##### Proof:
- $|a| \notin \mathbb{N}$:
	- $\implies$:
		Suppose $i > j$ , then$$
		\begin{align}
			a^i &= a^j\\
			a^i a^{-j} &= e\\
			a^{i-j} &= e
		\end{align}$$
		As $i>j$ then $i-j>0$ and $a^{i-j}=e$ contradicts $|a| \notin \mathbb{N}$, therefore $i=j$.
	- $\impliedby$:
		If $i=j$ then $a^i = a^j$ trivially.
- $|a| \in \mathbb{N}$:
	- $\implies$:
		Let $|a| = n$, then$$
			\begin{align}
				a^i &= a^j\\
				a^i a^{-j} &= e\\
				a^{i-j} &= e
			\end{align}
		$$
		By [[Order divides exponent]], $n|i-j$.
	- $\impliedby$:
		Let $|a| = n$ and $i-j = kn$ for some $k\in \mathbb{Z}$, then by [[Order divides exponent]]$$
			\begin{align}
				e &= a^{i-j}\\
					&= a^i a^{-j}\\
				a^j &= a^i
			\end{align}
		$$