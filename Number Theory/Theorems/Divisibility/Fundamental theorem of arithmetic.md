---
tags:
  - theorem
  - number_theory
related topics:
  - "[[Divides]]"
  - "[[Divides|Prime]]"
---
Every integer $n>1$ is a prime or a product of primes. This product is unique save for the order of its factors.
##### Proof:
- Existence of the product:
	- Case $n=2$:
		$2$ is prime.
	- Case $n+1$:
		Let $S=\{d:d|n+1, 1<d<n+1\}$. If $S=\varnothing$ then $n+1$ is prime by definition. If $S\neq \varnothing$ by [[Well ordering principle]] let $p=min(S)$ which is prime by [[Least divisor is prime]]. Then for some $1<u<n+1$$$
		\begin{align}
			n+1 &= pu\\
				&= p \prod_{i} p_i \quad\text{by induction}
		\end{align}$$
		So $n+1$ is the product of primes.
	Therefore every $n$ is a prime or the product of primes.
- Uniqueness of the product:
	Let $n=\prod_{i=1}^{k} p_i = \prod_{i\in I_1}q_i$ such that $n \leq I_1$. Lets prove then by induction that $\prod_{i=t}^{k} p_i = \prod_{i\in I_t}q_i$ where $|I_t| = |I_{t+1}+1|$ as follows
	- Case $t=1$:
		$\prod_{i=1}^{k} p_i = \prod_{i\in I_1}q_i$ by hypothesis
	- Case $t+1$:$$
		\begin{align}
			\prod_{i\in I_t} q_i 
				&= \prod_{i=t}^{k} p_i
					\quad\text{by induction}\\
				&= p_t \prod_{i=t+1}^{k} p_i\\
			p_t 
				&\ \left|\ \prod_{i\in I_t} q_i\right.\\
			p_t &\ \ \big|\ qj
				\quad\text{for some $j\in I_t$}\tag{1}\\
			p_t &= q_j \quad\text{by primality of $q_j$}
		\end{align}$$Where $(1)$ is by [[Euclid's lemma|$p|ab \implies p|a \lor p|b$]]. Let $I_{t+1} = I_t - \{j\}$, then$$
		\begin{align}
			\prod_{i=t}^{k} p_i
				&= \prod_{i\in I_t} q_i 
					\quad\text{by induction}\\
				&= q_j \prod_{i\in I_{t+1}} q_i\\
			\prod_{i=t+1}^{k} p_i
				&= \prod_{i\in I_{t+1}} q_i
					\quad\text{as $p_t=q_j\neq 0$}
		\end{align}
		$$
	After step $k+1$ we get $\prod_{i=k+1}^k p_i = \prod_{i\in I_{k+1}} q_i = 1$ , so $I_{n+1} = \varnothing$ for the (empty) product of $q_i>1$ to equal $1$. Therefore $|I_1|=k$, furthermore $q_1,\dots,q_k$ is a permutation of $p_1,dots,p_k$ by taking $p_t \to q_j$ with $j\in I_t - I_{t+1}$ (which by construction is a singleton).