---
tags:
  - definition
  - set_theory
related topics:
  - "[[Function]]"
---
For functions $f:A\to B$ and $g:B\to C$ their composition $g\circ f: A \to C$ is defined as $g\circ f(a) = g(f(a))$. i.e. it makes the following [[Diagram|commute]]
![[Function composition.png]]

---
- Associativity:
	For functions $A \overset{f}{\to} B \overset{g}{\to} C \overset{h}{\to} D$, $h\circ(g\circ f)= (h\circ g)\circ f$ (function composition is associative). i.e. the following commutes
	![[Function composition associative.png]]
	Let $a\in A$, then$$
	\begin{align}
		\big(h\circ(g\circ f)\big)(a) 
			&= h\big((g\circ f)(a)\big)\\
			&= h\big(g(f(a))\big)\\
			&= (h\circ g)(f(a))\\
			&= ((h\circ g)\circ f)(a)
	\end{align}
	$$So $h\circ(g\circ f)= (h\circ g)\circ f$.