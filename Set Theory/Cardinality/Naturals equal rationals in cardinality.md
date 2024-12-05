---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Natural numbers]]"
  - "[[Integers]]"
  - "[[Rational numbers]]"
  - "[[Cardinality]]"
---
$|\mathbb{N}|=|\mathbb{Q}_{\geq 0}|$ i.e. the [[Cardinality]] of the set of [[Natural numbers]] equal that of the set of [[Rational numbers]].
##### Proof:
- $|\mathbb{N}|\leq|\mathbb{Q}_{\geq 0}|$:
	Every $n\in\mathbb{N}$ can be expressed as $\frac{n}{1}$, therefore $\mathbb{N}\subset\mathbb{Q}_{\geq 0}$ meaning $|\mathbb{N}|\leq|\mathbb{Q}_{\geq 0}|$.
- $|\mathbb{Q}_{\geq 0}| \leq |\mathbb{N}|$:
	For any $n\in\mathbb{N}$$$
	n =\frac{s(s+1)}{2}+t \quad s,t\in\mathbb{N}, \text{ such that $s$ is maximal}
	$$
	Consider the function$$
	\begin{align}
		\phi: \mathbb{N} &\to \mathbb{Q}_{\geq 0}\\
		n &\mapsto \frac{t}{s-t+1}
	\end{align}
	$$
	where $s$ and $t$ are as defined previously. Let $\frac{p}{q}$ be arbitrary in simplified form and $n=\frac{(p+q)(p+q-1)}{2}+p$, then
	- $p+q-1$ is maximal:
		Suppose that $n=\frac{(p+q)(p+q+1)}{2}+k$ for some $k\in\mathbb{N}$, then$$
		\begin{align}
			\frac{(p+q)(p+q-1)}{2}+p 
				&= \frac{(p+q)(p+q+1)}{2}+k\\
			(p+q)(p+q-1) + 2p
				&= (p+q)(p+q+1) + 2k\\
			(p+q)(p+q-1) - (p+q)(p+q+1)
				&= 2k - 2p\\
			-2(p+q) 
				&= 2(k-p)\\
			-p-q 
				&= k-p\\
			-q &= k
		\end{align}
		$$
		But $q\in\mathbb{N}$ so $0>k\notin\mathbb{N}$ which is a contradiction. If $n=\frac{(p+q+d)(p+q+d+1)}{2}+k'$ for some $d\in\mathbb{N}$ then $0>k\geq k'\notin\mathbb{N}$ making $p+q-1$ the maximal choice.
	- $n$ is the pre-image of $\frac{p}{q}$:
		As $p+q-1$ is maximal, then$$
		\begin{align}
			\phi\left(\frac{(p+q)(p+q-1)}{2}+p\right)
			&= \frac{p}{(p+q-1)-p+1}\\
			&= \frac{p}{q}
		\end{align}
		$$
		So $\phi$ is surjective.
	Then $|\mathbb{Q}_{\geq 0}|\leq |\mathbb{N}|$.