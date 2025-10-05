---
tags:
  - theorem
  - definition
  - math/category_theory
related topics:
  - "[[Power set]]"
  - "[[Category]]"
---
For a [[Set]] $S$, its power set $2^S$ induces a category (Say $2^S_ subset.eq $) defined by
- Objects:
	$$A inop("Obj")(2^S_ subset.eq ) <==> A subset.eq S$$
	Its objects are the subsets of $S$.
- Morphisms:
	$$
	(A,B) inop("Hom")_{2^S_ subset.eq }(A,B) <==> A subset.eq B
	$$
	there exists a single morphism from $A$ to $B$ when $A subset.eq B$, otherwise $op("Hom")_{2^S_ subset.eq }(A,B)=\emptyset$.
- Composition:
	$$a\overset{(a,b)}{ -> }b\overset{(b,c)}{ -> }c ==> a\overset{(a,c)}{ -> }c$$
---
$2^S_ subset.eq $ is a category.
##### Proof:
- Reflexivity:
	For any set $A$, $a in A ==> a in A$ (obviously) so $A subset.eq A$.
- Transitivity:
	Let sets $A subset.eq B subset.eq C$, if $a in A$ then $a in B$ (by $A subset.eq B$) and $a in C$ (by $B subset.eq C$), so $a in A ==> a in C$ meaning $A subset.eq C$.
So $ subset.eq $ is a [[Preorder]] on $2^S$ for any set $S$, and by [[Preorder induces category]] it induces a category.