---
tags:
  - theorem
  - math/category_theory
  - math/set_theory
related topics:
  - "[[Monic-epic|Epic]]"
  - "[[Injectivity and surjectivity|Surjectivity]]"
---
A [[Function]] $f:A -> B$ ($A != \emptyset$) is [[Injectivity and surjectivity|Surjective]] if and only if it is [[Monic-epic|Epic]].
##### Proof:
- Surjective $ ==> $ Epic:
	Let $g,h: B -> C$ such that $g compose f = h compose f$, and $b in B$. By surjectivity $f(a)=b$ for some $a in A$, then$$
	
		(g compose f)(a) &= (h compose f)(a)\
		g(f(a)) &= h(f(a))\
		g(b) &= h(b)\
		g &= h
	
	$$so $g compose f = h compose f$ implies $g=h$, making $f$ epic.
- Epic $ ==> $ Surjective:
	Let$$
	
		\begin{aligned}
			g : B & -> \{0,1\} & h : B & -> C\
			b& |-> 0 & b& |-> 
			
			
			\begin{cases}
				0 & \text{if $b in Im f$}\
				1 & \text{otherwise}
			\end{cases}
		\end{aligned}
	
	$$then as $f(a) in Im f$,$$
	
		g(f(a)) = &\hspace{0.4em}0 = h(f(a))\
		(g compose f)(a) &= (h compose f)(a)\
		g compose f &= h compose f\
		g &= h
			&\text{by $f$ epic}
	
	$$So $b in Im f$ for all $b in B$, making $f$ surjective.