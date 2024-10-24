---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Divisibility]]"
  - "[[Divisibility|Prime]]"
---
Every integer $n>1$ is a prime or a product of primes. This product is unique save for the order of its factors.
##### Proof:
- Existence of the product:
	- Case $n=2$:
		$2$ is prime.
	- Case $n+1$:
		Let $S=\{d:d|n+1, 1<d<n+1\}$. If $S=\emptyset$ then $n+1$ is prime by definition. If $S\neq \emptyset$ by [[Well ordering principle]] let $p=min(S)$ which is prime by [[Least divisor is prime]]. Then for some $1<u<n+1$$$
		\begin{align}
			n+1 &= pu\\
				&= p \prod_{i} p_i \quad\text{by induction}
		\end{align}$$
		So $n+1$ is the product of primes.
	Therefore every $n$ is a prime or the product of primes.
- Uniqueness of the product:
	Let $n=\prod_{i=0}^{k} p_i = \prod_{i=0}^c q_i$ for primes $p_i, q_j$ and $k\leq c$. Lets prove that $\prod_{i=n}^{k} p_i = \prod_{i\in I_n} q_i$ such that $I_0 = \{0,1,\dots,c\}$ and $I_{n+1} = I_n - \{j\}$ for some $j\in I_n$.
	- Step $n=0$:
		By hypothesis.
	- Step $n+1\leq k$:
		$\prod_{i=n}^{k} p_i = \prod_{i\in I_n} q_i$ by the step $n$. $p_n$ divides $\prod_{i=n}^{k} p_i = \prod_{i\in I_n} q_i$, so by [[Generalized Euclid's lemma]] it divides $q_j$ for some $j\in I_n$. As $q_j$ is prime its only prime factor is itself, so $p_i = q_j$ and $\prod_{i=n+1}^{k} p_i = \prod_{i\in I_{n+1}} q_i$ where $I_{n+1} = I_n - \{j\}$.
	After step $k$ we get $\prod_{i=k+1}^{k} p_i = \prod_{i\in I_{k+1}} q_i=1$ so $I_{k+1}=\emptyset$ and $k=c$. Therefore the mapping in the construction was bijective and $(p_i)_{i=0}^k$ and $(q_i)_{i=0}^c$ are equal up to permutation.
