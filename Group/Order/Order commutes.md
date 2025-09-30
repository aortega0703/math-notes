---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Order]]"
---
For a [[Group]] $G$ and $g,h\in G$, $|gh|=|hg|$.
##### Proof:
- $(aga^{-1})^n=ag^na^{-1}$:
	By induction on $n$.
	- $\mathcal{P}(0)$:
		$ag^0a^{-1}=aa^{-1}=e=(aga^{-1})^0$.
	- $\mathcal{P}(n)\implies\mathcal{P}(n+1)$:
		$$
		\begin{align}
			(aga^{-1})^{n+1} 
			&= (aga^{-1})^naga^{-1}\\
			&= ag^na^{-1}aga^{-1}
				&\text{by induction}\\
			&= ag^nga^{-1}\\
			&= ag^{n+1}a^{-1}
		\end{align}
		$$
	So $(aga^{-1})^n=ag^na^{-1}$ for all $n$.
- $|aga^{−1} | = |g|$:
	- $|aga^{-1}|\leq |g|$:
		$(aga^{-1})^{|g|}=ag^{|g|}a^{-1}=aa^{-1}=e$, so $|aga^{-1}|\leq |g|$.
	- $|g|\leq|aga^{-1}|$:
		Let $|aga^{-1}|=n$, then$$
	\begin{align}
		e &= (aga^{-1})^n\\
		&= ag^na^{-1}\\
		a&=ag^n\\
		e&=g^n
	\end{align}
	$$So $|g|\leq n=|aga^{-1}|$.
	Then $|aga^{−1} | = |g|$.
- $|gh| = |hg|$:
	$|gh|=|g(hg)g^{-1}| = hg$.