---
tags:
  - theorem
  - category_theory
  - set_theory
related topics:
  - "[[Monic-epic|Monic]]"
  - "[[Injectivity and surjectivity|Injectivity]]"
---
A [[Function]] $f:A\to B$ ($A\neq \emptyset$) is [[Injectivity and surjectivity|Injective]] if and only if it is [[Monic-epic|Monic]].
##### Proof:
- Injective $\implies$ Monic:
	Let $g,h: S \to A$ such that $f \circ g = f \circ h$, then$$
	\begin{align}
		(f\circ g)(s) &= (f\circ h)(s)\\
		f(g(s)) &= f(h(s))\\
		g(s) &= h(s)
			&\text{by $f$ injective}\\
		g &= h
	\end{align}
	$$So $f \circ g = f \circ h$ implies $g = h$, making $f$ monic.
- Monic $\implies$ Injective:
	Let $x,y\in A$ and$$
	\begin{align}
		\begin{aligned}
			x': S &\to A\\
			s&\mapsto x
		\end{aligned}\qquad
		\begin{aligned}
			y': S &\to A\\
			s&\mapsto y
		\end{aligned}
	\end{align}
	$$Let $f(x) = f(y)$, then$$
	\begin{align}
		f(x'(s)) &= f(y'(s))\\
		(f \circ x')(s) &= (f \circ y')(s)\\
		f \circ x' &= f \circ y'\\
		x' &= y'
			&\text{by $f$ monic}\\
		x'(s) &= y'(s)\\
		x &= y
	\end{align}
	$$So $f(x) = f(y)$ implies $x=y$, making $f$ injective.