---
tags:
  - theorem
  - abstract_algebra
  - to_do
related topics:
  - "[[Cyclic group]]"
  - "[[Order]]"
  - "[[Greatest Common Divisor|GCD]]"
---
For a group $G$ and $a\in G$
- $\langle a^i \rangle = \langle a^j \rangle$ if and only if $\operatorname{gcd}(|a|,i) = \operatorname{gcd}(|a|,j)$.
- $|a^i| = |a^j|$ if and only if $\operatorname{gcd}(|a|,i) = \operatorname{gcd}(|a|,j)$.
##### Proof:
- $\implies$:$$
	\begin{align}
		\langle a^i \rangle 
			&= \langle a^j \rangle\\
		|a^i| 
			&= |a^j|\\
		\frac{|a|}{\operatorname{gcd}(|a|,i)}
			&= \frac{|a|}{\operatorname{gcd}(|a|,j)}
			\tag{1}\\
		\operatorname{gcd}(|a|,i)
			&= \operatorname{gcd}(|a|,j)
	\end{align}$$$(1)$ by [[Order of power element]].
- $\impliedby$:$$
	\begin{align}
		\operatorname{gcd}(|a|,i) &= \operatorname{gcd}(|a|,j)\\
		a^{\operatorname{gcd}(|a|,i)} &= a^{\operatorname{gcd}(|a|,j)}\\
		\langle a^{\operatorname{gcd}(|a|,i)}\rangle &= \langle a^{\operatorname{gcd}(|a|,j)}\rangle\\
		\langle a^i \rangle &= \langle a^j \rangle
	\end{align} \tag{2}
	$$$(2)$ by [[Order of power element]].
The previous proves the first statement, and the second one follows directly from it.