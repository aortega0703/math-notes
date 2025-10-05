---
tags:
  - definition
  - math/set_theory
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
  - Cartesian product
  - Quotient
  - Exponentiation
---
A [[Set]] can be defined via _operations_ on other sets. 
- Union:
	For sets $S,T$ their union$$
		S\cup T=\{x\ |\ x in S \lor x in T\}
	$$is the set whose elements are in either $S$ or $T$ (or possibly both). This generalizes for a family of sets $T$ as$$
		\bigcup_{S in T} S = \{s\ |\ \exists S in T.s in S\}
	$$for the set whose elements are in any of the elements of $T$.
- Intersection:
	For sets $S,T$ their intersection$$
		S\cap T = \{x\ |\ x in S \land x in T\}
	$$is the set whose elements are in both $S$ and $T$. This generalizes for a family of sets $T$ as$$
		\bigcap_{S in T} S=\{s\ |\ \forall S in T. s in S\}
	$$for the set whose elements are in all of the elements of $T$. Sets are said to be _disjoint_ when their intersection is the [[Set|Empty set]].
- Difference:
	For sets $S,T$ their difference$$
		S-T = \{x\ |\ x in S \land x\notin T\}
	$$is the set of elements of $S$ that are not in $T$.
- Product:
	For sets $S,T$ their product$$
		S times T = \{(s,t)\ |\ s in S \land t in T\}
	$$is the set whose elements are [[Ordered pair|ordered pairs]] $(s,t)$ with $s in S$ and $t in T$. This generalizes for a family of sets $S$ [[Index|indexed]] by $I$ as$$
		\prod_{i in I} S_i = \left.\left\{ f:I -> \bigcup_{i in I}S_i\ \right|\ f(i) in S_i\right\}
	$$
- Quotient:
	For a set $S$ and an [[Equivalence relation]] $\sim$, the _quotient_ of $S$ with respect to $\sim$ (denoted $S/\sim$) is the set of equivalence classes of $S$ with respect to $\sim$.
- Exponentiation:
	For sets $S,T$$$
		T^S = \{f\ |\ f: S -> T\}
	$$is the set of all functions from $S$ to $T$.