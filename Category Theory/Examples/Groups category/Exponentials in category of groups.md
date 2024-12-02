---
tags:
  - theorem
  - abstract_algebra
  - category_theory
related topics:
  - "[[Category of groups]]"
  - "[[Exponential object]]"
---
For any [[Group]] $G$ and set $A$, $G^A = \text{Hom}_\mathbf{Set}(A, G)$ is a group with the operation $$
\begin{align}
	+:G^A\times G^A &\to G^A\\
	f,g&\mapsto f(\_)\cdot g(\_)
\end{align}
$$
##### Proof:
- Closed under $+$:
	Let $f,g\in G^A$ and $a\in A$, then $(f+g)(a)=f(a)\cdot g(a)\in G$ as $G$ is closed under $\cdot$ by the group axioms, so $G^A$ is closed under $+$.
- Associativity:
	Let $f,g,h\in G^A$ and $a\in A$, then$$
	\begin{align}
		((f+g)+h)(a)
		&= (f+g)(a)\cdot h(a)\\
		&= f(a) \cdot g(a) \cdot h(a)\\
		&= f(a) \cdot (g+h)(a)\\
		&= (f+(g+h))(a)
	\end{align}
	$$And by [[Set|Extensionality]] this implies $(f+g)+h=f+(g+h)$ making $+$ associative.
- Identity:
	Consider$$
	\begin{align}
		e: A &\to G\\
		a &\mapsto e_G
	\end{align}
	$$and let $f\in G^A$, and $a\in A$. Then$$
	\begin{align}
		(f+e)(a)
		&= f(a)\cdot e(a)\\
		&= f(a) \cdot e_G\\
		&= f(a)
	\end{align}
	$$which by [[Set|Extensionality]] implies $f+e=f$, and similarly $e+f=f$. Then $e$ is an identity element in $G^A$.
- Inverses:
	Let $f\in G^A$ and consider$$
	\begin{align}
		-f: A &\to G\\
		a &\mapsto (f(a))^{-1}
	\end{align}
	$$let $a\in A$, then$$
	\begin{align}
		(f+(-f))(a)
		&= f(a) \cdot (f(a))^{-1}\\
		&= e_G\\
		&= e(a)
	\end{align}
	$$which by [[Set|Extensionality]] implies $f+(-f)=e$, and similarly $-f+f=e$. Then $-f$ is the inverse for the arbitrary element $f$ in $G^A$.
Then $G^A$ satisfies the group axioms and is therefore a group.