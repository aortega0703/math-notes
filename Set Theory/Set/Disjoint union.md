---
tags:
  - definition
  - set_theory
related topics:
  - "[[Set operations]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
For [[Set|sets]] $S,T$ their disjoint union is[^1][^2]$$
	S+T \cong S'\cup T'
$$where $S'\cong S$, $T'\cong T$ and $S'\cap T'=\emptyset$. A common construction of their disjoint union is$$
S+T \cong (S\times\{0\}) \cup (T\times\{1\})
$$being the set whose elements are [[Ordered pair|ordered pairs]] $(i,x)$ with $i= 0$ if $x\in S$ and $i=1$ if $x\in T$. This generalizes for a family of sets $S$ [[Index|indexed]] by $I$ as[^2]$$
	\sum_{i\in I}S_i \cong \{(s,i)\ |\ s\in S_i\}
$$
---

[^1]: $=$ is not used for the choice of $S'$ and $T'$ is arbitrary as long as they are disjoint, so $S+B$ may be a different set depending on the choice for $S'$ and $T'$. $\cong$ is used however as all sets that meet the criteria are isomorphic (by [[Disjoint union is well-defined up to isomorphism]]).
[^2]: The usual notation is $+$ or $\amalg$ for the binary case, and $\sum$ or $\coprod$ for the general case.