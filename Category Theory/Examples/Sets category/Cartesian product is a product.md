---
tags:
  - theorem
  - math/category_theory
  - math/set_theory
related topics:
  - "[[Product]]"
  - "[[Set Product]]"
---
For sets $A,B$, the [[Set operations|Cartesian product]] $A times B$ is a [[Product]] in $\mathbf{Set}$.
##### Proof:
Let $X$ be a set with functions $f:X -> A$ and $g:X -> B$. Consider$$

	f times g:X& -> A times B\
	x &\mapsto \big(f(x),\ g(x)\big)

$$then for $x in X$$$

	(x)(f times g)\,;\pi_1
	&=\big(f(x),g(x)\big)\pi_1\
	&= f(x)

$$So $(f times g)\,;\pi_1=f$. Similarly $(f times g)\,;\pi_2=g$. This function is unique as any function that makes the diagram commute must have a first coordinate $f(x)$ and a second coordinate $g(x)$, which is precisely the definition of $f times g$. Then $A times B$ is a product with $\pi_1$ and $\pi_2$.