---
tags:
  - definition
  - set_theory
  - needs_source
related topics:
  - "[[Set]]"
reference:
  - "Aluffi, P. (2009). Algebra: Chapter 0"
aliases:
  - Disjoint
  - Union
  - Intersection
  - Difference
---
A [[Set]] can be defined via _operations_ on other sets. 
- Union:
	For sets $S,T$ their union$$
		S\cup T=\{x\ |\ x\in S \lor x\in T\}
	$$is the set whose elements are in either $S$ or $T$ (or possibly both). This generalizes for a family of sets $T$ as$$
		\bigcup_{S\in T} S = \{s\ |\ \exists S\in T.s\in S\}
	$$for the set whose elements are in any of the elements of $T$.
- Intersection:
	For sets $S,T$ their intersection$$
		S\cap T = \{x\ |\ x\in S \land x\in T\}
	$$is the set whose elements are in both $S$ and $T$. This generalizes for a family of sets $T$ as$$
		\bigcap_{S\in T} S=\{s\ |\ \forall S\in T. s\in S\}
	$$for the set whose elements are in all of the elements of $T$. Sets are said to be _disjoint_ when their intersection is the [[Set|Empty set]].
- Difference:
	For sets $S,T$ their difference$$
		S-T = \{x\ |\ x\in S \land x\notin T\}
	$$is the set of elements of $S$ that are not in $T$.
- Product:
	For sets $S,T$ their product$$
		S\times T = \{(s,t)\ |\ s\in S \land t\in T\}
	$$is the set whose elements are [[Ordered pair|ordered pairs]] $(s,t)$ with $s\in S$ and $t\in T$. This generalizes for a family of sets $S$ [[Index|indexed]] by $I$ as$$
		\prod_{i\in I} S_i = \left.\left\{ f:I\to\bigcup_{i\in I}S_i\ \right|\ f(i)\in S_i\right\}
	$$
- Disjoint union:
	For sets $S,T$ their disjoint union$$
		S+T = (S\times\{0\}) \cup (T\times\{1\})
	$$is the set whose elements are ordered pairs $(i,x)$ with $i= 0$ if $x\in S$ and $i=1$ if $x\in T$. This generalizes for a family of sets $S$ [[Index|indexed]] by $I$ as$$
		\coprod_{i\in I}S_i = \{(s,i)\ |\ s\in S_i\}
	$$