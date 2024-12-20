---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Identity function]]"
---
For $A\overset{f}{\to} B\overset{g}{\to}C$$$
g\circ\operatorname{id}_B=g,\quad \operatorname{id}_B\circ f = f$$
which is to say, the following commute
![[Identity function left cancel.png]]![[Identity function right cancel.png]]
##### Proof:
- $g\circ\operatorname{id}_B=g$:
	Let $b\in B$, then$$
	\begin{align}
		(g\circ \operatorname{id}_B)(b) 
			&= g(\operatorname{id}_B(b))\\
			&= g(b)\\
		g\circ \operatorname{id}_B &= g
	\end{align}
	$$
- $\operatorname{id}_B\circ f = f$:
	Let $a\in A$, then$$
	\begin{align}
		(\operatorname{id}_B\circ f)(a)
			&= \operatorname{id}_B(f(a))\\
			&= f(a)\\
		\operatorname{id}_B\circ f &= f
	\end{align}
	$$