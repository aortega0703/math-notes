---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Injectivity and surjectivity|Bijectivity]]"
---
A function $f: A\to B$ is [[Injectivity and surjectivity|Bijective]] if and only if it has an inverse, i.e. there is a function $f^{-1}: B\to A$ such that $(g\circ f)(a)= a$ and $(f\circ g)(b) = b$ for all $a\in A$ and $b\in B$, or equivalently, that makes the following [[Diagram|diagrams]] commute
![[Inverse left cancel.png]]
![[Inverse right cancel.png]]
##### Proof:
- $f$ is bijective $\implies$ $f^{-1}$ exists:
	Let $b\in B$, by surjectivity $b=f(a)$ for some $a\in A$, and by injectivity such $a$ is unique. So every $b\in B$ maps to a unique $a\in A$ making $f^{-1}:B\to A$ a function defined as $f^{-1}(b)= a$ with $f(a)=b$. Then$$
	\begin{align}
		(f^{-1}\circ f)(a) 
			&= f^{-1}(f(a))\\
			&= f^{-1}(b)
				&\text{for some $b$ s.t. $f(a)=b$}\\
			&= a
	\end{align}$$And$$
	\begin{align}
		(f\circ f^{-1})(b)
			&= f(f^{-1}(b))\\
			&= f(a)
				&\text{for some $a$ s.t. $f(a)=b$}\\
			&= b
	\end{align}
	$$Therefore $f$ has an inverse function $f^{-1}$.
- $f^{-1}$ exists $\implies$ $f$ is bijective:
	- Injectivity:
		Let $a, a'\in A$ such that $f(a) = f(a')$, then $f^{-1}(f(a)) = f^{-1}(f(a'))$ making $a=a'$. So $f$ is injective.
	- Surjectivity:
		Let $b\in B$, then $f^{-1}(b)= a$ for some $a\in A$, meaning $f(f^{-1}(b))=f(a)$ making $b=f(a)$. So $f$ is surjective.