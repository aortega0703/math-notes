---
tags:
  - theorem
  - math/set_theory
  - to_do
related topics:
  - "[[Set operations|Quotient]]"
  - "[[Injectivity and surjectivity|Injectivity]]"
  - "[[Injectivity and surjectivity|Surjectivity]]"
---
For a [[Function]] $f:A -> B$ and its [[Kernel]] $\sim$, $f$ decomposes as follows
![[Canonical decomposition.png]]
where $[\cdot]$ is the [[Canonical projection]], $i$ is the [[Inclusion map]], and$$

	\tilde{f} : A/\!\!\sim& arrow.r.tilde Im f\
	[a] & |-> f(a)

$$is a [[Injectivity and surjectivity|Bijection]].
##### Proof:
- $\tilde{f}$ is well-defined:
	Let $[a],[b] in A/\!\!\sim$ such that $[a]=[b]$, then $a\sim b$ and $f(a)=f(b)$, so $\tilde{f}[a]=\tilde{f}[b]$. As $[a]=[b]$ maps to a single element in the codomain, it makes $\tilde{f}$ well-defined.
- $\tilde{f}$ is a bijection:
	- Injectivity:
		Let $[a],[b] in A/\!\!\sim$ such that $\tilde{f}[a]=\tilde{f}[b]$, then$$
		
			f(a) &= f(b)\
			a &\sim b\
			[a] &= [b]
		
		$$
		So $\tilde{f}$ is injective
	- Surjectivity:
		Let $b in Im f$, then by definition of $ Im $, $f(a)=b$ for some $a in A$. So $\tilde{f}[a]=b$ making $\tilde{f}$ surjective.
- $i\tilde{f}[\cdot]=f$:
	Let $a in A$, then $a\overset{[\cdot]}{ |-> }[a]\overset{\tilde{f}}{ |-> } f(a) \overset{i}{ |-> } f(a)$ so $i\tilde{f}[\cdot]=f$.