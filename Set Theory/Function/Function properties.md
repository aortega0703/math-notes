---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Function]]"
  - "[[Function|Function composition]]"
aliases:
  - Inverse function
---
For functions $f: A\to B$, $g: B \to C$, and $h:C \to D$
1. If $f$ and $g$ are injective, then $g\circ f$ is injective.
2. If $f$ and $g$ are surjective, then $g\circ f$ is surjective.
##### Proof:
1. Let $a,a'\in A$ such that $(g\circ f)(a) = (g\circ f)(a')$, then$$
	\begin{align}
		(g\circ f)(a) &= (g\circ f)(a')\\
		g(f(a)) &= g(f(a'))\\
		f(a) &= f(a')\\
		a &= a'
	\end{align}$$So $(g\circ f)(a) = (g\circ f)(a') \implies a = a'$.
2. Let $c\in C$, then$$
	\begin{align}
		c &= g(b)&\text{for some $b\in B$}\\
		b &= f(a)&\text{for some $a\in A$}\\
		c &= g(f(a))\\
		&= (g\circ f)(a)
	\end{align}$$So for all $c\in C$, $c=(g\circ f)(a)$ for some $a\in A$.