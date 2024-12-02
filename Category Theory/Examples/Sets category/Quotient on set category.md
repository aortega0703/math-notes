---
tags:
  - theorem
  - definition
  - category_theory
related topics:
  - "[[Category of sets]]"
  - "[[Initial-final object|Initial object]]"
  - "[[Set operations|Quotient]]"
  - "[[Coslice category]]"
---
For an [[Equivalence relation]] $\sim$ in a [[Set]] $S$, $S/\!\!\sim$ is an initial object in the [[Subcategory]] (say $\mathcal{C}$) of $S/\mathbf{Set}$ where$$
	(A,f)\in\text{Obj}(\mathcal{C})\iff \forall s_1,s_2\in S. s_1\sim s_2 \implies f(s_1)=f(s_2)
$$
##### Proof:
- $(S/\!\!\sim,\pi)\in\text{Obj}(\mathcal{C})$:
	Let $\pi:S\twoheadrightarrow S/\!\!\sim$ be the [[Canonical projection]] and $s_1,s_2\in S$ such that $s_1\sim s_2$. By definition $\pi(s_1)=[s_1]=[s_2]=\pi(s_2)$ so $(S/\!\!\sim,\pi)\in\text{Obj}(\mathcal{C})$.
- There exists a morphism $(S/\!\!\sim,\pi)\overset{\tilde{f}}{\to}(A, f)$:
	Let$$
	\begin{align}
		\tilde{f}:S/\!\!\sim&\to A\\
		[s]&\mapsto f(s)
	\end{align}
	$$For $s_1,s_2\in S$ such that $s_1\sim s_2$, $f(s_1)=f(s_2)$ by definition of $\mathcal{C}$. So $\tilde{f}([s_1])=\tilde{f}([s_2])$ meaning $\tilde{f}$ is well-defined. Then for any $s\in S$, $(\tilde{f}\pi)(s) = \tilde{f}([s]) = f(s)$ so $\tilde{f}$ makes the following commute
	![[Quotient is initial.png]]
	Therefore $(S/\!\!\sim,\pi)\overset{\tilde{f}}{\to}(A, f)$ in $\mathcal{C}$.
- $(S/\!\!\sim,\pi)\overset{\tilde{f}}{\to}(A, f)$ is unique:
	Suppose there is some $g$ such that $(g\pi)(s) = f(s)$, that would just mean $g[s]=f(s)$ which means $g=\tilde{f}$ so the arrow is unique.
Therefore $(S/\!\!\sim,\pi)$ is initial in $\mathcal{C}$.