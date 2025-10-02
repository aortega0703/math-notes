---
tags:
  - theorem
  - math/category_theory
related topics:
  - "[[Category]]"
---
For [[Category|Morphisms]] $A_1\overset{f_1}{\to}A_2\overset{f_2}{\to}\dots\overset{f_n}{\to}A_{n+1}$, all compositions are equal to each other regardless of parenthesis placement.
##### Proof:
Let $P(n)$ be the case for $n$ morphisms. Lets prove by [[Strong induction]] that $P(n)$ holds for all $n>2$.
- $P(2)$:
	The only choice for parenthesis is $(f_2 f_1)$.
- $P(n-1)\implies P(n)$:
	Any composition of $n$ morphisms is of the form $PK$ (composition is binary) where $P$ is the composition of $n-k$ functions and $K$ is the composition of $k$ functions ($1 lt.eq k< n$). By induction$$
	P=((\dots((f_{n}f_{n-1})f_{n-2})\dots)f_{k+1}), quad K=((\dots((f_k f_{k-1})f_{k-2})\dots) f_1)
	$$Let $Q=((\dots((f_{k}f_{k-1})f_{k-2})\dots)f_{2})$, then $PK=P(Q f_1)= (PQ)f_1$. As $PQ$ is the composition of $n-1$ functions, by induction$$
		PQ = ((\dots((f_{n}f_{n-1})f_{n-2})\dots)f_{2})
	$$so $PK=((\dots((f_{n}f_{n-1})f_{n-2})\dots)f_{1})$.
Therefore parenthesis placement is irrelevant in categories.