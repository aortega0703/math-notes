---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Injectivity and surjectivity|Surjectivity]]"
---
For a [[Function]] $f:A\to B$ ($A\neq \emptyset$), $f$ is [[Injectivity and surjectivity|Surjective]] if and only it has a right inverse i.e. there exists a function $g:B \to A$ such that $f\circ g = \operatorname{id}_B$.
##### Proof:
- Surjective $\implies$ right inverse:
	Let $\sim$ be the [[Kernel]] of $f$ and$$
	\begin{align}
		g_1:B&\to A/\!\!\sim\\
		b&\mapsto [a] &&\text{where $f(a)=b$}\\
		g_2:A/\!\!\sim &\to A\\
		[a]&\mapsto s &&\text{with $s\in [a]$ chosen arbitrarily}
	\end{align}
	$$
	- $g_1$ is well-defined:
		As $f$ is surjective there is always some $a\in A$ such that $f(a)=b$, so $g_1$ is defined for all values in its domain. Let $a_1,a_2\in A$ such that $f(a_1)=f(a_2)=b$, then $a_1\sim a_2$ and $g_1(b)=[a_1]=[a_2]$ so the image of $b$ is unique. Then $g_1$ is well defined.
	- $g_2$ is well-defined:
		By [[Axiom of choice]].
	- $f\circ(g_2\circ g_1)=\operatorname{id}_B$:
		Let $b\in B$, then$$
		\begin{align}
			(f\circ(g_2\circ g_1))(b) 
				&= (f\circ g_2)([a]) &\text{where $f(a)=b$}\\
			&= f(s) &\text{where $f(s)=b$}\\
			&= b
		\end{align}	
		$$So $g=g_2\circ g_1$ is a right inverse of $f$.
- Right inverse $\implies$ surjective:
	Let $b\in B$, then$$
	\begin{align}
		b&=\operatorname{id}_B(b)\\
		&=(f\circ g)(b)\\
		&=f(g(b))
	\end{align}
	$$so $f(a)=b$ for some $a\in A$ (namely $a=g(b)$), making $f$ surjective.