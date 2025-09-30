---
tags:
  - theorem
  - math/abstract_algebra
  - category_theory
related topics:
  - "[[Notes/Category Theory/Examples/Groups category/Category of groups]]"
  - "[[Initial-final object|Zero object]]"
---
In $\mathbf{Grp}$, the [[Group|Trivial group]] is a [[Initial-final object|Zero object]].
##### Proof:
Let $G$ be a group
- Initial:
	By [[Group homomorphisms preserve identity]] there is exactly one [[Group homomorphism]] $\phi: \{e\} \to G$, namely $\phi(e)=e_G$.
- Final:
	By [[Singletons are final objects in category of sets]] there is exactly one function$$
	\begin{align}
		\phi:G&\to \{e\}\\
		g&\mapsto e
	\end{align}
	$$For any $g,g'\in G$, $\phi(g)\phi(g')=ee=e=\phi(gg')$ so $\phi$ is a homomorphism.
As there is exactly one morphism from and to any other object $G$, the trivial group $\{e\}$ is a zero object.