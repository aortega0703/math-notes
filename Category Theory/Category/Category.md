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
A _category_ $\mathcal{C}$ is composed of
- A collection of _objects_ $\operatorname{ob}(\mathcal{C})$.
- A collection of _morphisms/arrows_ $\operatorname{arr}(\mathcal{C})$.
so that:
- Each morphism has a _domain_ and _codomain_ object. The notation $f: X\to Y$ (or $X\overset{f}{\to}Y$) signifies that $f$ is a morphism with domain $X$ and codomain $Y$.
- Each object $X$ has an _identity morphism_ $\operatorname{id}_X : X\to X$.
- For any pair of morphisms $X \overset{f}{\to} Y \overset{g}{\to} Z$, there exists a _composite morphism_ $gf: X \to Z$.
and composition is:
- (Unital with identity) For any $f: X\to Y$, $\operatorname{id}_Y f = f \operatorname{id}_X = f$.
- (Associative) For any morphisms $A\overset{f}{\to} B\overset{g}{\to} C\overset{h}{\to} D$, $(hg)f = h(gf)$, (thus denoted simply $hgf$).
---
- Commutative diagram:
	A _diagram_ is said to _commute_ when all paths with a common beginning and end are equal.
- Hom-set:
	The collection$$
		\operatorname{Hom}(X,Y) = \{f in\operatorname{arr}(\mathcal{C})\ |\ f : X \to Y\}
	$$usually receives the name of _Hom-set_ as in set of homomorphisms (even if not containing homomorphisms, or not a set).
- Small category:
	A category is called _small_ when $\operatorname{op}(\mathcal{C})$ is a set, otherwise it is _large_. A category is _locally small_ when every $\operatorname{Hom}(X,Y)$ is a set.
- Endomorphism:
	A morphism $f: A\to A$ is called an _endomorphism_. $\operatorname{Hom}(A,A)$ is denoted $\operatorname{End}(A)$.
- Discrete Category:
	A category is _discrete_ when it only contains identity morphisms.