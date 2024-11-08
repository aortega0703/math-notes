---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Integers]]"
---
For any $n\in\mathbb{N}$$$
\sum_{k=1}^n k = \frac{n(n+1)}{2}
$$
##### Proof:
By induction on $n$.
- $\mathcal{P}(0)$:
	$\sum_{k=1}^0 k=0=\frac{0(0+1)}{2}$.
- $\mathcal{P}(n)\implies\mathcal{P}(n+1)$:
	$$
	\begin{align}
		\sum_{k=1}^{n+1} k
		&= \sum_{k=1}^n k + (n+1)\\
		&= \frac{n(n+1)}{2} + (n+1)
			&\text{by inductive step}\\
		&= \left(\frac{n}{2}+1\right)(n+1)\\
		&= \frac{(n+2)(n+1)}{2}
	\end{align}
	$$
Then $\sum_{k=1}^n k = \frac{n(n+1)}{2}$ for all $n\in\mathbb{N}$.