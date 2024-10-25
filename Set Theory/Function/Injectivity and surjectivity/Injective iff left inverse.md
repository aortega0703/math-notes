---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Injectivity and surjectivity|Injectivity]]"
---
For a [[Function]] $f:A\to B$ ($A\neq \emptyset$), $f$ is [[Injectivity and surjectivity|Injective]] if and only it has a left inverse i.e. there exists a function $g:B \to A$ such that $g\circ f = \operatorname{id}_A$.
##### Proof:
- Injective $\implies$ left inverse:
	Let $s\in A$ and$$
	\begin{align}
		g: B &\to A\\
		b &\mapsto
		\begin{cases}
			a &\text{if $b\in \operatorname{Im}f$ and $f(a)=b$}\\
			s &\text{otherwise}
		\end{cases}
	\end{align}
	$$as $f$ is injective $f(a_1) = f(a_2)$ implies $a_1=a_2$ for all $a_1,a_2\in A$, so there is a unique $a\in A$ such that $f(a)=b$ for $b\in\operatorname{Im} f$. Then $g$ is well defined. Clearly $g(f(a))=a$ so $g$ is a left inverse of $f$.
- Left inverse $\implies$ injective:
	Let $a_1, a_2\in A$ such that $f(a_1) = f(a_2)$, then$$
	\begin{align}
		g(f(a_1)) &= g(f(a_2))\\
		(g\circ f)(a_1) &= (g\circ f)(a_2)\\
		\operatorname{id}_A (a_1) &= \operatorname{id}_A (a_2)\\
		a_1 &= a_2
	\end{align}
	$$So $f(a_1) = f(a_2) \implies a_1 = a_2$ making $f$ injective.