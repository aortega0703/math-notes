---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Cardinality]]"
  - "[[Natural numbers]]"
  - "[[Integers]]"
---
$|\mathbb{N}|=|\mathbb{Z}|$ i.e. the [[Cardinality]] of the set of [[Natural numbers]] equals that of the [[Integers]].
##### Proof:
- $|\mathbb{N}|\leq |\mathbb{Z}|$:
	Trivially as $\mathbb{N}\subset\mathbb{Z}$.
- $|\mathbb{Z}|\leq |\mathbb{N}|$:
	Consider$$
	\begin{align}
		\phi: \mathbb{N} &\to \mathbb{Z}\\
		n &\mapsto (-1)^n\left\lceil \frac{n}{2}\right\rceil
	\end{align}
	$$
	Let $z\in\mathbb{Z}$
	-  $z=0$:
		then $\phi(0)=0=z$. 
	- $z<0$:
		Consider$$
		\begin{align}
			\phi(2|z|-1)
			&= (-1)^{2|z|-1}\left\lceil\frac{2|z|-1}{2}\right\rceil\\
			&= (-1)|z|\left\lceil\frac{-1}{2}\right\rceil\\
			&= (-1)|z|\\
			&= z
		\end{align}
		$$
		and $0<2|z|-1\in\mathbb{N}$.
	- $z>0$:
		Consider$$
		\begin{align}
			\phi(2|z|)
			&= (-1)^{2|z|}\left\lceil \frac{2|z|}{2}\right\rceil\\
			&= |z|\\
			&= z
		\end{align}
		$$
		and $0 < 2|z| \in\mathbb{N}$.
	Then $\phi$ is surjective meaning $|\mathbb{Z}|\leq|\mathbb{N}|$.
Therefore $|\mathbb{N}|=|\mathbb{Z}|$.