---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Integers]]"
mathLink: $a = qb + r$
---
For $a,b\in \mathbb{Z}$ with $b>0$, exist unique $q,r\in\mathbb{Z}$ such that $a=bq+r$ with $0\leq r < b$.
##### Proof:
- Existence:
	Let $S=\{a-bk: k\in\mathbb{Z},\ 0\leq a-bk\}$. $S$ is not empty by cases on $a$
	- Case $a\geq 0$:
		$a-b(0)= a \geq 0$, so $0\in S$.
	- Case $a < 0$:
		$a-b(a) = (1-b)a = -(b-1)a \geq 0$, so $a\in S$.
	By [[Well ordering principle]] there is a least element $r\in S$. Let $q$ such that $r=a-bq$ and suppose $r\geq b$, then$$
	\begin{align}
		a-bq &\geq b\\
		a-bq-b &\geq 0\\
		a-b(q+1) &\geq 0\\
		a-b(q+1)&\in S\\
		q+1 &> q\\
		b(q+1) &> bq\\
		a - b(q+1) &< a - bq = r
	\end{align}$$Which is a contradiction as $r$ is chosen as the least element, therefore $r<b$. So therefore there exist some $q,r$ with the desired property.
- Uniqueness:
	Suppose $r,r',q,q'$ such that $r=a-bq$ and $r'=a- bq'$ with $r'\geq r$, then$$
	\begin{align}
		r + bq &= r' + bq'\\
		bq - bq' &= r'- r\\
		0\leq b(q-q') &= r'-r \leq r'< b
	\end{align}$$As $0\leq b(q-q') < b$ then $q-q'=0$ and $r'-r=0$ so $q,r$ are unique.