---
tags:
  - definition
  - math/set_theory
related topics:
  - "[[Set]]"
  - "[[Subset]]"
reference:
  - "Gallian, J. A. Contemporary Abstract Algebra"
---
A _partition_ of a [[Set]] $S$ is a collection $P$ such that its elements
- Nonempty subsets of $S$:
	For all $p in P$, $p in P ==> p subset.eq S\land p != \emptyset$.
- Cover $S$:
	$\displaystyle\bigcup_{p in P} p = S$
- Are disjoint:
	For all $p,q in P$, $p\cap q != \emptyset ==> p=q$
---
- The sets in a partition receive the name of _cells_.
- The cell containing $s$ is denoted by $\overline{s}$.
