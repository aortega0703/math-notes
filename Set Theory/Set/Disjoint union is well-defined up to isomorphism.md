---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Injectivity and surjectivity|Bijection]]"
  - "[[Disjoint union]]"
---
If $A' \cong A''$ and $B' \cong B''$, and $A'\cap B' = \emptyset$ and $A''\cap B'' = \emptyset$, then $A' \cup B' \cong A'' \cup B''$. Meaning $A \amalg B$ is well-defined up to isomorphism.
##### Proof:
As $A' \cong A''$ and $B' \cong B''$ let $f_A: A'\overset{\sim}{\to} A''$ and $f_B: B'\overset{\sim}{\to}B''$ be their corresponding bijections. Let$$
\begin{align}
	f: A'\cup B' &\overset{\sim}{\to} A'' \cup B''\\
	s &\mapsto
	\begin{cases}
		f_A(s) &\text{if $s\in A'$}\\
		f_B(s) &\text{if $s\in B'$}
	\end{cases}
\end{align}
$$
- $f$ is well-defined:
	$f_A(s)$ and $f_B(s)$ are both well-defined. Then for $f$ to be ill-defined it has to map $s$ to both $f_A(s)$ and $f_A(s)$, meaning $s\in A' \cap B'=\emptyset$, as there is no such $s$, $f$ is well-defined.
- $f$ is injective:
	Let $s_1,s_2\in A'\cup B'$ such that $f(s_1)=f(s_2)$.
	- Case $s_1, s_2 \in A'$:$$
		\begin{align}
			f(s_1) &= f(s_2)\\
			f_A(s_1) &= f_A(s_2)\\
			s_1 &= s_2
				&\text{by $f_A$ injective}
		\end{align}
		$$
	- Case $s_1, s_2\in B'$:$$
		\begin{align}
			f(s_1) &= f(s_2)\\
			f_B(s_1) &= f_B(s_2)\\
			s_1 &= s_2
				&\text{by $f_B$ injective}
		\end{align}
		$$
	- Case $s_1\in A'$, $s_2\in B'$ (or vice versa):
		As $f_A(s_1)\in A''$ then $f_B(s_2)=f_A(s_1)\in A''$ so $f_B(s_2)\in A'' \cap B''$. As $A''\cap B''=\emptyset$ there are no such $s_1$ and $s_2$.
- $f$ is surjective:
	Let $s\in A''\cup B''$
	- $s\in A''$:$$
		\begin{align}
			s&=f_A(a') &\text{by $f_A$ surjective}\\
			s&=f(a') &\text{for some $a'\in A'$}
		\end{align}
		$$
	- $s\in B''$:$$
		\begin{align}
			s&=f_B(b') &\text{by $f_B$ surjective}\\
			s&=f(b') &\text{for some $b'\in B'$}
		\end{align}
		$$
So $f$ is a bijection, therefore $A'\cup B' \cong A'' \cup B''$.