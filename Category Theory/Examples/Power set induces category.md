---
tags:
  - theorem
  - definition
  - math/category_theory
related topics:
  - "[[Power set]]"
  - "[[Category]]"
---
For a [[Set]] $S$, its power set $2^S$ induces a category (Say $2^S_\subseteq$) defined by
- Objects:
	$$A in\operatorname{Obj}(2^S_\subseteq)  <==> A \subseteq S$$
	Its objects are the subsets of $S$.
- Morphisms:
	$$
	(A,B) in\operatorname{Hom}_{2^S_\subseteq}(A,B)  <==> A\subseteq B
	$$
	there exists a single morphism from $A$ to $B$ when $A\subseteq B$, otherwise $\operatorname{Hom}_{2^S_\subseteq}(A,B)=\emptyset$.
- Composition:
	$$a\overset{(a,b)}{\to}b\overset{(b,c)}{\to}c \implies a\overset{(a,c)}{\to}c$$
---
$2^S_\subseteq$ is a category.
##### Proof:
- Reflexivity:
	For any set $A$, $a in A \implies a in A$ (obviously) so $A\subseteq A$.
- Transitivity:
	Let sets $A\subseteq B\subseteq C$, if $a in A$ then $a in B$ (by $A\subseteq B$) and $a in C$ (by $B\subseteq C$), so $a in A \implies a in C$ meaning $A\subseteq C$.
So $\subseteq$ is a [[Preorder]] on $2^S$ for any set $S$, and by [[Preorder induces category]] it induces a category.