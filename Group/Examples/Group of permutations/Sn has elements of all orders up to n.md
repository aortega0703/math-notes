---
tags:
  - theorem
  - math/abstract_algebra
related topics:
  - "[[Group of permutations]]"
  - "[[Order]]"
---
For $1 lt.eq d lt.eq n$, there is some $\sigma in S_n$ with [[Order]] $d$.
##### Proof:
By induction on $n$.
- $\mathcal{P}(1)$:
	$e in S_1$ by definition of [[Group]], and $|e|=1$.
- $\mathcal{P}(n)\implies \mathcal{P}(n+1)$:
	- Case $d lt.eq n$:
		By induction there is some $\sigma in S_n$ such that $|\sigma|=d$, consider$$
		
			\sigma':  ZZ/(n+1) ZZ &\to  ZZ/(n+1) ZZ\
			s &\mapsto
			\begin{cases}
				\sigma(s) &\text{if $s lt.eq n$}\
				n+1 &\text{if $s=n+1$}
			\end{cases}
		
		$$
		- Injectivity:
			Let $1 lt.eq s,s' lt.eq n+1$. If $s,s' lt.eq n$ then $\sigma'(s)=\sigma(s)$ and $\sigma'(s')=\sigma(s')$, so $\sigma'(s)=\sigma'(s')$ implies $s=s'$ by injectivity of $\sigma$.  If $s lt.eq n$ and $s'=n+1$ (or vice versa) then $\sigma'(s)=\sigma(n)<n+1=\sigma'(s)'$. So $\sigma'(s)=\sigma'(s')$ implies $s=s'$ for all $s,s'$ making $\sigma'$ injective.
		- Surjectivity:
			Let $1 lt.eq s lt.eq n+1$. If $s lt.eq n$ then $s=\sigma(s')=\sigma'(s')$ for some $s' lt.eq n$ by surjectivity of $\sigma$. If $s=n+1$ then $s=\sigma'(n+1)$. So $\text{Im}(\sigma') = \text{Cod}(\sigma')$ making $\sigma'$ surjective.
		Then $\sigma'$ is a bijection (it permutes $ ZZ/(n+1) ZZ$) so $\sigma' in S_{n+1}$.
		- $|\sigma'| lt.eq d$:
			Let $1 lt.eq s lt.eq n+1$. If $s lt.eq n$ then $\sigma'^d(s)=\sigma^d(s)=s$. If $s=n+1$ then $\sigma'^d(s)=n+1=s$. So $\sigma'^d=e$.
		- $|\sigma'| \geq d$:
			Let $1 lt.eq d'< d$. As $|\sigma|=d$ there is some $1 lt.eq s lt.eq n$ such that $s !=\sigma^{d'}(s)=\sigma'^{d'}(s)$, so $\sigma'^{d'} != e$.
		Then $\sigma' in S_{n+1}$ with $|\sigma'|=d$.
	- Case $d = n+1$:
		Consider$$
		
			\sigma:  ZZ/(n+1) ZZ &\to  ZZ/(n+1) ZZ\
			s &\mapsto
			\begin{cases}
				s+1 &\text{if $s lt.eq n$}\
				1 &\text{if $s=n+1$}
			\end{cases}
		
		$$
		- Injectivity:
			Let $1 lt.eq s,s' lt.eq n+1$ and assume $\sigma(s)=\sigma(s')$, then $s+1=s'+1$, so $s=s'$ making $\sigma$ injective.
		- Surjectivity:
			Let $1 lt.eq s lt.eq n+1$. If $s>1$ then $s=s-1+1=\sigma(s-1)$. If $s=1$ then $s=\sigma(n+1)$. Then $\sigma$ is surjective.
		Then $\sigma$ is a bijection (it permutes $ ZZ/(n+1) ZZ$) so $\sigma in S_{n+1}$.
		- $|\sigma| lt.eq d$:
			Let $1 lt.eq s lt.eq n+1$, then $\sigma^{n+1-s}(s)=s+(n+1-s)=n+1$ and $\sigma^s(n+1)=s$, so $\sigma^{n+1}(s)=\sigma^{n+1-s+s}(s)=(\sigma^{n+1-s}\sigma^s)(s)=\sigma^s(n+1)=s$. Then $\sigma^{n+1}=e$.
		- $|\sigma|\geq d$:
			Let $1<d'< n+1$, then $\sigma^{d'}(n+1)=d'<n+1$, so $\sigma^{d'} != e$.
		Then $\sigma in S_{n+1}$ with $|\sigma|=d$.
	Therefore there is some $\sigma in S_{n+1}$ with $|\sigma|=d$ for all $d lt.eq n+1$.
Therefore there is some $\sigma in S_{n}$ with $|\sigma|=d$ for all $d lt.eq n$.