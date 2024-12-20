---
tags:
  - theorem
  - set_theory
  - to_do
related topics:
  - "[[Set operations|Quotient]]"
  - "[[Injectivity and surjectivity|Injectivity]]"
  - "[[Injectivity and surjectivity|Surjectivity]]"
---
For a [[Function]] $f:A\to B$ and its [[Kernel]] $\sim$, $f$ decomposes as follows
![[Canonical decomposition.png]]
where $[\cdot]$ is the [[Canonical projection]], $i$ is the [[Inclusion map]], and$$
\begin{align}
	\tilde{f} : A/\!\!\sim&\overset{\sim}{\to} \operatorname{Im}f\\
	[a] &\mapsto f(a)
\end{align}
$$is a [[Injectivity and surjectivity|Bijection]].
##### Proof:
- $\tilde{f}$ is well-defined:
	Let $[a],[b]\in A/\!\!\sim$ such that $[a]=[b]$, then $a\sim b$ and $f(a)=f(b)$, so $\tilde{f}[a]=\tilde{f}[b]$. As $[a]=[b]$ maps to a single element in the codomain, it makes $\tilde{f}$ well-defined.
- $\tilde{f}$ is a bijection:
	- Injectivity:
		Let $[a],[b]\in A/\!\!\sim$ such that $\tilde{f}[a]=\tilde{f}[b]$, then$$
		\begin{align}
			f(a) &= f(b)\\
			a &\sim b\\
			[a] &= [b]
		\end{align}
		$$
		So $\tilde{f}$ is injective
	- Surjectivity:
		Let $b\in \operatorname{Im}f$, then by definition of $\operatorname{Im}$, $f(a)=b$ for some $a\in A$. So $\tilde{f}[a]=b$ making $\tilde{f}$ surjective.
- $i\tilde{f}[\cdot]=f$:
	Let $a\in A$, then $a\overset{[\cdot]}{\mapsto}[a]\overset{\tilde{f}}{\mapsto} f(a) \overset{i}{\mapsto} f(a)$ so $i\tilde{f}[\cdot]=f$.