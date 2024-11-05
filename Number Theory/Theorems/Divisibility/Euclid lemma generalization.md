---
tags:
  - theorem
  - number_theory
---
If $d$ divides $ab$ and $\gcd(a,d) = 1$, then $d$ divides $b$.
##### Proof:
By [[Division algorithm]]
$$
\begin{align}
	1 &= as + dt\\
	b &= abs +dbt\\
	&= qds + dbt\\
	&= d(qs+bt)
\end{align}
$$
So $d$ divides $b$.