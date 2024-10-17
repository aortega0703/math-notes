---
related topics:
  - "[[Group]]"
  - "[[Order]]"
tags:
  - theorem
  - abstract_algebra
mathLink: $a^{k} = e \iff |a| \text{ divides }k$
---
For a [[Group]] $G$ and $a\in G$ with $|a| \in \mathbb{Z}^+$, $a^{k} =e$ if and only if $|a|$ divides $k$.
##### Proof:
- $\implies$:
	Let $|a| = n$, by [[Division algorithm]] let $k=qn + r$ with $0\leq r < n$, then	$$
	\begin{align}
		a^k &= e\\
		a^{qn + r} &= e\\
		a^{qn}a^r &= e\\
		a^r &= e
	\end{align}
	$$ The last step begin covered by the $\impliedby$ part of the proof. By definition $n$ is the least positive integer such that $a^n=e$ so $r=0$ and $k$ divides $n$
- $\impliedby$:
	Let $|a| = n$ and $k=qn$ for some $q\in \mathbb{Z}$, then by induction
	- Case $q=0$:
		$a^{0n} = a^0 = e$ by definition.
	- Case $q+1$:$$
		\begin{align}
			a^{(q+1)n} &= a^{qn + n}\\
				&= a^{qn}a^n\\
				&= a^n\quad\text{by induction}\\
				&= e
		\end{align}$$So $a^{qn} = e$ for all $q\geq 0$, then$$
	\begin{align}
		a^{-qn} &= a^{-qn} e\\
			&= a^{-qn} a^{qn}\\
			&= e
	\end{align}$$Therefore $a^{qn}=e$ for all $q\in\mathbb{Z}$.