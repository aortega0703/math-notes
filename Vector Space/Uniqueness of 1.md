---
tags:
  - theorem
  - math/linear_algebra
related topics:
  - "[[Vector Space]]"
  - "[[Field]]"
---
A [[Vector Space]] $V\neq\{\mathbf{0}\}$ over $F$, has a unique identity for scalar multiplication.

##### Proof:
Let $v\neq \mathbf{0}\in V$, and suppose $1\neq 1'\in F$ be identities for scalar multiplication in $V$, then
$$
\begin{align}
	1v 
		&= v\\
		&= 1'v\\
	1v - 1'v
		&= \mathbf{0}\\
	(1-1')v &= \mathbf{0}\\
	(1-1')^{-1} (1-1') v &= \mathbf{0} \tag{1}\\
	1v = \mathbf{0}\\
	v = \mathbf{0}
\end{align}
$$
which is a contradiction as $v\neq \mathbf{0}$ , so $1=1'$ making $1$ unique.
[^1]: by [[Uniqueness of additive inverse in Fields]] and [[Multiplication by 0 (vector)]].