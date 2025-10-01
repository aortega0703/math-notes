---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Power set]]"
  - "[[Set operations|Exponentiation]]"
---
For a set $S$, $\mathcal{P}(S) \cong \{0,1\}^S$ (justifying the notation $2^S$ for power sets).
##### Proof:
Let$$

	m_A: S &\to \{0,1\}\
	s &\mapsto
	\begin{cases}
		0 &\text{if $s\notin A$}\
		1 &\text{if $s in A$}
	\end{cases}

$$be the membership function associated to each $A\subseteq S$ and$$

	f: \mathcal{P}(S) &\overset{\sim}{\to} \{0,1\}^S\
	A &\mapsto m_A

$$send each $A\subseteq S$ to its membership function $m_A$.
- Injectivity:
	Let $A,B\subseteq S$ such that $f(A)=f(B)$, then $m_A=m_B$. Let $s in S$, then $m_A(s)=m_B(s)$, implying $s in A  <==> s in B$, which by [[Set|Extensionality]] means $A=B$. So $f$ is injective. 
- Surjectivity:
	Let $g: S \to \{0,1\}$ be an arbitrary, and $G = \{s in S\ |\ g(s)=1\}\subseteq S$. By construction $f(G)=m_G=g$ so $f$ is surjective.
So there is a bijection between $\mathcal{P}(S)$ and $\{0,1\}^S$.