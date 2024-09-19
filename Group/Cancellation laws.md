---
related topics:
  - "[[Group]]"
tags:
  - theorem
  - abstract_algebra
---
In a [[Group]] $G$, $ba = ca \implies b=c$ and $ab = ac \implies b=c$ for all $a,b,c\in G$.
##### Proof:
- $ba = ca \implies b=c$:$$
	\begin{align}
		ba &= ca\\
		baa^{-1} &= ca a^{-1}\\
		be &= ce\\
		b&=c
	\end{align}$$
- $ab = ac \implies b=c$:$$
	\begin{align}
		ab &= ac\\
		a^{-1} ab &= a^{-1} a c\\
		eb &= ec\\
		b &= c
	\end{align}$$