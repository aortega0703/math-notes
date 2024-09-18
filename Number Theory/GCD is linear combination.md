---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Greatest Common Divisor|GCD]]"
mathLink: $\operatorname{gcd}(a,b)=as+bt$
---
For $a,b\in\mathbb{Z}$ with $a,b\neq 0$, there exist $s,t\in\mathbb{Z}$ such that $\operatorname{gcd}(a,b)=as+bt$. Moreover $\operatorname{gcd}(a,b)$ is the smallest positive integer of the form $as+bt$.
##### Proof:
Let $S=\{d=as+bt: s,t\in\mathbb{Z}, d>0\}$ and by [[Well ordering principle]] let $d=\operatorname{min}(S)$.
- $d$ is a common divisor: 
	By [[Division algorithm]] there exist unique $q,r\in\mathbb{Z}$ such that $a=qd+r$ with $0\leq r < d$. To show that $r=0$ suppose $r>0$, then$$
	\begin{align}
		r &= a - qd\\
			&= a - q(as + bt)\quad\text{for some $s,t\in\mathbb{Z}$}\\
			&= a(1-qs) + b(-qt)\\
		r &\in S
	\end{align}$$Which is a contradiction with $r<g$ since $g$ is the smallest element in $S$. Therefore $r=0$ and $d$ divides $a$.
- $d$ is the greatest common divisor:
	Suppose there is another common divisor $d'$ such that $a=nd'$ and $b=md'$, then$$
	\begin{align}
		d &= as + bt\quad\text{for some $s,t\in\mathbb{Z}$}\\
			&= (nd')s + (md')t\\
			&= (ns + mt)d'
	\end{align}$$If $ns + mt<0$ then $d'<0$ so $d'< d$. If $ns + mt > 0$ then $d'\leq d$. Finally $ns + mt \neq 0$ as it would make $g=0$. Therefore $d \geq d'$ for all divisors $d'$.