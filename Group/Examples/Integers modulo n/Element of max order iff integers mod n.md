---
tags:
  - theorem
  - abstract_algebra
related topics:
  - "[[Order]]"
  - "[[Integers modulo n (group)]]"
---
For a [[Group]] $G$, there is some $g\in G$ such that $|g| = |G|$ if and only if $G \cong \mathbb{Z}/|G|\mathbb{Z}$.
##### Proof:
- $|g|=|G| \implies G\cong \mathbb{Z}/n\mathbb{Z}$:
	By [[Equality of different exponents criterion]] $g^i=g^k \iff i \equiv j\ (\text{mod }|g|)$. Then $|\langle g\rangle|=|g|=|G|$ so $\langle g\rangle=G$. Now consider$$
	\begin{align}
		\begin{aligned}
			\phi: G &\to \mathbb{Z}/|G|\mathbb{Z}\\
			g^k &\mapsto [k]_{|G|}
		\end{aligned}\qquad
		\begin{aligned}
			\phi^{-1}: \mathbb{Z}/|G|\mathbb{Z} &\to G\\
			[k]_{|G|} &\mapsto g^k
		\end{aligned}
	\end{align}
	$$
	- $\phi$ and $\phi^{-1}$ are well defined:
		Consider $a,b\in\mathbb{Z}$ such that $[a]_{|G|}=[b]_{|G|}$, then by definition of [[Congruence under modulo]] $|G|=|g|$ divides $b-a$, so$$
		\begin{align}
			\phi^{-1}([a]_{|G|})
			&= g^a\\
			&= g^a e\\
			&= g^a g^{|g|k}\\
			&= g^a g^{b-a}\\
			&= g^{a+b-a}\\
			&= g^b\\
			&= \phi^{-1}([b]_{|G|})
		\end{align}
		$$
		So $\phi^{-1}$ is well defined. $\phi$ is trivially well defined as well.
	- $\phi$ and $\phi^{-1}$ are [[Group homomorphism|group homomorphisms]]:
		Let $g^i,g^j\in G$ and $[a]_{|G|},[b]_{|G|}\in\mathbb{Z}/|G|\mathbb{Z}$, then by [[Mod Distributes Over Addition]]$$
		\begin{align}
			\begin{aligned}
				\phi(g^i g^j)
				&= \phi(g^{i+j})\\
				&= [i+j]_{|G|}\\
				&= [i]_{|G|}+[j]_{|G|}\\
				&= \phi(g^i) + \phi(j)
			\end{aligned}\qquad
			\begin{aligned}
				\phi^{-1}([a]_{|G|}+[b]_{|G|})
				&= \phi^{-1}([a+b]_{|G|})\\
				&= g^{a+b}\\
				&= g^a g^b\\
				&= \phi^{-1}([a]_{|G|})\phi^{-1}([b]_{|G|})
			\end{aligned}
		\end{align}
		$$
		So both $\phi$ and $\phi^{-1}$ are homomorphisms.
	- $\phi$ and $\phi^{-1}$ are inverses:
		Let $g^{k}\in G$ and $[a]_{|G|}\in\mathbb{Z}/|G|\mathbb{Z}$, then$$
		\begin{align}
			\begin{aligned}
				(g^k)(\phi\phi^{-1})
				&= ([k]_{|G|})\phi^{-1}\\
				&= g^k
			\end{aligned}\qquad
			\begin{aligned}
				([a]_{|G|})(\phi^{-1}\phi)
				&= (g^a)\phi\\
				&= [a]_{|G|}
			\end{aligned}
		\end{align}
		$$So by [[Set|Extensionality]] $\phi\phi^{-1}=\text{id}_G$ and $\phi^{-1}\phi=\text{id}_{\mathbb{Z}/|G|\mathbb{Z}}$, so $\phi$ and $\phi^{-1}$ are inverses.
	Then $G \cong \mathbb{Z}/|G|\mathbb{Z}$.
- $G \cong \mathbb{Z}/|G|\mathbb{Z} \implies |g|=|G|$:
	Let $\phi:G\overset{\sim}{\to}\mathbb{Z}/|G|\mathbb{Z}$ be an isomorphism. $\big|[1]_{|G|}\big|=|G|$, so by [[Group isomorphism preserves order]] $\big|\phi([1]_{|G|})\big|=|G|$.