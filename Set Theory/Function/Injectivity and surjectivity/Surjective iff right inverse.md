---
tags:
  - theorem
  - math/set_theory
related topics:
  - "[[Injectivity and surjectivity|Surjectivity]]"
---
For a [[Function]] $f:A -> B$ ($A != \emptyset$), $f$ is [[Injectivity and surjectivity|Surjective]] if and only it has a right inverse i.e. there exists a function $g:B -> A$ such that $f compose g = op("id")_B$.
##### Proof:
- Surjective $ ==> $ right inverse:
	Let $\sim$ be the [[Kernel]] of $f$ and$$
	
		g_1:B& -> A/\!\!\sim\
		b& |-> [a] &&\text{where $f(a)=b$}\
		g_2:A/\!\!\sim & -> A\
		[a]& |-> s &&\text{with $s in [a]$ chosen arbitrarily}
	
	$$
	- $g_1$ is well-defined:
		As $f$ is surjective there is always some $a in A$ such that $f(a)=b$, so $g_1$ is defined for all values in its domain. Let $a_1,a_2 in A$ such that $f(a_1)=f(a_2)=b$, then $a_1\sim a_2$ and $g_1(b)=[a_1]=[a_2]$ so the image of $b$ is unique. Then $g_1$ is well defined.
	- $g_2$ is well-defined:
		By [[Axiom of choice]].
	- $f compose (g_2 compose g_1)=op("id")_B$:
		Let $b in B$, then$$
		
			(f compose (g_2 compose g_1))(b) 
				&= (f compose g_2)([a]) &\text{where $f(a)=b$}\
			&= f(s) &\text{where $f(s)=b$}\
			&= b
			
		$$So $g=g_2 compose g_1$ is a right inverse of $f$.
- Right inverse $ ==> $ surjective:
	Let $b in B$, then$$
	
		b&=op("id")_B(b)\
		&=(f compose g)(b)\
		&=f(g(b))
	
	$$so $f(a)=b$ for some $a in A$ (namely $a=g(b)$), making $f$ surjective.