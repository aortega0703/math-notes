---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Group of permutations]]"
  - "[[Order]]"
---
For $1\leq d\leq n$, there is some $\sigma\in S_n$ with [[Order]] $d$.
##### Proof:
By induction on $n$.
- $\mathcal{P}(1)$:
	$e\in S_1$ by definition of [[Group]], and $|e|=1$.
- $\mathcal{P}(n)\implies \mathcal{P}(n+1)$:
	- Case $d\leq n$:
		By induction there is some $\sigma\in S_n$ such that $|\sigma|=d$, consider$$
		\begin{align}
			\sigma': \mathbb{Z}/(n+1)\mathbb{Z} &\to \mathbb{Z}/(n+1)\mathbb{Z}\\
			s &\mapsto
			\begin{cases}
				\sigma(s) &\text{if $s\leq n$}\\
				n+1 &\text{if $s=n+1$}
			\end{cases}
		\end{align}
		$$
		- Injectivity:
			Let $1\leq s,s'\leq n+1$. If $s,s'\leq n$ then $\sigma'(s)=\sigma(s)$ and $\sigma'(s')=\sigma(s')$, so $\sigma'(s)=\sigma'(s')$ implies $s=s'$ by injectivity of $\sigma$.  If $s\leq n$ and $s'=n+1$ (or vice versa) then $\sigma'(s)=\sigma(n)<n+1=\sigma'(s)'$. So $\sigma'(s)=\sigma'(s')$ implies $s=s'$ for all $s,s'$ making $\sigma'$ injective.
		- Surjectivity:
			Let $1\leq s\leq n+1$. If $s\leq n$ then $s=\sigma(s')=\sigma'(s')$ for some $s'\leq n$ by surjectivity of $\sigma$. If $s=n+1$ then $s=\sigma'(n+1)$. So $\text{Im}(\sigma') = \text{Cod}(\sigma')$ making $\sigma'$ surjective.
		Then $\sigma'$ is a bijection (it permutes $\mathbb{Z}/(n+1)\mathbb{Z}$) so $\sigma'\in S_{n+1}$.
		- $|\sigma'|\leq d$:
			Let $1\leq s\leq n+1$. If $s\leq n$ then $\sigma'^d(s)=\sigma^d(s)=s$. If $s=n+1$ then $\sigma'^d(s)=n+1=s$. So $\sigma'^d=e$.
		- $|\sigma'| \geq d$:
			Let $1\leq d'< d$. As $|\sigma|=d$ there is some $1\leq s\leq n$ such that $s\neq\sigma^{d'}(s)=\sigma'^{d'}(s)$, so $\sigma'^{d'}\neq e$.
		Then $\sigma'\in S_{n+1}$ with $|\sigma'|=d$.
	- Case $d = n+1$:
		Consider$$
		\begin{align}
			\sigma: \mathbb{Z}/(n+1)\mathbb{Z} &\to \mathbb{Z}/(n+1)\mathbb{Z}\\
			s &\mapsto
			\begin{cases}
				s+1 &\text{if $s\leq n$}\\
				1 &\text{if $s=n+1$}
			\end{cases}
		\end{align}
		$$
		- Injectivity:
			Let $1\leq s,s'\leq n+1$ and assume $\sigma(s)=\sigma(s')$, then $s+1=s'+1$, so $s=s'$ making $\sigma$ injective.
		- Surjectivity:
			Let $1\leq s\leq n+1$. If $s>1$ then $s=s-1+1=\sigma(s-1)$. If $s=1$ then $s=\sigma(n+1)$. Then $\sigma$ is surjective.
		Then $\sigma$ is a bijection (it permutes $\mathbb{Z}/(n+1)\mathbb{Z}$) so $\sigma\in S_{n+1}$.
		- $|\sigma|\leq d$:
			Let $1\leq s\leq n+1$, then $\sigma^{n+1-s}(s)=s+(n+1-s)=n+1$ and $\sigma^s(n+1)=s$, so $\sigma^{n+1}(s)=\sigma^{n+1-s+s}(s)=(\sigma^{n+1-s}\sigma^s)(s)=\sigma^s(n+1)=s$. Then $\sigma^{n+1}=e$.
		- $|\sigma|\geq d$:
			Let $1<d'< n+1$, then $\sigma^{d'}(n+1)=d'<n+1$, so $\sigma^{d'}\neq e$.
		Then $\sigma\in S_{n+1}$ with $|\sigma|=d$.
	Therefore there is some $\sigma\in S_{n+1}$ with $|\sigma|=d$ for all $d\leq n+1$.
Therefore there is some $\sigma\in S_{n}$ with $|\sigma|=d$ for all $d\leq n$.