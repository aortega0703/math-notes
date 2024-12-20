---
related topics:
  - "[[Group]]"
  - "[[Subgroup]]"
tags:
  - theorem
  - abstract_algebra
---
### Criteria 1
For a [[Group]] $G$ and $H\subseteq G$ non-empty, $H$ is a [[Subgroup]] of $G$ if and only if $a,b\in H \implies ab^{-1} \in H$.
##### Proof:
- $\implies$:
	By hypothesis $H$ is a group so it has inverses and is closed under $\cdot$.
- $\impliedby$:
	For $H$ to be a group it has to have
	- Associativity:
		Let $a,b,c \in H\subseteq G$, then $(ab)c=a(bc)$ by associativity of $\cdot$.
	- Identity for $\cdot$: 
		Let $a\in H$, then$$
		\begin{align}
			a &\in H\\
			a a^{-1} = e&\in H
		\end{align}$$
	- Inverses for $\cdot$: $$
	\begin{align}
		e,a &\in H\\
		ea^{-1}=a^{-1}&\in H
	\end{align}$$
	As $H$ satisfies all previous criteria, it is a group (and thus a subgroup of $G$).
	
### Criteria 2
For a [[Group]] $G$ and $H\subseteq G$ non-empty, $H$ is a [[Subgroup]] of $G$ if and only if $H$ is closed under $\cdot$ and is closed under inverses.
##### Proof:
- $\implies$:
	By hypothesis $H$ is a group so it is closed under $\cdot$ and is closed under inverses.
- $\impliedby$:
	- Associativity:
		Let $a,b,c \in H\subseteq G$, then $(ab)c=a(bc)$ by associativity of $\cdot$.
	- Identity for $\cdot$:
		Let $a\in H$, then$$
		\begin{align}
			a^{-1} &\in H\\
			a a^{-1}=e &\in H
		\end{align}$$
	- Inverses for $\cdot$:
		Let $a\in H$, then $a^{-1}\in H$ is given by the hypothesis.