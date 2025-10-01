---
tags:
  - theorem
  - set_theory
related topics:
  - "[[Set operations|Exponentiation]]"
  - "[[Cardinality]]"
mathLink: $\left|B^A\right|=|B|^{|A|}$
---
For finite [[Set|sets]] $A,B$,$$
\left|B^A\right|=|B|^{|A|}
$$
##### Proof:
Enumerate the elements of $A$ as $a_1, a_2, \dots, a_{|A|}$. The proof proceeds by induction on $\{a_1,a_2,\dots, a_n\}$.
- Case $n=1$:
	Let$$
	
		f_k: \{a_1\} &\to B\
		a &\mapsto b_k
	
	$$where $1 lt.eq k lt.eq |B|$. There are clearly $|B|$ such functions so $|B^{\{a_1\}}|=|B|= |B|^1=|B|^{\{a_1\}}$.
- Case $n+1$:
	Let $f:\{a_1,a_2,\dots, a_n\}\to B$ and$$
	
		g_k: \{a_1, a_2, \dots, a_n, a_{n+1}\} &\to B\
		a &\mapsto
		\begin{cases}
			f(a) &\text{if $a in\operatorname{Dom} f$}\
			b_k &\text{otherwise}
		\end{cases}
	
	$$where $1 lt.eq k lt.eq |B|$. There are clearly $|B|$ such functions for each $f$, by induction there are $|B|^{n}$ possible $f$'s, so $|B^{\{a_1, \dots, a_{n+1}\}}|=|B|^n |B|=|B|^{n+1}=|B|^{|\{a_1,\dots,a_{n+1}\}|}$.
Then $\left|B^A\right|=|B|^{|A|}$ holds for finite sets of arbitrary size $A,B$.