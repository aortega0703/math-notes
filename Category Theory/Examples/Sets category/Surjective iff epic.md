---
tags:
  - theorem
  - math/category_theory
  - math/set_theory
related topics:
  - "[[Monic-epic|Epic]]"
  - "[[Injectivity and surjectivity|Surjectivity]]"
---
A [[Function]] $f:A\to B$ ($A != \emptyset$) is [[Injectivity and surjectivity|Surjective]] if and only if it is [[Monic-epic|Epic]].
##### Proof:
- Surjective $\implies$ Epic:
	Let $g,h: B\to C$ such that $g\circ f = h \circ f$, and $b in B$. By surjectivity $f(a)=b$ for some $a in A$, then$$
	
		(g\circ f)(a) &= (h \circ f)(a)\
		g(f(a)) &= h(f(a))\
		g(b) &= h(b)\
		g &= h
	
	$$so $g\circ f = h \circ f$ implies $g=h$, making $f$ epic.
- Epic $\implies$ Surjective:
	Let$$
	
		\begin{aligned}
			g : B &\to \{0,1\} & h : B &\to C\
			b&\mapsto 0 & b&\mapsto
			
			
			\begin{cases}
				0 & \text{if $b in \operatorname{Im}f$}\
				1 & \text{otherwise}
			\end{cases}
		\end{aligned}
	
	$$then as $f(a) in \operatorname{Im}f$,$$
	
		g(f(a)) = &\hspace{0.4em}0 = h(f(a))\
		(g\circ f)(a) &= (h\circ f)(a)\
		g\circ f &= h\circ f\
		g &= h
			&\text{by $f$ epic}
	
	$$So $b in \operatorname{Im}f$ for all $b in B$, making $f$ surjective.