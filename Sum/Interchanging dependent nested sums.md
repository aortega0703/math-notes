---
tags:
  - theorem
mathLink: $\sum_{i=1}^n \sum_{j=1}^i a_i b_j = \sum_{i=1}^n \sum_{j=i}^n a_j b_i$
---
#theorem 
$$\sum_{i=1}^n \sum_{j=1}^i a_i b_j = \sum_{i=1}^n \sum_{j=i}^n a_j b_i$$
##### Proof:
By induction
- Case $n=0$: empty sums equal $0$.
- Case $n+1$: $$
	\begin{align}
		\sum_{i=1}^{n+1} \sum_{j=1}^i a_i b_j
		&= \sum_{i=1}^n \sum_{j=1}^i a_i b_j 
			+ \sum_{j=1}^{n+1} a_{n+1} b_j\\
		&= \sum_{i=1}^n \sum_{j=i}^n a_j b_i 
			+ \sum_{j=1}^n a_{n+1} b_j 
			+ a_{n+1}b_{n+1}\\
		&= \sum_{i=1}^n \left(
			\sum_{j=i}^n a_j + a_{n+1}
			\right) b_i 
			+ a_{n+1}b_{n+1}\\
		&= \sum_{i=1}^n \left(
			\sum_{j=i}^{n+1} a_j
			\right) b_i 
			+ a_{n+1}b_{n+1}\\
		&= \sum_{i=1}^{n+1} \left(
			\sum_{j=i}^{n+1} a_j
			\right) b_i\\
		&= \sum_{i=1}^{n+1} \sum_{j=i}^{n+1} a_j b_i\\
	\end{align}
	$$
Therefore both sums are equal.