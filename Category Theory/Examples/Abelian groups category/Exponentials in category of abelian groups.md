---
tags:
  - theorem
  - abstract_algebra
  - category_theory
related topics:
  - "[[Category of abelian groups]]"
  - "[[Exponential object]]"
---
For any [[Abelian group]] $G$ and set $A$, $G^A = \text{Hom}_\mathbf{Set}(A, G)$ is an abelian group with the operation $$
\begin{align}
	+:G^A\times G^A &\to G^A\\
	f,g&\mapsto f(\_)\cdot g(\_)
\end{align}
$$
##### Proof:
- $G^A$ is a [[Group]]:
	By [[Exponentials in category of groups]].
- Commutativity:
	Let $f,g\in G^A$ and $a\in A$, then$$
	\begin{align}
		(f+g)(a)
		&= f(a)\cdot g(a)\\
		&= g(a)\cdot f(a)\\
		&= (g+f)(a)
	\end{align}
	$$which by [[Set|Extensionality]] implies $f+g=g+f$, so $G^A$ is an abelian group.