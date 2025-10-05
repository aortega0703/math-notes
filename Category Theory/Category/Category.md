---
tags:
  - definition
  - math/category_theory
reference:
  - Riehl, E. Category Theory in Context (2017)
  - "Aluffi, P. (2009). Algebra: Chapter 0"
aliases:
  - Morphism
  - Object
  - Identity morphism
---
A _category_ $cal(C)$ is composed of
- A collection of _objects_ $op("ob")(cal(C))$.
- A collection of _morphisms/arrows_ $op("arr")(cal(C))$.
so that:
- Each morphism has a _domain_ and _codomain_ object. The notation $f: X -> Y$ (or $X\overset{f}{ -> }Y$) signifies that $f$ is a morphism with domain $X$ and codomain $Y$.
- Each object $X$ has an _identity morphism_ $op("id")_X : X -> X$.
- For any pair of morphisms $X \overset{f}{ -> } Y \overset{g}{ -> } Z$, there exists a _composite morphism_ $gf: X -> Z$.
and composition is:
- (Unital with identity) For any $f: X -> Y$, $op("id")_Y f = f op("id")_X = f$.
- (Associative) For any morphisms $A\overset{f}{ -> } B\overset{g}{ -> } C\overset{h}{ -> } D$, $(hg)f = h(gf)$, (thus denoted simply $hgf$).
---
- Commutative diagram:
	A _diagram_ is said to _commute_ when all paths with a common beginning and end are equal.
- Hom-set:
	The collection$$
		op("Hom")(X,Y) = \{f inop("arr")(cal(C))\ |\ f : X -> Y\}
	$$usually receives the name of _Hom-set_ as in set of homomorphisms (even if not containing homomorphisms, or not a set).
- Small category:
	A category is called _small_ when $op("op")(cal(C))$ is a set, otherwise it is _large_. A category is _locally small_ when every $op("Hom")(X,Y)$ is a set.
- Endomorphism:
	A morphism $f: A -> A$ is called an _endomorphism_. $op("Hom")(A,A)$ is denoted $op("End")(A)$.
- Discrete Category:
	A category is _discrete_ when it only contains identity morphisms.