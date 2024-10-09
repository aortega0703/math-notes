---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Divides|Prime]]"
---
There is no maximum prime gap. That is, the distance between two consecutive primes can be arbitrarily large.
##### Proof:
Let $k\geq 2$, then$$
\begin{align}
	k! &\equiv 0&&(\operatorname{mod}\ n),\text{ for all $2\leq n\leq k$}\\
	k! + n &\equiv 0 &&(\operatorname{mod}\ n)\\
\end{align}
$$Therefore $k! + 2,\ k! + 3,\dots,\ k! + k$ are all composite, making for a prime gap of at least $k-1$. As $k$ can be arbitrarily large there is no maximum prime gap.