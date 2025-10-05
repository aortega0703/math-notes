---
tags:
  - theorem
  - math/category_theory
  - math/set_theory
related topics:
  - "[[Monic-epic|Monic]]"
  - "[[Injectivity and surjectivity|Injectivity]]"
---
A [[Function]] $f:A -> B$ ($A != \emptyset$) is [[Injectivity and surjectivity|Injective]] if and only if it is [[Monic-epic|Monic]].
##### Proof:
- Injective $ ==> $ Monic:
	Let $g,h: S -> A$ such that $f compose g = f compose h$, then$$
	
		(f compose g)(s) &= (f compose h)(s)\
		f(g(s)) &= f(h(s))\
		g(s) &= h(s)
			&\text{by $f$ injective}\
		g &= h
	
	$$So $f compose g = f compose h$ implies $g = h$, making $f$ monic.
- Monic $ ==> $ Injective:
	Let $x,y in A$ and$$
	
		\begin{aligned}
			x': S & -> A\
			s& |-> x
		\end{aligned}\qquad
		\begin{aligned}
			y': S & -> A\
			s& |-> y
		\end{aligned}
	
	$$Let $f(x) = f(y)$, then$$
	
		f(x'(s)) &= f(y'(s))\
		(f compose x')(s) &= (f compose y')(s)\
		f compose x' &= f compose y'\
		x' &= y'
			&\text{by $f$ monic}\
		x'(s) &= y'(s)\
		x &= y
	
	$$So $f(x) = f(y)$ implies $x=y$, making $f$ injective.