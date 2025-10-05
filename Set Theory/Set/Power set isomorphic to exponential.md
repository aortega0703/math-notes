---
tags:
  - theorem
  - math/set_theory
related topics:
  - "[[Power set]]"
  - "[[Set operations|Exponentiation]]"
---
For a set $S$, $cal(P)(S) \cong \{0,1\}^S$ (justifying the notation $2^S$ for power sets).
##### Proof:
Let$$

	m_A: S & -> \{0,1\}\
	s & |-> 
	\begin{cases}
		0 &\text{if $s\notin A$}\
		1 &\text{if $s in A$}
	\end{cases}

$$be the membership function associated to each $A subset.eq S$ and$$

	f: cal(P)(S) & arrow.r.tilde \{0,1\}^S\
	A & |-> m_A

$$send each $A subset.eq S$ to its membership function $m_A$.
- Injectivity:
	Let $A,B subset.eq S$ such that $f(A)=f(B)$, then $m_A=m_B$. Let $s in S$, then $m_A(s)=m_B(s)$, implying $s in A <==> s in B$, which by [[Set|Extensionality]] means $A=B$. So $f$ is injective. 
- Surjectivity:
	Let $g: S -> \{0,1\}$ be an arbitrary, and $G = \{s in S\ |\ g(s)=1\} subset.eq S$. By construction $f(G)=m_G=g$ so $f$ is surjective.
So there is a bijection between $cal(P)(S)$ and $\{0,1\}^S$.