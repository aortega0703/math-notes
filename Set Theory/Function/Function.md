---
tags:
  - definition
  - math/set_theory
aliases:
  - Mapping
  - Domain
  - Image
  - Function composition
  - Graph
reference:
  - Gallian, J. A. Contemporary Abstract Algebra
  - "Aluffi, P. (2009). Algebra: Chapter 0"
---
For [[Set]]s $A,B$
- A _function_ $f$ from $A$ to $B$ (denoted $f:A -> B$) assigns to each $a in A$ exactly one $b in B$ (in notation $f(a)=b$). It can be defined as a set $Gamma _f subset.eq A times B$ (its _graph_) such that $forall a in A.space exists ! b in B. (a,b) in Gamma _f$ where $(a,b) in Gamma _f <==> f(a)=b$.
- The action of $f$ on some element $a$ is sometimes indicated as $a |-> f(a)$.
For a function $f:A -> B$ and some $a in A$
- $A$ is called the _domain_ of $f$.
- $B$ is called the _co-domain_ of $f$.
- $f(a)$ is called the _image_ of $a$ under $f$.
---
- Function composition:
	For functions $A limits(->)^f B limits(->)^g C$ there is a function$$
	
		g compose f: A & -> C\
		a & |-> g(f(a))
	
	$$
- Image of a subset of the domain:
	For a function $f:A -> B$ and $S subset.eq A$, the image of $S$ is defined as$$
		f(S) =\{f(a) in B ;space a in S\} subset.eq B
	$$
- Image of the function:
	For a function $f:A -> B$, the image of $f$ is defined as$$
		 op("Im") (f) = \{f(a) in B: a in A\} subset.eq B
	$$Note that $f(A)= op("Im") (f)$.
- Pre-image of a subset of the co-domain:
	For a function $f:A -> B$ and $S subset.eq B$, the pre-image of $S$ is defined as$$
		f^(-1)(S) = \{a in A: exists b in B. f(a)=b\} subset.eq A
	$$Note that $f^(-1)(B)=A$. If $S=\{b\}$ then $f^(-1)(S)$ or simply $f^(-1)(b)$ is called the _fiber_ over $b$.
- Restriction of a function:
	For a function $f:A -> B$ and $A' subset.eq A$, the _restriction_ of $f$ to $A'$ ($f|_(A'): S -> B$) is defined as$$
		f|_(A') (a) = f(a)
	$$Note that $f|_(A')=f compose i$ where $i: A' -> A$ is an inclusion function.