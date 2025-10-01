---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Integers]]"
mathLink: $a = qb + r$
---
For $a,b in  ZZ$ with $b>0$, exist unique $q,r in ZZ$ such that $a=bq+r$ with $0 lt.eq r < b$.
##### Proof:
- Existence:
	Let $S=\{a-bk: k in ZZ,\ 0 lt.eq a-bk\}$. $S$ is not empty by cases on $a$
	- Case $a\geq 0$:
		$a-b(0)= a \geq 0$, so $0 in S$.
	- Case $a < 0$:
		$a-b(a) = (1-b)a = -(b-1)a \geq 0$, so $a in S$.
	By [[Well ordering principle]] there is a least element $r in S$. Let $q$ such that $r=a-bq$ and suppose $r\geq b$, then$$
	
		a-bq &\geq b\
		a-bq-b &\geq 0\
		a-b(q+1) &\geq 0\
		a-b(q+1)& in S\
		q+1 &> q\
		b(q+1) &> bq\
		a - b(q+1) &< a - bq = r
	$$Which is a contradiction as $r$ is chosen as the least element, therefore $r<b$. So therefore there exist some $q,r$ with the desired property.
- Uniqueness:
	Suppose $r,r',q,q'$ such that $r=a-bq$ and $r'=a- bq'$ with $r'\geq r$, then$$
	
		r + bq &= r' + bq'\
		bq - bq' &= r'- r\
		0 lt.eq b(q-q') &= r'-r  lt.eq r'< b
	$$As $0 lt.eq b(q-q') < b$ then $q-q'=0$ and $r'-r=0$ so $q,r$ are unique.