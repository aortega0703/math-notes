---
tags:
  - theorem
  - math/linear_algebra
related topics:
  - "[[Vector Space]]"
  - "[[Field]]"
---
In a [[Vector Space]] $V$ over $F$, $av=\mathbf{0}$ implies $a=0$ or $v=\mathbf{0}$ for all $v\in V$ and $a\in F$.
##### Proof:
By cases
- Case $a\neq 0$:$$
	\begin{align}
		av &= \mathbf{0}\\
		a^{-1}av &= \mathbf{0}\tag{1}\\
		v &= \mathbf{0}
	\end{align}$$
[^1]: by [[Multiplication by 0 (vector)]].
- Case $v\neq \mathbf{0}$:$$
	\begin{align}
		av &= \mathbf{0}\\
		av + v &= v\\
		av + 1v &= v\\
		(a+1)v &= v\\
		a+1 &= 1\tag{2}\\
		a &= 0
	\end{align}$$
[^2]: by [[Vector Space/Uniqueness of 1|Uniqueness of 1]].
Therefore either $a=0$ or $v=\mathbf{0}$.