---
tags:
  - theorem
  - math/set_theory
related topics:
  - "[[Function|Function composition]]"
  - "[[Injectivity and surjectivity|Injectivity]]"
  - "[[Injectivity and surjectivity|Surjectivity]]"
  - "[[Injectivity and surjectivity|Bijectivity]]"
aliases:
  - Inverse function
---
For functions $f: A -> B$ and $g: B -> C$
1. If $f$ and $g$ are injective, then $g compose f$ is injective.
2. If $f$ and $g$ are surjective, then $g compose f$ is surjective.
3. If $f$ and $g$ are bijective, then $g compose f$ is bijective.
##### Proof:
1. Let $a,a' in A$ such that $(g compose f)(a) = (g compose f)(a')$, then$$
	
		(g compose f)(a) &= (g compose f)(a')\
		g(f(a)) &= g(f(a'))\
		f(a) &= f(a')\
		a &= a'
	$$So $(g compose f)(a) = (g compose f)(a') ==> a = a'$.
2. Let $c in C$, then$$
	
		c &= g(b)&\text{for some $b in B$}\
		b &= f(a)&\text{for some $a in A$}\
		c &= g(f(a))\
		&= (g compose f)(a)
	$$So for all $c in C$, $c=(g compose f)(a)$ for some $a in A$.
3. By $(1)$ $g compose f$ is injective and by $(2)$ $g compose f$ is surjective, so $g compose f$ is bijective.