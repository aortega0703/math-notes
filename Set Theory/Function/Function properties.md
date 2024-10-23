---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Function]]"
  - "[[Function|Function composition]]"
aliases:
  - Inverse function
---
For functions $f: A\to B$, $g: B \to C$, and $h:C \to D$
1. $h\circ(g\circ f)= (h\circ g)\circ f$ (function composition is associative). i.e. the following commutes
	![[Function composition associative.png]]
2. If $f$ and $g$ are injective, then $g\circ f$ is injective.
3. If $f$ and $g$ are surjective, then $g\circ f$ is surjective.
4. If $f$ is bijective, there is a function $f^{-1}:B\to A$ such that $(f^{-1}\circ f)(a)=a$ and $(f\circ f^{-1})(b)=b$ for all $a\in A$ and $b\in B$.
##### Proof:
1. Let $a\in A$, then$$
	\begin{align}
		\big(h\circ(g\circ f)\big)(a) 
			&= h\big((g\circ f)(a)\big)\\
			&= h\big(g(f(a))\big)\\
			&= (h\circ g)(f(a))\\
			&= ((h\circ g)\circ f)(a)
	\end{align}
	$$So $h\circ(g\circ f)= (h\circ g)\circ f$.
2. Let $a,a'\in A$ such that $(g\circ f)(a) = (g\circ f)(a')$, then$$
	\begin{align}
		(g\circ f)(a) &= (g\circ f)(a')\\
		g(f(a)) &= g(f(a'))\\
		f(a) &= f(a')\\
		a &= a'
	\end{align}$$So $(g\circ f)(a) = (g\circ f)(a') \implies a = a'$.
3. Let $c\in C$, then$$
	\begin{align}
		c &= g(b)&\text{for some $b\in B$}\\
		b &= f(a)&\text{for some $a\in A$}\\
		c &= g(f(a))\\
		&= (g\circ f)(a)
	\end{align}$$So for all $c\in C$, $c=(g\circ f)(a)$ for some $a\in A$.
4. Let $b\in B$, by surjectivity $b=f(a)$ for some $a\in A$, and by injectivity such $a$ is unique. Therefore every $b\in B$ maps to a unique $a\in A$, then $f^{-1}:B\to A$ is a function defined as $f^{-1}(b)= a$ with $f(a)=b$. Then$$
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