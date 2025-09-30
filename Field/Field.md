---
tags:
  - definition
  - math/abstract_algebra
related topics:
  - "[[Set]]"
  - "[[Binary Operation]]"
---
A field is a [[Set]] $F$ with [[Binary Operation|Binary Operations]] $+, \cdot: F\times F \to F$ (addition and multiplication) that has (for $a,b,c\in F$)
- Commutativity:$$ \begin{align}
	a + b &= b + a\\
	ab &= ba
	\end{align}$$ 
- Associativity:$$ 
	\begin{align}
		(a + b) + c &= a + (b + c)\\
		(ab) c &= a(bc)
	\end{align}$$
- Distributivity:$$
	a(b+c) = ab + ac
	$$
- Identities for $+,\cdot$:$$
	\begin{align}
		0&\in F\quad s.t.&\hspace{-1.5em} 0 + a &= a\\
		1&\in F\quad s.t.& 1a&=a\\
		0&\neq1
	\end{align}$$
- Inverses for $+,\cdot$: $$
	\begin{align}
		-a &\in F \quad s.t.& \hspace{-1.5em}-a + a &= 0\\
		a\neq 0 \implies a^{-1} &\in F\quad s.t.& a^{-1}a &= 1
	\end{align}$$
